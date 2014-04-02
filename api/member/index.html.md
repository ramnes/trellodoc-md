# member[¶](index.html.md#member)

## GET /1/members/[idMember or username][¶](index.html.md#get-1-members-idmember-or-username)

  * **Notes:** If you specify `me` as the username, this call will respond as if you had supplied the username associated with the supplied token
  * **Required permissions:** read
  * **Arguments**
    * `actions` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addAttachmentToCard`
        * `addChecklistToCard`
        * `addMemberToBoard`
        * `addMemberToCard`
        * `addMemberToOrganization`
        * `addToOrganizationBoard`
        * `commentCard`
        * `copyCommentCard`
        * `convertToCardFromCheckItem`
        * `copyBoard`
        * `createBoard`
        * `createCard`
        * `copyCard`
        * `createList`
        * `createOrganization`
        * `deleteAttachmentFromCard`
        * `deleteBoardInvitation`
        * `deleteCard`
        * `deleteOrganizationInvitation`
        * `disablePowerUp`
        * `emailCard`
        * `enablePowerUp`
        * `makeAdminOfBoard`
        * `makeNormalMemberOfBoard`
        * `makeNormalMemberOfOrganization`
        * `makeObserverOfBoard`
        * `memberJoinedTrello`
        * `moveCardFromBoard`
        * `moveListFromBoard`
        * `moveCardToBoard`
        * `moveListToBoard`
        * `removeAdminFromBoard`
        * `removeAdminFromOrganization`
        * `removeChecklistFromCard`
        * `removeFromOrganizationBoard`
        * `removeMemberFromCard`
        * `unconfirmedBoardInvitation`
        * `unconfirmedOrganizationInvitation`
        * `updateBoard`
        * `updateCard`
        * `updateCheckItemStateOnCard`
        * `updateChecklist`
        * `updateList`
        * `updateMember`
        * `updateOrganization`
        * `updateCard:idList`
        * `updateCard:closed`
        * `updateCard:desc`
        * `updateCard:name`
        * `updateList:closed`
        * `updateList:name`
    * `actions_entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `actions_limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `0` to `1000`
    * `action_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `action_since` (optional)
      * **Valid Values:** A date, `null` or `lastView`
    * `action_before` (optional)
      * **Valid Values:** A date, or `null`
    * `cards` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `visible`
        * `open`
        * `closed`
        * `all`
    * `card_fields` (optional)
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
    * `card_members` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_member_fields` (optional)
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
    * `card_attachments` (optional)
      * **Default:** `false`
      * **Valid Values:** A boolean value or &quot;cover&quot; for only card cover attachments
    * `card_attachment_fields` (optional)
      * **Default:** `url,previews`
      * **Valid Values:** `all` or a comma-separated list of:
        * `bytes`
        * `date`
        * `edgeColor`
        * `idMember`
        * `isUpload`
        * `mimeType`
        * `name`
        * `previews`
        * `url`
    * `card_stickers` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `boards` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `members`
        * `organization`
        * `public`
        * `open`
        * `closed`
        * `pinned`
        * `unpinned`
        * `starred`
    * `board_fields` (optional)
      * **Default:** `name,closed,idOrganization,pinned`
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
    * `board_actions` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addAttachmentToCard`
        * `addChecklistToCard`
        * `addMemberToBoard`
        * `addMemberToCard`
        * `addMemberToOrganization`
        * `addToOrganizationBoard`
        * `commentCard`
        * `copyCommentCard`
        * `convertToCardFromCheckItem`
        * `copyBoard`
        * `createBoard`
        * `createCard`
        * `copyCard`
        * `createList`
        * `createOrganization`
        * `deleteAttachmentFromCard`
        * `deleteBoardInvitation`
        * `deleteCard`
        * `deleteOrganizationInvitation`
        * `disablePowerUp`
        * `emailCard`
        * `enablePowerUp`
        * `makeAdminOfBoard`
        * `makeNormalMemberOfBoard`
        * `makeNormalMemberOfOrganization`
        * `makeObserverOfBoard`
        * `memberJoinedTrello`
        * `moveCardFromBoard`
        * `moveListFromBoard`
        * `moveCardToBoard`
        * `moveListToBoard`
        * `removeAdminFromBoard`
        * `removeAdminFromOrganization`
        * `removeChecklistFromCard`
        * `removeFromOrganizationBoard`
        * `removeMemberFromCard`
        * `unconfirmedBoardInvitation`
        * `unconfirmedOrganizationInvitation`
        * `updateBoard`
        * `updateCard`
        * `updateCheckItemStateOnCard`
        * `updateChecklist`
        * `updateList`
        * `updateMember`
        * `updateOrganization`
        * `updateCard:idList`
        * `updateCard:closed`
        * `updateCard:desc`
        * `updateCard:name`
        * `updateList:closed`
        * `updateList:name`
    * `board_actions_entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `board_actions_format` (optional)
      * **Default:** `list`
      * **Valid Values:** One of:
        * `count`
        * `list`
        * `minimal`
    * `board_actions_since` (optional)
      * **Valid Values:** A date, `null` or `lastView`
    * `board_actions_limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `0` to `1000`
    * `board_action_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `board_lists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`
    * `board_memberships` (optional)
      * **Default:** `none`
      * **Valid Values:** `all` or a comma-separated list of:
        * `me`
        * `normal`
        * `admin`
        * `active`
        * `deactivated`
    * `board_organization` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `board_organization_fields` (optional)
      * **Default:** `name,displayName`
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
    * `boardsInvited` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `members`
        * `organization`
        * `public`
        * `open`
        * `closed`
        * `pinned`
        * `unpinned`
        * `starred`
    * `boardsInvited_fields` (optional)
      * **Default:** `name,closed,idOrganization,pinned`
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
    * `boardStars` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `organizations` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `members`
        * `public`
        * `all`
    * `organization_fields` (optional)
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
    * `organization_paid_account` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `organizationsInvited` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `members`
        * `public`
        * `all`
    * `organizationsInvited_fields` (optional)
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
    * `notifications` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addedAttachmentToCard`
        * `addedToBoard`
        * `addedToCard`
        * `addedToOrganization`
        * `addedMemberToCard`
        * `addAdminToBoard`
        * `addAdminToOrganization`
        * `cardDueSoon`
        * `changeCard`
        * `closeBoard`
        * `commentCard`
        * `createdCard`
        * `invitedToBoard`
        * `invitedToOrganization`
        * `removedFromBoard`
        * `removedFromCard`
        * `removedMemberFromCard`
        * `removedFromOrganization`
        * `mentionedOnCard`
        * `unconfirmedInvitedToBoard`
        * `unconfirmedInvitedToOrganization`
        * `updateCheckItemStateOnCard`
        * `makeAdminOfBoard`
        * `makeAdminOfOrganization`
        * `declinedInvitationToBoard`
        * `declinedInvitationToOrganization`
        * `memberJoinedTrello`
    * `notifications_entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `notifications_limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `1` to `1000`
    * `notification_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `unread`
        * `type`
        * `date`
        * `data`
        * `idMemberCreator`
    * `notification_memberCreator` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `notification_memberCreator_fields` (optional)
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
    * `notification_before` (optional)
      * **Valid Values:** An id, or `null`
    * `notification_since` (optional)
      * **Valid Values:** An id, or `null`
    * `tokens` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `paid_account` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `boardBackgrounds` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `default`
        * `premium`
        * `custom`
        * `all`
    * `customBoardBackgrounds` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `customStickers` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `customEmoji` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
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
  * **Examples**
    
    https://api.trello.com/1/members/bobtester?fields=username,fullName,url&boards=all&board_fields=name&organizations=all&organization_fields=displayName&key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "id": "4ee7df1be582acdec80000ae",
        "username": "bobtester",
        "fullName": "Bob Tester",
        "url": "https://trello.com/bobtester",
        "organizations": [],
        "boards": [{
            "name": "Example Board",
            "id": "4eea4ffc91e31d1746000046"
        }, {
            "name": "Public Board",
            "id": "4ee7e707e582acdec800051a"
        }]
    }
```

