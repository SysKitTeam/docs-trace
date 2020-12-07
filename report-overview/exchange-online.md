---
title: Exchange Online
description: >-
  This article lists the currently supported Exchange Online reports with all of
  the properties that SysKit Trace loads.
date: 9/22/2020
---

# Exchange Online

## Reports

### Accepted Domains

| Name | Description |
| :--- | :--- |
| **Name** | Specify the Fully Qualified Domain Name for the accepted domain. |
| **Domain Type** | The type of accepted domain.  Currently the EXOAcceptedDomain DSC Resource accepts a value of 'Authoritative' and 'InternalRelay'. |
| **Match Sub Domains** | The 'Match Sub Domains' property must be false on Authoritative domains. The default value is false. |
| **Outbound Only** | The 'Outbound Only' must be false on Authoritative domains. The default value is false. |

### Address Book Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name that you want this address book policy to be called. |
| **Address Lists** | The 'Address Lists' property specifies the address lists that will be used by mailbox users who are assigned this address book policy. This property accepts multiple values. |
| **Global Address List** | The 'Global Address List' property specifies the identity of the global address list \(GAL\) that will be used by mailbox users who are assigned this address book policy. You can specify only one GAL for each address book policy. |
| **Offline Address Book** | The 'Offline Address Book' property specifies the identity of the offline address book \(OAB\) that will be used by mailbox users who are assigned this address book policy. You can specify only one OAB for each address book policy. |
| **Room List** | The 'Room List' property specifies the name of the room address list. |

### Address Lists

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies a unique name for the address list. |
| **Conditional Company** | The 'Conditional Company' property specifies a precanned filter that's based on the value of the recipient's Company property. |
| **Conditional Custom Attribute 1** | The 'Conditional Custom Attribute 1' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute1 property. |
| **Conditional Custom Attribute 10** | The 'Conditional Custom Attribute 10' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute10 property. |
| **Conditional Custom Attribute 11** | The 'Conditional Custom Attribute 11' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute11 property. |
| **Conditional Custom Attribute 12** | The 'Conditional Custom Attribute 12' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute12 property. |
| **Conditional Custom Attribute 13** | The 'Conditional Custom Attribute 13' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute13 property. |
| **Conditional Custom Attribute 14** | The 'Conditional Custom Attribute 14' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute14 property. |
| **Conditional Custom Attribute 15** | The 'Conditional Custom Attribute 15' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute15 property. |
| **Conditional Custom Attribute 2** | The 'Conditional Custom Attribute 2' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute2 property. |
| **Conditional Custom Attribute 3** | The 'Conditional Custom Attribute 3' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute3 property. |
| **Conditional Custom Attribute 4** | The 'Conditional Custom Attribute 4' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute4 property. |
| **Conditional Custom Attribute 5** | The 'Conditional Custom Attribute 5' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute5 property. |
| **Conditional Custom Attribute 6** | The 'Conditional Custom Attribute 6' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute6 property. |
| **Conditional Custom Attribute 7** | The 'Conditional Custom Attribute 7' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute7 property. |
| **Conditional Custom Attribute 8** | The 'Conditional Custom Attribute 8' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute8 property. |
| **Conditional Custom Attribute 9** | The 'Conditional Custom Attribute 9' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute9 property. |
| **Conditional Department** | The 'Conditional Department' property specifies a precanned filter that's based on the value of the recipient's Department property. |
| **Conditional State Or Province** | The 'Conditional State Or Province' property specifies a precanned filter that's based on the value of the recipient's StateOrProvince property. |
| **Display Name** | The 'Display Name' property specifies the display name of the address list. |
| **Included Recipients** | The 'Included Recipients' property specifies a precanned filter that's based on the recipient type. |
| **Recipient Filter** | The 'Recipient Filter' property specifies a custom OPath filter that's based on the value of any available recipient property. |

### Advanced Threat Protection Policy

| Name | Description |
| :--- | :--- |
| **Enabled For SharePoint, Teams, OneDrive** | The 'Enabled For SharePoint, Teams, OneDrive' property specifies whether ATP is enabled for SharePoint Online, OneDrive for Business and Microsoft Teams. Default is False. |
| **Enable Safe Links For Clients** | The 'Enable Safe Links For Clients' property specifies whether Safe Links is enabled for Office 365 ProPlus clients. Default is False. |
| **Block Urls** | The 'Block Urls' property specifies the URLs that are always blocked by Safe Links scanning. You can specify multiple values separated by commas. |
| **Track Clicks** | The 'Track Clicks' property specifies whether to track user clicks related to blocked URLs. Default is True. |
| **Allow Click Through** | The 'Allow Click Through' property specifies whether to allow users to click through to the original blocked URL in Office 365 ProPlus. Default is True. |

### Anti Phish Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the antiphishing policy that you want to modify. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. |
| **Phish Threshold Level** | The 'Phish Threshold Level' property specifies the tolerance level that's used by machine learning in the handling of phishing messages. |
| **Authentication Fail Action** | The 'Authentication Fail Action' property specifies the action to take when the message fails composite authentication. |
| **Targeted Domain Protection Action** | The 'Targeted Domain Protection Action' property specifies the action to take on detected domain impersonation messages for the domains specified by the 'Targeted Domains To Protect' parameter. |
| **Targeted User Protection Action** | The 'Targeted User Protection Action' property specifies the action to take on detected user impersonation messages for the users specified by the 'Targeted Users To Protect' parameter. |
| **Enabled** | Specify if this policy should be enabled. Default is True. |
| **Enable Antispoof Enforcement** | The 'Enable Antispoof Enforcement' property specifies whether to enable or disable antispoofing protection for the policy. |
| **Enable Mailbox Intelligence** | The 'Enable Mailbox Intelligence' property specifies whether to enable or disable mailbox intelligence \(the first contact graph\) in domain and user impersonation protection. |
| **Enable Organization Domains Protection** | The 'Enable Organization Domains Protection' property specifies whether to enable domain impersonation protection for all registered domains in the Office 365 organization. |
| **Enable Similar Domains Safety Tips** | The 'Enable Similar Domains Safety Tips' property specifies whether to enable safety tips that are shown to recipients in messages for domain impersonation detections. |
| **Enable Similar Users Safety Tips** | The 'Enable Similar Users Safety Tips' property specifies whether to enable safety tips that are shown to recipients in messages for user impersonation detections. |
| **Enable Targeted Domains Protection** | The 'Enable Targeted Domains Protection' property specifies whether to enable domain impersonation protection for a list of specified domains. |
| **Enable Targeted User Protection** | The 'Enable Targeted User Protection' property specifies whether to enable user impersonation protection for the users specified by the 'Targeted Users To Protect' parameter. |
| **Enable Unusual Characters Safety Tips** | The 'Enable Unusual Characters Safety Tips' property specifies whether to enable safety tips that are shown to recipients in messages for unusual characters in domain and user impersonation detections. |
| **Is Default** | Make this the default antiphishing policy. |
| **Excluded Domains** | The 'Excluded Domains' property specifies trusted domains that are excluded from scanning by antiphishing protection. You can specify multiple domains separated by commas. |
| **Excluded Senders** | The 'Excluded Senders' property specifies a list of trusted sender email addresses that are excluded from scanning by antiphishing protection. You can specify multiple email addresses separated by commas. |
| **Targeted Domain Action Recipients** | The 'Targeted Domain Action Recipients' property specifies the recipients to add to detected domain impersonation messages when the 'Targeted Domain Protection Action' property is set to the value Redirect or BccMessage. A valid value for this property is an email address. You can specify multiple email addresses separated by commas. |
| **Targeted Domains To Protect** | The 'Targeted Domains To Protect' property specifies the domains that are included in domain impersonation protection when the 'Enable Targeted Domains Protection' property is set to True. |
| **Targeted User Action Recipients** | The 'Targeted User Action Recipients' property specifies the replacement or additional recipients for detected user impersonation messages when the 'Targeted User Protection Action' property is set to the value Redirect or BccMessage. A valid value for this property is an email address. You can specify multiple email addresses separated by commas. |
| **Targeted Users To Protect** | The 'Targeted Users To Protect' property specifies the users that are included in user impersonation protection when the 'Enable Targeted User Protection' property is set to True. |

