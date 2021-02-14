---
title: SharePoint
description: >-
  This article lists the currently supported SharePoint reports with all of the
  properties that SysKit Trace loads.
date: 9/22/2020
---

# SharePoint

## Reports

### Apps

| Name | Description |
| :--- | :--- |
| **App Name** | The name of the App. |

### Company Themes

| Name | Description |
| :--- | :--- |
| **Name** | The name of the theme, which appears in the theme picker UI and is also used by administrators and developers to refer to the theme in PowerShell cmdlets or calls to the SharePoint REST API. |
| **Is Inverted** | This value should be false for light themes and true for dark themes; it controls whether SharePoint uses dark or light theme colors to render text on colored backgrounds. |

### Home Site

| Name | Description |
| :--- | :--- |
| **Url** | The URL of the home site collection. |

### Hub Sites

| Name | Description |
| :--- | :--- |
| **Url** | The URL of the site collection. |
| **Title** | The title of the hub site. |
| **Description** | The description of the hub site. |
| **Logo Url** | The url to the logo of the hub site. |
| **Requires Join Approval** | Does the hub site require approval to join. |
| **Allowed To Join** | The users or mail-enabled security groups which are allowed to associate their site with a hub site. |
| **Site Design Id** | The guid of the site design to link to the hub site. |

### Org Assets Library

| Name | Description |
| :--- | :--- |
| **Name** | Display name of the library. |
| **Asset Type** | Specifies the asset type of this library. |
| **Asset Type** | Specifies the file type in this library. |
| **Library Url** | Indicates the absolute URL of the library to be designated as a central location for organization assets. |
| **Thumbnail Url** | Indicates the absolute URL of the library to be designated as a central location for organization Indicates the URL of the background image used when the library is publicly displayed. If no thumbnail URL is indicated, the card will have a gray background. |

### Policies

