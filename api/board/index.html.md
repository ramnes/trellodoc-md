# board[¶](index.html.md#board)

## GET /1/boards/[board_id][¶](index.html.md#get-1-boards-board-id)

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
    * `actions_format` (optional)
      * **Default:** `list`
      * **Valid Values:** One of:
        * `count`
        * `list`
        * `minimal`
    * `actions_since` (optional)
      * **Valid Values:** A date, `null` or `lastView`
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
    * `action_member` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `action_member_fields` (optional)
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
    * `action_memberCreator` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
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
    * `card_attachments` (optional)
      * **Default:** `false`
      * **Valid Values:** A boolean value or &quot;cover&quot; for only card cover attachments
    * `card_attachment_fields` (optional)
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
    * `card_checklists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `all`
    * `card_stickers` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `boardStars` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `mine`
    * `lists` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`
    * `list_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`
    * `memberships` (optional)
      * **Default:** `none`
      * **Valid Values:** `all` or a comma-separated list of:
        * `me`
        * `normal`
        * `admin`
        * `active`
        * `deactivated`
    * `memberships_member` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `memberships_member_fields` (optional)
      * **Default:** `fullName,username`
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
    * `members` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `normal`
        * `admins`
        * `owners`
        * `all`
    * `member_fields` (optional)
      * **Default:** `avatarHash,initials,fullName,username,confirmed`
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
    * `membersInvited` (optional)
      * **Default:** `none`
      * **Valid Values:** One of:
        * `none`
        * `normal`
        * `admins`
        * `owners`
        * `all`
    * `membersInvited_fields` (optional)
      * **Default:** `avatarHash,initials,fullName,username`
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
    * `organization_memberships` (optional)
      * **Default:** `none`
      * **Valid Values:** `all` or a comma-separated list of:
        * `me`
        * `normal`
        * `admin`
        * `active`
        * `deactivated`
    * `myPrefs` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `fields` (optional)
      * **Default:** `name,desc,descData,closed,idOrganization,pinned,url,shortUrl,prefs,labelNames`
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
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046?lists=open&list_fields=name&fields=name,desc&key=[application_key]&token=[optional_auth_token]

```json    
    {
        "id": "4eea4ffc91e31d1746000046",
        "name": "Example Board",
        "desc": "This board is used in the API examples",
        "lists": [{
            "id": "4eea4ffc91e31d174600004a",
            "name": "To Do Soon"
        }, {
            "id": "4eea4ffc91e31d174600004b",
            "name": "Doing"
        }, {
            "id": "4eea4ffc91e31d174600004c",
            "name": "Done"
        }]
    }
```

## GET /1/boards/[board_id]/[field][¶](index.html.md#get-1-boards-board-id-field)

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
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/idOrganization?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "4efe2c2f2e1efe7a4c0002c9"
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/name?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "Example Board"
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/closed?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": false
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/desc?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "This board is used in the API examples"
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/descData?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/pinned?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/starred?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/invited?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": false
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/invitations?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/url?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "https://trello.com/b/OXiBYZoj/example-board"
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/prefs?key=[application_key]&token=[optional_auth_token]
    
```json
    {
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
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/shortLink?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "OXiBYZoj"
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/memberships?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
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
    }]
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/powerUps?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/dateLastActivity?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/subscribed?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/labelNames?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "yellow": "Low Priority",
        "red": "High Priority",
        "purple": "",
        "orange": "Medium Priority",
        "green": "",
        "blue": ""
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/dateLastView?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/shortUrl?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "https://trello.com/b/OXiBYZoj"
    }
```

