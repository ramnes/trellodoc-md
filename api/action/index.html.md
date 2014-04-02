[![](https://d2isj6rbqore70.cloudfront.net/trellogo-
docs.png)](../../index.html) [Go to trello.com →](../../../index.html)

### Navigation

  * [Trello documentation](../../index.html) »
  * [API Reference (Beta)](../index.html) »

# action[¶](index.html#action)

## GET /1/actions/[idAction][¶](index.html#get-1-actions-idaction)

  * **Required permissions:** read
  * **Arguments**
    * `entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `member` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `member_fields` (optional)
      * **Default:** `avatarHash,fullName,initials,username`
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
    * `memberCreator` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `memberCreator_fields` (optional)
      * **Default:** `avatarHash,fullName,initials,username`
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

## GET /1/actions/[idAction]/[field][¶](index.html#get-1-actions-idaction-
field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`

## GET /1/actions/[idAction]/board[¶](index.html#get-1-actions-idaction-board)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `desc`
        * `descData`
        * `closed`
        * `idOrganization`
        * `invited`
        * `pinned`
        * `starred`
        * `url`
        * `prefs`
        * `invitations`
        * `memberships`
        * `shortLink`
        * `subscribed`
        * `labelNames`
        * `powerUps`
        * `dateLastActivity`
        * `dateLastView`
        * `shortUrl`

## GET /1/actions/[idAction]/board/[field][¶](index.html#get-1-actions-
idaction-board-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `desc`
        * `descData`
        * `closed`
        * `idOrganization`
        * `invited`
        * `pinned`
        * `starred`
        * `url`
        * `prefs`
        * `invitations`
        * `memberships`
        * `shortLink`
        * `subscribed`
        * `labelNames`
        * `powerUps`
        * `dateLastActivity`
        * `dateLastView`
        * `shortUrl`

## GET /1/actions/[idAction]/card[¶](index.html#get-1-actions-idaction-card)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `badges`
        * `checkItemStates`
        * `closed`
        * `dateLastActivity`
        * `desc`
        * `descData`
        * `due`
        * `idBoard`
        * `idChecklists`
        * `idList`
        * `idMembers`
        * `idMembersVoted`
        * `idShort`
        * `idAttachmentCover`
        * `manualCoverAttachment`
        * `labels`
        * `name`
        * `pos`
        * `shortLink`
        * `shortUrl`
        * `subscribed`
        * `url`

## GET /1/actions/[idAction]/card/[field][¶](index.html#get-1-actions-
idaction-card-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `badges`
        * `checkItemStates`
        * `closed`
        * `dateLastActivity`
        * `desc`
        * `descData`
        * `due`
        * `idBoard`
        * `idChecklists`
        * `idList`
        * `idMembers`
        * `idMembersVoted`
        * `idShort`
        * `idAttachmentCover`
        * `manualCoverAttachment`
        * `labels`
        * `name`
        * `pos`
        * `shortLink`
        * `shortUrl`
        * `subscribed`
        * `url`

## GET /1/actions/[idAction]/entities[¶](index.html#get-1-actions-idaction-
entities)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/actions/[idAction]/list[¶](index.html#get-1-actions-idaction-list)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`

## GET /1/actions/[idAction]/list/[field][¶](index.html#get-1-actions-
idaction-list-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`

## GET /1/actions/[idAction]/member[¶](index.html#get-1-actions-idaction-
member)

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

## GET /1/actions/[idAction]/member/[field][¶](index.html#get-1-actions-
idaction-member-field)

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

## GET /1/actions/[idAction]/memberCreator[¶](index.html#get-1-actions-
idaction-membercreator)

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

## GET /1/actions/[idAction]/memberCreator/[field][¶](index.html#get-1
-actions-idaction-membercreator-field)

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

## GET /1/actions/[idAction]/organization[¶](index.html#get-1-actions-
idaction-organization)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `displayName`
        * `desc`
        * `descData`
        * `idBoards`
        * `invited`
        * `invitations`
        * `memberships`
        * `prefs`
        * `powerUps`
        * `products`
        * `url`
        * `website`
        * `logoHash`
        * `premiumFeatures`

## GET /1/actions/[idAction]/organization/[field][¶](index.html#get-1-actions-
idaction-organization-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `displayName`
        * `desc`
        * `descData`
        * `idBoards`
        * `invited`
        * `invitations`
        * `memberships`
        * `prefs`
        * `powerUps`
        * `products`
        * `url`
        * `website`
        * `logoHash`
        * `premiumFeatures`

## PUT /1/actions/[idAction][¶](index.html#put-1-actions-idaction)

  * **Required permissions:** read
  * **Arguments**
    * `text` (optional)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/actions/[idAction]/text[¶](index.html#put-1-actions-idaction-text)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## DELETE /1/actions/[idAction][¶](index.html#delete-1-actions-idaction)

  * **Required permissions:** read
  * **Arguments:** None

### Search

### [Documentation Home](../../index.html)

  * [action](index.html#)
    * [GET /1/actions/[idAction]](index.html#get-1-actions-idaction)
    * [GET /1/actions/[idAction]/[field]](index.html#get-1-actions-idaction-field)
    * [GET /1/actions/[idAction]/board](index.html#get-1-actions-idaction-board)
    * [GET /1/actions/[idAction]/board/[field]](index.html#get-1-actions-idaction-board-field)
    * [GET /1/actions/[idAction]/card](index.html#get-1-actions-idaction-card)
    * [GET /1/actions/[idAction]/card/[field]](index.html#get-1-actions-idaction-card-field)
    * [GET /1/actions/[idAction]/entities](index.html#get-1-actions-idaction-entities)
    * [GET /1/actions/[idAction]/list](index.html#get-1-actions-idaction-list)
    * [GET /1/actions/[idAction]/list/[field]](index.html#get-1-actions-idaction-list-field)
    * [GET /1/actions/[idAction]/member](index.html#get-1-actions-idaction-member)
    * [GET /1/actions/[idAction]/member/[field]](index.html#get-1-actions-idaction-member-field)
    * [GET /1/actions/[idAction]/memberCreator](index.html#get-1-actions-idaction-membercreator)
    * [GET /1/actions/[idAction]/memberCreator/[field]](index.html#get-1-actions-idaction-membercreator-field)
    * [GET /1/actions/[idAction]/organization](index.html#get-1-actions-idaction-organization)
    * [GET /1/actions/[idAction]/organization/[field]](index.html#get-1-actions-idaction-organization-field)
    * [PUT /1/actions/[idAction]](index.html#put-1-actions-idaction)
    * [PUT /1/actions/[idAction]/text](index.html#put-1-actions-idaction-text)
    * [DELETE /1/actions/[idAction]](index.html#delete-1-actions-idaction)

### Browse

  * Prev: [API Reference (Beta)](../index.html)
  * Next: [board](../board/index.html)

### You are here:

  * [Trello documentation](../../index.html)
    * [API Reference (Beta)](../index.html)
      * action

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.