### Anti Spam Settings

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the Hosted Content Filter Policy that you want to modify. |
| **Is Default** | The 'Is Default' property makes the specified content filter policy the default content filter policy. The default value is False. |
| **Add X Header Value** | The 'Add X Header Value' property specifies the X-header value to add to spam messages when an action property is set to the value AddXHeader. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. |
| **Allowed Sender Domains** | The 'Allowed Sender Domains' property specifies trusted domains that aren't processed by the spam filter. |
| **Allowed Senders** | The 'Allowed Senders' property specifies a list of trusted senders that aren't processed by the spam filter. |
| **Blocked Sender Domains** | The 'Blocked Sender Domains' property specifies domains that are always marked as spam sources. |
| **Blocked Senders** | The 'Blocked Senders' property specifies senders that are always marked as spam sources. |
| **Bulk Spam Action** | The 'Bulk Spam Action' property specifies the action to take on messages that are classified as bulk email. |
| **Bulk Threshold** | The 'Bulk Threshold' property specifies the Bulk Complaint Level \(BCL\) threshold setting. Valid values are from 1 - 9, where 1 marks most bulk email as spam, and 9 allows the most bulk email to be delivered. The default value is 7. |
| **Download Link** | The 'Download Link' property shows or hides a link in end-user spam notification messages to download the Junk Email Reporting Tool plugin for Outlook. Valid input for this property is True or False. The default value is False. |
| **Enable End User Spam Notifications** | The 'Enable End User Spam Notification' property enables for disables sending end-user spam quarantine notification messages. Valid input for this property is True or False. The default value is False. |
| **Enable Language Block List** | The 'Enable Language Block List' property enables or disables blocking email messages that are written in specific languages, regardless of the message contents. Valid input for this property is True or False. The default value is False. |
| **Enable Region Block List** | The 'Enable Region Block List' property enables or disables blocking email messages that are sent from specific countries or regions, regardless of the message contents. Valid input for this property is True or False. The default value is False. |
| **End User Spam Notification Custom From Address** | The 'End User Spam Notification Custom From Address' property specifies a custom From address for end-user spam notification messages. Valid input for this property is an SMTP email address or an empty string. |
| **End User Spam Notification Custom From Name** | The 'End User Spam Notification Custom From Name' property specifies a custom display name in the From field for end-user spam notification messages. |
| **End User Spam Notification Custom Subject** | The 'End User Spam Notification Custom Subject' property specifies a custom subject for end-user spam notification messages. |
| **End User Spam Notification Frequency** | The 'End User Spam Notification Frequency' property specifies the repeat interval in days that end-user spam notification messages are sent. Valid input for this property is an integer between 1 and 15. The default value is 3. |
| **End User Spam Notification Language** | The 'End User Spam Notification Language' property specifies the language of end-user spam notification messages. The default value is Default. This means the default language of end-user spam notification messages is the default language of the cloud-based organization. |
| **High Confidence Spam Action** | The 'High Confidence Spam Action' property specifies the action to take on messages that are classified as high confidence spam. |
| **Increase Score With Biz Or Info Urls** | The 'Increase Score With Biz Or Info Urls' property increases the spam score of messages that contain links to .biz or .info domains. Valid values for this property are Off, On or Test. The default value is Off. |
| **Increase Score With Image Links** | The 'Increase Score With Image Links' property increases the spam score of messages that contain image links to remote websites. Valid values for this property are Off, On or Test. The default value is Off. |
| **Increase Score With Numeric Ips** | The 'Increase Score With Numeric Ips' property increases the spam score of messages that contain links to IP addresses. Valid values for this property are Off, On or Test. The default value is Off. |
| **Increase Score With Redirect To Other Port** | The 'Increase Score With Redirect To Other Port' property increases the spam score of messages that contain links that redirect to other TCP ports. Valid values for this property are Off, On or Test. The default value is Off. |
| **Inline Safety Tips Enabled** | The 'Inline Safety Tips Enabled' property specifies whether to enable or disable safety tips that are shown to recipients in messages. The default is True. |
| **Language Block List** | The 'Language Block List' property specifies the languages to block when messages are blocked based on their language. Valid input for this property is a supported ISO 639-1 lowercase two-letter language code. You can specify multiple values separated by commas. This property is only use when the 'Enable Region Block List' property is set to True. |
| **Mark As Spam Bulk Mail** | The 'Mark As Spam Bulk Mail' property classifies the message as spam when the message is identified as a bulk email message. Valid values for this property are Off, On or Test. The default value is On. |
| **Mark As Spam Embed Tags In Html** | The 'Mark As Spam Embed Tags In Html' property classifies the message as spam when the message contains HTML &lt;embed&gt; tags. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Empty Messages** | The 'Mark As Spam Empty Messages' property classifies the message as spam when the message is empty. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Form Tags In Html** | The 'Mark As Spam Form Tags In Html' property classifies the message as spam when the message contains HTML &lt;form&gt; tags. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Frames In Html** | The 'Mark As Spam Frames In Html' property classifies the message as spam when the message contains HTML &lt;frame&gt; or &lt;iframe&gt; tags. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam From Address Auth Fail** | The 'Mark As Spam From Address Auth Fail' property classifies the message as spam when Sender ID filtering encounters a hard fail. Valid values for this property are Off or On. The default value is Off. |
| **Mark As Spam JavaScript In Html** | The 'Mark As Spam JavaScript In Html' property classifies the message as spam when the message contains JavaScript or VBScript. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Ndr Backscatter** | The 'Mark As Spam Ndr Backscatter' property classifies the message as spam when the message is a non-delivery report \(NDR\) to a forged sender. Valid values for this property are Off or On. The default value is Off. |
| **Mark As Spam Object Tags In Html** | The 'Mark As Spam Object Tags In Html' property classifies the message as spam when the message contains HTML &lt;object&gt; tags. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Sensitive Word List** | The 'Mark As Spam Sensitive Word List' property classifies the message as spam when the message contains words from the sensitive words list. Valid values for this property are Off, On or Test. The default value is Off. |
| **Mark As Spam Spf Record Hard Fail** | The 'Mark As Spam Spf Record Hard Fail' property classifies the message as spam when Sender Policy Framework \(SPF\) record checking encounters a hard fail. Valid values for this property are Off or On. The default value is Off. |
| **Mark As Spam Web Bugs In Html** | The 'Mark As Spam Web Bugs In Html' property classifies the message as spam when the message contains web bugs. Valid values for this property are Off, On or Test. The default value is Off. |
| **Modify Subject Value** | The 'Modify Subject Value' property specifies the text to prepend to the existing subject of spam messages when an action property is set to the value ModifySubject. |
| **Phish Spam Action** | The 'Phish Spam Action' property specifies the action to take on messages that are classified as phishing. |
| **Quarantine Retention Period** | The 'Quarantine Retention Period' property specifies the length of time in days that spam messages remain in the quarantine. Valid input for this property is an integer between 1 and 30. The default value is 15. |
| **Redirect To Recipients** | The 'Redirect To Recipients' property specifies the replacement recipients in spam messages when an action property is set to the value Redirect. The action parameters that use the value of 'Redirect To Recipients' are 'High Confidence Spam Action' and SpamAction. |
| **Region Block List** | The 'Region Block List' property specifies the region to block when messages are blocked based on their source region. Valid input for this property is a supported ISO 3166-1 uppercase two-letter country code. You can specify multiple values separated by commas. This property is only used when the 'Enable Region Block List' property is set to True. |
| **Spam Action** | The 'Spam Action' property specifies the action to take on messages that are classified as spam \(not high confidence spam, bulk email, or phishing\). |
| **Test Mode Action** | The 'Test Mode Action' property specifies the additional action to take on messages that match any of the IncreaseScoreWith or MarkAsSpam parameters that are set to the value Test. |
| **Test Mode Bcc To Recipients** | The 'Test Mode Bcc To Recipients' property specifies the blind carbon copy recipients to add to spam messages when the 'Test Mode Action' action property is set to the value BccMessage. |
| **Zap Enabled** | The 'Zap Enabled' property specifies whether to enable zero-hour auto purge \(ZAP\) for spam. ZAP detects unread spam messages that have already been delivered to the user's Inbox. The default value is True. |

### Application Access Policies

| Name | Description |
| :--- | :--- |
| **App ID** | The 'App ID' property specifies the GUID of the apps to include in the policy. |
| **Policy Scope Group Id** | The 'Policy Scope Group Id' property specifies the recipient to define in the policy. You can use any value that uniquely identifies the recipient. |
| **Access Right** | The 'Access Right' property specifies the permission that you want to assign in the application access policy. |
| **Description** | The 'Description' property specifies a description for the policy. |

### Availability Address Spaces

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the availability address space you want to modify. |
| **Access Method** | The 'Access Method' property specifies how the free/busy data is accessed. Valid values are: PerUserFB, OrgWideFB, OrgWideFBBasic, InternalProxy. |
| **Credentials** | The 'Credentials' property specifies the username and password that's used to access the Availability services in the target forest. |
| **Forest Name** | The 'Forest Name' property specifies the SMTP domain name of the target forest for users whose free/busy data must be retrieved. If your users are distributed among multiple SMTP domains in the target forest, run the Add-AvailabilityAddressSpace command once for each SMTP domain. |
| **Target Autodiscover Epr** | The 'Target Autodiscover Epr' property specifies the Autodiscover URL of Exchange Web Services for the external organization. Exchange uses Autodiscover to automatically detect the correct server endpoint for external requests. |

### Availability Config

| Name | Description |
| :--- | :--- |
| **Org Wide Account** | Specify the 'Org Wide Account' for the availability config. |

### CAS Mailbox Plans

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the CAS Mailbox Plan that you want to modify. |
| **Active Sync Enabled** | The 'Active Sync Enabled' property enables or disables access to the mailbox by using Exchange Active Sync. Default is True. |
| **IMAP Enabled** | The 'IMAP Enabled' property enables or disables access to the mailbox by using IMAP4 clients. The default value is True for all CAS mailbox plans except ExchangeOnlineDeskless which is False by default. |
| **OWA Mailbox Policy** | The 'OWA Mailbox Policy' property specifies the Outlook on the web \(formerly known as Outlook Web App\) mailbox policy for the mailbox plan. The default value is OwaMailboxPolicy-Default. You can use the Get-OwaMailboxPolicy cmdlet to view the available Outlook on the web mailbox policies. |
| **POP Enabled** | The 'POP Enabled' property enables or disables access to the mailbox by using POP3 clients. Default is True. |

### Client Access Rules

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the client access rule that you want to modify. |
| **Action** | The 'Action' property specifies the action for the client access rule. Valid values for this property are AllowAccess and DenyAccess. |
| **Any Of Authentication Types** | The 'Any Of Authentication Types' property specifies a condition for the client access rule that is based on the client's authentication type. Valid values for this property are AdfsAuthentication, BasicAuthentication, CertificateBasedAuthentication, NonBasicAuthentication, OAuthAuthentication. |
| **Any Of Client IP Addresses Or Ranges** | The 'Any Of Client IP Addresses Or Ranges' property specifies a condition for the client access rule that is based on the client's IP address. Valid values for this property are: A single IP address, an IP address range, a CIDR IP. |
| **Any Of Protocols** | The 'Any Of Protocols' property specifies a condition for the client access rule that is based on the client's protocol. Valid values for this property are ExchangeActiveSync, ExchangeAdminCenter, ExchangeWebServices, IMAP4, OfflineAddressBook, OutlookAnywhere, OutlookWebApp, POP3, PowerShellWebServices, RemotePowerShell, REST, UniversalOutlook. |
| **Enabled** | The 'Enabled' property specifies whether the client access rule is enabled or disabled. Default is True. |
| **Except Any Of Authentication Types** | The 'Except Any Of Authentication Types' property specifies an exception for the client access rule that is based on the client's authentication type. Valid values for this property are AdfsAuthentication, BasicAuthentication, CertificateBasedAuthentication, NonBasicAuthentication, OAuthAuthentication. |
| **Except Any Of Client IP Addresses Or Ranges** | The 'Except Any Of Client IP Addresses Or Ranges' property specifies an exception for the client access rule that is based on the client's IP address. Valid values for this property are: A single IP address, an IP address range, a CIDR IP. |
| **Except Any Of Protocols** | The 'Except Any Of Protocols' property specifies an exception for the client access rule that is based on the client's protocol. Valid values for this property are ExchangeActiveSync, ExchangeAdminCenter, ExchangeWebServices, IMAP4, OfflineAddressBook, OutlookAnywhere, OutlookWebApp, POP3, PowerShellWebServices, RemotePowerShell, REST, UniversalOutlook. |
| **Except Username Matches Any Of Patterns** | The 'Except Username Matches Any Of Patterns' property specifies an exception for the client access rule that is based on the user's account name. |
| **Priority** | The 'Priority' property specifies a priority value for the client access rule. A lower integer value indicates a higher priority, and a higher priority rule is evaluated before a lower priority rule. The default value is 1. |
| **Rule Scope** | The 'Rule Scope' property specifies the scope of the client access rule. Valid values are All and Users. |
| **User Recipient Filter** | The 'User Recipient Filter' property specifies a condition for the client access rule that uses OPath filter syntax to identify the user. |
| **Username Matches Any Of Patterns** | The 'Username Matches Any Of Patterns' property specifies a condition for the client access rule that is based on the user's account name. |

### DKIM Signing Config

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the DKIM signing policy that you want to modify.  This should be the FQDN. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. |
| **Body Canonicalization** | The 'Body Canonicalization' property specifies the canonicalization algorithm that's used to create and verify the message body part of the DKIM signature. This value effectively controls the sensitivity of DKIM to changes to the message body in transit. Valid values are 'Simple' or 'Relaxed'.  'Relaxed' is the default. |
| **Header Canonicalization** | The 'Header Canonicalization' property specifies the canonicalization algorithm that's used to create and verify the message header part of the DKIM signature. This value effectively controls the sensitivity of DKIM to changes to the message headers in transit. Valid values are 'Simple' or 'Relaxed'.  'Relaxed' is the default. |
| **Key Size** | The 'Key Size' property specifies the size in bits of the public key that's used in the DKIM signing policy. The only available value is 1024. |
| **Enabled** | The 'Enabled' property specifies whether the DKIM Signing Configuration is enabled or disabled. Default is True. |