## GET /1/boards/[board_id]/actions[¶](index.html.md#get-1-boards-board-id-actions)

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
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/actions?filter=addMemberToCard,removeMemberFromCard&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea523791e31d17460002a0",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "card": {
                "id": "4eea522c91e31d174600027e",
                "name": "Figure out how to read a user's board list"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "idMember": "4ee7df74e582acdec80000b6"
        },
        "type": "addMemberToCard",
        "date": "2011-12-15T20:01:59.688Z",
        "member": {
            "id": "4ee7df74e582acdec80000b6",
            "avatarHash": "c9903e2464563d83e38df3afd685dc6c",
            "fullName": "David Tester",
            "initials": "DT",
            "username": "davidtester"
        },
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }, {
        "id": "4eea515291e31d17460001f9",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "card": {
                "id": "4eea502b91e31d1746000071",
                "name": "Find out where the Trello API documentation is"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "idMember": "4ee7df1be582acdec80000ae"
        },
        "type": "addMemberToCard",
        "date": "2011-12-15T19:58:10.748Z",
        "member": {
            "id": "4ee7df1be582acdec80000ae",
            "avatarHash": null,
            "fullName": "Bob Tester",
            "initials": "BT",
            "username": "bobtester"
        },
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }, {
        "id": "4eea515091e31d17460001e7",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "card": {
                "id": "4eea501f91e31d1746000062",
                "name": "Get a key to use in my API requests"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "idMember": "4ee7df74e582acdec80000b6"
        },
        "type": "addMemberToCard",
        "date": "2011-12-15T19:58:08.053Z",
        "member": {
            "id": "4ee7df74e582acdec80000b6",
            "avatarHash": "c9903e2464563d83e38df3afd685dc6c",
            "fullName": "David Tester",
            "initials": "DT",
            "username": "davidtester"
        },
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }, {
        "id": "4eea504191e31d174600009f",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "card": {
                "id": "4eea503d91e31d174600008f",
                "name": "Learn about the Trello API"
            },
            "board": {
                "id": "4eea4ffc91e31d1746000046",
                "name": "Example Board"
            },
            "idMember": "4ee7deffe582acdec80000ac"
        },
        "type": "addMemberToCard",
        "date": "2011-12-15T19:53:37.323Z",
        "member": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        },
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }]
```

## GET /1/boards/[board_id]/boardStars[¶](index.html.md#get-1-boards-board-id-boardstars)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `mine`
      * **Valid Values:** One of:
        * `none`
        * `mine`

## GET /1/boards/[board_id]/cards[¶](index.html.md#get-1-boards-board-id-cards)

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
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/cards?fields=name,idList,url&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea503791e31d1746000080",
        "name": "Finish my awesome application",
        "idList": "4eea4ffc91e31d174600004a",
        "url": "https://trello.com/c/XlG8S7ll/3-finish-my-awesome-application"
    }, {
        "id": "4eea503d91e31d174600008f",
        "name": "Learn about the Trello API",
        "idList": "4eea4ffc91e31d174600004b",
        "url": "https://trello.com/c/Y9eWwKiQ/4-learn-about-the-trello-api"
    }, {
        "id": "4eea522c91e31d174600027e",
        "name": "Figure out how to read a user's board list",
        "idList": "4eea4ffc91e31d174600004b",
        "url": "https://trello.com/c/RUbgIc74/6-figure-out-how-to-read-a-user-s-board-list"
    }, {
        "id": "4eea501f91e31d1746000062",
        "name": "Get a key to use in my API requests",
        "idList": "4eea4ffc91e31d174600004c",
        "url": "https://trello.com/c/RruF3Yv1/1-get-a-key-to-use-in-my-api-requests"
    }, {
        "id": "4eea502b91e31d1746000071",
        "name": "Find out where the Trello API documentation is",
        "idList": "4eea4ffc91e31d174600004c",
        "url": "https://trello.com/c/WOpDiqbn/2-find-out-where-the-trello-api-documentation-is"
    }]
```

## GET /1/boards/[board_id]/cards/[filter][¶](index.html.md#get-1-boards-board-id-cards-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `visible`
        * `open`
        * `closed`
        * `all`

## GET /1/boards/[board_id]/cards/[card_id][¶](index.html.md#get-1-boards-board-id-cards-idcard)

  * **Required permissions:** read
  * **Arguments**
    * `idCard` (required)
      * **Valid Values:** The id (or short id) of a card on the board
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
    * `members` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `member_fields` (optional)
      * **Default:** `avatarHash,initials,fullName,username`
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
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `checkItemState_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idCheckItem`
        * `state`
    * `labels` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
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

