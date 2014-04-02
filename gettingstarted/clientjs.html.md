# client.js[¶](clientjs.html.md#client-js)

Add the Trello API client library to your page like so:

    
```html
    <head>
      <!-- ...  -->
    
      <!-- The client library requires jQuery  -->
      <script src="http://code.jquery.com/jquery-1.7.1.min.js"></script>
      <script src="https://api.trello.com/1/client.js?key=substitutewithyourapplicationkey"></script>
    
      <!-- ...  -->
    </head>
```

This will create a `Trello` object, which you can use to interact with the
Trello API.

## Authorizing[¶](clientjs.html.md#authorizing)

Call `Trello.authorize(opts)` with the following options:

  * `type`
    * `"redirect"` or `"popup"`
    * default is `"redirect"`
    * Whether authorization should be done in a new window, or by leaving the current page
  * `name`
    * name of your application, which is displayed during the authorization process
  * `persist`
    * `true` or `false`
    * Default is `true`
    * If `true`, the token will be saved to local storage.
  * `interactive`
    * `true` or `false`
    * Default is `true`
    * If `false`, don't redirect or popup, only use the stored token
  * `scope`
    * Object like `{ read: allowRead, write: allowWrite, account: allowAccount }`
    * Default is read-only, i.e. `{ read: true, write: false, account: false }`
    * Each permission is a boolean
  * `expiration`
    * `"1hour"`, `"1day"`, `"30days"`, `"never"`
    * Default is `"30days"`
    * When the token should expire
  * `success`
    * Optional function to be called on success
  * `error`
    * Optional function to be called on error

If using `type: "redirect"`, the token will be returned to the current
`location.href`. When it is returned, call `authorize` with `interactive:
false` to get the token.

## Using the API[¶](clientjs.html.md#using-the-api)

You can use the API via a single call: `Trello.rest(method, path[, params],
success, error)`

  * `method`
    * `"GET"`, `"POST"`, `"PUT"`, `"DELETE"`
  * `path`
    * API path to use, such as `"members/me"`
  * `params`
    * Parameters to the API path, such as `{ fields: "username,fullName" }`
    * Default is `{}`
  * `success`
    * Optional function to be called on success
  * `error`
    * Optional function to be called on error

There are also a number of convenience methods, with similar signatures. One
for each HTTP method:

  * `Trello.get(path[, params], success, error)`
  * `Trello.post(path[, params], success, error)`
  * `Trello.put(path[, params], success, error)`
  * `Trello.delete(path[, params], success, error)`

An alias for `delete`:

  * `Trello.del(path[, params], success, error)`

And one for [``](clientjs.html.md#id1)GET``ting on each collection:

  * `Trello.actions.get(id[, params], success, error)`
  * `Trello.cards.get(id[, params], success, error)`
  * `Trello.checklists.get(id[, params], success, error)`
  * `Trello.boards.get(id[, params], success, error)`
  * `Trello.lists.get(id[, params], success, error)`
  * `Trello.members.get(id[, params], success, error)`
  * `Trello.organizations.get(id[, params], success, error)`

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