### Email Address Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name of the email address policy. The maximum length is 64 characters. |
| **Priority** | The 'Priority' property specifies the order that the email address policies are evaluated. By default, every time that you add a new email address policy, the policy is assigned a priority of N+1, where N is the number of email address policies that you've created. |
| **Enabled Email Address Templates** | The 'Enabled Email Address Templates' property specifies the rules in the email address policy that are used to generate email addresses for recipients. |
| **Enabled Primary SMTP Address Template** | The 'Enabled Primary SMTP Address Template' property specifies the specifies the rule in the email address policy that's used to generate the primary SMTP email addresses for recipients. You can use this property instead of the 'Enabled Email Address Templates' if the policy only applies the primary email address and no additional proxy addresses. |
| **Managed By Filter** | The 'Managed By Filter' property specifies the email address policies to apply to Office 365 groups based on the properties of the users who create the Office 365 groups. |

### Global Address Lists

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name of the GAL. The maximum length is 64 characters. |
| **Conditional Company** | The 'Conditional Company' property specifies a precanned filter that's based on the value of the recipient's Company property. |
| **Conditional Custom Attribute 1** | The 'Conditional Custom Attribute 1' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute1 property. |
| **Conditional Custom Attribute 10** | The 'Conditional Custom Attribute 10' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute10 property. |
| **Conditional Custom Attribute 11** | The 'Conditional Custom Attribute 11' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute11 property. |
| **Conditional Custom Attribute 12** | The 'Conditional Custom Attribute 12' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute12 property. |
| **Conditional Custom Attribute 13** | The 'Conditional Custom Attribute 13' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute13 property. |
| **Conditional Custom Attribute 14** | The 'Conditional Custom Attribute 14' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute14 property. |
| **Conditional Custom Attribute 15** | The 'Conditional Custom Attribute 15' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute15 property. |
| **Conditional Custom Attribute 2** | The 'Conditional Custom Attribute 2' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute2 property. |
| **Conditional Custom Attribute 3** | The 'Conditional Custom Attribute 3' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute3 property. |
| **Conditional Custom Attribute 4** | The 'Conditional Custom Attribute 4' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute4 property. |
| **Conditional Custom Attribute 5** | The 'Conditional Custom Attribute 5' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute5 property. |
| **Conditional Custom Attribute 6** | The 'Conditional Custom Attribute 6' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute6 property. |
| **Conditional Custom Attribute 7** | The 'Conditional Custom Attribute 7' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute7 property. |
| **Conditional Custom Attribute 8** | The 'Conditional Custom Attribute 8' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute8 property. |
| **Conditional Custom Attribute 9** | The 'Conditional Custom Attribute 9' property specifies a precanned filter that's based on the value of the recipient's CustomAttribute9 property. |
| **Conditional Department** | The 'Conditional Department' property specifies a precanned filter that's based on the value of the recipient's Department property. |
| **Conditional State Or Province** | The 'Conditional State Or Province' property specifies a precanned filter that's based on the value of the recipient's StateOrProvince property. |
| **Included Recipients** | The 'Included Recipients' property specifies a precanned filter that's based on the recipient type. |
| **Recipient Filter** | The 'Recipient Filter' property specifies an OPath filter that's based on the value of any available recipient property. |

### Hosted Connection Filter Policy

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the Hosted Connection Filter Policy that you want to modify. |
| **Is Default** | The 'Is Default' property makes the specified policy the default connection filter policy. Default is False. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. |
| **Enable Safe List** | The 'Enable Safe List' property enables or disables use of the safe list. The safe list is a dynamic allow list in the Microsoft datacenter that requires no customer configuration. Valid input for this property is True or False. The default value is False. |
| **IP Allow List** | The 'IP Allow List' property specifies IP addresses from which messages are always allowed. Messages from the IP addresses you specify won't be identified as spam, despite any other spam characteristics of the messages. Valid values for this property are: A single IP address, an IP address range, a CIDR IP. |
| **IP Block List** | The 'IP Block List' property specifies IP addresses from which messages are never allowed. Messages from the IP addresses you specify are blocked without any further spam scanning. Valid values for this property are: A single IP address, an IP address range, a CIDR IP. |

### Hosted Outbound Spam Filter Policy

| Name | Description |
| :--- | :--- |
| **Bcc Suspicious Outbound Additional Recipients** | The 'Bcc Suspicious Outbound Additional Recipients' property specifies the recipients to add to the Bcc field of outgoing spam messages. Valid input for this property is an email address. Separate multiple email addresses with commas. |
| **Bcc Suspicious Outbound Mail** | The 'Bcc Suspicious Outbound Mail' property enables or disables adding recipients to the Bcc field of outgoing spam messages. Valid input for this property is True or False. The default value is False. You specify the additional recipients using the 'Bcc Suspicious Outbound Additional Recipients' parameter. |
| **Notify Outbound Spam** | The 'Notify Outbound Spam' property enables or disables sending notification messages to administrators when an outgoing message is determined to be spam. Valid input for this property is True or False. The default value is False. You specify the administrators to notify by using the 'Notify Outbound Spam Recipients' parameter. |
| **Notify Outbound Spam Recipients** | The 'Notify Outbound Spam Recipients' property specifies the administrators to notify when an outgoing message is determined to be spam. Valid input for this property is an email address. Separate multiple email addresses with commas. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. |

### Individual Sharing Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name of the sharing policy. The maximum length is 64 characters. |
| **Default** | The 'Default' switch specifies that the sharing policy is the default sharing policy for all mailboxes. |
| **Enabled** | The 'Enabled' property specifies whether to enable the sharing policy. Valid values for this property are True or False. |
| **Domains** | The 'Domains' property specifies domains to which this policy applies and the sharing policy action. |

### Mail Tips

| Name | Description |
| :--- | :--- |
| **Mail Tips All Tips Enabled** | Specifies whether MailTips are enabled. |
| **Mail Tips Group Metrics Enabled** | Specifies whether MailTips that rely on group metrics data are enabled. |
| **Mail Tips Large Audience Threshold** | Specifies what a large audience is. |
| **Mail Tips Mailbox Sourced Tips Enabled** | Specifies whether MailTips that rely on mailbox data \(out-of-office or full mailbox\) are enabled. |
| **Mail Tips External Recipients Tips Enabled** | Specifies whether MailTips for external recipients are enabled. |

### Mailbox Settings

| Name | Description |
| :--- | :--- |
| **Display Name** | The display name of the Shared Mailbox. |
| **Time Zone** | The name of the Time Zone to assign to the mailbox. |
| **Locale** | The code of the 'Locale' to assign to the mailbox. |

### Malware Filter Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the malware filter policy you want to modify. |
| **Action** | The 'Action' property specifies the action to take when malware is detected in a message. Possible values are DeleteMessage, DeleteAttachmentAndUseDefaultAlertText and DeleteAttachmentAndUseCustomAlertText. The default value is DeleteMessage. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description for the policy. If the value contains spaces, enclose the value in quotation marks. |
| **Custom Alert Text** | The 'Custom Alert Text' property specifies the custom text to use in the replacement attachment named Malware Alert Text.txt. If the value contains spaces, enclose the value in quotation marks. |
| **Custom External Body** | The 'Custom External Body' property specifies the body of the custom notification message for malware detections in messages from external senders. If the value contains spaces, enclose the value in quotation marks. |
| **Custom External Subject** | The 'Custom External Subject' property specifies the subject of the custom notification message for malware detections in messages from external senders. If the value contains spaces, enclose the value in quotation marks. |
| **Custom From Address** | The 'Custom From Address' property specifies the From address of the custom notification message for malware detections in messages from internal or external senders. |
| **Custom From Name** | The 'Custom From Name' property specifies the From name of the custom notification message for malware detections in messages from internal or external senders. If the value contains spaces, enclose the value in quotation marks. |
| **Custom Internal Body** | The 'Custom Internal Body' property specifies the body of the custom notification message for malware detections in messages from internal senders. If the value contains spaces, enclose the value in quotation marks. |
| **Custom Internal Subject** | The 'Custom Internal Subject' property specifies the subject of the custom notification message for malware detections in messages from internal senders. If the value contains spaces, enclose the value in quotation marks. |
| **Custom Notifications** | The 'Custom Notifications' property enables or disables custom notification messages for malware detections in messages from internal or external senders. Valid values are: True\|False. |
| **Enable External Sender Admin Notifications** | The 'Enable External Sender Admin Notifications' property enables or disables sending malware detection notification messages to an administrator for messages from external senders. Valid values are: True\|False. |
| **Enable External Sender Notifications** | The 'Enable External Sender Notifications' property enables or disables notification messages for malware detections in messages from external senders. Valid values are: True\|False. |
| **Enable File Filter** | The 'Enable File Filter' property enables or disables common attachment blocking - also known as the Common Attachment Types Filter. Valid values are: True\|False. |
| **Enable Internal Sender Admin Notifications** | The 'Enable Internal Sender Admin Notifications' property enables or disables sending malware detection notification messages to an administrator for messages from internal senders. Valid values are: True \| False. |
| **Enable Internal Sender Notifications** | The 'Enable Internal Sender Notifications' property enables or disables notification messages for malware detections in messages from internal senders. Valid values are: True\|False. |
| **External Sender Admin Address** | The 'External Sender Admin Address' property specifies the email address of the administrator who will receive notification messages for malware detections in messages from external senders. |
| **File Types** | The 'File Types' property specifies the file types that are automatically blocked by common attachment blocking \(also known as the Common Attachment Types Filter\), regardless of content. |
| **Internal Sender Admin Address** | The 'Internal Sender Admin Address' property specifies the email address of the administrator who will receive notification messages for malware detections in messages from internal senders. |
| **Is Default** | MakeDefault makes this malware filter policy the default policy. Valid values are: True\|False. |
| **Zap Enabled** | The 'Zap Enabled' property enables or disables zero-hour auto purge \(ZAP\) for malware. ZAP detects malware in unread messages that have already been delivered to the user's Inbox. Valid values are: True\|False. |

### Management Roles

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the role. The maximum length of the name is 64 characters. |
| **Parent** | The 'Parent' property specifies the identity of the role to copy. |
| **Description** | The 'Description' property specifies the description that's displayed when the management role is viewed using the Get-ManagementRole cmdlet. |

### Offline Address Books

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name of the Offline Address Book. The maximum length is 64 characters. |
| **Address Lists** | The 'Address Lists' property specifies the address lists or global address lists that are included in the OAB. You can use any value that uniquely identifies the address list. |
| **Diff Retention Period** | The 'Diff Retention Period' property specifies the number of days that the OAB difference files are stored on the server. |
| **Is Default** | The 'Is Default' property specifies whether the OAB is used by all mailboxes and mailbox databases that don't have an OAB specified. |

### On-Premises Organizations

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the identity of the on-premises organization object. |
| **Hybrid Domains** | The 'Hybrid Domains' property specifies the domains that are configured in the hybrid deployment between an Office 365 tenant and an on-premises Exchange organization. The domains specified in this property must match the domains listed in the HybridConfiguration Active Directory object for the on-premises Exchange organization configured by the Hybrid Configuration wizard. |
| **Inbound Connector** | The 'Inbound Connector' property specifies the name of the inbound connector configured on the Microsoft Exchange Online Protection \(EOP\) service for a hybrid deployment configured with an on-premises Exchange organization. |
| **Outbound Connector** | The 'Outbound Connector' property specifies the name of the outbound connector configured on the EOP service for a hybrid deployment configured with an on-premises Exchange organization. |
| **Organization Name** | The 'Organization Name' property specifies the Active Directory object name of the on-premises Exchange organization. |
| **Organization Guid** | The 'Organization Guid' property specifies the globally unique identifier \(GUID\) of the on-premises Exchange organization object in the Office 365 tenant. |
| **Organization Relationship** | The 'Organization Relationship' property specifies the organization relationship configured by the Hybrid Configuration wizard on the Office 365 tenant as part of a hybrid deployment with an on-premises Exchange organization. This organization relationship defines the federated sharing features enabled on the Office 365 tenant. |
| **Comment** | The 'Comment' property specifies an optional comment. |

