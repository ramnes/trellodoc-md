# checklist[¶](index.html.md#checklist)

## GET /1/checklists/[idChecklist][¶](index.html.md#get-1-checklists-idchecklist)

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
    * `checkItems` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `checkItem_fields` (optional)
      * **Default:** `name,nameData,pos,state`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `nameData`
        * `type`
        * `pos`
        * `state`
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `idBoard`
        * `idCard`
        * `pos`
  * **Examples**
    
    https://api.trello.com/1/checklists/4eea6ae1a5da7f5a49000092?fields=name&cards=all&card_fields=name&key=[application_key]&token=[optional_auth_token]

```json
    {
        "id": "4eea6ae1a5da7f5a49000092",
        "name": "API Checklist",
        "checkItems": [{
            "state": "complete",
            "id": "4eea6aeda5da7f5a490000b9",
            "name": "See if there is a call",
            "nameData": null,
            "pos": 16751
        }, {
            "state": "incomplete",
            "id": "4eea6af1a5da7f5a490000cc",
            "name": "Figure out how to use the call",
            "nameData": null,
            "pos": 33544
        }, {
            "state": "incomplete",
            "id": "4eea6af4a5da7f5a490000e1",
            "name": "Add it to the code",
            "nameData": null,
            "pos": 50647
        }],
        "cards": [{
            "id": "4eea522c91e31d174600027e",
            "name": "Figure out how to read a user's board list"
        }]
    }
```

## GET /1/checklists/[idChecklist]/[field][¶](index.html.md#get-1-checklists-idchecklist-field)

  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `idBoard`
        * `idCard`
        * `pos`

## GET /1/checklists/[idChecklist]/board[¶](index.html.md#get-1-checklists-idchecklist-board)

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

## GET /1/checklists/[idChecklist]/board/[field][¶](index.html.md#get-1-checklists-idchecklist-board-field)

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

## GET /1/checklists/[idChecklist]/cards[¶](index.html.md#get-1-checklists-idchecklist-cards)

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

## GET /1/checklists/[idChecklist]/cards/[filter][¶](index.html.md#get-1-checklists-idchecklist-cards-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`

## GET /1/checklists/[idChecklist]/checkItems[¶](index.html.md#get-1-checklists-idchecklist-checkitems)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `fields` (optional)
      * **Default:** `name,nameData,pos,state`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `nameData`
        * `type`
        * `pos`
        * `state`
  * **Examples**
    
    https://api.trello.com/1/checklists/4eea6ae1a5da7f5a49000092/checkItems?key=[application_key]&token=[optional_auth_token]

```json    
    [{
        "state": "complete",
        "id": "4eea6aeda5da7f5a490000b9",
        "name": "See if there is a call",
        "nameData": null,
        "pos": 16751
    }, {
        "state": "incomplete",
        "id": "4eea6af1a5da7f5a490000cc",
        "name": "Figure out how to use the call",
        "nameData": null,
        "pos": 33544
    }, {
        "state": "incomplete",
        "id": "4eea6af4a5da7f5a490000e1",
        "name": "Add it to the code",
        "nameData": null,
        "pos": 50647
    }]
```

## GET /1/checklists/[idChecklist]/checkItems/[idCheckItem][¶](index.html.md#get-1-checklists-idchecklist-checkitems-idcheckitem)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `name,nameData,pos,state`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `nameData`
        * `type`
        * `pos`
        * `state`
    * `idCheckItem` (required)
      * **Valid Values:** id of the checkitem to retrieve

## PUT /1/checklists/[idChecklist][¶](index.html.md#put-1-checklists-idchecklist)

  * **Required permissions:** read
  * **Arguments**
    * `name` (optional)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `idCard` (optional)
      * **Valid Values:** The id of the card that the checklist is on
    * `pos` (optional)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/checklists/[idChecklist]/idCard[¶](index.html.md#put-1-checklists-idchecklist-idcard)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** The id of the card that the checklist is on

## PUT /1/checklists/[idChecklist]/name[¶](index.html.md#put-1-checklists-idchecklist-name)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/checklists/[idChecklist]/pos[¶](index.html.md#put-1-checklists-idchecklist-pos)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## POST /1/checklists[¶](index.html.md#post-1-checklists)

  * **Required permissions:** write
  * **Arguments**
    * `name` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `idBoard` (optional)
      * **Valid Values:** id of the board that the checklist should be added to
    * `idCard` (optional)
      * **Valid Values:** id of the card that the checklist should be added to
    * `pos` (optional)
      * **Default:** `bottom`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.
    * `idChecklistSource` (optional)
      * **Valid Values:** The id of the source checklist to copy into a new checklist.

## POST /1/checklists/[idChecklist]/checkItems[¶](index.html.md#post-1-checklists-idchecklist-checkitems)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `pos` (optional)
      * **Default:** `bottom`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.
    * `checked` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`

## DELETE /1/checklists/[idChecklist][¶](index.html.md#delete-1-checklists-idchecklist)

  * **Required permissions:** write
  * **Arguments:** None

## DELETE /1/checklists/[idChecklist]/checkItems/[idCheckItem][¶](index.html.md#delete-1-checklists-idchecklist-checkitems-idcheckitem)

  * **Required permissions:** write
  * **Arguments**
    * `idCheckItem` (required)
      * **Valid Values:** the id of the check item to remove

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