## GET /1/members/[idMember or username]/[field][¶](index.html.md#get-1-members-idmember-or-username-field)

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

## GET /1/members/[idMember or username]/actions[¶](index.html.md#get-1-members-idmember-or-username-actions)

  * **Required permissions:** read
  * **Arguments**
    * `entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `addAttachmentToCard`
        * `addChecklistToCard`
        * `addMemberToBoard`
        * `addMemberToCard`
        * `addMemberToOrganization`
        * `addToOrganizationBoard`
        * `commentCard`
        * `copyCommentCard`
        * `convertToCardFromCheckItem`
        * `copyBoard`
        * `createBoard`
        * `createCard`
        * `copyCard`
        * `createList`
        * `createOrganization`
        * `deleteAttachmentFromCard`
        * `deleteBoardInvitation`
        * `deleteCard`
        * `deleteOrganizationInvitation`
        * `disablePowerUp`
        * `emailCard`
        * `enablePowerUp`
        * `makeAdminOfBoard`
        * `makeNormalMemberOfBoard`
        * `makeNormalMemberOfOrganization`
        * `makeObserverOfBoard`
        * `memberJoinedTrello`
        * `moveCardFromBoard`
        * `moveListFromBoard`
        * `moveCardToBoard`
        * `moveListToBoard`
        * `removeAdminFromBoard`
        * `removeAdminFromOrganization`
        * `removeChecklistFromCard`
        * `removeFromOrganizationBoard`
        * `removeMemberFromCard`
        * `unconfirmedBoardInvitation`
        * `unconfirmedOrganizationInvitation`
        * `updateBoard`
        * `updateCard`
        * `updateCheckItemStateOnCard`
        * `updateChecklist`
        * `updateList`
        * `updateMember`
        * `updateOrganization`
        * `updateCard:idList`
        * `updateCard:closed`
        * `updateCard:desc`
        * `updateCard:name`
        * `updateList:closed`
        * `updateList:name`
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `0` to `1000`
    * `format` (optional)
      * **Default:** `list`
      * **Valid Values:** One of:
        * `count`
        * `list`
        * `minimal`
    * `since` (optional)
      * **Valid Values:** A date, `null` or `lastView`
    * `before` (optional)
      * **Valid Values:** A date, or `null`
    * `page` (optional)
      * **Default:** `0`
      * **Valid Values:** Page * limit must be less than 1000
    * `idModels` (optional)
      * **Valid Values:** Only return actions related to these model ids
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
  * **Examples**
    
    https://api.trello.com/1/members/bobtester/actions?limit=3&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4f9aff63b7ecafcb4a0007dd",
        "idMemberCreator": "4ee7df1be582acdec80000ae",
        "data": {
            "board": {
                "name": "Public Board",
                "id": "4ee7e707e582acdec800051a"
            },
            "old": {
                "desc": "A board that everyone can see"
            }
        },
        "type": "updateBoard",
        "date": "2012-04-27T20:19:47.471Z",
        "memberCreator": {
            "id": "4ee7df1be582acdec80000ae",
            "avatarHash": null,
            "fullName": "Bob Tester",
            "initials": "BT",
            "username": "bobtester"
        }
    }, {
        "id": "4f9aff63b7ecafcb4a00076f",
        "idMemberCreator": "4ee7df1be582acdec80000ae",
        "data": {
            "board": {
                "name": "Public Board",
                "id": "4ee7e707e582acdec800051a"
            },
            "old": {
                "desc": "A board that everyone can see"
            }
        },
        "type": "updateBoard",
        "date": "2012-04-27T20:19:47.311Z",
        "memberCreator": {
            "id": "4ee7df1be582acdec80000ae",
            "avatarHash": null,
            "fullName": "Bob Tester",
            "initials": "BT",
            "username": "bobtester"
        }
    }, {
        "id": "4f8d7434093deff913000317",
        "idMemberCreator": "4ee7df1be582acdec80000ae",
        "data": {
            "board": {
                "name": "Public Board",
                "id": "4ee7e707e582acdec800051a"
            },
            "old": {
                "closed": false
            }
        },
        "type": "updateBoard",
        "date": "2012-04-17T13:46:28.680Z",
        "memberCreator": {
            "id": "4ee7df1be582acdec80000ae",
            "avatarHash": null,
            "fullName": "Bob Tester",
            "initials": "BT",
            "username": "bobtester"
        }
    }]
```