### Organization Config

| Name | Description |
| :--- | :--- |
| **Activity Based Authentication Timeout Enabled** | The 'Activity Based Authentication Timeout Enabled' property specifies whether the timed logoff feature is enabled. The default value is True. |
| **Activity Based Authentication Timeout Interval** | The 'Activity Based Authentication Timeout Interval' property specifies the time span for logoff. This valus is a time span: hh:mm:ss where hh = hours, mm = minutes and ss = seconds. Valid values for this property are from 00:05:00 to 08:00:00 \(5 minutes to 8 hours\). The default value is 06:00:00 \(6 hours\). |
| **Activity Based Authentication Timeout With Single Sign On Enabled** | The 'Activity Based Authentication Timeout With Single Sign On Enabled' property specifies whether to keep single sign-on enabled. The default value is True. |
| **Apps For Office Enabled** | The 'Apps For Office Enabled' property specifies whether to enable apps for Outlook features. By default, the property is set to True. If the flag is set to False, no new apps can be activated for any user in the organization. |
| **Async Send Enabled** | The 'Async Send Enabled' property specifies whether to enable or disable async send in Outlook on the web. |
| **Audit Disabled** | The 'Audit Disabled' property specifies whether to disable or enable mailbox auditing for the organization. |
| **Auto Expanding Archive** | The 'Auto Expanding Archive' switch enables the unlimited archiving feature \(called auto-expanding archiving\) in an Exchange Online organization. |
| **Bookings Enabled** | The 'Bookings Enabled' property specifies whether to enable Microsoft Bookings in an Exchange Online organization. |
| **Bookings Payments Enabled** | The 'Bookings Payments Enabled' property specifies whether to enable online payment node inside Bookings. |
| **Bookings Social Sharing Restricted** | The 'Bookings Social Sharing Restricted' property allows control of whether, or not, users can see social sharing options inside Bookings. |
| **Byte Encoder Type For 7 Bit Charsets** | The 'Byte Encoder Type For 7 Bit Charsets' property specifies the 7-bit transfer encoding method for MIME format for messages sent to this remote domain. |
| **Connectors Actionable Messages Enabled** | The 'Connectors Actionable Messages Enabled' property specifies whether to enable or disable actionable buttons in messages \(connector cards\) from connected apps on Outlook on the web. |
| **Connectors Enabled** | The 'Connectors Enabled' property specifies whether to enable or disable all connected apps in organization. |
| **Connectors Enabled For Outlook** | The 'Connectors Enabled For Outlook' property specifies whether to enable or disable connected apps in Outlook on the web. |
| **Connectors Enabled For SharePoint** | The 'Connectors Enabled For SharePoint' property specifies whether to enable or disable connected apps on Sharepoint. |
| **Connectors Enabled For Teams** | The 'Connectors Enabled For Teams' property specifies whether to enable or disable connected apps on Teams. |
| **Connectors Enabled For Yammer** | The 'Connectors Enabled For Yammer' property specifies whether to enable or disable connected apps on Yammer. |
| **Default Authentication Policy** | The 'Default Authentication Policy' property specifies the authentication policy that's used for the whole organization. |
| **Default Group Access Type** | The 'Default Group Access Type' property specifies the default access type for Office 365 groups. |
| **Default Public Folder Age Limit** | The 'Default Public Folder Age Limit' property specifies the default age limit for the contents of public folders across the entire organization. Content in a public folder is automatically deleted when this age limit is exceeded. This attribute applies to all public folders in the organization that don't have their own AgeLimit setting. This value is a time span: dd.hh:mm:ss where d = days, h = hours, m = minutes, and s = seconds. The value can also be null. The default value is blank \(null\). |
| **Default Public Folder Deleted Item Retention** | The 'Default Public Folder Deleted Item Retention' property specifies the default value of the length of time to retain deleted items for public folders across the entire organization. This attribute applies to all public folders in the organization that don't have their own RetainDeletedItemsFor attribute set. |
| **Default Public Folder Issue Warning Quota** | The 'Default Public Folder Issue Warning Quota' property specifies the default value across the entire organization for the public folder size at which a warning message is sent to this folder's owners, warning that the public folder is almost full. This attribute applies to all public folders within the organization that don't have their own warning quota attribute set. The default value of this attribute is unlimited. The valid input range for this property is from 0 through 2199023254529 bytes\(2 TB\). A value of unlimited specifies no size limit is imposed on the public folder. |
| **Default Public Folder Max Item Size** | The 'Default Public Folder Max Item Size' property specifies the default maximum size for posted items within public folders across the entire organization. Items larger than the value of the 'Default Public Folder Max Item Size' property are rejected. This attribute applies to all public folders within the organization that don't have their own MaxItemSize attribute set. The default value of this attribute is unlimited. |
| **Default Public Folder Moved Item Retention** | The 'Default Public Folder Moved Item Retention' property specifies how long items that have been moved between mailboxes are kept in the source mailbox for recovery purposes before being removed by the Public Folder Assistant. |
| **Default Public Folder Prohibit Post Quota** | The 'Default Public Folder Prohibit Post Quota' property specifies the size of a public folder at which users are notified that the public folder is full. Users can't post to a folder whose size is larger than the 'Default Public Folder Prohibit Post Quota' property value. The default value of this attribute is unlimited. |
| **Direct Reports Group Auto Creation Enabled** | The 'Direct Reports Group Auto Creation Enabled' property specifies whether to enable or disable the automatic creation of direct report Office 365 groups. |
| **Distribution Group Default OU** | The 'Distribution Group Default OU' property specifies the container where distribution groups are created by default. |
| **Distribution Group Name Blocked Words List** | The 'Distribution Group Name Blocked Words List' property specifies words that can't be included in the names of distribution groups. Separate multiple values with commas. |
| **Distribution Group Naming Policy** | The 'Distribution Group Naming Policy' property specifies the template applied to the name of distribution groups that are created in the organization. You can enforce that a prefix or suffix be applied to all distribution groups. Prefixes and suffixes can be either a string or an attribute, and you can combine strings and attributes. |
| **Elc Processing Disabled** | The 'Elc Processing Disabled' property specifies whether to enable or disable the processing of mailboxes by the Managed Folder Assistant. |
| **End User DL Upgrade Flows Disabled** | The 'End User DL Upgrade Flows Disabled' property specifies whether to prevent users from upgrading their own distribution groups to Office 365 groups in an Exchange Online organization. |
| **Ews Allow Entourage** | The 'Ews Allow Entourage' property specifies whether to enable or disable Entourage 2008 to access Exchange Web Services \(EWS\) for the entire organization. |
| **Ews Allow List** | The 'Ews Allow List' property specifies the applications that are allowed to access EWS or REST when the 'Ews Application Access Policy' property is set to EwsAllowList. Other applications that aren't specified by this property aren't allowed to access EWS or REST. You identify the application by its user agent string value. Wildcard characters \(\*\) are supported. |
| **Ews Allow Mac Outlook** | The 'Ews Allow Mac Outlook' property enables or disables access to mailboxes by Outlook for Mac clients that use Exchange Web Services \(for example, Outlook for Mac 2011 or later\). |
| **Ews Allow Outlook** | The 'Ews Allow Outlook' property enables or disables access to mailboxes by Outlook clients that use Exchange Web Services. Outlook uses Exchange Web Services for free/busy, out-of-office settings, and calendar sharing. |
| **Ews Application Access Policy** | The 'Ews Application Access Policy' property specifies the client applications that have access to EWS and REST. |
| **Ews Block List** | The 'Ews Block List' property specifies the applications that aren't allowed to access EWS or REST when the 'Ews Application Access Policy' property is set to EnforceBlockList. All other applications that aren't specified by this property are allowed to access EWS or REST. You identify the application by its user agent string value. Wildcard characters \(\*\) are supported. |
| **Ews Enabled** | The 'Ews Enabled' property specifies whether to globally enable or disable EWS access for the entire organization, regardless of what application is making the request. |
| **Exchange Notification Enabled** | The 'Exchange Notification Enabled' property enables or disables Exchange notifications sent to administrators regarding their organizations. Valid input for this property is True or False. |
| **Exchange Notification Recipients** | The 'Exchange Notification Recipients' property specifies the recipients for Exchange notifications sent to administrators regarding their organizations. If the 'Exchange Notification Enabled' property is set to False, no notification messages are sent. Multiple values are separated with commas. If this property isn't set, Exchange notifications are sent to all administrators. |
| **Focused Inbox On** | The 'Focused Inbox On' property enables or disables Focused Inbox for the organization. |
| **Hierarchical Address Book Root** | The 'Hierarchical Address Book Root' property specifies the user, contact, or group to be used as the root organization for a hierarchical address book in the Exchange organization. You can use any value that uniquely identifies the recipient. |
| **IP List Blocked** | The 'IP List Blocked' property specifies the blocked IP addresses that aren't allowed to connect to Exchange Online organization. These settings affect client connections that use Basic authentication where on-premises Active Directory Federation Services \(ADFS\) servers federate authentication with Azure Active Directory. Note that the new settings might take up to 4 hours to fully propagate across the service. |
| **Lean Popout Enabled** | The 'Lean Popout Enabled' property specifies whether to enable faster loading of pop-out messages in Outlook on the web for Internet Explorer and Microsoft Edge. |
| **Link Preview Enabled** | The 'Link Preview Enabled' property specifies whether link preview of URLs in email messages is allowed for the organization. |
| **Mail Tips All Tips Enabled** | The 'Mail Tips All Tips Enabled' property specifies whether MailTips are enabled. The default value is True. |
| **Mail Tips External Recipients Tips Enabled** | The 'Mail Tips External Recipients Tips Enabled' property specifies whether MailTips for external recipients are enabled. The default value is False. |
| **Mail Tips Group Metrics Enabled** | The 'Mail Tips Group Metrics Enabled' property specifies whether MailTips that rely on group metrics data are enabled. The default value is True. |
| **Mail Tips Large Audience Threshold** | The 'Mail Tips Large Audience Threshold' property specifies what a large audience is. The default value is 25. |
| **Mail Tips Mailbox Sourced Tips Enabled** | The 'Mail Tips Mailbox Sourced Tips Enabled' property specifies whether MailTips that rely on mailbox data \(out-of-office or full mailbox\) are enabled. |
| **OAuth2 Client Profile Enabled** | The 'OAuth2 Client Profile Enabled' property enables or disables modern authentication in the Exchange organization. |
| **Outlook Mobile GCC Restrictions Enabled** | The 'Outlook Mobile GCC Restrictions Enabled' property specifies whether to enable or disable features within Outlook for iOS and Android that are not FedRAMP compliant for Office 365 US Government Community Cloud \(GCC\) customers. |
| **Outlook Pay Enabled** | The 'Outlook Pay Enabled' property enables or disables Payments in Outlook in the Office 365 organization. |
| **Public Computers Detection Enabled** | The 'Public Computers Detection Enabled' property specifies whether Outlook on the web will detect when a user signs from a public or private computer or network, and then enforces the attachment handling settings from public networks. The default is False. However, if you set this property to True, Outlook on the web will determine if the user is signing in from a public computer, and all public attachment handling rules will be applied and enforced. |
| **Public Folders Enabled** | The 'Public Folders Enabled' property specifies how public folders are deployed in your organization. |
| **Public Folder Show Client Control** | The 'Public Folder Show Client Control' property enables or disables access to public folders in Microsoft Outlook. |
| **Read Tracking Enabled** | The 'Read Tracking Enabled' property specifies whether the tracking for read status for messages in an organization is enabled. The default value is False. |
| **Remote Public Folder Mailboxes** | The 'Remote Public Folder Mailboxes' property specifies the identities of the public folder objects \(represented as mail user objects locally\) corresponding to the public folder mailboxes created in the remote forest. The public folder values set here are used only if the public folder deployment is a remote deployment. |
| **Site Mailbox Creation URL** | The 'Site Mailbox Creation URL' property specifies the URL that's used to create site mailboxes. Site mailboxes improve collaboration and user productivity by allowing access to both SharePoint documents and Exchange email in Outlook 2013 or later. |
| **SMTP Actionable Messages Enabled** | The 'SMTP Actionable Messages Enabled' property specifies whether to enable or disable action buttons in email messages in Outlook on the web. |
| **Visible Meeting Update Properties** | The 'Visible Meeting Update Properties' property specifies whether meeting message updates will be auto-processed on behalf of attendees. Auto-processed updates are applied to the attendee's calendar item, and then the meeting message is moved to the deleted items. The attendee never sees the update in their inbox, but their calendar is updated. |
| **Web Push Notifications Disabled** | The 'Web Push Notifications Disabled' property specifies whether to enable or disable Web Push Notifications in Outlook on the Web. This feature provides web push notifications which appear on a user's desktop while the user is not using Outlook on the Web. This brings awareness of incoming messages while they are working elsewhere on their computer. |
| **Web Suggested Replies Disabled** | The 'Web Suggested Replies Disabled' property specifies whether to enable or disable Suggested Replies in Outlook on the web. This feature provides suggested replies to emails so users can easily and quickly respond to messages. |