| Name | Description |
| :--- | :--- |
| **Display Start A Site Option** | Determines whether tenant users see the Start a Site menu option. |
| **Start A Site Form Url** | Specifies URL of the form to load in the Start a Site dialog. The valid values are:&lt;emptyString&gt; \(default\) - Blank by default, this will also remove or clear any value that has been set.Full URL - Example: [https://contoso.sharepoint.com/path/to/form](https://contoso.sharepoint.com/path/to/form). |
| **IP Address Enforcement** | Allows access from network locations that are defined by an administrator. |
| **IP Address Allow List** | Configures multiple IP addresses or IP address ranges \(IPv4 or IPv6\). Use commas to separate multiple IP addresses or IP address ranges. |
| **IP Address WAC Token Lifetime** | Office webapps TokenLifeTime in minutes. |
| **Comments On Site Pages Disabled** | When this feature is set to true, comments on site pages will be disabled. |
| **Social Bar On Site Pages Disabled** | Disables or enables the Social Bar. It will give users the ability to like a page, see the number of views, likes, and comments on a page, and see the people who have liked a page. |
| **Disallow Infected File Download** | Prevents the Download button from being displayed on the Virus Found warning page. |
| **External Services Enabled** | Enables external services for a tenant. External services are defined as services that are not in the Office 365 datacenters. |
| **Email Attestation Required** | Sets email attestation to required. |
| **Email Attestation Re-Auth Days** | Sets email attestation re-auth days. |

### Property Bag

| Name | Description |
| :--- | :--- |
| **Url** | Url of the site where to configure the property bag property. |
| **Key** | Key that should be configured. |
| **Value** | Value of the assigned key. |

### Search Managed Properties

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' of the Managed Property. |
| **Type** | The 'Type' of the Managed Property. |
| **Description** | Description of the Managed Property. |
| **Searchable** | Enables querying against the content of the managed property.  The content of this managed property is included in the full-text index. For example, if the property is 'author', a simple query for 'Smith' returns items containing the word 'Smith' and items whose author property contains 'Smith'. |
| **Full Text Index** | Defines which full-text index the Managed Property is stored in. |
| **Full Text Context** | Defines the context of a managed property within its full-text index. |
| **Queryable** | Enables querying against the specific Managed Property. The Managed Property field name must be included in the query, either specified in the query itself or included in the query programmatically. If the Managed Property is 'author', the query must contain 'author:Smith'. |
| **Retrievable** | Enables the content of this managed property to be returned in search results. Enable this setting for managed properties that are relevant to present in search results. |
| **Allow Multiple Values** | Allow multiple values of the same type in this managed property. For example, if this is the 'author' managed property, and a document has multiple authors, each author name will be stored as a separate value in this managed property. |
| **Refinable** | Yes: Enables using the property as a refiner for search results in the front end. You must manually configure the refiner in the web part. Yes - latent: Enables switching refinable to active later, without having to do a full re-crawl when you switch. Both options require a full crawl to take effect. |
| **Sortable** | Yes: Enables sorting the result set based on the property before the result set is returned. Use for example for large result sets that cannot be sorted and retrieved at the same time. Yes - latent: Enables switching sortable to active later, without having to do a full re-crawl when you switch. Both options require a full crawl to take effect. |
| **Safe** | Enables this managed property to be returned for queries executed by anonymous users. Enable this setting for managed properties that do not contain sensitive information and are appropriate for anonymous users to view. |
| **Aliases** | Define an alias for a managed property if you want to use the alias instead of the managed property name in queries and in search results. Use the original managed property and not the alias to map to a crawled property. Use an alias if you don't want to or don't have permission to create a new managed property. |
| **Token Normalization** | Enable to return results independent of letter casing and diacritics\(for example accented characters\) used in the query. |
| **Complete Matching** | By default, search returns partial matches between queries against this managed property and its content. Select Complete Matching for search to return exact matches instead. If a managed property 'Title' contains 'Contoso Sites', only the query Title: 'Contoso Sites' will give a result. |
| **Language Neutral Tokenization** | By default, search depends on language when it breaks queries and content into parts \(tokenization\). Language neutral tokenization is used when there is multilingual content and this managed property contains tags that are based on metadata term sets or other identifiers. |
| **Finer Query Tokenization** | By default, search tokenizes queries coarser than content. If a managed property 'ID' contains the string '1-23-456\#7', and you query ID:'1-23', you might not get a partial match because search didn't break the query into small enough parts. Finer query tokenization are to be considered if the content of this managed property contains separators such as dots and dashes. Finer query tokenization makes queries against this managed property slower. |
| **Mapped Crawled Properties** | Names of the crawled properties that are mapped to this managed property. |
| **Company Name Extraction** | Enables the system to extract company name entities from the managed property when crawling new or updated items. Afterwards, the extracted entities can be used to set up refiners in the web part. |

### Search Result Sources

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' of the Result Source. |
| **Description** | Description of the Result Source. |
| **Protocol** | The protocol of the Result Source. |
| **Source URL** | Address of the root site collection of the remote SharePoint farm or Exchange server. |
| **Type** | The 'SharePoint Search Results' type will search over the entire index. The 'People Search Results' enables query processing specific to People Search, such as phonetic name matching or nickname matching. Only people profiles will be returned from a People Search source. |
| **Query Transform** | Incoming queries are changed to use this new query text instead. The incoming query is included in the new text with the query variable '{searchTerms}'. |
| **Show Partial Search** | Show partial search or not. |
| **Use Autodiscover** | Specifies if AutoDiscover should be used for the Exchange Source URL. |

### Sharing

| Name | Description |
| :--- | :--- |
| **Sharing Capability** | Configures anonymous link types for folders. |
| **Show Everyone Claim** | Enables the administrator to hide the Everyone claim in the People Picker. |
| **Show All Users Claim** | Enables the administrator to hide the All Users claim groups in People Picker. |
| **Show Everyone Except External Users Claim** | Enables the administrator to hide the Everyone except external users claim in the People Picker. |
| **Provision Shared With Everyone Folder** | Creates a Shared with Everyone folder in every user's new OneDrive for Business document library. |
| **Enable Guest Sign In Acceleration** | Accelerates guest-enabled site collections as well as member-only site collections when the SignInAccelerationDomain property is set. |
| **Bcc External Sharing Invitations** | When the feature is enabled, all external sharing invitations that are sent will blind copy the e-mail messages listed in the BccExternalSharingsInvitationList. |
| **Bcc External Sharing Invitations List** | Specifies a list of e-mail addresses to be BCC'd when the BCC for External Sharing feature is enabled. Multiple addresses can be specified by creating a comma separated list with no spaces. |
| **Require Anonymous Links Expire In Days** | Specifies all anonymous links that have been created \(or will be created\) will expire after the set number of days . |
| **Sharing Allowed Domain List** | Specifies a list of email domains that is allowed for sharing with the external collaborators. |
| **Sharing Blocked Domain List** | Specifies a list of email domains that is blocked or prohibited for sharing with the external collaborators. |
| **Sharing Domain Restriction Mode** | Specifies the external sharing mode for domains. |
| **Default Sharing Link Type** | Lets administrators choose what type of link appears is selected in the 'Get a link' sharing dialog box in OneDrive for Business and SharePoint Online. |
| **Prevent External Users From Resharing** | Allow or deny external users re-sharing. |
| **Show People Picker Suggestions For Guest Users** | Enables the administrator to hide the guest users claim in the People Picker. |
| **File Anonymous Link Type** | Configures anonymous link types for files. |
| **Folder Anonymous Link Type** | Configures anonymous link types for folders. |
| **Notify Owners When Items Reshared** | When this property is set to True and another user re-shares a document from a user’s OneDrive for Business, the OneDrive for Business owner is notified by e-mail. |
| **Default Link Permission** | Specifies the link permission on the tenant level. |
| **Require Accepting Account Match Invited Account** | Ensures that an external user can only accept an external sharing invitation with an account matching the invited email address.Administrators who desire increased control over external collaborators should consider enabling this feature. False \(default\) - When a document is shared with an external user, bob@contoso.com, it can be accepted by any user with access to the invitation link in the original e-mail.True - User must accept this invitation with bob@contoso.com. |

### Site Design Rights

| Name | Description |
| :--- | :--- |
| **Site Design Title** | The title of the site design. |
| **User Principals** | List of user principals with site design rights. |
| **Rights** | Rights granted to user principals. |

### Site Designs

| Name | Description |
| :--- | :--- |
| **Title** | The title of the site design. |
| **Site Script Names** | The names of the site design scripts. |
| **Web Template** | Web template to which the site design is applied to when invoked. |
| **Description** | Description of site design. |
| **Is Default** | Is site design applied by default to web templates. |
| **Preview Image Alt Text** | Site design alternate preview image text. |
| **Preview Image Url** | Site design preview image url. |
| **Version** | Site design version number. |

### Site Groups

| Name | Description |
| :--- | :--- |
| **Url** | The URL of the site. |
| **Group Name** | The name of the site group. |
| **Owner** | The owner \(email address\) of the site group. |
| **Permission Levels** | The permission level of the site group. |

### Site Script

| Name | Description |
| :--- | :--- |
| **Title** | The title of the site script. |
| **Description** | The description of the site script. |

### Sites

| Name | Description |
| :--- | :--- |
| **Url** | The URL of the site collection. |
| **Title** | The title of the site collection. |
| **Owner** | Specifies the owner of the site. |
| **Compatibility Level** | Specifies the version of templates used on the site collection. |
| **Locale Id** | Specifies the language of the site collection. Defaults to the current language of the web connected to. |
| **Template** | Specifies with template of site to create. |
| **Time Zone Id** | TimeZone ID of the site collection. |
| **Is Hub Site** | Specifies if this site is a hub site. |
| **Hub Url** | The URL of the Hub site the site collection needs to get connected to. |
| **Description** | The description of the site collection. |
| **Allow Self Service Upgrade** | Specifies if the site administrator can upgrade the site collection. |
| **Deny Add And Customize Pages** | Determines whether the Add And Customize Pages right is denied on the site collection. For more information about permission levels, see User permissions and permission levels in SharePoint. |
| **Lock State** | Specifies the lock state on a site. Valid values are: NoAccess, ReadOnly and Unlock. When the lock state of a site is ReadOnly, a message will appear on the site stating that the site is under maintenance and it is read-only. When the lock state of a site is NoAccess, all traffic to the site will be blocked. |
| **Sharing Capability** | Specifies what the sharing capabilities are for the site. Possible values: Disabled, ExternalUserSharingOnly, ExternalUserAndGuestSharing, ExistingExternalUserSharingOnly. |
| **Site Defined Sharing Capability** | Specifies the stored value of the site sharing capability. Note that the effective capability also depends on the tenant wide setting. |
| **Comments On Site Pages Disabled** | Specifies if comments on site pages are enabled or disabled. |
| **Social Bar On Site Pages Disabled** | Disables or enables the Social Bar for Site Collection. |
| **Disable App Views** | Disables App Views. |
| **Disable Company Wide Sharing Links** | Disables Company wide sharing links. |
| **Disable Flows** | Disables Microsoft Flow for this site. |
| **Sharing Allowed Domain List** | Specifies a list of email domains that is allowed for sharing with the external collaborators. |
| **Sharing Blocked Domain List** | Specifies a list of email domains that is blocked for sharing with the external collaborators. |
| **Sharing Domain Restriction Mode** | Specifies the external sharing mode for domains. |
| **Show People Picker Suggestions For Guest Users** | To enable the option to search for existing guest users at Site Collection Level, set this property to True. |
| **Default Sharing Link Type** | Specifies the default link type for the site collection. None - Respect the organization default sharing link type. AnonymousAccess - Sets the default sharing link for this site to an Anonymous Access or Anyone link. Internal - Sets the default sharing link for this site to the 'organization' link or company shareable link. Direct - Sets the default sharing link for this site to the 'Specific people' link. |
| **Default Link Permission** | Specifies the default link permission for the site collection. None - Respect the organization default link permission. View - Sets the default link permission for the site to 'view' permissions. Edit - Sets the default link permission for the site to 'edit' permissions. |
| **Default Link To Existing Access** | When set to TRUE, the 'Default Sharing Link Type' will be overriden and the default sharing link will a People with Existing Access link \(which does not modify permissions\). When set to FALSE \(the default\), the default sharing link type is controlled by the 'Default Sharing Link Type' parameter. |
| **Override Tenant Anonymous Link Expiration Policy** | False - Respect the organization-level policy for anonymous or anyone link expiration. True - Override the organization-level policy for anonymous or anyone link expiration \(can be more or less restrictive\). |
| **Anonymous Link Expiration In Days** | Specifies that all anonymous/anyone links that have been created \(or will be created\) will expire after the set number of days. Only applies if 'Override Tenant Anonymous Link Expiration Policy' is set to true. To remove the expiration requirement, set the value to zero \(0\). |
| **Override Tenant External User Expiration Policy** | False - Respect the organization-level policy for external user expiration. True - Override the organization-level policy for external user expiration \(can be more or less restrictive\). |
| **External User Expiration In Days** | Specifies that all external users will expire after the set number of days. Only applies if 'Override Tenant External User Expiration Policy' is set to true. To remove the expiration requirement, set the value to zero \(0\). |
| **Storage Maximum Level** | Specifies the storage quota for this site collection in megabytes. This value must not exceed the company's available quota. |
| **Storage Warning Level** | Specifies the warning level for the storage quota in megabytes. This value must not exceed the values set for the 'Storage Maximum Level' parameter. |
| **Restricted To Region** | Defines geo-restriction settings for this site. |
| **Allow Downloading Non Web Viewable Files** | Specifies if non web viewable files can be downloaded. |
| **Allow Editing** | Prevents users from editing Office files in the browser and copying and pasting Office file contents out of the browser window. |
| **Conditional Access Policy** | Specifies the policy for access from unmanaged devices. |
| **Limited Access File Type** | This property can be used when the Conditional Access Policy is set to AllowLimitedAccess for both the organization-wide setting and the site-level setting. |

### Storage Entities

| Name | Description |
| :--- | :--- |
| **Site Url** | The url of site collection or tenant. |
| **Key** | The key of the storage entity. |
| **Value** | Value of the storage entity. |
| **Entity Scope** | Scope of the storage entity. |
| **Description** | Description of storage entity. |
| **Comment** | Comment for the storage entity. |

### Tenant CDN Policies

| Name | Description |
| :--- | :--- |
| **CDN Type** | Type of Content Delivery Network. Can be 'Private' or 'Public'. |
| **Exclude Restricted Site Classifications** | List of site classifications to exclude. |
| **Include File Extensions** | List of file extensions to include in the Policy. |

### Tenant Settings

| Name | Description |
| :--- | :--- |
| **Min Compatibility Level** | Specifies the lower bound on the compatibility level for new sites. |
| **Max Compatibility Level** | Specifies the upper bound on the compatibility level for new sites. |
| **Search Resolve Exact Email Or UPN** | Removes the search capability from People Picker. Note, recently resolved names will still appear in the list until browser cache is cleared or expired. |
| **Office Client ADAL Disabled** | When set to true this will disable the ability to use Modern Authentication that leverages ADAL across the tenant. |
| **Legacy Auth Protocols Enabled** | Setting this property prevents Office clients using non-modern authentication protocols from accessing SharePoint Online resources. |
| **Require Accepting Account Match Invited Account** | Ensures that an external user can only accept an external sharing invitation with an account matching the invited email address. |
| **Sign In Acceleration Domain** | Specifies the home realm discovery value to be sent to Azure Active Directory \(AAD\) during the user sign-in process. |
| **Use Persistent Cookies For Explorer View** | Lets SharePoint issue a special cookie that will allow this feature to work even when Keep Me Signed In is not selected. |
| **User Voice For Feedback Enabled** | Allow feedback via UserVoice. |
| **Public Cdn Enabled** | Configure PublicCDN. |
| **Public Cdn Allowed File Types** | Configure filetypes allowed for PublicCDN. |
| **Use Find People In People Picker** | When set to True, users aren't able to share with security groups or SharePoint groups. |
| **Notifications In SharePoint Enabled** | When set to True, users aren't able to share with security groups or SharePoint groups. |
| **Hide Default Themes** | Defines if the default themes are visible or hidden. |

