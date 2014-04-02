# Authorizing a Client[¶](authorize.html.md#authorizing-a-client)

If you're authorizing a web client, you may want to check out
[_client.js_](clientjs.html.md), a wrapper for the API in javascript.

You can get a token from Trello with the GET route

    
    https://trello.com/1/authorize

This takes the following parameters:

  * `callback_method`
    * `"postMessage"` or `"fragment"`
    * Defines how the token is returned to you. Generally, `"postMessage"` is used if the authorization is done in a popup, and `"fragment"` if it is done by redirect. For details on how to use these, see [_client.js_](clientjs.html.md)
  * `return_url`
    * URL the token should be returned to
    * If the token is being passed by fragment, this is where the user will be redirected after authorization
    * If the token is being passed by postMessage, this will be used as the `origin` for the postMessage
  * `scope`
    * Comma-separated list of one or more of `"read"`, `"write"`, `"account"`
    * Read: reading of boards, organizations, etc. on behalf of the user
    * Write: writing of boards, organizations, etc. on behalf of the user
    * Account: writing of member info, and marking notifications read
  * `expiration`
    * `"1hour"`, `"1day"`, `"30days"`, `"never"`
    * When the token should expire
  * `name`
    * Name of the application
    * Displayed during the authorization process
  * `key`
    * Application key
    * To get one, check out [_Getting an Application Key_](index.html.md#application-key)

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
