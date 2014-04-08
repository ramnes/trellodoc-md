# card[¶](index.html.md#card)

## GET /1/cards/[card_id or shortlink][¶](index.html.md#get-1-cards-card-id-or-shortlink)

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
    * `action_memberCreator_fields` (optional)
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
    * `membersVoted` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `memberVoted_fields` (optional)
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
    * `checkItemState_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idCheckItem`
        * `state`
    * `checklists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `checklist_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `idBoard`
        * `idCard`
        * `pos`
    * `board` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `board_fields` (optional)
      * **Default:** `name,desc,descData,closed,idOrganization,pinned,url,prefs`
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
    * `list_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`
    * `stickers` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `sticker_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `top`
        * `left`
        * `zIndex`
        * `rotate`
        * `image`
        * `imageUrl`
        * `imageScaled`
    * `fields` (optional)
      * **Default:** `badges,checkItemStates,closed,dateLastActivity,desc,descData,due,idBoard,idChecklists,idList,idMembers,idShort,idAttachmentCover,manualCoverAttachment,labels,name,pos,shortUrl,url`
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
    
    https://api.trello.com/1/cards/4eea503d91e31d174600008f?fields=name,idList&member_fields=fullName&key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "id": "4eea503d91e31d174600008f",
        "name": "Learn about the Trello API",
        "idList": "4eea4ffc91e31d174600004b"
    }
```

## GET /1/cards/[card_id or shortlink]/[field][¶](index.html.md#get-1-cards-card-id-or-shortlink-field)

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

## GET /1/cards/[card_id or shortlink]/actions[¶](index.html.md#get-1-cards-card-id-or-shortlink-actions)

  * **Required permissions:** read
  * **Arguments**
    * `entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `filter` (optional)
      * **Default:** `commentCard,updateCard:idList`
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

## GET /1/cards/[card_id or shortlink]/attachments[¶](index.html.md#get-1-cards-card-id-or-shortlink-attachments)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
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
    * `filter` (optional)
      * **Default:** `true`
      * **Valid Values:** A boolean value or &quot;cover&quot; for only card cover attachments

## GET /1/cards/[card_id or shortlink]/attachments/[attachment_id][¶](index.html.md#get-1-cards-card-id-or-shortlink-attachments-idattachment)

  * **Required permissions:** read
  * **Arguments**
    * `idAttachment` (required)
      * **Valid Values:** The id of the attachment.
    * `fields` (optional)
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

## GET /1/cards/[card_id or shortlink]/board[¶](index.html.md#get-1-cards-card-id-or-shortlink-board)

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

## GET /1/cards/[card_id or shortlink]/board/[field][¶](index.html.md#get-1-cards-card-id-or-shortlink-board-field)

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

## GET /1/cards/[card_id or shortlink]/checkItemStates[¶](index.html.md#get-1-cards-card-id-or-shortlink-checkitemstates)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idCheckItem`
        * `state`

## GET /1/cards/[card_id or shortlink]/checklists[¶](index.html.md#get-1-cards-card-id-or-shortlink-checklists)

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
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `idBoard`
        * `idCard`
        * `pos`

## GET /1/cards/[card_id or shortlink]/list[¶](index.html.md#get-1-cards-card-id-or-shortlink-list)

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

## GET /1/cards/[card_id or shortlink]/list/[field][¶](index.html.md#get-1-cards-card-id-or-shortlink-list-field)

  * **Required permissions:** read
  * **Arguments**
    * `field` (required)
      * **Valid Values:** One of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`

## GET /1/cards/[card_id or shortlink]/members[¶](index.html.md#get-1-cards-card-id-or-shortlink-members)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
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

## GET /1/cards/[card_id or shortlink]/membersVoted[¶](index.html.md#get-1-cards-card-id-or-shortlink-membersvoted)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
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

## GET /1/cards/[card_id or shortlink]/stickers[¶](index.html.md#get-1-cards-card-id-or-shortlink-stickers)

  * **Required permissions:** read
  * **Arguments**
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `top`
        * `left`
        * `zIndex`
        * `rotate`
        * `image`
        * `imageUrl`
        * `imageScaled`

## GET /1/cards/[card_id or shortlink]/stickers/[sticker_id][¶](index.html.md#get-1-cards-card-id-or-shortlink-stickers-idsticker)

  * **Required permissions:** read
  * **Arguments**
    * `idSticker` (required)
      * **Valid Values:** The id of the sticker
    * `fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `top`
        * `left`
        * `zIndex`
        * `rotate`
        * `image`
        * `imageUrl`
        * `imageScaled`

