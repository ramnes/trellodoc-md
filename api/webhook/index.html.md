# webhook[¶](index.html.md#webhook)

## GET /1/webhooks/[webhook_id][¶](index.html.md#get-1-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/webhooks/[webhook_id]/[field][¶](index.html.md#get-1-webhooks-idwebhook-field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `description`
        * `idModel`
        * `callbackURL`
        * `active`

## PUT /1/webhooks/[webhook_id][¶](index.html.md#put-1-webhooks-idwebhook)

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

## PUT /1/webhooks/[¶](index.html.md#put-1-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model that should be hooked

## PUT /1/webhooks/[webhook_id]/active[¶](index.html.md#put-1-webhooks-idwebhook-active)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/webhooks/[webhook_id]/callbackURL[¶](index.html.md#put-1-webhooks-idwebhook-callbackurl)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request

## PUT /1/webhooks/[webhook_id]/description[¶](index.html.md#put-1-webhooks-idwebhook-description)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/webhooks/[webhook_id]/idModel[¶](index.html.md#put-1-webhooks-idwebhook-idmodel)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** id of the model to be monitored

## POST /1/webhooks[¶](index.html.md#post-1-webhooks)

  * **Required permissions:** read
  * **Arguments**
    * `description` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `callbackURL` (required)
      * **Valid Values:** A valid URL that is reachable with a HEAD request
    * `idModel` (required)
      * **Valid Values:** id of the model that should be hooked

## DELETE /1/webhooks/[webhook_id][¶](index.html.md#delete-1-webhooks-idwebhook)

  * **Required permissions:** read
  * **Arguments:** None

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