## GET /1/members/[idMember or username]/boardBackgrounds[¶](index.html.md#get-1-members-idmember-or-username-boardbackgrounds)

  * **Required permissions:** read, own
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `default`
        * `premium`
        * `custom`
        * `all`

## GET /1/members/[idMember or username]/boardBackgrounds/[idBoardBackground][¶](index.html.md#get-1-members-idmember-or-username-boardbackgrounds-idboardbackground)

  * **Required permissions:** read, own, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** An id
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `brightness`
        * `fullSizeUrl`
        * `scaled`
        * `tile`

## GET /1/members/[idMember or username]/boardStars[¶](index.html.md#get-1-members-idmember-or-username-boardstars)

  * **Required permissions:** read, own
  * **Arguments:** None

## GET /1/members/[idMember or username]/boards[¶](index.html.md#get-1-members-idmember-or-username-boards)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `members`
        * `organization`
        * `public`
        * `open`
        * `closed`
        * `pinned`
        * `unpinned`
        * `starred`
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
    * `actions` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addAttachmentToCard`
        * `addChecklistToCard`
        * `addMemberToBoard`
        * `addMemberToCard`
        * `addMemberToOrganization`
        * `addToOrganizationBoard`
        * `commentCard`
        * `copyCommentCard`
        * `convertToCardFromCheckItem`
        * `copyBoard`
        * `createBoard`
        * `createCard`
        * `copyCard`
        * `createList`
        * `createOrganization`
        * `deleteAttachmentFromCard`
        * `deleteBoardInvitation`
        * `deleteCard`
        * `deleteOrganizationInvitation`
        * `disablePowerUp`
        * `emailCard`
        * `enablePowerUp`
        * `makeAdminOfBoard`
        * `makeNormalMemberOfBoard`
        * `makeNormalMemberOfOrganization`
        * `makeObserverOfBoard`
        * `memberJoinedTrello`
        * `moveCardFromBoard`
        * `moveListFromBoard`
        * `moveCardToBoard`
        * `moveListToBoard`
        * `removeAdminFromBoard`
        * `removeAdminFromOrganization`
        * `removeChecklistFromCard`
        * `removeFromOrganizationBoard`
        * `removeMemberFromCard`
        * `unconfirmedBoardInvitation`
        * `unconfirmedOrganizationInvitation`
        * `updateBoard`
        * `updateCard`
        * `updateCheckItemStateOnCard`
        * `updateChecklist`
        * `updateList`
        * `updateMember`
        * `updateOrganization`
        * `updateCard:idList`
        * `updateCard:closed`
        * `updateCard:desc`
        * `updateCard:name`
        * `updateList:closed`
        * `updateList:name`
    * `actions_entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `actions_limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `0` to `1000`
    * `actions_format` (optional)
      * **Default:** `list`
      * **Valid Values:** One of:
        * `count`
        * `list`
        * `minimal`
    * `actions_since` (optional)
      * **Valid Values:** A date, `null` or `lastView`
    * `action_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `memberships` (optional)
      * **Default:** `none`
      * **Valid Values:** `all` or a comma-separated list of:
        * `me`
        * `normal`
        * `admin`
        * `active`
        * `deactivated`
    * `organization` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `organization_fields` (optional)
      * **Default:** `name,displayName`
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
    * `lists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`
  * **Examples**
    
    https://api.trello.com/1/members/bobtester/boards?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea4ffc91e31d1746000046",
        "name": "Example Board",
        "desc": "This board is used in the API examples",
        "descData": null,
        "closed": false,
        "idOrganization": "4efe2c2f2e1efe7a4c0002c9",
        "invited": false,
        "pinned": null,
        "starred": null,
        "url": "https://trello.com/b/OXiBYZoj/example-board",
        "prefs": {
            "permissionLevel": "public",
            "voting": "members",
            "comments": "members",
            "invitations": "members",
            "selfJoin": false,
            "cardCovers": true,
            "background": "blue",
            "backgroundColor": "#23719F",
            "backgroundImage": null,
            "backgroundImageScaled": null,
            "backgroundTile": false,
            "backgroundBrightness": "unknown",
            "canBePublic": true,
            "canBeOrg": true,
            "canBePrivate": true,
            "canInvite": true
        },
        "invitations": [],
        "memberships": [{
            "id": "4eea4ffc91e31d174600004d",
            "idMember": "4ee7deffe582acdec80000ac",
            "memberType": "admin",
            "unconfirmed": false
        }, {
            "id": "4eea507991e31d17460000fc",
            "idMember": "4ee7df1be582acdec80000ae",
            "memberType": "normal",
            "unconfirmed": false
        }, {
            "id": "4eea50bc91e31d174600016d",
            "idMember": "4ee7df74e582acdec80000b6",
            "memberType": "normal",
            "unconfirmed": false
        }],
        "shortLink": "OXiBYZoj",
        "subscribed": null,
        "labelNames": {
            "yellow": "Low Priority",
            "red": "High Priority",
            "purple": "",
            "orange": "Medium Priority",
            "green": "",
            "blue": ""
        },
        "powerUps": [],
        "dateLastActivity": null,
        "dateLastView": null,
        "shortUrl": "https://trello.com/b/OXiBYZoj"
    }, {
        "id": "4ee7e707e582acdec800051a",
        "name": "Public Board",
        "desc": "A board that everyone can see",
        "descData": null,
        "closed": false,
        "idOrganization": "",
        "invited": false,
        "pinned": null,
        "starred": null,
        "url": "https://trello.com/b/IwLRbh3F/public-board",
        "prefs": {
            "permissionLevel": "public",
            "voting": "public",
            "comments": "public",
            "invitations": "members",
            "selfJoin": false,
            "cardCovers": true,
            "background": "blue",
            "backgroundColor": "#23719F",
            "backgroundImage": null,
            "backgroundImageScaled": null,
            "backgroundTile": false,
            "backgroundBrightness": "unknown",
            "canBePublic": true,
            "canBeOrg": true,
            "canBePrivate": true,
            "canInvite": true
        },
        "invitations": [],
        "memberships": [{
            "id": "4ee7e707e582acdec8000521",
            "idMember": "4ee7df3ce582acdec80000b2",
            "memberType": "admin",
            "unconfirmed": false
        }, {
            "id": "4ee7e72fe582acdec8000573",
            "idMember": "4ee7df1be582acdec80000ae",
            "memberType": "normal",
            "unconfirmed": false
        }, {
            "id": "514c5f9cb569140000000016",
            "idMember": "514c5f9cb569140000000014",
            "memberType": "normal",
            "unconfirmed": false
        }],
        "shortLink": "IwLRbh3F",
        "subscribed": null,
        "labelNames": {
            "yellow": "",
            "red": "Bug",
            "purple": "Blocked",
            "orange": "",
            "green": "Working On",
            "blue": ""
        },
        "powerUps": [],
        "dateLastActivity": null,
        "dateLastView": null,
        "shortUrl": "https://trello.com/b/IwLRbh3F"
    }]
