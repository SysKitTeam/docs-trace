---
title: Teams
description: >-
  This article lists the currently supported Teams reports with all of the
  properties that SysKit Trace loads.
date: 9/22/2020
---

# Teams

## Reports

### Calling Policies

| Name | Description |
| :--- | :--- |
| **Name** | Name of the Teams Calling Policy. |
| **Allow Private Calling** | Controls all calling capabilities in Teams. Turning this off will turn off all calling functionality in Teams. If you use Skype for Business for calling, this policy will not affect calling functionality in Skype for Business. |
| **Allow Voicemail** | Enables inbound calls to be routed to voice mail. Valid options are: AlwaysEnabled, AlwaysDisabled, UserOverride. |
| **Allow Call Groups** | Enables inbound calls to be routed to call groups. |
| **Allow Delegation** | Enables inbound calls to be routed to delegates; allows delegates to make outbound calls on behalf of the users for whom they have delegated permissions. |
| **Allow Call Forwarding To User** | Enables call forwarding or simultaneous ringing of inbound calls to other users in the tenant. |
| **Allow Call Forwarding To Phone** | Enables call forwarding or simultaneous ringing of inbound calls to any phone number. |
| **Prevent Toll Bypass** | Setting this property to True will send calls through PSTN and incur charges rather than going through the network and bypassing the tolls. |
| **Busy On Busy Enabled Type** | Setting this property lets you configure how incoming calls are handled when a user is already in a call or conference or has a call placed on hold. New or incoming calls will be rejected with a busy signal. Valid options are: Enabled, Disabled. |

### Channels Policies

| Name | Description |
| :--- | :--- |
| **Name** | Identity of the Teams Channel Policy. |
| **Description** | Description of the Teams Channel Policy. |
| **Allow Org Wide Team Creation** | Determines whether a user is allowed to create an org-wide team. |
| **Allow Private Team Discovery** | Determines whether a user is allowed to discover private teams in suggestions and search results. |
| **Allow Private Channel Creation** | Determines whether a user is allowed to create a private channel. |

### Emergency Call Routing Policies

| Name | Description |
| :--- | :--- |
| **Name** | Identity of the Teams Emergency Call Routing Policy. |
| **Description** | Description of the Teams Emergency Call Routing Policy. |
| **Allow Enhanced Emergency Services** | Flag to enable Enhanced Emergency Services. |

### Emergency Calling Policies

| Name | Description |
| :--- | :--- |
| **Name** | Identity of the Teams Emergency Calling Policy. |
| **Description** | Description of the Teams Emergency Calling Policy. |
| **Notification Dial Out Number** | This property represents PSTN number which can be dialed out if 'Notification Mode' is set to either of the two Conference values. |
| **Notification Group** | NotificationGroup is a email list of users and groups to be notified of an emergency call. |
| **Notification Mode** | The type of conference experience for security desk notification. |

### Live Events Policies

| Name | Description |
| :--- | :--- |
| **Name** | The identifier of the Teams Meeting Broadcast Policy. |
| **Allow Broadcast Scheduling** | Specifies whether this user can create broadcast events in Teams. This settng impacts broadcasts that use both self-service and external encoder production methods. |
| **Allow Broadcast Transcription** | Specifies whether real-time transcription and translation can be enabled in the broadcast event. Note: this setting is applicable to broadcast events that use Teams Meeting production only and does not apply when external encoder is used as production method. |
| **Broadcast Attendee Visibility Mode** | Specifies the attendee visibility mode of the broadcast events created by this user.  This setting controls who can watch the broadcast event - e.g. anyone can watch this event including anonymous users or only authenticated users in my company can watch the event.  Note: this setting is applicable to broadcast events that use Teams Meeting production only and does not apply when external encoder is used as production method. |
| **Broadcast Recording Mode** | Specifies whether broadcast events created by this user are always recorded, never recorded or user can choose whether to record or not. Note: this setting is applicable to broadcast events that use Teams Meeting production only and does not apply when external encoder is used as production method. |