### Organization Sharing Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name of the organization relationship. The maximum length is 64 characters. |
| **Archive Access Enabled** | The 'Archive Access Enabled' property specifies whether the organization relationship has been configured to provide remote archive access. |
| **Delivery Report Enabled** | The 'Delivery Report Enabled' property specifies whether Delivery Reports should be shared over the organization relationship. |
| **Domain Names** | The 'Domain Names' property specifies the SMTP domains of the external organization. The domains are separated by commas. |
| **Enabled** | The 'Enabled' property specifies whether to enable the organization relationship. |
| **Free Busy Access Enabled** | The 'Free Busy Access Enabled' property specifies whether the organization relationship should be used to retrieve free/busy information from the external organization. |
| **Free Busy Access Level** | The 'Free Busy Access Level' property specifies the maximum amount of detail returned to the requesting organization. Valid values are: None, AvailabilityOnly or LimitedDetails. |
| **Free Busy Access Scope** | The 'Free Busy Access Scope' property specifies a mail-enabled security group in the internal organization that contains users whose free/busy information is accessible by an external organization. You can use any value that uniquely identifies the group. |
| **Mailbox Move Enabled** | The 'Mailbox Move Enabled' property specifies whether the organization relationship enables moving mailboxes to or from the external organization. |
| **Mail Tips Access Enabled** | The 'Mail Tips Access Enabled' property specifies whether MailTips for users in this organization are returned over this organization relationship. |
| **Mail Tips Access Level** | The 'Mail Tips Access Level' property specifies the level of MailTips data externally shared over this organization relationship. This property can have the following values: All, Limited, None. |
| **Mail Tips Access Scope** | The 'Mail Tips Access Scope' property specifies a mail-enabled security group in the internal organization that contains users whose free/busy information is accessible by an external organization. You can use any value that uniquely identifies the group. |
| **Organization Contact** | The 'Organization Contact' property specifies the email address that can be used to contact the external organization \(for example, administrator@fourthcoffee.com\). |
| **Photos Enabled** | The 'Photos Enabled' property specifies whether photos for users in the internal organization are returned over the organization relationship. |
| **Target Application Uri** | The 'Target Application Uri' property specifies the target Uniform Resource Identifier \(URI\) of the external organization. The 'Target Application Uri' property is specified by Exchange when requesting a delegated token to retrieve free and busy information, for example, mail.contoso.com. |
| **Target Autodiscover Epr** | The 'Target Autodiscover Epr' property specifies the Autodiscover URL of Exchange Web Services for the external organization. Exchange uses Autodiscover to automatically detect the correct Exchangeserver endpoint to use for external requests. |
| **Target Owa URL** | The 'Target Owa URL' property specifies the Outlook on the web \(formerly Outlook Web App\) URL of the external organization that's defined in the organization relationship. It is used for Outlook on the web redirection in a cross-premise Exchange scenario. Configuring this attribute enables users in the organization to use their current Outlook on the web URL to access Outlook on the web in the external organization. |
| **Target Sharing Epr** | The 'Target Sharing Epr' property specifies the URL of the target Exchange Web Services for the external organization. |

### Outlook Web App Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the unique name for the policy. The maximum length is 64 characters. |
| **Action For Unknown File And MIME Types** | The 'Action For Unknown File And MIME Types' property specifies how to handle file types that aren't specified in the Allow, Block, and Force Save lists for file types and MIME types. |
| **Active Sync Integration Enabled** | The 'Active Sync Integration Enabled' property specifies whether to enable or disable Exchange ActiveSync settings in Outlook on the web. |
| **Additional Storage Providers Available** | The 'Additional Storage Providers Available' property specifies whether to allow additional storage providers \(for example, Box, Dropbox, Facebook, Google Drive, Egnyte, personal OneDrive\) attachments in Outlook on the web. |
| **All Address Lists Enabled** | The 'All Address Lists Enabled' property specifies which address lists are available in Outlook on the web. |
| **Allow Copy Contacts To Device Address Book** | The 'Allow Copy Contacts To Device Address Book' property specifies whether users can copy the contents of their Contacts folder to a mobile device's native address book when using Outlook on the web for devices. |
| **Classic Attachments Enabled** | The 'Classic Attachments Enabled' property specifies whether users can attach local files as regular email attachments in Outlook on the web. |
| **Conditional Access Policy** | The 'Conditional Access Policy' property specifies the Outlook on the Web Policy for limited access. For this feature to work properly, you also need to configure a Conditional Access policy in the Azure Active Directory Portal. |
| **Default Theme** | The 'Default Theme' property specifies the default theme that's used in Outlook on the web when the user hasn't selected a theme. The default value is blank \(null\). |
| **Direct File Access On Private Computers Enabled** | The 'Direct File Access On Private Computers Enabled' property specifies the left-click options for attachments in Outlook on the web for private computer sessions. |
| **Direct File Access On Public Computers Enabled** | The 'Direct File Access On Private Computers Enabled' property specifies the left-click options for attachments in Outlook on the web for public computer sessions. |
| **Disable Facebook** | The 'Disable Facebook' switch specifies whether users can synchronize their Facebook contacts to their Contacts folder in Outlook on the web. By default, Facebook integration is enabled. |
| **Display Photos Enabled** | The 'Display Photos Enabled' property specifies whether users see sender photos in Outlook on the web. |
| **Explicit Logon Enabled** | The 'Explicit Logon Enabled' property specifies whether to allow a user to open someone else's mailbox in Outlook on the web \(provided that user has permissions to the mailbox\). |
| **External Image Proxy Enabled** | The 'External Image Proxy Enabled' property specifies whether to load all external images through the Outlook external image proxy. |
| **External SP My Site Host URL** | The 'External SP My Site Host URL' specifies the My Site Host URL for external users. |
| **Force Save Attachment Filtering Enabled** | The 'Force Save Attachment Filtering Enabled' property specifies whether files are filtered before they can be saved from Outlook on the web. |
| **Force Wac Viewing First On Private Computers** | The 'Force Wac Viewing First On Private Computers' property specifies whether private computers must first preview an Office file as a web page in Office Online Server \(formerly known as Office Web Apps Server and Web Access Companion Server\) before opening the file in the local application. |
| **Force Wac Viewing First On Public Computers** | The 'Force Wac Viewing First On Public Computers' property specifies whether public computers must first preview an Office file as a web page in Office Online Server before opening the file in the local application. |
| **Fre Cards Enabled** | The 'Fre Cards Enabled' property specifies whether the theme, signature, and phone cards are available in Outlook on the web. |
| **Global Address List Enabled** | The 'Global Address List Enabled' property specifies whether the global address list is available in Outlook on the web. |
| **Group Creation Enabled** | The 'Group Creation Enabled' property specifies whether Office 365 group creation is available in Outlook on the web. |
| **Instant Messaging Enabled** | The 'Instant Messaging Enabled' property specifies whether instant messaging is available in Outlook on the web. |
| **Instant Messaging Type** | The 'Instant Messaging Type' property specifies the type of instant messaging provider in Outlook on the web. |
| **Interesting Calendars Enabled** | The 'Interesting Calendars Enabled' property specifies whether interesting calendars are available in Outlook on the web. |
| **Internal SP My Site Host URL** | The 'Internal SP My Site Host URL' specifies the My Site Host URL for internal users. |
| **IRM Enabled** | The 'IRM Enabled' property specifies whether Information Rights Management \(IRM\) features are available in Outlook on the web. |
| **Is Default** | The 'Is Default' switch specifies whether the Outlook on the web policy is the default policy that's used to configure the Outlook on the web settings for new mailboxes. |
| **Journal Enabled** | The 'Journal Enabled' property specifies whether the Journal folder is available in Outlook on the web. |
| **Local Events Enabled** | The 'Local Events Enabled' property specifies whether local events calendars are available in Outlook on the web. |
| **Logon And Error Language** | The 'Logon And Error Language' property specifies the language that used in Outlook on the web for forms-based authentication and for error messages when a user's current language setting can't be read. A valid value is a supported Microsoft Windows Language Code Identifier \(LCID\). For example, 1033 is US English. |
| **Notes Enabled** | The 'Notes Enabled' property specifies whether the Notes folder is available in Outlook on the web. |
| **Organization Enabled** | When the 'Organization Enabled' property is set to False, the Automatic Reply option doesn't include external and internal options, the address book doesn't show the organization hierarchy, and the Resources tab in Calendar forms is disabled. |
| **On Send Addins Enabled** | The 'On Send Addins Enabled' property specifies whether to enable or disable on send add-ins in Outlook on the web \(add-ins that support events when a user clicks Send\). |
| **Outbound Charset** | The 'Outbound Charset' property specifies the character set that's used for outgoing messages in Outlook on the web. |
| **Outlook Beta Toggle Enabled** | The 'Outlook Beta Toggle Enabled' property specifies whether to enable or disable the Outlook on the web Preview toggle. The Preview toggle allows users to try the new Outlook on the web experience. |
| **OWA Light Enabled** | The 'OWA Light Enabled' property controls the availability of the light version of Outlook on the web. |
| **Personal Account Calendars Enabled** | The 'Personal Account Calendars Enabled' property specifies whether to allow users to connect to their personal Outlook.com or Google Calendar in Outlook on the web. |
| **Phonetic Support Enabled** | The 'Phonetic Support Enabled' property specifies phonetically spelled entries in the address book. This property is available for use in Japan. |
| **Places Enabled** | The 'Places Enabled' property specifies whether to enable or disable Places in Outlook on the web. Places lets users search, share, and map location details by using Bing. |
| **Premium Client Enabled** | The 'Premium Client Enabled' property controls the availability of the full version of Outlook Web App. |
| **Print Without Download Enabled** | The 'Print Without Download Enabled' specifies whether to allow printing of supported files without downloading the attachment in Outlook on the web. |
| **Public Folders Enabled** | The 'Public Folders Enabled' property specifies whether a user can browse or read items in public folders in Outlook Web App. |
| **Recover Deleted Items Enabled** | The 'Recover Deleted Items Enabled' property specifies whether a user can use Outlook Web App to view, recover, or delete permanently items that have been deleted from the Deleted Items folder. |
| **Reference Attachments Enabled** | The 'Reference Attachments Enabled' property specifies whether users can attach files from the cloud as linked attachments in Outlook on the web. |
| **Reminders And Notifications Enabled** | The 'Reminders And Notifications Enabled' property specifies whether notifications and reminders are enabled in Outlook on the web. |
| **Report Junk Email Enabled** | The 'Report Junk Email Enabled' property specifies whether users can report messages to Microsoft or unsubscribe from messages in Outlook on the web. |
| **Rules Enabled** | The 'Rules Enabled' property specifies whether a user can view, create, or modify server-side rules in Outlook on the web. |
| **Satisfaction Enabled** | The 'Satisfaction Enabled' property specifies whether to enable or disable the satisfaction survey. |
| **Save Attachments To Cloud Enabled** | The 'Save Attachments To Cloud Enabled' property specifies whether users can save regular email attachments to the cloud. |
| **Search Folders Enabled** | The 'Search Folders Enabled' property specifies whether Search Folders are available in Outlook on the web. |
| **Set Photo Enabled** | The 'Set Photo Enabled' property specifies whether users can add, change, and remove their sender photo in Outlook on the web. |
| **Set Photo URL** | The 'Set Photo URL' property controls where users go to select their photo. Note that you can't specify a URL that contains one or more picture files, as there is no mechanism to copy a URL photo to the properties of the users' Exchange Online mailboxes. |
| **Signatures Enabled** | The 'Signatures Enabled' property specifies whether to enable or disable the use of signatures in Outlook on the web. |
| **Skip Create Unified Group Custom Sharepoint Classification** | The 'Skip Create Unified Group Custom Sharepoint Classification' property specifies whether to skip a custom SharePoint page during the creation of Office 365 Groups in Outlook web app. |
| **Team Snap Calendars Enabled** | The 'Team Snap Calendars Enabled' property specifies whether to allow users to connect to their personal TeamSnap calendars in Outlook on the web. |
| **Text Messaging Enabled** | The 'Text Messaging Enabled' property specifies whether users can send and receive text messages in Outlook on the web. |
| **Theme Selection Enabled** | The 'Theme Selection Enabled' property specifies whether users can change the theme in Outlook on the web. |
| **UM Integration Enabled** | The 'UM Integration Enabled' property specifies whether Unified Messaging \(UM\) integration is enabled in Outlook on the web. |
| **Use GB 18030** | The 'Use GB 18030' property specifies whether to use the GB18030 character set instead of GB2312 in Outlook on the web. |
| **Use ISO 885915** | The 'Use ISO 885915' property specifies whether to use the character set ISO8859-15 instead of ISO8859-1 in Outlook on the web. |
| **User Voice Enabled** | The 'User Voice Enabled' property specifies whether to enable or disable Outlook UserVoice in Outlook on the web. Outlook UserVoice is a customer feedback area that's available in Office 365. |
| **Wac Editing Enabled** | The 'Wac Editing Enabled' property specifies whether to enable or disable editing documents in Outlook on the web by using Office Online Server \(formerly known as Office Web Apps Server and Web Access Companion Server\). |
| **Wac External Services Enabled** | The 'Wac External Services Enabled' property specifies whether to enable or disable external services when viewing documents in Outlook on the web \(for example, machine translation\) by using Office Online Server. |
| **Wac OMEX Enabled** | The 'Wac OMEX Enabled' property specifies whether to enable or disable apps for Outlook in Outlook on the web in Office Online Server. |
| **Wac Viewing On Private Computers Enabled** | The 'Wac Viewing On Private Computers Enabled' property specifies whether to enable or disable web viewing of supported Office documents private computer sessions in Office Online Server \(formerly known as Office Web Apps Server and Web Access Companion Server\). By default, all Outlook on the web sessions are considered to be on private computers. |
| **Wac Viewing On Public Computers Enabled** | The 'Wac Viewing On Public Computers Enabled' property specifies whether to enable or disable web viewing of supported Office documents in public computer sessions in Office Online Server. |
| **Weather Enabled** | The 'Weather Enabled' property specifies whether to enable or disable weather information in the calendar in Outlook on the web. |
| **Web Parts Frame Options Type** | The 'Web Parts Frame Options Type' property specifies what sources can access web parts in IFRAME or FRAME elements in Outlook on the web. |
| **Nps Surveys Enabled** | The 'Nps Surveys Enabled' property specifies whether to enable or disable the Net Promoter Score \(NPS\) survey in Outlook on the web. The survey allows uses to rate Outlook on the web on a scale of 1 to 5, and to provide feedback and suggested improvements in free text. |

