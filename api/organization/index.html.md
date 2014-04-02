# organization[¶](index.html.md#organization)

## GET /1/organizations/[idOrg or name][¶](index.html.md#get-1-organizations-idorg-or-name)

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
      * **Default:** `avatarHash,fullName,initials,username,confirmed`
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
    * `member_activity` (optional)
      * **Default:** `false`
      * **Valid Values:** `true` or `false`; works for premium organizations only.
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
    * `boards` (optional)
      * **Default:** `none`
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
    * `paid_account` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `fields` (optional)
      * **Default:** `name,displayName,desc,descData,url,website,logoHash,products,powerUps`
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
  * **Examples**
    
    https://api.trello.com/1/organizations/publicorg?members=all&member_fields=username,fullName&fields=name,desc&key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "id": "4ee7e59ae582acdec8000291",
        "name": "publicorg",
        "desc": "This is a test organization",
        "members": [{
            "id": "4ee7df3ce582acdec80000b2",
            "username": "alicetester",
            "fullName": "Alice Tester"
        }, {
            "id": "4ee7df74e582acdec80000b6",
            "username": "davidtester",
            "fullName": "David Tester"
        }, {
            "id": "4ee7e2e1e582acdec8000112",
            "username": "edtester",
            "fullName": "Ed Tester"
        }, {
            "id": "514c6011b569140000000028",
            "username": "inviteghost8",
            "fullName": "Invite Ghost 8"
        }]
    }
```

## GET /1/organizations/[idOrg or name]/[field][¶](index.html.md#get-1-organizations-idorg-or-name-field)

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
  * **Examples**
    
    https://api.trello.com/1/organizations/exampleorg/name?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "exampleorg"
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/descData?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/desc?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "This is a sample organization"
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/idBoards?key=[application_key]&token=[optional_auth_token]
    
```json
    ["4eea4ffc91e31d1746000046"]
```
    
    https://api.trello.com/1/organizations/exampleorg/displayName?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "Example Org"
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/invited?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": false
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/prefs?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "permissionLevel": "public",
        "orgInviteRestrict": [],
        "externalMembersDisabled": false,
        "associatedDomain": null,
        "boardVisibilityRestrict": {
            "private": "org",
            "org": "org",
            "public": "org"
        }
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/memberships?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4efe2c2f2e1efe7a4c0002cd",
        "idMember": "4ee7deffe582acdec80000ac",
        "memberType": "admin",
        "unconfirmed": false
    }]
```
    
    https://api.trello.com/1/organizations/exampleorg/invitations?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```
    
    https://api.trello.com/1/organizations/exampleorg/powerUps?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```
    
    https://api.trello.com/1/organizations/exampleorg/url?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "https://trello.com/exampleorg"
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/products?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```
    
    https://api.trello.com/1/organizations/exampleorg/website?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": "http://example.org"
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/logoHash?key=[application_key]&token=[optional_auth_token]
    
```json
    {
        "_value": null
    }
```
    
    https://api.trello.com/1/organizations/exampleorg/premiumFeatures?key=[application_key]&token=[optional_auth_token]
    
```json
    []
```

## GET /1/organizations/[idOrg or name]/actions[¶](index.html.md#get-1-organizations-idorg-or-name-actions)

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
    
    https://api.trello.com/1/organizations/exampleorg/actions?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4efe2c2f2e1efe7a4c0002cb",
        "idMemberCreator": "4ee7deffe582acdec80000ac",
        "data": {
            "organization": {
                "id": "4efe2c2f2e1efe7a4c0002c9",
                "name": "Example Org"
            }
        },
        "type": "createOrganization",
        "date": "2011-12-30T21:25:03.806Z",
        "memberCreator": {
            "id": "4ee7deffe582acdec80000ac",
            "avatarHash": null,
            "fullName": "Joe Tester",
            "initials": "JT",
            "username": "joetester"
        }
    }]
```

## GET /1/organizations/[idOrg or name]/boards[¶](index.html.md#get-1-organizations-idorg-or-name-boards)

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
    
    https://api.trello.com/1/organizations/exampleorg/boards?key=[application_key]&token=[optional_auth_token]
    
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
    }]