### Live Events Settings

| Name | Description |
| :--- | :--- |
| **Support URL** | Specifies a URL where broadcast event attendees can find support information or FAQs specific to that event. The URL will be displayed to the attendees during the broadcast. |
| **Allow Sdn Provider For Broadcast Meeting** | If set to True, Teams meeting broadcast streams are enabled to take advantage of the network and bandwidth management capabilities of the Software Defined Network \(SDN\) provider. |
| **Sdn Provider Name** | Specifies the Software Defined Network \(SDN\) provider's name. This property is only required if 'Allow Sdn Provider For Broadcast Meeting' is set to True. |
| **Sdn License Id** | Specifies the Software Defined Network \(SDN\) license identifier. This is required and provided by some SDN providers. This property is only required if 'Allow Sdn Provider For Broadcast Meeting' is set to True. |
| **Sdn Api Template Url** | Specifies the Software Defined Network \(SDN\) provider's HTTP API endpoint. This information is provided by the SDN provider. This property is only required if 'Allow Sdn Provider For Broadcast Meeting' is set to True. |

### Meeting Policies

| Name | Description |
| :--- | :--- |
| **Name** | Name of the Teams Meeting Policy. |
| **Description** | Description of the Teams Meeting Policy. |
| **Allow Channel Meeting Scheduling** | Determines whether a user can schedule channel meetings. Note this only restricts from scheduling and not from joining a meeting scheduled by another user. |
| **Allow Meet Now** | Determines whether a user can start ad-hoc meetings. |
| **Allow IP Video** | Determines whether video is enabled in a user's meetings or calls. |
| **Allow Anonymous Users To Start Meeting** | Determines whether anonymous users can initiate a meeting. |
| **Allow Private Meeting Scheduling** | Determines whether a user can schedule private meetings. Note this only restricts from scheduling and not from joining a meeting scheduled by another user. |
| **Auto Admitted Users** | Determines what types of participants will automatically be added to meetings organized by this user. EveryoneInCompany specifies that every external user is placed in the lobby but all users in the company are allowed to join the meeting immediately. Everyone admits anonymous users by default. EveryoneInSameAndFederatedCompany specifies that  federated users are allowed to join like company's users, but all other external users are placed in a lobby. |
| **Allow Cloud Recording** | Determines whether cloud recording is allowed in a user's meetings. |
| **Allow Outlook Add In** | Determines whether a user can schedule Teams Meetings in Outlook desktop client. |
| **Allow PowerPoint Sharing** | Determines whether Powerpoint sharing is allowed in a user’s meetings. |
| **Allow Participant Give Request Control** | Determines whether participants can request or give control of screen sharing during meetings scheduled by this user. |
| **Allow External Participant Give Request Control** | Determines whether external participants can request or give control of screen sharing during meetings scheduled by this user. |
| **Allow Shared Notes** | Determines whether users are allowed to take shared notes. |
| **Allow Whiteboard** | Determines whether whiteboard is allowed in a user’s meetings. |
| **Allow Transcription** | Determines whether real-time and/or post-meeting captions and transcriptions are allowed in a user's meetings. |
| **Media Bit Rate Kb** | Determines the media bit rate for audio/video/app sharing transmissions in meetings. |
| **Screen Sharing Mode** | Determines the mode in which a user can share a screen in calls or meetings. SingleApplication allows a user to share an application at a given point in time. EntireScreen allow a user to share anything on their screens. Disabled prohibits users from sharing their screens. |
| **Allow PSTN Users To Bypass Lobby** | Determines whether PSTN users should be automatically admitted to the meetings. Set this to TRUE to allow the PSTN user to be able bypass the meetinglobby. Set this to FALSE to prohibit the PSTN user from bypassing the meetinglobby. |

### Meeting Settings