## GET /1/boards/[board_id]/checklists[¶](index.html.md#get-1-boards-board-id-checklists)

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
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/checklists?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea6ae1a5da7f5a49000092",
        "name": "API Checklist",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "4eea522c91e31d174600027e",
        "pos": 16384,
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
        }]
    }, {
        "id": "51114ce37f727e1c0f0000c6",
        "name": "List of Checks",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "51114ce37f727e1c0f0000b7",
        "pos": null,
        "checkItems": [{
            "state": "incomplete",
            "id": "51114ce47f727e1c0f0000d7",
            "name": "Check Item",
            "nameData": null,
            "pos": 16384
        }, {
            "state": "incomplete",
            "id": "51114ce47f727e1c0f0000e0",
            "name": "Check Item",
            "nameData": null,
            "pos": 32768
        }, {
            "state": "incomplete",
            "id": "51114ce47f727e1c0f0000e8",
            "name": "Check Item",
            "nameData": null,
            "pos": 49152
        }]
    }, {
        "id": "511171af63d9b4401c0000c6",
        "name": "List of Checks",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "511171af63d9b4401c0000b8",
        "pos": null,
        "checkItems": [{
            "state": "incomplete",
            "id": "511171b063d9b4401c0000d8",
            "name": "Check Item",
            "nameData": null,
            "pos": 16384
        }, {
            "state": "incomplete",
            "id": "511171b063d9b4401c0000e2",
            "name": "Check Item",
            "nameData": null,
            "pos": 32768
        }, {
            "state": "incomplete",
            "id": "511171b063d9b4401c0000e9",
            "name": "Check Item",
            "nameData": null,
            "pos": 49152
        }]
    }, {
        "id": "511554378fca26b25a0000c6",
        "name": "List of Checks",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "511554378fca26b25a0000b9",
        "pos": null,
        "checkItems": [{
            "state": "incomplete",
            "id": "511554378fca26b25a0000d7",
            "name": "Check Item",
            "nameData": null,
            "pos": 16384
        }, {
            "state": "incomplete",
            "id": "511554388fca26b25a0000de",
            "name": "Check Item",
            "nameData": null,
            "pos": 32768
        }, {
            "state": "incomplete",
            "id": "511554388fca26b25a0000e9",
            "name": "Check Item",
            "nameData": null,
            "pos": 49152
        }]
    }, {
        "id": "511a5be1db9f14a2090000c8",
        "name": "List of Checks",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "511a5be0db9f14a2090000b7",
        "pos": null,
        "checkItems": [{
            "state": "incomplete",
            "id": "511a5be1db9f14a2090000dd",
            "name": "Check Item",
            "nameData": null,
            "pos": 16384
        }, {
            "state": "incomplete",
            "id": "511a5be1db9f14a2090000e3",
            "name": "Check Item",
            "nameData": null,
            "pos": 32768
        }, {
            "state": "incomplete",
            "id": "511a5be2db9f14a2090000ea",
            "name": "Check Item",
            "nameData": null,
            "pos": 49152
        }]
    }, {
        "id": "511e770d01f822ae4a0000c7",
        "name": "List of Checks",
        "idBoard": "4eea4ffc91e31d1746000046",
        "idCard": "511e770d01f822ae4a0000b7",
        "pos": 16384,
        "checkItems": [{
            "state": "incomplete",
            "id": "511e770e01f822ae4a0000dd",
            "name": "Check Item",
            "nameData": null,
            "pos": 16384
        }, {
            "state": "incomplete",
            "id": "511e770e01f822ae4a0000e3",
            "name": "Check Item",
            "nameData": null,
            "pos": 32768
        }, {
            "state": "incomplete",
            "id": "511e770e01f822ae4a0000ea",
            "name": "Check Item",
            "nameData": null,
            "pos": 49152
        }]
    }]