### Partner Application

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies a new name for the partner application. |
| **Application Identifier** | The 'Application Identifier' property specifies a unique application identifier for the partner application that uses an authorization server. |
| **Accept Security Identifier Information** | The 'Accept Security Identifier Information' property specifies whether Exchange should accept security identifiers \(SIDs\) from another trusted Active Directory forest for the partner application. |
| **Account Type** | The 'Account Type' property specifies the type of Microsoft account that's required for the partner application. |
| **Enabled** | The 'Enabled' property specifies whether the partner application is enabled. |
| **Linked Account** | The 'Linked Account' property specifies a linked Active Directory user account for the application. |

### Policy Tip Config

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the custom Policy Tip you want to modify. |
| **Value** | The 'Value' property specifies the text that's displayed by the Policy Tip. |

### Remote Domains

| Name | Description |
| :--- | :--- |
| **Name** | Specifies the 'Name' for the remote domain. |
| **Domain Name** | The 'Domain Name' property specifies the SMTP domain that is established as a remote domain. A valid value is an SMTP domain \(for example, contoso.com\). The maximum length is 256 characters. |
| **Allowed OOF Type** | The 'Allowed OOF Type' property specifies the type of automatic replies or out-of-office \(also known as OOF\) notifications than can be sent to recipients in the remote domain. Valid values are: External, ExternalLegacy, InternalLegacy or None. |
| **Auto Forward Enabled** | The 'Auto Forward Enabled' property specifies whether to allow messages that are auto-forwarded by client email programs in your organization. |
| **Auto Reply Enabled** | The 'Auto Reply Enabled' property specifies whether to allow messages that are automatic replies from client email programs in your organization \(for example, automatic reply messages that are generated by rules in Outlook\). |
| **Byte Encoder Type For 7 Bit Charsets** | The 'Byte Encoder Type For 7 Bit Charsets' property specifies the 7-bit transfer encoding method for MIME format for messages sent to this remote domain. |
| **Character Set** | The 'Character Set' property specifies a character set for MIME messages without defined character sets that are sent from your organization to recipients in the remote domain. |
| **Content Type** | The 'Content Type' property specifies the outbound message content type and formatting. |
| **Delivery Report Enabled** | The 'Delivery Report Enabled' property specifies whether to allow delivery reports from client software in your organization to recipients in the remote domain. |
| **Display Sender Name** | The 'Display Sender Name' property specifies whether to show the sender's Display Name in the From email address for messages sent to recipients in the remote domain. |
| **Is Internal** | The 'Is Internal' property specifies whether the recipients in the remote domain are considered to be internal recipients. |
| **Line Wrap Size** | The 'Line Wrap Size' property specifies the line-wrap size for messages to recipients in the remote domain. Valid values are an integer from 0 through 132 or the value to unlimited. The default value is unlimited. |
| **Meeting Forward Notification Enabled** | The 'Meeting Forward Notification Enabled' property specifies whether to enable meeting forward notifications for recipients in the remote domain. |
| **Non Mime Character Set** | The 'Non Mime Character Set' property specifies a character set for plain text messages without defined character sets that are sent from your organization to recipients in the remote domain. |
| **Preferred Internet Code Page For Shift Jis** | The 'Preferred Internet Code Page For Shift Jis' property specifies the specific code page to use for Shift JIS character encoding in messages that are sent to recipients in the remote domain. |
| **Required Charset Coverage** | The 'Required Charset Coverage' property specifies a percentage threshold for characters in a message that must match to apply your organization's preferred character set before switching to automatic character set detection. |
| **Target Delivery Domain** | The 'Target Delivery Domain' property specifies whether the remote domain is used in cross-forest deployments to generate target email addresses for new mail users that represent users in the other organization \(for example, all mailboxes hosted on Exchange Online are represented as mail users in your on-premises organization\). |
| **TNEF Enabled** | The 'TNEF Enabled' property specifies whether Transport Neutral Encapsulation Format \(TNEF\) message encoding is used on messages sent to the remote domain. |
| **Trusted Mail Inbound Enabled** | The 'Trusted Mail Inbound Enabled' property specifies whether messages from senders in the remote domain are treated as trusted messages. |
| **Trusted Mail Outbound Enabled** | The 'Trusted Mail Outbound Enabled' property specifies whether messages sent to recipients in the remote domain are treated as trusted messages. |
| **Use Simple Display Name** | The 'Use Simple Display Name' property specifies whether the sender's simple display name is used for the From email address in messages sent to recipients in the remote domain. |

### Role Assignment Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the assignment policy. The maximum length is 64 characters. |
| **Description** | The 'Description' property specifies the description that's displayed when the role assignment policy is viewed using the Get-RoleAssignmentPolicy cmdlet. |
| **Is Default** | The 'Is Default' switch specifies if the assignment policy is the default assignment policy. |
| **Roles** | The 'Roles' property specifies the management roles assigned to the role assignment policy. |

### Safe Attachment Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the safe attachment policy. |
| **Action** | The 'Action' property specifies the action of the Safe Attachments policy. |
| **Action On Error** | The 'Action On Error' property specifies the error handling option for Safe Attachments scanning \(what to do if scanning times out or an error occurs\). Valid values are: True: The action specified by the Action property is applied to messages even when the attachments aren't successfully scanned. False: The action specified by the Action property isn't applied to messages when the attachments aren't successfully scanned. This is the default value. |
| **Admin Display Name** | The 'Admin Display Name' property specifies a description of the policy. |
| **Enable** | Specify if this policy should be enabled. Default is True. |
| **Redirect** | The 'Redirect' property specifies whether to send detected malware attachments to another email address. Valid values are: True: Malware attachments are sent to the email address specified by the 'Redirect Address' parameter. False: Malware attachments aren't sent to another email address. This is the default value. |
| **Redirect Address** | The 'Redirect Address' property specifies the email address where detected malware attachments are sent when the Redirect property is set to the value True. |