| Name | Description |
| :--- | :--- |
| **Logo URL** | URL to a logo image. This is included in the meeting invite. |
| **Legal URL** | URL to a website containing legal information and meeting disclaimers. This is included in the meeting invite. |
| **Help URL** | URL to a website where users can obtain assistance on joining the meeting.This is included in the meeting invite. |
| **Custom Footer Text** | Text to be used on custom meeting invitations. |
| **Disable Anonymous Join** | Determines whether anonymous users are blocked from joining meetings in the tenant. |
| **Enable QoS** | Determines whether Quality of Service Marking for real-time media \(audio, video, screen/app sharing\) is enabled in the tenant. |
| **Client Audio Port** | Determines the starting port number for client audio. Minimum allowed value: 1024 Maximum allowed value: 65535 Default value: 50000. |
| **Client Audio Port Range** | Determines the total number of ports available for client audio. Default value is 20. |
| **Client Video Port** | Determines the starting port number for client video. Minimum allowed value: 1024 Maximum allowed value: 65535 Default value: 50020. |
| **Client Video Port Range** | Determines the total number of ports available for client video. Default value is 20. |
| **Client App Sharing Port** | Determines the starting port number for client screen sharing or application sharing. Minimum allowed value: 1024 Maximum allowed value: 65535 Default value: 50040. |
| **Client Media Port Range Enabled** | Determines whether custom media port and range selections need to be enforced. When set to True, clients will use the specified port range for media traffic. When set to False \(the default value\) for any available port \(from port 1024 through port 65535\) will be used to accommodate media traffic. |
| **Client App Sharing Port Range** | Determines the total number of ports available for client sharing or application sharing. Default value is 20. |

### Messaging Policies

| Name | Description |
| :--- | :--- |
| **Name** | Name of the teams messaging policy. |
| **Allow Giphy** | Determines whether a user is allowed to access and post Giphys. |
| **Allow Memes** | Determines whether a user is allowed to access and post memes. |
| **Allow Owner Delete Message** | Determines whether owners are allowed to delete all the messages in their team. |
| **Allow Stickers** | Determines whether a user is allowed to access and post stickers. |
| **Allow Url Previews** | Use this setting to turn automatic URL previewing on or off in messages. |
| **Allow User Chat** | Determines whether a user is allowed to chat. |
| **Allow User Delete Message** | Determines whether a user is allowed to delete their own messages. |
| **Allow User Translation** | Determines whether a user is allowed to translate messages to their client languages. |
| **Allow Immersive Reader** | Determines whether a user is allowed to use Immersive Reader for reading conversation messages. |
| **Allow Remove User** | Determines whether a user is allowed to remove a user from a conversation. |
| **Allow Priority Messages** | Determines whether a user is allowed to send priorities messages. |
| **Description** | Provide a description of your policy to identify purpose of creating it. |
| **Giphy Rating Type** | Determines the Giphy content restrictions applicable to a user. Possible values are STRICT, MODERATE or NORESTRICTION. |
| **Read Receipts Enabled Type** | Use this setting to specify whether read receipts are user controlled, enabled for everyone, or disabled. Possible values are UserPreference, Everyone or None. |
| **Channels In Chat List Enabled Type** | Possible values are: DisabledUserOverride, EnabledUserOverride. |
| **Audio Message Enabled Type** | Determines whether a user is allowed to send audio messages. Possible values are: ChatsAndChannels, ChatsOnly, Disabled. |
| **Tenant** | Globally unique identifier \(GUID\) of the tenant account whose external user communication policy are being created. |

### Pstn Usage

| Name | Description |
| :--- | :--- |
| **Usage** | An online PSTN usage \(such as Local or Long Distance\) that can be used in conjunction with voice routes and voice routing policies. |

### Teams