```

## GET /1/boards/[board_id]/lists[¶](index.html.md#get-1-boards-board-id-lists)

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
        * `name`
        * `closed`
        * `idBoard`
        * `pos`
        * `subscribed`
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/lists?cards=open&card_fields=name&fields=name&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4eea4ffc91e31d174600004a",
        "name": "To Do Soon",
        "cards": [{
            "id": "4eea503791e31d1746000080",
            "name": "Finish my awesome application"
        }]
    }, {
        "id": "4eea4ffc91e31d174600004b",
        "name": "Doing",
        "cards": [{
            "id": "4eea503d91e31d174600008f",
            "name": "Learn about the Trello API"
        }, {
            "id": "4eea522c91e31d174600027e",
            "name": "Figure out how to read a user's board list"
        }]
    }, {
        "id": "4eea4ffc91e31d174600004c",
        "name": "Done",
        "cards": [{
            "id": "4eea501f91e31d1746000062",
            "name": "Get a key to use in my API requests"
        }, {
            "id": "4eea502b91e31d1746000071",
            "name": "Find out where the Trello API documentation is"
        }]
    }]
```

## GET /1/boards/[board_id]/lists/[filter][¶](index.html.md#get-1-boards-board-id-lists-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `open`
        * `closed`
        * `all`

## GET /1/boards/[board_id]/members[¶](index.html.md#get-1-boards-board-id-members)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** One of:
        * `none`
        * `normal`
        * `admins`
        * `owners`
        * `all`
    * `fields` (optional)
      * **Default:** `fullName,username`
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
    * `activity` (optional)
      * **Default:** `false`
      * **Valid Values:** `true` or `false`; works for premium organizations only.
  * **Examples**
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/members?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4ee7df1be582acdec80000ae",
        "fullName": "Bob Tester",
        "username": "bobtester"
    }, {
        "id": "4ee7df74e582acdec80000b6",
        "fullName": "David Tester",
        "username": "davidtester"
    }, {
        "id": "4ee7deffe582acdec80000ac",
        "fullName": "Joe Tester",
        "username": "joetester"
    }]
```
    
    https://api.trello.com/1/boards/4eea4ffc91e31d1746000046/members?filter=admins&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4ee7deffe582acdec80000ac",
        "fullName": "Joe Tester",
        "username": "joetester"
    }]
```

## GET /1/boards/[board_id]/members/[filter][¶](index.html.md#get-1-boards-board-id-members-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `normal`
        * `admins`
        * `owners`
        * `all`

## GET /1/boards/[board_id]/members/[member_id]/cards[¶](index.html.md#get-1-boards-board-id-members-idmember-cards)

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
    * `board` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `board_fields` (optional)
      * **Default:** `name,desc,closed,idOrganization,pinned,url,prefs`
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
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name

## GET /1/boards/[board_id]/membersInvited[¶](index.html.md#get-1-boards-board-id-membersinvited)

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

## GET /1/boards/[board_id]/membersInvited/[field][¶](index.html.md#get-1-boards-board-id-membersinvited-field)

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

## GET /1/boards/[board_id]/memberships[¶](index.html.md#get-1-boards-board-id-memberships)

  * **Required permissions:** read
  * **Arguments**
    * `filter` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `me`
        * `normal`
        * `admin`
        * `active`
        * `deactivated`
    * `member` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `member_fields` (optional)
      * **Default:** `fullName,username`
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

## GET /1/boards/[board_id]/memberships/[membership_id][¶](index.html.md#get-1-boards-board-id-memberships-idmembership)

  * **Required permissions:** read
  * **Arguments**
    * `idMembership` (required)
      * **Valid Values:** A membership document id
    * `member` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `member_fields` (optional)
      * **Default:** `fullName,username`
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

## GET /1/boards/[board_id]/myPrefs[¶](index.html.md#get-1-boards-board-id-myprefs)

  * **Required permissions:** read
  * **Arguments:** None

## GET /1/boards/[board_id]/organization[¶](index.html.md#get-1-boards-board-id-organization)

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

## GET /1/boards/[board_id]/organization/[field][¶](index.html.md#get-1-boards-board-id-organization-field)

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