```

## GET /1/members/[idMember or username]/boards/[filter][¶](index.html.md#get-1-members-idmember-or-username-boards-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** `all` or a comma-separated list of:
        * `members`
        * `organization`
        * `public`
        * `open`
        * `closed`
        * `pinned`
        * `unpinned`
        * `starred`

## GET /1/members/[idMember or username]/boardsInvited[¶](index.html.md#get-1-members-idmember-or-username-boardsinvited)

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

## GET /1/members/[idMember or username]/boardsInvited/[field][¶](index.html.md#get-1-members-idmember-or-username-boardsinvited-field)

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

## GET /1/members/[idMember or username]/cards[¶](index.html.md#get-1-members-idmember-or-username-cards)

  * **Required permissions:** read
  * **Arguments**
    * `actions` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addAttachmentToCard`
        * `addChecklistToCard`
        * `addMemberToBoard`
        * `addMemberToCard`
        * `addMemberToOrganization`
        * `addToOrganizationBoard`
        * `commentCard`
        * `copyCommentCard`
        * `convertToCardFromCheckItem`
        * `copyBoard`
        * `createBoard`
        * `createCard`
        * `copyCard`
        * `createList`
        * `createOrganization`
        * `deleteAttachmentFromCard`
        * `deleteBoardInvitation`
        * `deleteCard`
        * `deleteOrganizationInvitation`
        * `disablePowerUp`
        * `emailCard`
        * `enablePowerUp`
        * `makeAdminOfBoard`
        * `makeNormalMemberOfBoard`
        * `makeNormalMemberOfOrganization`
        * `makeObserverOfBoard`
        * `memberJoinedTrello`
        * `moveCardFromBoard`
        * `moveListFromBoard`
        * `moveCardToBoard`
        * `moveListToBoard`
        * `removeAdminFromBoard`
        * `removeAdminFromOrganization`
        * `removeChecklistFromCard`
        * `removeFromOrganizationBoard`
        * `removeMemberFromCard`
        * `unconfirmedBoardInvitation`
        * `unconfirmedOrganizationInvitation`
        * `updateBoard`
        * `updateCard`
        * `updateCheckItemStateOnCard`
        * `updateChecklist`
        * `updateList`
        * `updateMember`
        * `updateOrganization`
        * `updateCard:idList`
        * `updateCard:closed`
        * `updateCard:desc`
        * `updateCard:name`
        * `updateList:closed`
        * `updateList:name`
    * `attachments` (optional)
      * **Default:** `false`
      * **Valid Values:** A boolean value or &quot;cover&quot; for only card cover attachments
    * `attachment_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `bytes`
        * `date`
        * `edgeColor`
        * `idMember`
        * `isUpload`
        * `mimeType`
        * `name`
        * `previews`
        * `url`
    * `stickers` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `members` (optional)
      * **Default:** `false`
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
    * `checkItemStates` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `checklists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `limit` (optional)
      * **Valid Values:** a number from `1` to `1000`
    * `since` (optional)
      * **Valid Values:** A date, or `null`
    * `before` (optional)
      * **Valid Values:** A date, or `null`
    * `filter` (optional)
      * **Default:** `visible`
      * **Valid Values:** One of:
        * `none`
        * `visible`
        * `open`
        * `closed`
        * `all`
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