| Name | Description |
| :--- | :--- |
| **Display Name** | Display Name of the Team. |
| **Description** | Description of Team. |
| **Group ID** | The ID of the associated O365 group. |
| **Mail Nick Name** | MailNickName of O365 group associated with Team. |
| **Owner** | Owners of the Team. |
| **Visibility** | Visibility of the Team. |
| **Allow Add Remove Apps** | Allow add or remove apps from the Team. |
| **Allow Giphy** | Allow giphy in Team. |
| **Giphy Content Rating** | Giphy content rating of the Team. |
| **Allow Stickers And Memes** | Allow stickers and mimes in the Team. |
| **Allow Custom Memes** | Allow custom memes in Team. |
| **Allow User Edit Messages** | Allow members to edit messages within Team. |
| **Allow User Delete Messages** | Allow members to delete messages within Team. |
| **Allow Owner Delete Messages** | Allow owners to delete messages within Team. |
| **Allow Delete Channels** | Allow members to delete channels within Team. |
| **Allow Create Update Remove Connectors** | Allow members to manage connectors within Team. |
| **Allow Create Update Remove Tabs** | Allow members to manage tabs within Team. |
| **Allow Team Mentions** | Allow mentions in Team. |
| **Allow Channel Mentions** | Allow channel mention in Team. |
| **Allow Guest Create Update Channels** | Allow guests to create and update channels in Team. |
| **Allow Guest Delete Channels** | Allow guests to delete channel in Team. |
| **Allow Create Update Channels** | Allow members to create and update channels within Team. |

### Teams Settings

| Name | Description |
| :--- | :--- |
| **Allow Box** | Designates whether users are able to leverage Box as a third party storage solution in Microsoft Teams. If True, users will be able to add Box in the client and interact with the files stored there. |
| **Allow DropBox** | Designates whether users are able to leverage DropBox as a third party storage solution in Microsoft Teams. If True, users will be able to add DropBox in the client and interact with the files stored there. |
| **Allow Email Into Channel** | When set to True, mail hooks are enabled, and users can post messages to a channel by sending an email to the email address of Teams channel. |
| **Allow Google Drive** | Designates whether users are able to leverage GoogleDrive as a third party storage solution in Microsoft Teams. If True, users will be able to add Google Drive in the client and interact with the files stored there. |
| **Allow Guest User** | Designates whether or not guest users in your organization will have access to the Teams client. If True, guests in your tenant will be able to access the Teams client. Note that this setting has a core dependency on Guest Access being enabled in your Office 365 tenant. |
| **Allow Organization Tab** | When set to True, users will be able to see the organizational chart icon other users' contact cards, and when clicked, this icon will display the detailed organizational chart. |
| **Allow Resource Account Send Message** | Surface Hub uses a device account to provide email and collaboration services \(IM, video, voice\). This device account is used as the originating identity \(the from party\) when sending email, IM, and placing calls. As this account is not coming from an individual, identifiable user, it is deemed anonymous because it originated from the Surface Hub's device account. If set to True, these device accounts will be able to send chat messages in Skype for Business Online \(does not apply to Microsoft Teams\). |
| **Allow Scoped People Search and Access** | If set to True, the Exchange address book policy \(ABP\) will be used to provide customized view of the global address book for each user. This is only a virtual separation and not a legal separation. |
| **Allow Share File** | Designates whether users are able to leverage ShareFile as a third party storage solution in Microsoft Teams. If True, users will be able to add ShareFile in the client and interact with the files stored there. |
| **Allow Skype Business Interop** | When set to True, Teams conversations automatically show up in Skype for Business for users that aren't enabled for Teams. |
| **Content Pin** | This setting applies only to Skype for Business Online \(not Microsoft Teams\) and defines whether the user must provide a secondary form of authentication to access the meeting content from a resource device account. Meeting content is defined as files that are shared to the Content Bin - files that have been attached to the meeting. |
| **Resource Account Content Access** | Require a secondary form of authentication to access meeting content. |
| **Restricted Sender List** | Senders domains can be further restricted to ensure that only allowed SMTP domains can send emails to the Teams channels. This is a comma-separated string of the domains you'd like to allow to send emails to Teams channels. |
| **Allow Egnyte** | Designates whether users are able to leverage Egnyte as a third party storage solution in Microsoft Teams. If True, users will be able to add Egnyte in the client and interact with the files stored there. |

### Teams Upgrade