## PUT /1/cards/[card_id or shortlink][¶](index.html.md#put-1-cards-card-id-or-shortlink)

  * **Required permissions:** read
  * **Arguments**
    * `name` (optional)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `closed` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `labels` (optional)
    * `idMembers` (optional)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `idAttachmentCover` (optional)
      * **Valid Values:** Id of the image attachment of this card to use as its cover, or null for no cover
    * `idList` (optional)
      * **Valid Values:** id of the list the card should be moved to
    * `idBoard` (optional)
      * **Valid Values:** id of the board the card should be moved to
    * `pos` (optional)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.
    * `due` (optional)
      * **Valid Values:** A date, or `null`
    * `subscribed` (optional)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/cards/[card_id or shortlink]/actions/[action_id]/comments[¶](index.html.md#put-1-cards-card-id-or-shortlink-actions-idaction-comments)

  * **Notes:** This can only be done by the original author of the comment.
  * **Required permissions:** read
  * **Arguments**
    * `idAction` (required)
      * **Valid Values:** The id of the action.
    * `text` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem/[checkitem_id]/name[¶](index.html.md#put-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem-idcheckitem-name)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** The id of the checkitem to modify.
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem/[checkitem_id]/pos[¶](index.html.md#put-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem-idcheckitem-pos)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** The id of the checkitem to modify.
    * `value` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem/[checkitem_id]/state[¶](index.html.md#put-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem-idcheckitem-state)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** The id of the checkitem to modify.
    * `value` (required)
      * **Valid Values:** One of:
        * `true`
        * `false`
        * `complete`
        * `incomplete`

## PUT /1/cards/[card_id or shortlink]/checklist/[checklistcurrent_id]/checkItem/[checkitem_id][¶](index.html.md#put-1-cards-card-id-or-shortlink-checklist-idchecklistcurrent-checkitem-idcheckitem)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklistCurrent` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** The id of the checkitem to modify.
    * `name` (optional)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `state` (optional)
      * **Valid Values:** One of:
        * `true`
        * `false`
        * `complete`
        * `incomplete`
    * `idChecklist` (optional)
      * **Valid Values:** An id, or `null`
    * `pos` (optional)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/cards/[card_id or shortlink]/closed[¶](index.html.md#put-1-cards-card-id-or-shortlink-closed)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/cards/[card_id or shortlink]/desc[¶](index.html.md#put-1-cards-card-id-or-shortlink-desc)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/cards/[card_id or shortlink]/due[¶](index.html.md#put-1-cards-card-id-or-shortlink-due)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A date, or `null`

## PUT /1/cards/[card_id or shortlink]/idAttachmentCover[¶](index.html.md#put-1-cards-card-id-or-shortlink-idattachmentcover)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** Id of the image attachment of this card to use as its cover, or null for no cover

## PUT /1/cards/[card_id or shortlink]/idBoard[¶](index.html.md#put-1-cards-card-id-or-shortlink-idboard)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** id of the board the card should be moved to
    * `idList` (optional)
      * **Valid Values:** id of the list that the card should be moved to on the new board

## PUT /1/cards/[card_id or shortlink]/idList[¶](index.html.md#put-1-cards-card-id-or-shortlink-idlist)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** id of the list the card should be moved to

## PUT /1/cards/[card_id or shortlink]/idMembers[¶](index.html.md#put-1-cards-card-id-or-shortlink-idmembers)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings

## PUT /1/cards/[card_id or shortlink]/labels[¶](index.html.md#put-1-cards-card-id-or-shortlink-labels)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)

## PUT /1/cards/[card_id or shortlink]/name[¶](index.html.md#put-1-cards-card-id-or-shortlink-name)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/cards/[card_id or shortlink]/pos[¶](index.html.md#put-1-cards-card-id-or-shortlink-pos)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## PUT /1/cards/[card_id or shortlink]/stickers/[sticker_id][¶](index.html.md#put-1-cards-card-id-or-shortlink-stickers-idsticker)

  * **Required permissions:** write
  * **Arguments**
    * `idSticker` (required)
      * **Valid Values:** The id of the sticker to modify
    * `top` (optional)
    * `left` (optional)
    * `zIndex` (optional)
      * **Valid Values:** Valid Z values for stickers, must be an integer
    * `rotate` (optional)

## PUT /1/cards/[card_id or shortlink]/subscribed[¶](index.html.md#put-1-cards-card-id-or-shortlink-subscribed)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## POST /1/cards[¶](index.html.md#post-1-cards)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `pos` (optional)
      * **Default:** `bottom`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.
    * `due` (required)
      * **Valid Values:** A date, or `null`
    * `labels` (optional)
    * `idList` (required)
      * **Valid Values:** id of the list that the card should be added to
    * `idMembers` (optional)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `idCardSource` (optional)
      * **Valid Values:** The id of the card to copy into a new card.
    * `keepFromSource` (optional)
      * **Default:** `all`
      * **Valid Values:** Properties of the card to copy over from the source.

## POST /1/cards/[card_id or shortlink]/actions/comments[¶](index.html.md#post-1-cards-card-id-or-shortlink-actions-comments)

  * **Required permissions:** comments
  * **Arguments**
    * `text` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## POST /1/cards/[card_id or shortlink]/attachments[¶](index.html.md#post-1-cards-card-id-or-shortlink-attachments)

  * **Required permissions:** write
  * **Arguments**
    * `file` (optional)
      * **Valid Values:** A file
    * `url` (optional)
      * **Valid Values:** A URL starting with [http://](http://) or [https://](https://) or `null`
    * `name` (optional)
      * **Valid Values:** a string with a length from `0` to `256`
    * `mimeType` (optional)
      * **Valid Values:** a string with a length from `0` to `256`

## POST /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem[¶](index.html.md#post-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `pos` (optional)
      * **Default:** `bottom`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## POST /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem/[checkitem_id]/convertToCard[¶](index.html.md#post-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem-idcheckitem-converttocard)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** The id of the checkitem to modify.

## POST /1/cards/[card_id or shortlink]/checklists[¶](index.html.md#post-1-cards-card-id-or-shortlink-checklists)

  * **Required permissions:** write
  * **Arguments**
    * `value` (optional)
      * **Valid Values:** The id of the checklist to add to the card, or null to create a new one.
    * `name` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `idChecklistSource` (optional)
      * **Valid Values:** The id of the source checklist to copy into a new checklist.

## POST /1/cards/[card_id or shortlink]/idMembers[¶](index.html.md#post-1-cards-card-id-or-shortlink-idmembers)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** The id of the member to add to the card

## POST /1/cards/[card_id or shortlink]/labels[¶](index.html.md#post-1-cards-card-id-or-shortlink-labels)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `green`
        * `yellow`
        * `orange`
        * `red`
        * `purple`
        * `blue`

## POST /1/cards/[card_id or shortlink]/markAssociatedNotificationsRead[¶](index.html.md#post-1-cards-card-id-or-shortlink-markassociatednotificationsread)

  * **Required permissions:** read
  * **Arguments:** None

## POST /1/cards/[card_id or shortlink]/membersVoted[¶](index.html.md#post-1-cards-card-id-or-shortlink-membersvoted)

  * **Required permissions:** voting
  * **Arguments**
    * `value` (required)
      * **Valid Values:** The id of the member to vote &#39;yes&#39; on the card

## POST /1/cards/[card_id or shortlink]/stickers[¶](index.html.md#post-1-cards-card-id-or-shortlink-stickers)

  * **Required permissions:** write
  * **Arguments**
    * `image` (required)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `top` (required)
    * `left` (required)
    * `zIndex` (required)
      * **Valid Values:** Valid Z values for stickers, must be an integer
    * `rotate` (optional)
      * **Default:** `0`

## DELETE /1/cards/[card_id or shortlink][¶](index.html.md#delete-1-cards-card-id-or-shortlink)

  * **Required permissions:** write
  * **Arguments:** None

## DELETE /1/cards/[card_id or shortlink]/actions/[action_id]/comments[¶](index.html.md#delete-1-cards-card-id-or-shortlink-actions-idaction-comments)

  * **Notes:** This can only be done by the original author of the comment, or someone with higher permissions than the original author.
  * **Required permissions:** comments
  * **Arguments**
    * `idAction` (required)
      * **Valid Values:** The id of the action.

## DELETE /1/cards/[card_id or shortlink]/attachments/[attachment_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-attachments-idattachment)

  * **Required permissions:** write
  * **Arguments**
    * `idAttachment` (required)
      * **Valid Values:** The id of the attachment to remove from the card.

## DELETE /1/cards/[card_id or shortlink]/checklist/[checklist_id]/checkItem/[checkitem_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-checklist-idchecklist-checkitem-idcheckitem)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist.
    * `idCheckItem` (required)
      * **Valid Values:** the id of the check item to remove

## DELETE /1/cards/[card_id or shortlink]/checklists/[checklist_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-checklists-idchecklist)

  * **Required permissions:** write
  * **Arguments**
    * `idChecklist` (required)
      * **Valid Values:** The id of the checklist to remove from the card

## DELETE /1/cards/[card_id or shortlink]/idMembers/[member_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-idmembers-idmember)

  * **Required permissions:** write
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** The id of the member to remove from the card

## DELETE /1/cards/[card_id or shortlink]/labels/[color][¶](index.html.md#delete-1-cards-card-id-or-shortlink-labels-color)

  * **Required permissions:** write
  * **Arguments**
    * `color` (required)
      * **Valid Values:** One of:
        * `green`
        * `yellow`
        * `orange`
        * `red`
        * `purple`
        * `blue`

## DELETE /1/cards/[card_id or shortlink]/membersVoted/[member_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-membersvoted-idmember)

  * **Required permissions:** voting
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** The id of the member whose vote to rescind

## DELETE /1/cards/[card_id or shortlink]/stickers/[sticker_id][¶](index.html.md#delete-1-cards-card-id-or-shortlink-stickers-idsticker)

  * **Required permissions:** write
  * **Arguments**
    * `idSticker` (required)
      * **Valid Values:** The id of the sticker to remove

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