```

## GET /1/organizations/[idOrg or name]/boards/[filter][¶](index.html.md#get-1-organizations-idorg-or-name-boards-filter)

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

## GET /1/organizations/[idOrg or name]/members[¶](index.html.md#get-1-organizations-idorg-or-name-members)

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
    
    https://api.trello.com/1/organizations/exampleorg/members?filter=admins&key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4ee7deffe582acdec80000ac",
        "fullName": "Joe Tester",
        "username": "joetester"
    }]
```
    
    https://api.trello.com/1/organizations/exampleorg/members?key=[application_key]&token=[optional_auth_token]
    
```json
    [{
        "id": "4ee7deffe582acdec80000ac",
        "fullName": "Joe Tester",
        "username": "joetester"
    }]
```

## GET /1/organizations/[idOrg or name]/members/[filter][¶](index.html.md#get-1-organizations-idorg-or-name-members-filter)

  * **Arguments**
    * `filter` (required)
      * **Valid Values:** One of:
        * `none`
        * `normal`
        * `admins`
        * `owners`
        * `all`

## GET /1/organizations/[idOrg or name]/members/[idMember]/cards[¶](index.html.md#get-1-organizations-idorg-or-name-members-idmember-cards)

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

## GET /1/organizations/[idOrg or name]/membersInvited[¶](index.html.md#get-1-organizations-idorg-or-name-membersinvited)

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

## GET /1/organizations/[idOrg or name]/membersInvited/[field][¶](index.html.md#get-1-organizations-idorg-or-name-membersinvited-field)

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

## GET /1/organizations/[idOrg or name]/memberships[¶](index.html.md#get-1-organizations-idorg-or-name-memberships)

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

## GET /1/organizations/[idOrg or name]/memberships/[idMembership][¶](index.html.md#get-1-organizations-idorg-or-name-memberships-idmembership)

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

## PUT /1/organizations/[idOrg or name][¶](index.html.md#put-1-organizations-idorg-or-name)

  * **Required permissions:** read
  * **Arguments**
    * `prefs/orgInviteRestrict` (optional)
      * **Valid Values:** An email address with optional expansion tokens
    * `prefs/externalMembersDisabled` (optional)
      * **Valid Values:**
        * `true`
        * `false`
    * `prefs/associatedDomain` (optional)
      * **Valid Values:** The google apps domain to link this org to.
    * `prefs/boardVisibilityRestrict/private` (optional)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`
    * `prefs/boardVisibilityRestrict/org` (optional)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`
    * `prefs/boardVisibilityRestrict/public` (optional)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`
    * `name` (optional)
      * **Valid Values:** A string with a length of at least 3. Only lowercase letters, underscores, and numbers are allowed. Must be unique.
    * `displayName` (optional)
      * **Valid Values:** A string with a length of at least 1. Cannot begin or end with a space.
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `website` (optional)
      * **Valid Values:** A URL starting with [http://](http://) or [https://](https://) or `null`
    * `prefs/permissionLevel` (optional)
      * **Valid Values:** One of:
        * `private`
        * `public`

## PUT /1/organizations/[idOrg or name]/desc[¶](index.html.md#put-1-organizations-idorg-or-name-desc)

  * **Required permissions:** write, own
  * **Arguments**
    * `value` (required)
      * **Valid Values:** a string with a length from `0` to `16384`

## PUT /1/organizations/[idOrg or name]/displayName[¶](index.html.md#put-1-organizations-idorg-or-name-displayname)

  * **Required permissions:** write, own
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A string with a length of at least 1. Cannot begin or end with a space.

## PUT /1/organizations/[idOrg or name]/members[¶](index.html.md#put-1-organizations-idorg-or-name-members)

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

## PUT /1/organizations/[idOrg or name]/members/[idMember][¶](index.html.md#put-1-organizations-idorg-or-name-members-idmember)

  * **Required permissions:** write
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name
    * `type` (required)
      * **Valid Values:** One of:
        * `normal`
        * `observer`
        * `admin`

## PUT /1/organizations/[idOrg or name]/members/[idMember]/deactivated[¶](index.html.md#put-1-organizations-idorg-or-name-members-idmember-deactivated)

  * **Required permissions:** write, own, deactivated
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/organizations/[idOrg or name]/memberships/[idMembership][¶](index.html.md#put-1-organizations-idorg-or-name-memberships-idmembership)

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

## PUT /1/organizations/[idOrg or name]/name[¶](index.html.md#put-1-organizations-idorg-or-name-name)

  * **Required permissions:** write, own
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A string with a length of at least 3. Only lowercase letters, underscores, and numbers are allowed. Must be unique.

## PUT /1/organizations/[idOrg or name]/prefs/associatedDomain[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-associateddomain)

  * **Required permissions:** write, own, googleApps
  * **Arguments**
    * `value` (required)
      * **Valid Values:** The google apps domain to link this org to.

## PUT /1/organizations/[idOrg or name]/prefs/boardVisibilityRestrict/org[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-boardvisibilityrestrict-org)

  * **Required permissions:** write, own, restrictVis
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`

