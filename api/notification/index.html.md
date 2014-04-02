# notification[¶](index.html.md#notification)

## GET /1/notifications/[idNotification][¶](index.html.md#get-1-notifications-idnotification)

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
        * `unread`
        * `type`
        * `date`
        * `data`
        * `idMemberCreator`
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
    * `board` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `board_fields` (optional)
      * **Default:** `name`
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
    * `list` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_fields` (optional)
      * **Default:** `name`
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
    * `organization` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `organization_fields` (optional)
      * **Default:** `displayName`
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

## GET /1/notifications/[idNotification]/[field][¶](index.html.md#get-1-notifications-idnotification-field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `unread`
        * `type`
        * `date`
        * `data`
        * `idMemberCreator`

## GET /1/notifications/[idNotification]/board[¶](index.html.md#get-1-notifications-idnotification-board)

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

## GET /1/notifications/[idNotification]/board/[field][¶](index.html.md#get-1-notifications-idnotification-board-field)

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

## GET /1/notifications/[idNotification]/card[¶](index.html.md#get-1-notifications-idnotification-card)

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

## GET /1/notifications/[idNotification]/card/[field][¶](index.html.md#get-1-notifications-idnotification-card-field)

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

## GET /1/notifications/[idNotification]/entities[¶](index.html.md#get-1-notifications-idnotification-entities)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/notifications/[idNotification]/list[¶](index.html.md#get-1-notifications-idnotification-list)

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

## GET /1/notifications/[idNotification]/list/[field][¶](index.html.md#get-1-notifications-idnotification-list-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`

## GET /1/notifications/[idNotification]/member[¶](index.html.md#get-1-notifications-idnotification-member)

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

## GET /1/notifications/[idNotification]/member/[field][¶](index.html.md#get-1-notifications-idnotification-member-field)

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

## GET /1/notifications/[idNotification]/memberCreator[¶](index.html.md#get-1-notifications-idnotification-membercreator)

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

## GET /1/notifications/[idNotification]/memberCreator/[field][¶](index.html.md#get-1-notifications-idnotification-membercreator-field)

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

## GET /1/notifications/[idNotification]/organization[¶](index.html.md#get-1-notifications-idnotification-organization)

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

## GET /1/notifications/[idNotification]/organization/[field][¶](index.html.md#get-1-notifications-idnotification-organization-field)

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

## PUT /1/notifications/[idNotification][¶](index.html.md#put-1-notifications-idnotification)

  * **Required permissions:** read
  * **Arguments**
    * `unread` (optional)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/notifications/[idNotification]/unread[¶](index.html.md#put-1-notifications-idnotification-unread)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## POST /1/notifications/all/read[¶](index.html.md#post-1-notifications-all-read)

  * **Required permissions:** write
  * **Arguments:** None

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