## GET /1/members/[idMember or username]/cards/[filter][¶](index.html.md#get-1-members-idmember-or-username-cards-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `visible`
        * `open`
        * `closed`
        * `all`

## GET /1/members/[idMember or username]/customBoardBackgrounds[¶](index.html.md#get-1-members-idmember-or-username-customboardbackgrounds)

  * **Required permissions:** read, own, customBoardBackgrounds
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`

## GET /1/members/[idMember or username]/customBoardBackgrounds/[idBoardBackground][¶](index.html.md#get-1-members-idmember-or-username-customboardbackgrounds-idboardbackground)

  * **Required permissions:** read, own, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** An id
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `brightness`
        * `fullSizeUrl`
        * `scaled`
        * `tile`

## GET /1/members/[idMember or username]/customEmoji[¶](index.html.md#get-1-members-idmember-or-username-customemoji)

  * **Notes:** This gets the list of all of the user's uploaded emoji
  * **Required permissions:** read, own, customEmoji
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`

## GET /1/members/[idMember or username]/customEmoji/[idCustomEmoji][¶](index.html.md#get-1-members-idmember-or-username-customemoji-idcustomemoji)

  * **Required permissions:** read, own, customEmoji
  * **Arguments**
    * `idCustomEmoji` (required)
      * **Valid Values:** An id
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `url`
        * `name`

