# list[¶](index.html.md#list)

## GET /1/lists/[idList][¶](index.html.md#get-1-lists-idlist)

  * **Required permissions:** read
  * **Arguments**
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
    * `fields` (optional)
      * **Default:** `name,closed,idBoard,pos`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`
  * **Examples**
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a?fields=name&cards=open&card_fields=name&key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "id": "4eea4ffc91e31d174600004a",
        "name": "To Do Soon",
        "cards": [{
            "id": "4eea503791e31d1746000080",
            "name": "Finish my awesome application"
        }]
    }
```

## GET /1/lists/[idList]/[field][¶](index.html.md#get-1-lists-idlist-field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`
  * **Examples**
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/idBoard?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "4eea4ffc91e31d1746000046"
    }
```
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/pos?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": 16384
    }
```
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/closed?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": false
    }
```
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/name?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "To Do Soon"
    }
```
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/subscribed?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```

## GET /1/lists/[idList]/actions[¶](index.html.md#get-1-lists-idlist-actions)

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
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/actions?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4efe314cc72846af4e00008a",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "list": {
                "id": "4eea4ffc91e31d174600004a",
                "name": "To Do Soon"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "old": {
                "name": "To Do Later"
            }
        },
        "type": "updateList",
        "date": "2011-12-30T21:46:52.874Z",
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }, {
        "id": "4efe3147c72846af4e00006d",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "list": {
                "id": "4eea4ffc91e31d174600004a",
                "name": "To Do Later"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "old": {
                "name": "To Do Eventually"
            }
        },
        "type": "updateList",
        "date": "2011-12-30T21:46:47.843Z",
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }]
```

## GET /1/lists/[idList]/board[¶](index.html.md#get-1-lists-idlist-board)

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

## GET /1/lists/[idList]/board/[field][¶](index.html.md#get-1-lists-idlist-board-field)

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

## GET /1/lists/[idList]/cards[¶](index.html.md#get-1-lists-idlist-cards)

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
      * **Default:** `open`
      * **Valid Values:** One of:
        * `none`
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
  * **Examples**
    
    https://api.trello.com/1/lists/4eea4ffc91e31d174600004a/cards?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea503791e31d1746000080",
        "checkItemStates": [],
        "closed": false,
        "dateLastActivity": "2011-12-15T19:53:27.228Z",
        "desc": "",
        "descData": null,
        "idBoard": "4eea4ffc91e31d1746000046",
        "idList": "4eea4ffc91e31d174600004a",
        "idMembersVoted": [],
        "idShort": 3,
        "idAttachmentCover": null,
        "manualCoverAttachment": false,
        "name": "Finish my awesome application",
        "pos": 65536,
        "shortLink": "XlG8S7ll",
        "badges": {
            "votes": 0,
            "viewingMemberVoted": false,
            "subscribed": false,
            "fogbugz": "",
            "checkItems": 0,
            "checkItemsChecked": 0,
            "comments": 0,
            "attachments": 0,
            "description": false,
            "due": null
        },
        "due": null,
        "idChecklists": [],
        "idMembers": [],
        "labels": [],
        "shortUrl": "https://trello.com/c/XlG8S7ll",
        "subscribed": false,
        "url": "https://trello.com/c/XlG8S7ll/3-finish-my-awesome-application"
    }]
```

## GET /1/lists/[idList]/cards/[filter][¶](index.html.md#get-1-lists-idlist-cards-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`

## PUT /1/lists/[idList][¶](index.html.md#put-1-lists-idlist)

  * **Required permissions:** read
  * **Arguments**
    * `name` (optional)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `closed` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `idBoard` (optional)
      * **Valid Values:** id of the board the list should be moved to
    * `pos` (optional)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.
    * `subscribed` (optional)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/lists/[idList]/closed[¶](index.html.md#put-1-lists-idlist-closed)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/lists/[idList]/idBoard[¶](index.html.md#put-1-lists-idlist-idboard)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** id of the board the list should be moved to
    * `pos` (optional)
      * **Default:** `top`
      * **Valid Values:** position of the list on the new board

## PUT /1/lists/[idList]/name[¶](index.html.md#put-1-lists-idlist-name)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/lists/[idList]/pos[¶](index.html.md#put-1-lists-idlist-pos)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/lists/[idList]/subscribed[¶](index.html.md#put-1-lists-idlist-subscribed)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## POST /1/lists[¶](index.html.md#post-1-lists)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `idBoard` (required)
      * **Valid Values:** id of the board that the list should be added to
    * `idListSource` (optional)
      * **Valid Values:** The id of the list to copy into a new list.
    * `pos` (optional)
      * **Default:** `top`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## POST /1/lists/[idList]/archiveAllCards[¶](index.html.md#post-1-lists-idlist-archiveallcards)

  * **Required permissions:** write
  * **Arguments:** None

## POST /1/lists/[idList]/cards[¶](index.html.md#post-1-lists-idlist-cards)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labels` (optional)
    * `idMembers` (optional)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `due` (required)
      * **Valid Values:** A date, or `null`

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