## PUT /1/organizations/[idOrg or name]/prefs/boardVisibilityRestrict/private[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-boardvisibilityrestrict-private)

  * **Required permissions:** write, own, restrictVis
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`

## PUT /1/organizations/[idOrg or name]/prefs/boardVisibilityRestrict/public[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-boardvisibilityrestrict-public)

  * **Required permissions:** write, own, restrictVis
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `none`
        * `admin`
        * `org`

## PUT /1/organizations/[idOrg or name]/prefs/externalMembersDisabled[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-externalmembersdisabled)

  * **Required permissions:** write, own, disableExternalMembers
  * **Arguments**
    * `value` (required)
      * **Valid Values:**
        * `true`
        * `false`

## PUT /1/organizations/[idOrg or name]/prefs/orgInviteRestrict[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-orginviterestrict)

  * **Required permissions:** write, own, inviteOrg
  * **Arguments**
    * `value` (required)
      * **Valid Values:** An email address with optional expansion tokens

## PUT /1/organizations/[idOrg or name]/prefs/permissionLevel[¶](index.html.md#put-1-organizations-idorg-or-name-prefs-permissionlevel)

  * **Required permissions:** write, own
  * **Arguments**
    * `value` (required)
      * **Valid Values:** One of:
        * `private`
        * `public`

## PUT /1/organizations/[idOrg or name]/website[¶](index.html.md#put-1-organizations-idorg-or-name-website)

  * **Required permissions:** write, own
  * **Arguments**
    * `value` (required)
      * **Valid Values:** A URL starting with [http://](http://) or [https://](https://) or `null`

## POST /1/organizations[¶](index.html.md#post-1-organizations)

  * **Required permissions:** write
  * **Arguments**
    * `name` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `displayName` (optional)
      * **Valid Values:** A string with a length of at least 1. Cannot begin or end with a space.
    * `desc` (optional)
      * **Valid Values:** a string with a length from `0` to `16384`
    * `website` (optional)
      * **Valid Values:** A URL starting with [http://](http://) or [https://](https://) or `null`

## POST /1/organizations/[idOrg or name]/logo[¶](index.html.md#post-1-organizations-idorg-or-name-logo)

  * **Required permissions:** own, logo
  * **Arguments**
    * `file` (required)
      * **Valid Values:** A file

## POST /1/organizations/[idOrg or name]/unpaidAccount[¶](index.html.md#post-1-organizations-idorg-or-name-unpaidaccount)

  * **Required permissions:** own, write
  * **Arguments**
    * `products` (required)
      * **Valid Values:** An array of product ids

## DELETE /1/organizations/[idOrg or name][¶](index.html.md#delete-1-organizations-idorg-or-name)

  * **Required permissions:** write
  * **Arguments:** None

## DELETE /1/organizations/[idOrg or name]/logo[¶](index.html.md#delete-1-organizations-idorg-or-name-logo)

  * **Required permissions:** own, logo
  * **Arguments:** None

## DELETE /1/organizations/[idOrg or name]/members/[idMember][¶](index.html.md#delete-1-organizations-idorg-or-name-members-idmember)

  * **Required permissions:** write
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name

## DELETE /1/organizations/[idOrg or name]/members/[idMember]/all[¶](index.html.md#delete-1-organizations-idorg-or-name-members-idmember-all)

  * **Required permissions:** write, own, removal
  * **Arguments**
    * `idMember` (required)
      * **Valid Values:** An id, username, or organization name

## DELETE /1/organizations/[idOrg or name]/prefs/associatedDomain[¶](index.html.md#delete-1-organizations-idorg-or-name-prefs-associateddomain)

  * **Required permissions:** write, own, googleApps
  * **Arguments:** None

## DELETE /1/organizations/[idOrg or name]/prefs/orgInviteRestrict[¶](index.html.md#delete-1-organizations-idorg-or-name-prefs-orginviterestrict)

  * **Required permissions:** write, own, inviteOrg
  * **Arguments**
    * `value` (required)
      * **Valid Values:** An email address with optional expansion tokens

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