## GET /1/members/[idMember or username]/customStickers[¶](index.html.md#get-1-members-idmember-or-username-customstickers)

  * **Notes:** This gets a list of all of the user's uploaded stickers
  * **Required permissions:** read, own, customStickers
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`

## GET /1/members/[idMember or username]/customStickers/[idCustomSticker][¶](index.html.md#get-1-members-idmember-or-username-customstickers-idcustomsticker)

  * **Required permissions:** read, own, customStickers
  * **Arguments**
    * `idCustomSticker` (required)
      * **Valid Values:** An id
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `url`
        * `scaled`

## GET /1/members/[idMember or username]/notifications[¶](index.html.md#get-1-members-idmember-or-username-notifications)

  * **Notes:** You can only read the notifications for the member associated with the supplied token
  * **Required permissions:** read, own
  * **Arguments**
    * `entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `filter` (optional)
      * **Default:** `addedAttachmentToCard,addedToBoard,addedToCard,addedToOrganization,addedMemberToCard,addAdminToBoard,addAdminToOrganization,cardDueSoon,changeCard,closeBoard,commentCard,createdCard,invitedToBoard,invitedToOrganization,removedFromBoard,removedFromCard,removedMemberFromCard,removedFromOrganization,mentionedOnCard,unconfirmedInvitedToBoard,unconfirmedInvitedToOrganization,updateCheckItemStateOnCard,makeAdminOfBoard,makeAdminOfOrganization`
      * **Valid Values:** `all` or a comma-separated list of:
        * `addedAttachmentToCard`
        * `addedToBoard`
        * `addedToCard`
        * `addedToOrganization`
        * `addedMemberToCard`
        * `addAdminToBoard`
        * `addAdminToOrganization`
        * `cardDueSoon`
        * `changeCard`
        * `closeBoard`
        * `commentCard`
        * `createdCard`
        * `invitedToBoard`
        * `invitedToOrganization`
        * `removedFromBoard`
        * `removedFromCard`
        * `removedMemberFromCard`
        * `removedFromOrganization`
        * `mentionedOnCard`
        * `unconfirmedInvitedToBoard`
        * `unconfirmedInvitedToOrganization`
        * `updateCheckItemStateOnCard`
        * `makeAdminOfBoard`
        * `makeAdminOfOrganization`
        * `declinedInvitationToBoard`
        * `declinedInvitationToOrganization`
        * `memberJoinedTrello`
    * `read_filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `read`
        * `unread`
        * `all`
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `unread`
        * `type`
        * `date`
        * `data`
        * `idMemberCreator`
    * `limit` (optional)
      * **Default:** `50`
      * **Valid Values:** a number from `1` to `1000`
    * `page` (optional)
      * **Default:** `0`
      * **Valid Values:** a number from `0` to `100`
    * `before` (optional)
      * **Valid Values:** An id, or `null`
    * `since` (optional)
      * **Valid Values:** An id, or `null`
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

## GET /1/members/[idMember or username]/notifications/[filter][¶](index.html.md#get-1-members-idmember-or-username-notifications-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** `all` or a comma-separated list of:
        * `addedAttachmentToCard`
        * `addedToBoard`
        * `addedToCard`
        * `addedToOrganization`
        * `addedMemberToCard`
        * `addAdminToBoard`
        * `addAdminToOrganization`
        * `cardDueSoon`
        * `changeCard`
        * `closeBoard`
        * `commentCard`
        * `createdCard`
        * `invitedToBoard`
        * `invitedToOrganization`
        * `removedFromBoard`
        * `removedFromCard`
        * `removedMemberFromCard`
        * `removedFromOrganization`
        * `mentionedOnCard`
        * `unconfirmedInvitedToBoard`
        * `unconfirmedInvitedToOrganization`
        * `updateCheckItemStateOnCard`
        * `makeAdminOfBoard`
        * `makeAdminOfOrganization`
        * `declinedInvitationToBoard`
        * `declinedInvitationToOrganization`
        * `memberJoinedTrello`

## GET /1/members/[idMember or username]/organizations[¶](index.html.md#get-1-members-idmember-or-username-organizations)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `members`
        * `public`
        * `all`
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
    * `paid_account` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
  * **Examples**
    
    https://api.trello.com/1/members/alicetester/organizations?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4ee7e59ae582acdec8000291",
        "name": "publicorg",
        "displayName": "Test Public Organization",
        "desc": "This is a test organization",
        "descData": null,
        "idBoards": [],
        "invited": false,
        "invitations": [],
        "memberships": [{
            "id": "4ee7e59ae582acdec8000295",
            "idMember": "4ee7e2e1e582acdec8000112",
            "memberType": "admin",
            "unconfirmed": false
        }, {
            "id": "4ee7e600e582acdec8000355",
            "idMember": "4ee7df74e582acdec80000b6",
            "memberType": "normal",
            "unconfirmed": false
        }, {
            "id": "4ee7e671e582acdec80003e0",
            "idMember": "4ee7df3ce582acdec80000b2",
            "memberType": "normal",
            "unconfirmed": false
        }, {
            "id": "514c6011b56914000000002a",
            "idMember": "514c6011b569140000000028",
            "memberType": "normal",
            "unconfirmed": false
        }],
        "prefs": {
            "permissionLevel": "public",
            "orgInviteRestrict": null,
            "externalMembersDisabled": false,
            "associatedDomain": null,
            "boardVisibilityRestrict": {
                "private": "org",
                "org": "org",
                "public": "org"
            }
        },
        "powerUps": [],
        "products": [],
        "url": "https://trello.com/publicorg",
        "website": "http://example.com",
        "logoHash": null,
        "premiumFeatures": []
    }]
```