### Safe Links Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the  name of the policy. |
| **Admin Display Name** | The 'Admin Display Name' property specifies the description of the policy. |
| **Do Not Allow Click Through** | The 'Do Not Allow Click Through' property specifies whether to allow users to click through to the original URL. Valid values are: True: The user isn't allowed to click through to the original URL. This is the default value. False: The user is allowed to click through to the original URL. |
| **Do Not Rewrite Urls** | The 'Do Not Rewrite Urls' property specifies a URL that's skipped by Safe Links scanning. You can specify multiple values separated by commas. |
| **Do Not Track User Clicks** | The 'Do Not Track User Clicks' property specifies whether to track user clicks related to links in email messages. Valid values are: True: User clicks aren't tracked. This is the default value. False: User clicks are tracked. |
| **Enable For Internal Senders** | EnableForInternalSenders True or False. |
| **Is Enabled** | This property specifies whether the rule or policy is enabled. |
| **Scan Urls** | The 'Scan Urls' property specifies whether to enable or disable the scanning of links in email messages. Valid values are: True: Scanning links in email messages is enabled. False: Scanning links in email messages is disabled. This is the default value. |

### Shared Mailboxes

| Name | Description |
| :--- | :--- |
| **Display Name** | The display name of the Shared Mailbox. |
| **Primary SMTP Address** | The primary email address of the Shared Mailbox. |
| **Aliases** | Aliases for the Shared Mailbox. |

### Anti Phish Policies ⯈ Anti Phish Rules

| Name | Description |
| :--- | :--- |
| **Anti Phish Policy** | The 'Anti Phish Policy' property specifies the name of the antiphishing policy that's associated with the antiphishing rule. |
| **Enabled** | Specify if this rule should be enabled. Default is True. |
| **Priority** | The 'Priority' property specifies a priority value for the rule that determines the order of rule processing. A lower integer value indicates a higher priority, the value 0 is the highest priority, and rules can't have the same priority value. |
| **Comments** | The 'Comments' property specifies informative comments for the rule, such as what the rule is used for or how it has changed over time. The length of the comment can't exceed 1024 characters. |
| **Except If Recipient Domain Is** | The 'Except If Recipient Domain Is' property specifies an exception that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Except If Sent To** | The 'Except If Sent To' property specifies an exception that looks for recipients in messages. |
| **Except If Sent To Member Of** | The 'Except If Sent To Member Of' property specifies an exception that looks for messages sent to members of groups. |
| **Recipient Domain Is** | The 'Recipient Domain Is' property specifies a condition that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Sent To** | The 'Sent To' property specifies a condition that looks for recipients in messages. |
| **Sent To Member Of** | The 'Sent To Member Of' property looks for messages sent to members of groups. |

### Anti Spam Settings ⯈ Anti Spam Policies

| Name | Description |
| :--- | :--- |
| **Hosted Content Filter Policy** | The 'Hosted Content Filter Policy' property specifies the name of the HostedContentFilter policy that's associated with the HostedContentFilter rule. |
| **Enabled** | Specify if this rule should be enabled. Default is True. |
| **Priority** | The 'Priority' property specifies a priority value for the rule that determines the order of rule processing. A lower integer value indicates a higher priority, the value 0 is the highest priority, and rules can't have the same priority value. |
| **Comments** | The 'Comments' property specifies informative comments for the rule, such as what the rule is used for or how it has changed over time. The length of the comment can't exceed 1024 characters. |
| **Except If Recipient Domain Is** | The 'Except If Recipient Domain Is' property specifies an exception that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Except If Sent To** | The 'Except If Sent To' property specifies an exception that looks for recipients in messages. |
| **Except If Sent To Member Of** | The 'Except If Sent To Member Of' property specifies an exception that looks for messages sent to members of groups. |
| **Recipient Domain Is** | The 'Recipient Domain Is' property specifies a condition that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Sent To** | The 'Sent To' property specifies a condition that looks for recipients in messages. |
| **Sent To Member Of** | The 'Sent To Member Of' property looks for messages sent to members of groups. |

### Connectors ⯈ Inbound Connectors

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the inbound connector. |
| **Associated Accepted Domains** | The 'Associated Accepted Domains' property specifies the accepted domains that the connector applies to, thereby limiting its scope. For example, the connector can be applied to a specific accepted domain in your organization, such as contoso.com. |
| **Cloud Services Mail Enabled** | The 'Cloud Services Mail Enabled' property specifies whether the connector is used for hybrid mail flow between an on-premises Exchange environment and Microsoft Office 365. Specifically, this property controls how certain internal X-MS-Exchange-Organization-\* message headers are handled in messages that are sent between accepted domains in the on-premises and cloud organizations. These headers are collectively known as cross-premises headers. DO NOT USE MANUALLY! Valid values are: True \| False. |
| **Comment** | The 'Comment' property specifies an optional comment. |
| **Connector Source** | The 'Connector Source' property specifies how the connector is created. DO NOT CHANGE THIS! values are Default \(the default\) \| Migrated \| HybridWizard. |
| **Connector Type** | The 'Connector Type' property specifies a category for the domains that are serviced by the connector. Valid values are Partner and OnPremises. |
| **Enabled** | Specifies whether connector is enabled. |
| **Require Tls** | The 'Require Tls' property specifies that all messages received by this connector require TLS transmission. Valid values for this property are True or False. The default value is False. When the 'Require Tls' property is set to True, all messages received by this connector require TLS transmission. |
| **Restrict Domains To Certificate** | The 'Restrict Domains To Certificate' property specifies that Office 365 should identify incoming messages that are eligible for this connector by verifying that the remote server authenticates using a TLS certificate that has the 'Tls Sender Certificate Name' in the Subject. |
| **Restrict Domains To IP Addresses** | The 'Restrict Domains To IP Addresses' parameter, when set to True, automatically rejects mail from the domains specified by the 'Sender Domains' property if the mail originates from an IP address that isn't specified by the 'Sender IP Addresses' parameter. |
| **Sender Domains** | The 'Sender Domains' property specifies the remote domains from which this connector accepts messages, thereby limiting its scope. A wildcard character can specify all subdomains of a domain, as shown in the following example: \*.contoso.com. However, a wildcard character cannot be embedded, as shown in the following example: domain.\*.contoso.com. |
| **Sender IP Addresses** | The 'Sender IP Addresses' property specifies the remote IP addresses from which this connector accepts messages. |
| **Tls Sender Certificate Name** | The 'Tls Sender Certificate Name' property specifies the certificate used by the sender's domain when the 'Require Tls' property is set to True. Valid input for the 'Tls Sender Certificate Name' property is an SMTP domain. |
| **Treat Messages As Internal** | The 'Treat Messages As Internal' property specifies an alternative method to identify messages sent from an on-premises organization as internal messages. This property is usually only used when the on-premises organization doesn't use Exchange. |

### Connectors ⯈ Intra Organization Connectors

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the intraorg connector. |
| **Discovery Endpoint** | The 'Discovery Endpoint' property specifies the externally-accessible URL that's used for the Autodiscover service for the domain that's configured in the Intra-Organization connector. |
| **Enabled** | Specifies whether connector is enabled. |
| **Target Address Domains** | The 'Target Address Domains' property specifies the domain namespaces that will be used in the Intra-organization connector. These domains must have valid Autodiscover endpoints defined in their organizations. The domains and their associated Autodiscover endpoints are used by the Intra-Organization connector for feature and service connectivity. Multiple domains are separated by commas. |

### Connectors ⯈ Outbound Connectors

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the connector. |
| **Enabled** | Specifies whether connector is enabled. |
| **Use MX Record** | Specifies whether connector should use MXRecords for target resolution. |
| **Comment** | The 'Comment' property specifies an optional comment. |
| **Connector Source** | The 'Connector Source' property specifies how the connector is created. DO NOT CHANGE THIS! values are Default \(the default\) \| Migrated \| HybridWizard \| AdminUI. |
| **Connector Type** | The 'Connector Type' property specifies a category for the domains that are serviced by the connector. Valid values are Partner and OnPremises. |
| **Recipient Domains** | The 'Recipient Domains' property specifies the domain that the Outbound connector routes mail to. You can specify multiple domains separated by commas. |
| **Smart Hosts** | The 'Smart Hosts' property specifies the smart hosts the Outbound connector uses to route mail. This property is required if UseMxRecord property is set  to False. |
| **Tls Domain** | The 'Tls Domain' property specifies the domain name that the Outbound connector uses to verify the FQDN of the target certificate when establishing a TLS secured connection. This property is only used if the 'Tls Settings' property is set to DomainValidation. Valid input for the 'Tls Domain' property is an SMTP domain. A wildcard character can specify all subdomains of a domain, as shown in the following example: \*.contoso.com. However, a wildcard character cannot be embedded, as shown in the following example: domain.\*.contoso.com. |
| **Tls Settings** | The 'Tls Settings' property specifies the TLS authentication level that's used for outbound TLS connections established by this Outbound connector. Valid values are:EncryptionOnly \| CertificateValidation \| DomainValidation. |
| **Is Transport Rule Scoped** | The 'Is Transport Rule Scoped' property specifies whether the Outbound connector is associated with a transport rule \(also known as a mail flow rule\). Valid values are: True \| False. |
| **Route All Messages Via On Premises** | The 'Route All Messages Via On Premises' property specifies that all messages serviced by this connector are first routed through the on-premises messaging system \(Centralized mailrouting\). Valid values are: True \| False. |
| **Cloud Services Mail Enabled** | The 'Cloud Services Mail Enabled' property specifies whether the connector is used for hybrid mail flow between an on-premises Exchange environment and Microsoft Office 365. Specifically, this property controls how certain internal X-MS-Exchange-Organization-\* message headers are handled in messages that are sent between accepted domains in the on-premises and cloud organizations. These headers are collectively known as cross-premises headers. DO NOT USE MANUALLY! Valid values are: True \| False. |
| **All Accepted Domains** | The 'All Accepted Domains' property specifies whether the Outbound connector is used in hybrid organizations where message recipients are in accepted domains of the cloud-based organization. Valid values are: True \| False \(default\). |
| **Test Mode** | The 'Test Mode' property specifies whether you want to enabled or disable test mode for the Outbound connector. Valid values are: True \| False \(default\). |
| **Validation Recipients** | The 'Validation Recipients' property specifies the email addresses of the validation recipients for the Outbound connector. You can specify multiple email addresses separated by commas. |

### Malware Filter Policies ⯈ Malware Filter Rules

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the rule. |
| **Comments** | The 'Comments' property specifies informative comments for the rule, such as what the rule is used for or how it has changed over time. The length of the comment can't exceed 1024 characters. |
| **Enabled** | The 'Enabled' property enables or disables the malware filter rule. Valid input for this property is True or False. The default value is True. |
| **Except If Recipient Domain Is** | The 'Except If Recipient Domain Is' property specifies an exception that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Except If Sent To** | The 'Except If Sent To' property specifies an exception that looks for recipients in messages. |
| **Except If Sent To Member Of** | The 'Except If Sent To Member Of' property specifies an exception that looks for messages sent to members of groups. |
| **Malware Filter Policy** | The 'Malware Filter Policy' property specifies the malware filter policy to apply to messages that match the conditions defined by this malware filter rule. |
| **Priority** | The 'Priority' property specifies a priority value for the rule that determines the order of rule processing. A lower integer value indicates a higher priority, the value 0 is the highest priority, and rules can't have the same priority value. |
| **Recipient Domain Is** | The 'Recipient Domain Is' property specifies a condition that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Sent To** | The 'Sent To' property specifies a condition that looks for recipients in messages. You can use any value that uniquely identifies the recipient. |
| **Sent To Member Of** | The 'Sent To Member Of' property specifies a condition that looks for messages sent to members of distribution groups, dynamic distribution groups, or mail-enabled security groups. |

