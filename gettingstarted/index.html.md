# Getting Started[¶](index.html.md#getting-started)

## Introduction[¶](index.html.md#introduction)

Trello provides a simple
[RESTful](http://en.wikipedia.org/wiki/Representational_state_transfer) web
API where each type of resource (e.g. a card, a board, or a member) has a URI
that you can interact with.

For example, if you'd like to use the API to get information about the [Trello
Development board](http://trello.com/board/trello-development/4d5ea62fd76aa1136000000c),
you'd use the following URI:

    
    https://api.trello.com/1/boards/4d5ea62fd76aa1136000000c

**Notes:**

  * All API requests go to `https://api.trello.com`
  * The `/1` part of the URI is the API version
  * The `/boards` part means that we're addressing Trello's collection of boards
  * The `/4d5ea62fd76aa1136000000c` part is the id of the board that we want to interact with. You'll notice that the board id is also part of the [board's URL in Trello](http://trello.com/board/trello-development/4d5ea62fd76aa1136000000c)

The simplest thing you can do with a Trello resource URI is `GET` it. (When
using REST API via HTTP, you "read" something by using the HTTP `GET` method).

However, if you `GET` the aforementioned URI
(`https://api.trello.com/1/boards/4d5ea62fd76aa1136000000c`), for example by
pasting it in the address bar of a web browser, you won't get the board data;
instead you'll get an `invalid key` error (with a `401 Unauthorized` HTTP
status code). That's because all requests to the Trello API must include an
[application key](index.html.md#application-key), which Trello uses to identify
the application making the request.

## Getting an Application Key[¶](index.html.md#getting-an-application-key)

You can get your application key by logging into Trello, and then visiting
[https://trello.com/1/appKey/generate](https://trello.com/1/appKey/generate)

Your 32-character application key will be listed in the first box. For the
rest of the examples, we're going to assume that your application key is
`substitutewithyourapplicationkey`

If you're doing a `GET` request, you include your application in the query
string portion of the URL. If you `GET` [https://api.trello.com/1/board/4d5ea6
2fd76aa1136000000c?key=substitutewithyourapplicationkey](https://api.trello.co
m/1/board/4d5ea62fd76aa1136000000c?key=substitutewithyourapplicationkey)
you'll no longer get an error. Instead, you'll get a response that looks like
this:

    
```json
    {"id":"4d5ea62fd76aa1136000000c","name":"Trello Development","desc":"Trello board used by the Trello team to track work on Trello.  How meta!\n\nThe development of the Trello API is being tracked at https://trello.com/api\n\nThe development of Trello Mobile applications is being tracked at https://trello.com/mobile","closed":false,"idOrganization":"4e1452614e4b8698470000e0","url":"https://trello.com/board/trello-development/4d5ea62fd76aa1136000000c","prefs":{"voting":"public","permissionLevel":"public","invitations":"members","comments":"public"}}
```

All the responses to Trello API calls use JSON. You can make the response look
prettier by running it through a javascript beautifier, which will give you
something like this:

    
```json
    {
        "id": "4d5ea62fd76aa1136000000c",
        "name": "Trello Development",
        "desc": "Trello board used by the Trello team to track work on Trello.  How meta!\n\nThe development of the Trello API is being tracked at https://trello.com/api\n\nThe development of Trello Mobile applications is being tracked at https://trello.com/mobile",
        "closed": false,
        "idOrganization": "4e1452614e4b8698470000e0",
        "url": "https://trello.com/board/trello-development/4d5ea62fd76aa1136000000c",
        "prefs": {
            "voting": "public",
            "permissionLevel": "public",
            "invitations": "members",
            "comments": "public"
        }
    }
```

If you wanted to include additional information in the response, you could add
additional parameters (documented [here](http://trello.com/api/board/index.html#get-1-boards-
board-id)). For example, if you wanted to also get all the open lists and
cards on the Trello Development board, you could `GET` this URL:

    
    https://api.trello.com/1/board/4d5ea62fd76aa1136000000c?key=substitutewithyourapplicationkey&cards=open&lists=open

If you wanted to read a board of your own, you could get its id (the easiest
way is to visit the board in Trello and copy the id out of the URL), and
request

    
    https://api.trello.com/1/board/substitutewiththeboardid?key=substitutewithyourapplicationkey

However, unless your board is public (like the Trello Development board), when
you try to `GET` that URL, you'll get a `401 unauthorized` error. You can only
read a private board (or card, or organization) if the API knows that you have
permission to read that resource. You can tell the API that you've been
authorized to read private data by including a [token](index.html.md#token),
which is given to your by a user and which allows you to read (and potentially
write) things on their behalf.

**Notes:**

  * The application key is used only to let Trello know which application is making the request; it doesn't tell Trello who the request is being made on behalf of. For example, if you're using your own application key, you still need to generate a [token](index.html.md#token) to be able to access any of your private boards.

## Getting a Token from a User[¶](index.html.md#getting-a-token-from-a-user)

Full documentation for authorizing a client can be found at [_Authorizing a
Client_](authorize.html.md), and for authorizing via OAuth can be found at
[_Authorizing via OAuth_](oauth.html.md).

You can request a token from a user by directing them to an authorization URL,
like the following:

Request a token granting read-only access for 30 days (the default):

    
    https://trello.com/1/authorize?key=substitutewithyourapplicationkey&name=My+Application&expiration=30days&response_type=token

Request a token granting read-only access forever:

    
    https://trello.com/1/authorize?key=substitutewithyourapplicationkey&name=My+Application&expiration=never&response_type=token

Request a token granting read/write access for 1 day:

    
    https://trello.com/1/authorize?key=substitutewithyourapplicationkey&name=My+Application&expiration=1day&response_type=token&scope=read,write

If the user accepts your request, they'll be directed to a page where they
will be given a token (64 characters), which they can give back to your
application. If you add the token to your request, like so:

    
    https://api.trello.com/1/board/substitutewiththeboardid?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

... then you'll be able to read a board that's only visible to the user

Once you've gotten a token from a user, you can also make requests that give
you information about the user that authorized the token, like this:

Get the member's record:

    
    https://trello.com/1/members/me?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

Get the cards that a user is assigned to:

    
    https://trello.com/1/members/my/cards?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

Get the open boards that a user is a member of:

    
    https://trello.com/1/members/my/boards?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

Get the boards that a user has pinned to their boards menu:

    
    https://trello.com/1/members/my/boards/pinned?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

Get the organizations that a user is a member of:

    
    https://trello.com/1/members/my/organizations?key=substitutewithyourapplicationkey&token=substitutethispartwiththeauthorizationtokenthatyougotfromtheuser

Of course, having a user copy and paste a token into your application isn't
very pretty. The Trello API also supports basic
[OAuth](http://tools.ietf.org/html/rfc5849); you can use an OAuth library and
the following URLs:

    
    https://trello.com/1/OAuthGetRequestToken
    https://trello.com/1/OAuthAuthorizeToken
    https://trello.com/1/OAuthGetAccessToken

You'll also need your application secret (used to sign your requests). That's
listed in the second box on
[https://trello.com/1/appKey/generate](https://trello.com/1/appKey/generate).

## Using client.js[¶](index.html.md#using-client-js)

If you're developing an application that has a web interface, you can use the
Trello API client library, like so:

    
```html
    <head>
      <!-- ...  -->
    
      <!-- The client library requires jQuery  -->
      <script src="http://code.jquery.com/jquery-1.7.1.min.js"></script>
      <script src="https://api.trello.com/1/client.js?key=substitutewithyourapplicationkey"></script>
    
      <!-- ...  -->
    </head>
```

The un-minified, documented source of client.js is at
[https://trello.com/1/client.coffee](https://trello.com/1/client.coffee)

Documentation for using client.js is at [_client.js_](clientjs.html.md)

The client library can take care of getting the authorization token from the
user, and provides a wrapper around the `GET`, `PUT`, `POST` and `DELETE` HTTP
methods.

Examples using the client library:

  * [jsfiddle that reads a member's cards](http://jsfiddle.net/nNesx/)
  * [jsfiddle that adds a comment to a selected card](http://jsfiddle.net/E4rLn/)
  * [Trello Calendar](http://trellocalendar-francois2metz.dotcloud.com)

## Watching Models with Webhooks[¶](index.html.md#watching-models-with-webhooks)

Webhooks provide a way for third party applications to keep Trello data in
sync with their own servers. Webhooks can be registered to watch models, and
when a change happens on one of those models, the third party is informed.

Full documentation on Webhooks can be found at [_Webhooks_](webhooks.html.md).

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