## GET /1/members/[idMember or username]/organizations/[filter][¶](index.html.md#get-1-members-idmember-or-username-organizations-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `members`
        * `public`
        * `all`

## GET /1/members/[idMember or username]/organizationsInvited[¶](index.html.md#get-1-members-idmember-or-username-organizationsinvited)

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

## GET /1/members/[idMember or username]/organizationsInvited/[field][¶](index.html.md#get-1-members-idmember-or-username-organizationsinvited-field)

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

## GET /1/members/[idMember or username]/tokens[¶](index.html.md#get-1-members-idmember-or-username-tokens)

  * **Required permissions:** read, own, account
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`

## PUT /1/members/[idMember or username][¶](index.html.md#put-1-members-idmember-or-username)

  * **Required permissions:** read
  * **Arguments**
    * `fullName` (optional)
      * **Valid Values:** A string with a length of at least 4. Cannot begin or end with a space.
    * `initials` (optional)
      * **Valid Values:** A string with a length from 1 to 4. Cannot begin or end with a space
    * `username` (optional)
      * **Valid Values:** A string with a length of at least 3. Only lowercase letters, underscores, and numbers are allowed. Must be unique.
    * `bio` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `avatarSource` (optional)
      * **Valid Values:** One of:
        * `none`
        * `upload`
        * `gravatar`
    * `prefs/colorBlind` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs/minutesBetweenSummaries` (optional)
      * **Valid Values:** -1 (disabled), 1 or 60

## PUT /1/members/[idMember or username]/avatarSource[¶](index.html.md#put-1-members-idmember-or-username-avatarsource)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `none`
        * `upload`
        * `gravatar`

## PUT /1/members/[idMember or username]/bio[¶](index.html.md#put-1-members-idmember-or-username-bio)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/members/[idMember or username]/boardBackgrounds/[idBoardBackground][¶](index.html.md#put-1-members-idmember-or-username-boardbackgrounds-idboardbackground)

  * **Required permissions:** write, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** The id of the background to update
    * `tile` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `brightness` (optional)
      * **Valid Values:** One of:
        * `light`
        * `dark`
        * `unknown`