## PUT /1/boards/[board_id][¶](index.html.md#put-1-boards-board-id)

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
    * `subscribed` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `idOrganization` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `prefs/permissionLevel` (optional)
      * **Valid Values:** One of:
        * `private`
        * `org`
        * `public`
    * `prefs/selfJoin` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs/cardCovers` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs/invitations` (optional)
      * **Valid Values:** One of:
        * `members`
        * `admins`
    * `prefs/voting` (optional)
      * **Valid Values:** One of:
        * `members`
        * `org`
        * `public`
        * `disabled`
        * `observers`
    * `prefs/comments` (optional)
      * **Valid Values:** One of:
        * `members`
        * `org`
        * `public`
        * `disabled`
        * `observers`
    * `prefs/background` (optional)
      * **Valid Values:** A standard background name, or the id of a custom background
    * `prefs/cardAging` (optional)
      * **Valid Values:** One of:
        * `regular`
        * `pirate`
    * `prefs/calendarFeedEnabled` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `labelNames/green` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labelNames/yellow` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labelNames/orange` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labelNames/red` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labelNames/purple` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `labelNames/blue` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/closed[¶](index.html.md#put-1-boards-board-id-closed)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/desc[¶](index.html.md#put-1-boards-board-id-desc)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/idOrganization[¶](index.html.md#put-1-boards-board-id-idorganization)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/blue[¶](index.html.md#put-1-boards-board-id-labelnames-blue)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/green[¶](index.html.md#put-1-boards-board-id-labelnames-green)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/orange[¶](index.html.md#put-1-boards-board-id-labelnames-orange)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/purple[¶](index.html.md#put-1-boards-board-id-labelnames-purple)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/red[¶](index.html.md#put-1-boards-board-id-labelnames-red)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/labelNames/yellow[¶](index.html.md#put-1-boards-board-id-labelnames-yellow)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/boards/[board_id]/members[¶](index.html.md#put-1-boards-board-id-members)

  * **Required permissions:** write
  * **Arguments**
    * `email` (required)
      * **Valid Values:** An email address
    * `fullName` (required)
      * **Valid Values:** A string with a length of at least 4. Cannot begin or end with a space.
    * `type` (optional)
      * **Default:** `normal`
      * **Valid Values:** One of:
        * `normal`
        * `observer`
        * `admin`

## PUT /1/boards/[board_id]/members/[member_id][¶](index.html.md#put-1-boards-board-id-members-idmember)

  * **Required permissions:** write
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name
    * `type` (required)
      * **Valid Values:** One of:
        * `normal`
        * `observer`
        * `admin`

## PUT /1/boards/[board_id]/memberships/[membership_id][¶](index.html.md#put-1-boards-board-id-memberships-idmembership)

  * **Required permissions:** write
  * **Arguments**
    * `idMembership` (required)
      * **Valid Values:** An id
    * `type` (required)
      * **Valid Values:** One of:
        * `normal`
        * `observer`
        * `admin`
    * `member_fields` (optional)
      * **Default:** `fullName,username`
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

## PUT /1/boards/[board_id]/myPrefs/emailPosition[¶](index.html.md#put-1-boards-board-id-myprefs-emailposition)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `top`
        * `bottom`

## PUT /1/boards/[board_id]/myPrefs/idEmailList[¶](index.html.md#put-1-boards-board-id-myprefs-idemaillist)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** An id

## PUT /1/boards/[board_id]/myPrefs/showListGuide[¶](index.html.md#put-1-boards-board-id-myprefs-showlistguide)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/myPrefs/showSidebar[¶](index.html.md#put-1-boards-board-id-myprefs-showsidebar)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/myPrefs/showSidebarActivity[¶](index.html.md#put-1-boards-board-id-myprefs-showsidebaractivity)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/myPrefs/showSidebarBoardActions[¶](index.html.md#put-1-boards-board-id-myprefs-showsidebarboardactions)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/myPrefs/showSidebarMembers[¶](index.html.md#put-1-boards-board-id-myprefs-showsidebarmembers)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/name[¶](index.html.md#put-1-boards-board-id-name)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## PUT /1/boards/[board_id]/prefs/background[¶](index.html.md#put-1-boards-board-id-prefs-background)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A standard background name, or the id of a custom background

## PUT /1/boards/[board_id]/prefs/calendarFeedEnabled[¶](index.html.md#put-1-boards-board-id-prefs-calendarfeedenabled)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/prefs/cardAging[¶](index.html.md#put-1-boards-board-id-prefs-cardaging)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `regular`
        * `pirate`

## PUT /1/boards/[board_id]/prefs/cardCovers[¶](index.html.md#put-1-boards-board-id-prefs-cardcovers)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/prefs/comments[¶](index.html.md#put-1-boards-board-id-prefs-comments)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `members`
        * `org`
        * `public`
        * `disabled`
        * `observers`

## PUT /1/boards/[board_id]/prefs/invitations[¶](index.html.md#put-1-boards-board-id-prefs-invitations)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `members`
        * `admins`

## PUT /1/boards/[board_id]/prefs/permissionLevel[¶](index.html.md#put-1-boards-board-id-prefs-permissionlevel)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `private`
        * `org`
        * `public`

## PUT /1/boards/[board_id]/prefs/selfJoin[¶](index.html.md#put-1-boards-board-id-prefs-selfjoin)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/boards/[board_id]/prefs/voting[¶](index.html.md#put-1-boards-board-id-prefs-voting)

  * **Required permissions:** own, write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `members`
        * `org`
        * `public`
        * `disabled`
        * `observers`

## PUT /1/boards/[board_id]/subscribed[¶](index.html.md#put-1-boards-board-id-subscribed)

  * **Required permissions:** read
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## POST /1/boards[¶](index.html.md#post-1-boards)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `idOrganization` (optional)
      * **Valid Values:** The id or name of the organization to add the board to.
    * `idBoardSource` (optional)
      * **Valid Values:** The id of the board to copy into the new board
    * `keepFromSource` (optional)
      * **Default:** `all`
      * **Valid Values:** Components of the source board to copy.
    * `powerUps` (optional)
      * **Valid Values:** `all` or a comma-separated list of:
        * `voting`
        * `cardAging`
        * `calendar`
    * `prefs_permissionLevel` (optional)
      * **Default:** `private`
      * **Valid Values:** One of:
        * `private`
        * `org`
        * `public`
    * `prefs_voting` (optional)
      * **Default:** `disabled`
      * **Valid Values:** One of:
        * `members`
        * `observers`
        * `org`
        * `public`
        * `disabled`
    * `prefs_comments` (optional)
      * **Default:** `members`
      * **Valid Values:** One of:
        * `members`
        * `observers`
        * `org`
        * `public`
        * `disabled`
    * `prefs_invitations` (optional)
      * **Default:** `members`
      * **Valid Values:** One of:
        * `members`
        * `admins`
    * `prefs_selfJoin` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs_cardCovers` (optional)
      * **Default:** `true`
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs_background` (optional)
      * **Default:** `blue`
      * **Valid Values:** a string with a length from `0` to `16384`
    * `prefs_cardAging` (optional)
      * **Default:** `regular`
      * **Valid Values:** One of:
        * `regular`
        * `pirate`

## POST /1/boards/[board_id]/calendarKey/generate[¶](index.html.md#post-1-boards-board-id-calendarkey-generate)

  * **Required permissions:** read
  * **Arguments:** None

## POST /1/boards/[board_id]/checklists[¶](index.html.md#post-1-boards-board-id-checklists)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`

## POST /1/boards/[board_id]/emailKey/generate[¶](index.html.md#post-1-boards-board-id-emailkey-generate)

  * **Required permissions:** write
  * **Arguments:** None

## POST /1/boards/[board_id]/lists[¶](index.html.md#post-1-boards-board-id-lists)

  * **Required permissions:** write
  * **Arguments**
    * `name` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `pos` (optional)
      * **Default:** `top`
      * **Valid Values:** A position. `top`, `bottom`, or a positive number.

## POST /1/boards/[board_id]/markAsViewed[¶](index.html.md#post-1-boards-board-id-markasviewed)

  * **Required permissions:** read
  * **Arguments:** None

## POST /1/boards/[board_id]/powerUps[¶](index.html.md#post-1-boards-board-id-powerups)

  * **Required permissions:** write
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `voting`
        * `cardAging`
        * `calendar`

## DELETE /1/boards/[board_id]/members/[member_id][¶](index.html.md#delete-1-boards-board-id-members-idmember)

  * **Required permissions:** write
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name

## DELETE /1/boards/[board_id]/powerUps/[powerup][¶](index.html.md#delete-1-boards-board-id-powerups-powerup)

  * **Required permissions:** write
  * **Arguments**
    * `powerUp` (required)
      * **Valid Values:** One of:
        * `voting`
        * `cardAging`
        * `calendar`

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
