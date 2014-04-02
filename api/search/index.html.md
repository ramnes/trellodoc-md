# search[¶](index.html.md#search)

## GET /1/search[¶](index.html.md#get-1-search)

  * **Arguments**
    * `query` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `idBoards` (optional)
      * **Default:** `mine`
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `idOrganizations` (required)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `idCards` (optional)
      * **Valid Values:** A comma-separated list of objectIds, 24-character hex strings
    * `modelTypes` (optional)
      * **Default:** `all`
      * **Valid Values:** Search over actions is temporarily disabled and will return no results
    * `board_fields` (optional)
      * **Default:** `name,idOrganization`
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
    * `boards_limit` (optional)
      * **Default:** `10`
      * **Valid Values:** a number from `1` to `1000`
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
    * `cards_limit` (optional)
      * **Default:** `10`
      * **Valid Values:** a number from `1` to `1000`
    * `cards_page` (optional)
      * **Default:** `0`
      * **Valid Values:** a number from `0` to `100`
    * `card_board` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_list` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_members` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_stickers` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `card_attachments` (optional)
      * **Default:** `false`
      * **Valid Values:** A boolean value or &quot;cover&quot; for only card cover attachments
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
    * `organizations_limit` (optional)
      * **Default:** `10`
      * **Valid Values:** a number from `1` to `1000`
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
    * `members_limit` (optional)
      * **Default:** `10`
      * **Valid Values:** a number from `1` to `1000`
    * `action_fields` (optional)
      * **Default:** `all`
      * **Valid Values:** `all` or a comma-separated list of:
        * `idMemberCreator`
        * `data`
        * `type`
        * `date`
    * `actions_entities` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`
    * `actions_limit` (optional)
      * **Default:** `10`
      * **Valid Values:** a number from `0` to `1000`
    * `actions_since` (optional)
      * **Valid Values:** A date, a number of days, or `null`
    * `partial` (optional)
      * **Default:** `false`
      * **Valid Values:**
        * `true`
        * `false`

## GET /1/search/members[¶](index.html.md#get-1-search-members)

  * **Arguments**
    * `query` (required)
      * **Valid Values:** a string with a length from `1` to `16384`
    * `limit` (optional)
      * **Default:** `8`
      * **Valid Values:** a number from `1` to `20`
    * `idBoard` (optional)
      * **Valid Values:** An id, or `null`
    * `idOrganization` (optional)
      * **Valid Values:** An id, or `null`
    * `onlyOrgMembers` (optional)
      * **Default:** `false`
      * **Valid Values:** A boolean

(C) Copyright 2013, Fog Creek Software. Created using
[Sphinx](http://sphinx.pocoo.org/) 1.2b1.