## PUT /1/members/[idMember or username]/boardStars/[idBoardStar][¶](index.html.md#put-1-members-idmember-or-username-boardstars-idboardstar)

  * **Required permissions:** write, account
  * **Arguments**
    * `idBoardStar` (required)
      * **Valid Values:** The id of the board star to update
    * `pos` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/members/[idMember or username]/customBoardBackgrounds/[idBoardBackground][¶](index.html.md#put-1-members-idmember-or-username-customboardbackgrounds-idboardbackground)

  * **Required permissions:** write, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** The id of the background to update
    * `tile` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `brightness` (optional)
      * **Valid Values:** One of:
        * `light`
        * `dark`
        * `unknown`

## PUT /1/members/[idMember or username]/fullName[¶](index.html.md#put-1-members-idmember-or-username-fullname)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A string with a length of at least 4. Cannot begin or end with a space.

## PUT /1/members/[idMember or username]/initials[¶](index.html.md#put-1-members-idmember-or-username-initials)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A string with a length from 1 to 4. Cannot begin or end with a space

## PUT /1/members/[idMember or username]/prefs/colorBlind[¶](index.html.md#put-1-members-idmember-or-username-prefs-colorblind)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/members/[idMember or username]/prefs/minutesBetweenSummaries[¶](index.html.md#put-1-members-idmember-or-username-prefs-minutesbetweensummaries)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** -1 (disabled), 1 or 60

## PUT /1/members/[idMember or username]/username[¶](index.html.md#put-1-members-idmember-or-username-username)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A string with a length of at least 3. Only lowercase letters, underscores, and numbers are allowed. Must be unique.

## POST /1/members/[idMember or username]/avatar[¶](index.html.md#post-1-members-idmember-or-username-avatar)

  * **Required permissions:** own
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file

## POST /1/members/[idMember or username]/boardBackgrounds[¶](index.html.md#post-1-members-idmember-or-username-boardbackgrounds)

  * **Required permissions:** write, customBoardBackgrounds
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file

## POST /1/members/[idMember or username]/boardStars[¶](index.html.md#post-1-members-idmember-or-username-boardstars)

  * **Required permissions:** write, account, own
  * **Arguments**
    * `idBoard` (required)
      * **Valid Values:** The id of the board to star
    * `pos` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## POST /1/members/[idMember or username]/customBoardBackgrounds[¶](index.html.md#post-1-members-idmember-or-username-customboardbackgrounds)

  * **Required permissions:** write, customBoardBackgrounds
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file

## POST /1/members/[idMember or username]/customEmoji[¶](index.html.md#post-1-members-idmember-or-username-customemoji)

  * **Required permissions:** write, customEmoji
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file
    * `name` (required)
      * **Valid Values:** a string with a length from `2` to `64`

## POST /1/members/[idMember or username]/customStickers[¶](index.html.md#post-1-members-idmember-or-username-customstickers)

  * **Required permissions:** write, customStickers
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file

## POST /1/members/[idMember or username]/idBoardsPinned[¶](index.html.md#post-1-members-idmember-or-username-idboardspinned)

  * **Required permissions:** write, account
  * **Arguments**
    * `value` (required)
      * **Valid Values:** The id of the board to pin

## POST /1/members/[idMember or username]/oneTimeMessagesDismissed[¶](index.html.md#post-1-members-idmember-or-username-onetimemessagesdismissed)

  * **Required permissions:** own, trello.com
  * **Arguments**
    * `value` (required)
      * **Valid Values:** Type of message dismissed

## POST /1/members/[idMember or username]/unpaidAccount[¶](index.html.md#post-1-members-idmember-or-username-unpaidaccount)

  * **Required permissions:** own, write
  * **Arguments**
    * `products` (required)
      * **Valid Values:** An array of product ids

## DELETE /1/members/[idMember or username]/boardBackgrounds/[idBoardBackground][¶](index.html.md#delete-1-members-idmember-or-username-boardbackgrounds-idboardbackground)

  * **Required permissions:** write, own, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** An id

## DELETE /1/members/[idMember or username]/boardStars/[idBoardStar][¶](index.html.md#delete-1-members-idmember-or-username-boardstars-idboardstar)

  * **Required permissions:** write, own, account
  * **Arguments**
    * `idBoardStar` (required)
      * **Valid Values:** The id of the board star to delete

## DELETE /1/members/[idMember or username]/customBoardBackgrounds/[idBoardBackground][¶](index.html.md#delete-1-members-idmember-or-username-customboardbackgrounds-idboardbackground)

  * **Required permissions:** write, own, customBoardBackgrounds
  * **Arguments**
    * `idBoardBackground` (required)
      * **Valid Values:** An id

## DELETE /1/members/[idMember or username]/customStickers/[idCustomSticker][¶](index.html.md#delete-1-members-idmember-or-username-customstickers-idcustomsticker)

  * **Required permissions:** write, own, customStickers
  * **Arguments**
    * `idCustomSticker` (required)
      * **Valid Values:** An id

## DELETE /1/members/[idMember or username]/idBoardsPinned/[idBoard][¶](index.html.md#delete-1-members-idmember-or-username-idboardspinned-idboard)

  * **Required permissions:** write, account
  * **Arguments**
    * `idBoard` (required)
      * **Valid Values:** The id of the board to un-pin

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
