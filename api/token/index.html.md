[![](https://d2isj6rbqore70.cloudfront.net/trellogo-
docs.png)](../../index.html) [Go to trello.com →](../../../index.html)

### Navigation

  * [Trello documentation](../../index.html) »
  * [API Reference (Beta)](../index.html) »

# token[¶](index.html#token)

## GET /1/tokens/[token][¶](index.html#get-1-tokens-token)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `identifier`
        * `idMember`
        * `dateCreated`
        * `dateExpires`
        * `permissions`
    * `webhooks` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
  * **Examples**
    
    https://api.trello.com/1/tokens/91a6408305c1e5ec1b0b306688bc2e2f8fe67abf6a2ecec38c17e5b894fcf866?key=[application_key]&token=[optional_auth_token]
    
    {
        "id": "4ee7f1e00081da1fcb00014b",
        "identifier": "",
        "idMember": "4ee7df3ce582acdec80000b2",
        "dateCreated": "2011-12-14T00:46:24.534Z",
        "dateExpires": "2020-01-01T00:00:00.000Z",
        "permissions": [{
            "idModel": "*",
            "modelType": "*",
            "read": true,
            "write": false
        }]
    }

## GET /1/tokens/[token]/[field][¶](index.html#get-1-tokens-token-field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `identifier`
        * `idMember`
        * `dateCreated`
        * `dateExpires`
        * `permissions`

## GET /1/tokens/[token]/member[¶](index.html#get-1-tokens-token-member)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `avatarHash`
        * `bio`
        * `bioData`
        * `confirmed`
        * `fullName`
        * `idPremOrgsAdmin`
        * `initials`
        * `memberType`
        * `products`
        * `status`
        * `url`
        * `username`
        * `avatarSource`
        * `email`
        * `gravatarHash`
        * `idBoards`
        * `idBoardsInvited`
        * `idBoardsPinned`
        * `idOrganizations`
        * `idOrganizationsInvited`
        * `loginTypes`
        * `newEmail`
        * `oneTimeMessagesDismissed`
        * `prefs`
        * `status`
        * `trophies`
        * `uploadedAvatarHash`
        * `premiumFeatures`

## GET /1/tokens/[token]/member/[field][¶](index.html#get-1-tokens-token-
member-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `avatarHash`
        * `bio`
        * `bioData`
        * `confirmed`
        * `fullName`
        * `idPremOrgsAdmin`
        * `initials`
        * `memberType`
        * `products`
        * `status`
        * `url`
        * `username`
        * `avatarSource`
        * `email`
        * `gravatarHash`
        * `idBoards`
        * `idBoardsInvited`
        * `idBoardsPinned`
        * `idOrganizations`
        * `idOrganizationsInvited`
        * `loginTypes`
        * `newEmail`
        * `oneTimeMessagesDismissed`
        * `prefs`
        * `status`
        * `trophies`
        * `uploadedAvatarHash`
        * `premiumFeatures`

## GET /1/tokens/[token]/webhooks[¶](index.html#get-1-tokens-token-webhooks)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/tokens/[token]/webhooks/[idWebhook][¶](index.html#get-1-tokens-
token-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments**
    * `idWebhook` (required)
      * **Valid Values:** The id of the webhook

## PUT /1/tokens/[token]/webhooks[¶](index.html#put-1-tokens-token-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model to be monitored

## POST /1/tokens/[token]/webhooks[¶](index.html#post-1-tokens-token-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model to be monitored

## DELETE /1/tokens/[token][¶](index.html#delete-1-tokens-token)

  * **Required permissions:** write
  * **Arguments:** None

## DELETE /1/tokens/[token]/webhooks/[idWebhook][¶](index.html#delete-1
-tokens-token-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments**
    * `idWebhook` (required)
      * **Valid Values:** The id of the webhook

### Search

### [Documentation Home](../../index.html)

  * [token](index.html#)
    * [GET /1/tokens/[token]](index.html#get-1-tokens-token)
    * [GET /1/tokens/[token]/[field]](index.html#get-1-tokens-token-field)
    * [GET /1/tokens/[token]/member](index.html#get-1-tokens-token-member)
    * [GET /1/tokens/[token]/member/[field]](index.html#get-1-tokens-token-member-field)
    * [GET /1/tokens/[token]/webhooks](index.html#get-1-tokens-token-webhooks)
    * [GET /1/tokens/[token]/webhooks/[idWebhook]](index.html#get-1-tokens-token-webhooks-idwebhook)
    * [PUT /1/tokens/[token]/webhooks](index.html#put-1-tokens-token-webhooks)
    * [POST /1/tokens/[token]/webhooks](index.html#post-1-tokens-token-webhooks)
    * [DELETE /1/tokens/[token]](index.html#delete-1-tokens-token)
    * [DELETE /1/tokens/[token]/webhooks/[idWebhook]](index.html#delete-1-tokens-token-webhooks-idwebhook)

### Browse

  * Prev: [search](../search/index.html)
  * Next: [type](../type/index.html)

### You are here:

  * [Trello documentation](../../index.html)
    * [API Reference (Beta)](../index.html)
      * token

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.

