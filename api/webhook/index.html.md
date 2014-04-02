[![](https://d2isj6rbqore70.cloudfront.net/trellogo-
docs.png)](../../index.html) [Go to trello.com →](../../../index.html)

### Navigation

  * [Trello documentation](../../index.html) »
  * [API Reference (Beta)](../index.html) »

# webhook[¶](index.html#webhook)

## GET /1/webhooks/[idWebhook][¶](index.html#get-1-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/webhooks/[idWebhook]/[field][¶](index.html#get-1-webhooks-idwebhook-
field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `description`
        * `idModel`
        * `callbackURL`
        * `active`

## PUT /1/webhooks/[idWebhook][¶](index.html#put-1-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (optional)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (optional)
      * **Valid Values:** id of the model to be monitored
    * `active` (optional)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/webhooks/[¶](index.html#put-1-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model that should be hooked

## PUT /1/webhooks/[idWebhook]/active[¶](index.html#put-1-webhooks-idwebhook-
active)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/webhooks/[idWebhook]/callbackURL[¶](index.html#put-1-webhooks-
idwebhook-callbackurl)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request

## PUT /1/webhooks/[idWebhook]/description[¶](index.html#put-1-webhooks-
idwebhook-description)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/webhooks/[idWebhook]/idModel[¶](index.html#put-1-webhooks-idwebhook-
idmodel)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** id of the model to be monitored

## POST /1/webhooks[¶](index.html#post-1-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model that should be hooked

## DELETE /1/webhooks/[idWebhook][¶](index.html#delete-1-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments:** None

### Search

### [Documentation Home](../../index.html)

  * [webhook](index.html#)
    * [GET /1/webhooks/[idWebhook]](index.html#get-1-webhooks-idwebhook)
    * [GET /1/webhooks/[idWebhook]/[field]](index.html#get-1-webhooks-idwebhook-field)
    * [PUT /1/webhooks/[idWebhook]](index.html#put-1-webhooks-idwebhook)
    * [PUT /1/webhooks/](index.html#put-1-webhooks)
    * [PUT /1/webhooks/[idWebhook]/active](index.html#put-1-webhooks-idwebhook-active)
    * [PUT /1/webhooks/[idWebhook]/callbackURL](index.html#put-1-webhooks-idwebhook-callbackurl)
    * [PUT /1/webhooks/[idWebhook]/description](index.html#put-1-webhooks-idwebhook-description)
    * [PUT /1/webhooks/[idWebhook]/idModel](index.html#put-1-webhooks-idwebhook-idmodel)
    * [POST /1/webhooks](index.html#post-1-webhooks)
    * [DELETE /1/webhooks/[idWebhook]](index.html#delete-1-webhooks-idwebhook)

### Browse

  * Prev: [type](../type/index.html)

### You are here:

  * [Trello documentation](../../index.html)
    * [API Reference (Beta)](../index.html)
      * webhook

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.