### Mobile ⯈ Mobile Device Access Rules

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the name of the device access rule. |
| **Access Level** | The 'Access Level' property specifies whether the devices are allowed, blocked or quarantined. |
| **Characteristic** | The 'Characteristic' property specifies the device characteristic or category that's used by the rule. |
| **Query String** | The 'Query String' property specifies the device identifier that's used by the rule. This property uses a text value that's used with Characteristic property value to define the device. |

### Mobile ⯈ Mobile Device Mailbox Policies

| Name | Description |
| :--- | :--- |
| **Name** | The 'Name' property specifies the friendly name of the mobile device mailbox policy. |
| **Allow Apple Push Notifications** | The 'Allow Apple Push Notifications' property specifies whether push notifications are allowed to Apple mobile devices. |
| **Allow Bluetooth** | The 'Allow Bluetooth' property specifies whether the Bluetooth capabilities are allowed on the mobile phone. The available options are Disable, HandsfreeOnly, and Allow. The default value is Allow. |
| **Allow Browser** | The 'Allow Browser' property indicates whether Microsoft Pocket Internet Explorer is allowed on the mobile phone. This property doesn't affect third-party browsers. |
| **Allow Camera** | The 'Allow Camera' property specifies whether the mobile phone's camera is allowed. |
| **Allow Consumer Email** | The 'Allow Consumer Email' property specifies whether the mobile phone user can configure a personal email account on the mobile phone. |
| **Allow Desktop Sync** | The 'Allow Desktop Sync' property specifies whether the mobile phone can synchronize with a desktop computer through a cable. |
| **Allow External Device Management** | The 'Allow External Device Management' property specifies whether an external device management program is allowed to manage the mobile phone. |
| **Allow Google Push Notifications** | The 'Allow Google Push Notifications' property controls whether the user can receive push notifications from Google for Outlook on the web for devices. |
| **Allow HTML Email** | The 'Allow HTML Email' property specifies whether HTML email is enabled on the mobile phone. |
| **Allow Internet Sharing** | The 'Allow Internet Sharing' property specifies whether the mobile phone can be used as a modem to connect a computer to the Internet. |
| **Allow IrDA** | The 'Allow IrDA' property specifies whether infrared connections are allowed to the mobile phone. |
| **Allow Mobile OTA Update** | The 'Allow Mobile OTA Update' property specifies whether the Exchange ActiveSync mailbox policy can be sent to the mobile phone over a cellular data connection. |
| **Allow Microsoft Push Notifications** | The 'Allow Microsoft Push Notifications' property specifies whether push notifications are enabled on the mobile device. |
| **Allow Non Provisionable Devices** | The 'Allow Non Provisionable Devices' property specifies whether all mobile phones can synchronize with the server running Exchange. |
| **Allow POPIMAP Email** | The 'Allow POPIMAP Email' property specifies whether the user can configure a POP3 or IMAP4 email account on the mobile phone. |
| **Allow Remote Desktop** | The 'Allow Remote Desktop' property specifies whether the mobile phone can initiate a remote desktop connection. |
| **Allow Simple Password** | The 'Allow Simple Password' property specifies whether a simple device password is allowed. A simple device password is a password that has a specific pattern, such as 1111 or 1234. |
| **Allow SMIME Encryption Algorithm Negotiation** | The 'Allow SMIME Encryption Algorithm Negotiation' property specifies whether the messaging application on the mobile device can negotiate the encryption algorithm if a recipient's certificate doesn't support the specified encryption algorithm. |
| **Allow SMIME Soft Certs** | The 'Allow SMIME Soft Certs' property specifies whether S/MIME software certificates are allowed. |
| **Allow Storage Card** | The 'Allow Storage Card' property specifies whether the mobile phone can access information stored on a storage card. |
| **Allow Text Messaging** | The 'Allow Text Messaging' property specifies whether text messaging is allowed from the mobile phone. |
| **Allow Unsigned Applications** | The 'Allow Unsigned Applications' property specifies whether unsigned applications can be installed on the mobile phone. |
| **Allow Unsigned Installation Packages** | The 'Allow Unsigned Installation Packages' property specifies whether unsigned installation packages can be executed on the mobile phone. |
| **Allow Wi Fi** | The 'Allow Wi Fi' property specifies whether wireless Internet access is allowed on the mobile phone. |
| **Alphanumeric Password Required** | The 'Alphanumeric Password Required' property specifies whether the password for the mobile phone must be alphanumeric. |
| **Approved Application List** | The 'Approved Application List' property specifies a list of approved applications for the mobile phone. |
| **Attachments Enabled** | The 'Attachments Enabled' property specifies whether attachments can be downloaded. |
| **Device Encryption Enabled** | The 'Device Encryption Enabled' property specifies whether encryption is enabled. |
| **Device Policy Refresh Interval** | The 'Device Policy Refresh Interval' property specifies how often the policy is sent from the server to the mobile phone. |
| **Irm Enabled** | The 'Irm Enabled' property specifies whether Information Rights Management \(IRM\) is enabled for the mailbox policy. |
| **Is Default** | The 'Is Default' property specifies whether this policy is the default Mobile Device mailbox policy. |
| **Max Attachment Size** | The 'Max Attachment Size' property specifies the maximum size of attachments that can be downloaded to the mobile phone. |
| **Max Calendar Age Filter** | The 'Max Calendar Age Filter' property specifies the maximum range of calendar days that can be synchronized to the device. |
| **Max Email Age Filter** | The 'Max Email Age Filter' property specifies the maximum number of days of email items to synchronize to the mobile phone. |
| **Max Email Body Truncation Size** | The 'Max Email Body Truncation Size' property specifies the maximum size at which email messages are truncated when synchronized to the mobile phone. The value is specified in kilobytes \(KB\). |
| **Max Email HTML Body Truncation Size** | The 'Max Email HTML Body Truncation Size' property specifies the maximum size at which HTML-formatted email messages are synchronized to the mobile phone. The value is specified in KB. |
| **Max Inactivity Time Lock** | The MaxInactivityTimeDeviceLock property specifies the length of time that the mobile phone can be inactive before the password is required to reactivate it. |
| **Max Password Failed Attempts** | The 'Max Password Failed Attempts' property specifies the number of attempts a user can make to enter the correct password for the mobile phone. You can enter any number from 4 through 16 or the value Unlimited. |
| **Min Password Complex Characters** | The 'Min Password Complex Characters' property specifies the character sets that are required in the password of the mobile device. |
| **Min Password Length** | The 'Min Password Length' property specifies the minimum number of characters in the mobile device password. |
| **Password Enabled** | The 'Password Enabled' property specifies whether a password is required on the mobile device. |
| **Password Expiration** | The 'Password Expiration' property specifies how long a password can be used on a mobile device before the user is forced to change the password. |
| **Password History** | The 'Password History' property specifies the number of unique new passwords that need to be created on the mobile device before an old password can be reused. |
| **Password Recovery Enabled** | The 'Password Recovery Enabled' property specifies whether the recovery password for the mobile device is stored in Exchange. |
| **Require Device Encryption** | The 'Require Device Encryption' property specifies whether encryption is required on the mobile device. |
| **Require Encrypted SMIME Messages** | The 'Require Encrypted SMIME Messages' property specifies whether the mobile device must send encrypted S/MIME messages. |
| **Require Encryption SMIME Algorithm** | The 'Require Encryption SMIME Algorithm' property specifies the algorithm that's required to encrypt S/MIME messages on a mobile device. |
| **Require Manual Sync When Roaming** | The 'Require Signed SMIME Algorithm' property specifies the algorithm that's used to sign S/MIME messages on the mobile device. |
| **Require Signed SMIME Algorithm** | The 'Require Signed SMIME Algorithm' property specifies the algorithm that's used to sign S/MIME messages on the mobile device. |
| **Require Signed SMIME Messages** | The 'Require Signed SMIME Messages' property specifies whether the mobile device must send signed S/MIME messages. |
| **Require Storage Card Encryption** | The 'Require Storage Card Encryption' property specifies whether storage card encryption is required on the mobile device. |
| **Unapproved In ROM Application List** | The 'Unapproved In ROM Application List' property specifies a list of applications that can't be run in ROM on the mobile device. |
| **UNC Access Enabled** | The 'UNC Access Enabled' property specifies whether access to Microsoft Windows file shares is enabled from the mobile device. |
| **WSS Access Enabled** | The 'WSS Access Enabled' property specifies whether access to Microsoft Windows SharePoint Services is enabled from the mobile device. |

### Safe Attachment Policies ⯈ Safe Attachment Rules

| Name | Description |
| :--- | :--- |
| **Safe Attachment Policy** | The 'Safe Attachment Policy' property specifies the name of the SafeAttachment policy that's associated with the SafeAttachment rule. |
| **Enabled** | Specify if this rule should be enabled. Default is True. |
| **Priority** | The 'Priority' property specifies a priority value for the rule that determines the order of rule processing. A lower integer value indicates a higher priority, the value 0 is the highest priority, and rules can't have the same priority value. |
| **Comments** | The 'Comments' property specifies informative comments for the rule, such as what the rule is used for or how it has changed over time. The length of the comment can't exceed 1024 characters. |
| **Except If Recipient Domain Is** | The 'Except If Recipient Domain Is' property specifies an exception that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Except If Sent To** | The 'Except If Sent To' property specifies an exception that looks for recipients in messages. |
| **Except If Sent To Member Of** | The 'Except If Sent To Member Of' property specifies an exception that looks for messages sent to members of groups. |
| **Recipient Domain Is** | The 'Recipient Domain Is' property specifies a condition that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Sent To** | The 'Sent To' property specifies a condition that looks for recipients in messages. |
| **Sent To Member Of** | The 'Sent To Member Of' property looks for messages sent to members of groups. |

### Safe Links Policies ⯈ Safe Links Rules

| Name | Description |
| :--- | :--- |
| **Safe Links Policy** | The 'Safe Links Policy' property specifies the name of the SafeLink policy that's associated with the SafeLinksing rule. |
| **Enabled** | Specify if this rule should be enabled. Default is True. |
| **Priority** | The 'Priority' property specifies a priority value for the rule that determines the order of rule processing. A lower integer value indicates a higher priority, the value 0 is the highest priority, and rules can't have the same priority value. |
| **Comments** | The 'Comments' property specifies informative comments for the rule, such as what the rule is used for or how it has changed over time. The length of the comment can't exceed 1024 characters. |
| **Except If Recipient Domain Is** | The 'Except If Recipient Domain Is' property specifies an exception that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Except If Sent To** | The 'Except If Sent To' property specifies an exception that looks for recipients in messages. |
| **Except If Sent To Member Of** | The 'Except If Sent To Member Of' property specifies an exception that looks for messages sent to members of groups. |
| **Recipient Domain Is** | The 'Recipient Domain Is' property specifies a condition that looks for recipients with email address in the specified domains. Multiple domains are separated by commas. |
| **Sent To** | The 'Sent To' property specifies a condition that looks for recipients in messages. |
| **Sent To Member Of** | The 'Sent To Member Of' property looks for messages sent to members of groups. |

