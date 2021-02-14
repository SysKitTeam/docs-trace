---
title: Azure Active Directory
description: >-
  This article lists the currently supported Azure Active Directory reports with
  all of the properties that SysKit Trace loads.
date: 9/22/2020
---

# Azure Active Directory

## Reports

### Applications

| Name | Description |
| :--- | :--- |
| **Name** | Name of the app. |
| **Available To Other Tenants** | Indicates whether this application is available in other tenants. |
| **Group Membership Claims** | A bitmask that configures the groups claim issued in a user or OAuth 2.0 access token that the application expects. The bitmask values are: 0: None, 1: Security groups and Azure AD roles, 2: Reserved, and 4: Reserved. Setting the bitmask to 7 will get all of the security groups, distribution groups, and Azure AD directory roles that the signed-in user is a member of. |
| **Homepage** | The URL to the application's homepage. |
| **Identifier Uris** | User-defined URI\(s\) that uniquely identify a Web application within its Azure AD tenant, or within a verified custom domain. |
| **Known Client Applications** | Client applications that are tied to this resource application. |
| **Logout URL** | The logout url for this application. |
| **Oauth 2 Allow Implicit Flow** | Specifies whether this web application can request OAuth2.0 implicit flow tokens. The default is false. |
| **Oauth 2 Allow Url Path Matching** | Specifies whether, as part of OAuth 2.0 token requests, Azure AD will allow path matching of the redirect URI against the application's replyUrls. The default is false. |
| **Oauth 2 Require Post Response** | Set this to true if an Oauth2 post response is required. |
| **Public Client** | Specifies whether this application is a public client \(such as an installed application running on a mobile device\). Default is false. |
| **Reply URLs** | Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to. |
| **Saml Metadata Url** | The URL to the SAML metadata for the application. |

### Group Lifecycle Policy

| Name | Description |
| :--- | :--- |
| **Group Lifetime In Days** | The number of days a group can exist before it needs to be renewed. |
| **Managed Group Types** | This property allows the admin to select which office 365 groups the policy will apply to. 'None' will create the policy in a disabled state. 'All' will apply the policy to every Office 365 group in the tenant. 'Selected' will allow the admin to choose specific Office 365 groups that the policy will apply to. |
| **Alternate Notification Emails** | Notification emails for groups that have no owners will be sent to these email addresses. |

### Group Naming Policy

| Name | Description |
| :--- | :--- |
| **Prefix Suffix Naming Requirement** | Prefixes and suffixes to add to the group name. |
| **Custom Blocked Words List** | Comma delimited list of words that should be blocked from being included in groups' names. |

### Group Settings

| Name | Description |
| :--- | :--- |
| **Enable Group Creation** | The flag indicating whether Office 365 group creation is allowed in the directory by non-admin users. This setting does not require an Azure Active Directory Premium P1 license. |
| **Allow Guests To Be Group Owner** | Boolean indicating whether or not a guest user can be an owner of groups. |
| **Allow Guests To Access Groups** | Boolean indicating whether or not a guest user can have access to Office 365 groups content. This setting does not require an Azure Active Directory Premium P1 license. |
| **Guest Usage Guidelines Url** | The url of a link to the guest usage guidelines. |
| **Group Creation Allowed Group Name** | Name of the security group for which the members are allowed to create Office 365 groups even when 'Enable Group Creation' == false. |
| **Allow To Add Guests** | A boolean indicating whether or not is allowed to add guests to this directory. |
| **Usage Guidelines Url** | A link to the Group Usage Guidelines. |

### Groups

| Name | Description |
| :--- | :--- |
| **Display Name** | DisplayName of the AADMS Group. |
| **Mail Nickname** | Specifies a mail nickname for the group. If 'Mail Enabled' is False you must still specify a mail nickname. |
| **Description** | Specifies a description for the group. |
| **Group Types** | Specifies that the group is a dynamic group. To create a dynamic group, specify a value of DynamicMembership. |
| **Visibility** | This property determines the visibility of the group's content and members list. |
| **Membership Rule** | Specifies the membership rule for a dynamic group. |
| **Security Enabled** | Specifies whether the group is security enabled. For security groups, this value must be True. |
| **Mail Enabled** | Specifies whether this group is mail enabled. Currently, you cannot create mail enabled groups in Azure AD. |