| Name | Description |
| :--- | :--- |
| **Download Teams** | The 'Download Teams' property allows admins to control whether the Skype for Business client should automatically download Teams in the background. This Boolean setting is only honored on Windows clients, and only for certain values of the user's TeamsUpgradePolicy. If NotifySfbUser=true or if Mode=TeamsOnly in TeamsUpgradePolicy, this setting is honored. Otherwise it is ignored. |
| **SfB Meeting Join Ux** | The 'SfB Meeting Join Ux' property allows admins to specify which app is used to join Skype for Business meetings, even after the user has been upgraded to Teams. Allowed values are: 'SkypeMeetingsApp' and 'NativeLimitedClient'. 'NativeLimitedClient' means the existing Skype for Business rich client will be used, but since the user is upgraded, only meeting functionality is available. Calling and Messaging are done via Teams. 'SkypeMeetingsApp' means use the web-downloadable app. This setting can be useful for organizations that have upgraded to Teams and no longer want to install Skype for Business on their users' computers. |

### Tenant Dial Plan

| Name | Description |
| :--- | :--- |
| **Identity** | The 'Identity' property is a unique identifier that designates the name of the tenant dial plan. 'Identity' is an alphanumeric string that cannot exceed 49 characters. Valid characters are alphabetic or numeric characters, hyphen \(-\) and dot \(.\). The value should not begin with a \(.\). |
| **Description** | The 'Description' property describes the tenant dial plan - what it's for, what type of user it applies to and any other information that helps to identify the purpose of the tenant dial plan. Maximum characters: 512. |
| **External Access Prefix** | The 'External Access Prefix' property is a number \(or set of numbers\) that designates the call as external to the organization. \(For example, to tenant-dial an outside line, first press 9.\) This prefix is ignored by the normalization rules, although these rules are applied to the remainder of the number. The 'Optimize Device Dialing' property must be set to True for this value to take effect. This property must match the regular expression \[0-9\]{1, 4}: that is, it must be a value 0 through 9 and one to four digits in length. The default value is 9. |
| **Optimize Device Dialing** | Specifies if the dial plan should optimize device dialing or not. |
| **Simple Name** | The 'Simple Name' property is a display name for the tenant dial plan. This name must be unique among all tenant dial plans within the Skype for Business Server deployment.This string can be up to 49 characters long. Valid characters are alphabetic or numeric characters, hyphen \(-\), dot \(.\) and parentheses \(\(\)\). |

### Upgrade Policy

| Name | Description |
| :--- | :--- |
| **Identity** | Identity of the Teams Upgrade Policy. |
| **Users** | List of users that will be granted the Upgrade Policy to. |
| **Migrate Meetings To Teams** | Specifies whether to move existing Skype for Business meetings organized by the user to Teams. This property can only be true if the mode of the specified policy instance is either TeamsOnly or SfBWithTeamsCollabAndMeetings, and if the policy instance is being granted to a specific user. It not possible to trigger meeting migration when granting TeamsUpgradePolicy to the entire tenant. |

### Users

| Name | Description |
| :--- | :--- |
| **Role** | User role in Team. |
| **Team Name** | Team NAme. |
| **User** | UPN of user to add to Team. |

### Voice Routing Policy

| Name | Description |
| :--- | :--- |
| **Identity** | Identity of the Teams Voice Routing Policy. |
| **Online Pstn Usages** | A list of online PSTN usages \(such as Local or Long Distance\) that can be applied to this online voice routing policy. The online PSTN usage must be an existing usage \(PSTN usages can be retrieved by calling the Get-CsOnlinePstnUsage cmdlet\). |
| **Description** | Enables administrators to provide explanatory text to accompany an online voice routing policy. For example, the 'Description' might include information about the users the policy should be assigned to. |

### Teams ⯈ Channels

| Name | Description |
| :--- | :--- |
| **Team Name** | Name of the team the Channel belongs to. |
| **Display Name** | Current channel name. |
| **Description** | Channel description. |

