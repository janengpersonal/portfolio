# List of Feature Configurations

Below are lists of feature configurations in the **Company Settings > Feature Configurations**

---

## General Feature Configurations

| Name | Type | Description |
|------|------|-------------|
| Session duration (mins) | STRING | Session TTL of Vault token (in minutes) |
| Access token duration (mins) | STRING | TTL of JWT (in minutes) |
| Max session | STRING | Maximum session TTL of Vault token (in minutes) |
| Continuous evaluation | BOOLEAN | Perform a continuous evaluation on room condition module for a specific company |
| Client onboarding via SMS (for WeChat MiniApp Governed) | BOOLEAN | To enable/disable the WeChat MiniApp onboarding flow without email. |
| Client onboarding via SMS (for WeChat Governed) | BOOLEAN | To enable/disable the Wechat onboarding flow without email. |
| URL of Privacy Policy | STRING | Privacy Policy URL for the company (shown in AM profile) |
| Create federated users without federated roles | BOOLEAN | Whether to allow federated user creation (SSO login) if no federated role is found. TRUE = allow; FALSE = prevent |
| Override org unit from identity provider | BOOLEAN | Whether to override AM's Org Unit with the one provided by external IdP upon SSO login. TRUE = override with new value; FALSE = keep current value |
| Default organizational unit upon login | STRING | Default organizational unit assigned to user upon login |
| Naming convention | ENUM | Naming convention shown in Chats list & Contacts list |
| External company | BOOLEAN | Whether to show specific attributes in Client profile |
| Mandatory external company | BOOLEAN | Whether External Company should be a mandatory attribute in the client profile. TRUE = mandatory; FALSE = optional |
| Default company time zone | STRING | To configure default timezone |
| Default company language | STRING | Default language to fallback to |
| Mandatory email | BOOLEAN | Whether email address should be mandatory info in the Client profile or not. TRUE = mandatory; FALSE = optional |
| Default User-Client role | STRING | Default User-Client role to apply when Users invites new client or when assigning Clients to Users. |
| Sound for incoming messages from users | STRING | Sound played to notify users when there is an incoming message from another user. |
| Sound for incoming messages from clients | STRING | Sound played to notify users when there is an incoming message from client. |
| Preview URL | BOOLEAN | Whether users can preview the URL sent to chat (usually preview contains page title & description). TRUE = show preview; FALSE = not show. |
| Teams Native | BOOLEAN | To enable/disable Microsoft Teams channel for AM |
| Supported client languages | STRING | Set of available languages to localize the client-facing text |
| Email reminder of missed messages to users | BOOLEAN | Boolean flag of whether a company would like to remind their employees (AM user) of missed messages from client via email |
| Max duration for email reminder of missed messages (mins) | STRING | The maximum period (in minutes) user can stay offline and still not receive email reminder. |
| Leap Work mobile | STRING | Mobile app which is used by employees (AM user) of the company |
| Unique identifier for SSO login | STRING | Field on Azure Active Directory entity that corresponds to federated ID returned by Microsoft OIDC login, e.g. mail |
| Phone number validation strategy | ENUM | The strategy to validate client's phone number - whether it should be against other clients only |
| Max records in bulk import | STRING | Define maximum number of records (lines) in csv file allowed to import clients. |
| Mandatory User fields for SCIM | STRING | Define which fields in user profile are mandatory when synchronizing data from SCIM. |
| This feature configuration is deprecated and no longer effective. | | |
| License consumptions | BOOLEAN | To display the current license consumptions in the License info page or not |
| Mandatory tags | BOOLEAN | Whether the tags field is mandatory or not for new client invite. TRUE = mandatory; FALSE = optional |
| Send automatic template when User is unassigned | BOOLEAN | Whether to send automatic template that is sent when AM is unassigned |
| Send automatic template when User is reassigned | BOOLEAN | Whether to send automatic template that is sent when AM is reassigned |
| Organization Admin log in session timeout | STRING | Login session timeout for Organization Admin portal |
| Unique phone number | BOOLEAN | Whether to validate unique phone number upon client profile creation. TRUE = phone number must be unique; FALSE = phone number can be duplicated |
| Silent phone number verification upon OTP binding (WeChat MiniApp Governed) | BOOLEAN | Whether to enable silent phone number verification upon OTP binding. TRUE = response will not include error and error will not shown in miniapp; FALSE = some error message will be shown on miniapp |
| Send webpage link to users for further profile access (WeCom Native) | BOOLEAN | [WeCom user profile] To enable/disable the automatic sending of webpage link to WeCom users to grant futher profile access. TRUE = send; FALSE = not send |
| User Group auto-assignment strategy | ENUM | Define a strategy to auto assign User Group to client profile upon creation |
| Mandatory First & Last names | BOOLEAN | Whether First Name and Last Name are mandatory or not for in client profile. TRUE = mandatory; FALSE = optional |
| Onboarding guide on Organization Admin | BOOLEAN | To enable/disable in-app onboarding guide in Org Admin portal |
| User and client search mode | ENUM | Select the User and Client search mode. QUICK_SEARCH = search using no filter; FILTERED_SEARCH = search using a specific filter. |
| Block direct chats when permissions are lost | BOOLEAN | Whether to block existing 1:1 chats on a specific channel if a user loses permissions on such channel. TRUE = block; FALSE = allow. |
| Send onboarding email upon user creation | BOOLEAN | Default logic to send onboarding emails (including Leap Work credentials and mobile activation code) to users upon their creation or not. TRUE = send emails; FALSE = not send. |
| Auto promotion of NVC | BOOLEAN | Whether a contact will be auto-promoted when initiating inbound communication flow. TRUE = auto-promoted; FALSE = contact will become a prospect and requires manual promotion from the user. |
| Unique email address | BOOLEAN | Whether to validate unique email address upon client profile creation. TRUE = email must be unique; FALSE = email can be duplicated. |
| Enable consent form feature for miniapp channel at the wechat official account, configure things at wechatminiapp_DBConsentForm | BOOLEAN | [WeChat MiniApp] Enable the consent form for MiniApp |
| Whether BYOK encryption is enabled | BOOLEAN | Enable the BYOK encryption. By setting this to TRUE, the audit log messages will become BYOK encrypted. |
| BYOK encryption for Client Profile PII | BOOLEAN | Whether BYOK encryption is enabled for Client Profile PII. When the value is set to TRUE, Client Profile containing PII will be encrypted. However, they can only be searched using exact values. If set to FALSE, the PII fields will not be encrypted using your own key. The search functionalities |
| To enable Network-based SMS channel | BOOLEAN | Enable the Network-based SMS channel if set to TRUE. If set to FALSE, not enable this channel. |
| Define maximum number of records (users) per Bulk Integration run | STRING | The accepted maximum amount of users per Bulk Integration request. |
| Microsoft Outlook contact synchronization | BOOLEAN | Enable synchronization of business contacts from Microsoft Outlook. |
| Hide the Permission dialog | BOOLEAN | If set to TRUE, the system will not display the Permission dialog listing all required permissions you need to enable to access Leap Work mobile. If set to FALSE, the system will still display the Permission dialog. |
| Disable Auto correct/ complete | BOOLEAN | [Leap Work mobile] To disable auto correct/ auto complete. If set to TRUE, disable the functionality. If set to FALSE, enable the auto correct/ complete. |
| Enable Suggestion capability on Android | BOOLEAN | To enable Suggestion capability on Leap Work Android. If set to TRUE, enable the functionality, if set to FALSE, disable the functionality. |
| Desktop notification for unread messages | STRING | Show desktop notification for unread messages in Leap Work web. |
| Disable application logs local device | BOOLEAN | [Leap Work mobile] To disable Leap Work mobile app to store application logs to local device.  |
| Activation code expiration duration | STRING | The duration until the activation code to link mobile device expires. |
| Teams chat naming convention | STRING | Configure the name of the 1-1 and group chats in Teams. |
| Teams - Client naming convention in messages | STRING | Configure the naming of clients inside the MS Teams chat messages in standard card style. |
| Teams - Purview integration | BOOLEAN | Enable the Purview integration. If enabled, the system will block messages based on Purview DLP policies. |
| Teams - Purview DLP wait time for outgoing messages | JSON_MAP | Configure the initial wait time (in milliseconds) for Microsoft Purview DLP to notify the system of outgoing message violation. If the notification is received within this wait time, the message will not be delivered to the client. |
| Teams - Incoming file thumbnail | BOOLEAN | Enable thumbnails for incoming file messages in the Teams chats. |
| Purview integration - Automatic replies for incoming client messages | BOOLEAN | Enable automatic replies to external clients when their messages violate Purview DLP policies. This configuration is currently applicable to text messages. |
| Audio transcription | BOOLEAN | Enable the audio transcription for all Users in a company |
| Message authorship | BOOLEAN | Whether system should access impersonation probability of each message sent to chat room |
| Monitoring & alert when failed to connect to DLP | STRING | Enable monitoring and alerting for connecting to DLP's third party. |

---

## Verification attributes

| Name | Type | Description |
|------|------|-------------|
| Verification link in welcome message (WeCom Native) | BOOLEAN | [WeCom client verification] Whether clients would receive verification link in automatic welcome message when they are added as WeCom contact. TRUE = include verification link in automatic message; FALSE = not include. |
| Days for re-verification (WeCom Native) | STRING | [WeCom client re-verification] The number of days that the verification of a WeCom client expires. When this time is reached. |
| Days to remind users for client re-verification (WeCom Native) | STRING | [WeCom client re-verification] The interval (in days) to repeat WeCom native notification which reminds the in-charge user that the client has to re-do their verification. |
| Active chats - days of last message (WeCom Native) | STRING | [WeCom client re-verification] The last message of a 1:1 chat between user & client has to fall within this period (in days) from today in order for the chat to be considered as active. |
| MFA for clients based on tags (WeCom Native) | BOOLEAN | [WeCom client re-verification] Whether to trigger multiple-factor verification for clients with specific tag value(s) in their profile or not. TRUE = enable for specific clients; FALSE = not enable. |
| Tag value(s) to trigger MFA (WeCom Native) | STRING | [WeCom client re-verification] Specific tag value(s) that will trigger multiple-factor authentication once added to the profile of a client. |
| Terms & Conditions in the Input Phone Number screen (WeCom Native) | BOOLEAN | [WeCom client verification] Whether to include the Terms & Conditions screen in the Input Phone Number screen or not. TRUE = Terms & Conditions is shown as a checkbox in Input Phone Number screen. FALSE = Terms & Conditions is a separate screen before Input Phone Number screen. |
| Terms & Conditions URL (WeCom Native) | STRING | [WeCom client verification] The URL of Terms & Conditions in verification link when the T&C checkbox is combined with Phone number input screen. |
| Banner in verification email (WeCom Native) | STRING | Banner displayed in a verification email. |
| Terms & Conditions page content (WeCom Native) | JSON_MAP | [WeCom client verification] The Terms and Conditions content when the T&C page is separated from the Phone number page. |
| Days to clear verification progress (WeCom Native) | STRING | [WeCom client re-verification] Days to clear the status memory of remembering the verification progress. |
| Max verification OTP wrong input | NUMBER | [Workflow Verification] The max number times for clients to enter wrong verification code in a verification session. |
| Max new verification OTP request | NUMBER | [Workflow Verification] The max number of times for clients to request for new verification code in a verification session. |
| Max OTP duration (mins) | NUMBER | [Workflow Verification] The expired duration of an OTP in ad-hoc. |
| Periodic verification (WhatsApp Governed) | BOOLEAN | [WhatsApp Verification] To enable periodic verification for Clients in Governed WhatsApp channel. |
| Verification expiration duration (days) (WhatsApp Governed) | NUMBER | [WhatsApp Verification] The number of days that the verification of a WhatsApp client expires. |
| Device-change verification (WhatsApp Governed) | BOOLEAN | [WhatsApp Verification] To enable verification for Clients in Governed WhatsApp channel whenever they change to a new device. |
| Duration to skip ad-hoc verification (mins) | NUMBER | [Workflow Verification] The duration (in minutes) for client to skip ad-hoc verification after confirming on a media template. |
| Verification workflows excluded from verification skip rule | STRING | [Workflow Verification] Customize the list of verification workflows that are excluded from the skipping ad-hoc verification rule. |
| Periodic verification (WeChat MiniApp Governed) | BOOLEAN | [WeChat MiniApp Verification] To enable periodic verification for Clients in WeChat MiniApp channel. |
| Verification expiration duration (days) (WeChat MiniApp Governed) | NUMBER | [WeChat MiniApp Verification] The number of days that the verification of a WeChat MiniApp client expires |
| Manual periodic verification | BOOLEAN | [Client Verification] To allow AMs to manually enable periodic verification for clients or not. TRUE = periodic verification is manually enabled by AMs for each client after onboarding. FALSE = Client is automatically verified after onboarding |
| Device-change verification | BOOLEAN | [WeChat MiniApp Verification] To enable verification for Clients in WeChat MiniApp channel whenever they change to a new device |
| Reminder before verification expires (WeChat MiniApp Governed) | JSON_MAP | [Client Verification] To remind the client to re-verify their account before it expires or not |
| Reminder before verification expires (WhatsApp Governed) | JSON_MAP | [Client Verification] To remind the client to re-verify their account before it expires or not. |
| Onboarding verification (WhatsApp Governed) | BOOLEAN | [WhatsApp Verification] To enable onboarding verification for Clients in WhatsApp Governed channel. |

---

## Other features attributes

| Name | Type | Description |
|------|------|-------------|
| Verification link in welcome message | BOOLEAN | [Terms of Use] Whether user acceptance for Terms of Use should be enforced upon login. TRUE = show dialog to prompt acceptance; FALSE = not show. |
| Out-of-office (OOO) | BOOLEAN | [Out Of Office] Whether to enable Out Of Office feature at company level. TRUE = enable; FALSE = disable |
| Alternate contact for OOO | BOOLEAN | [Out Of Office] Whether to allow user to select an alternate contact to include in the automatic reply. TRUE = show; FALSE = hide |
| Max participants in a broadcast group | STRING | [Broadcast] Control number of maximum members allowed to add in a broadcast group |
| Prompt when sharing attachments with clients (web/desktop) | BOOLEAN | [External Recipient Confirmation] Whether to prompt user confirmation on external recipients whenever they try to share attachments to a chat involving clients on browser/desktop. TRUE = show confirmation popup; FALSE = not show |
| Prompt when sharing attachments with clients (mobile) | BOOLEAN | [External Recipient Confirmation] Whether to prompt user confirmation on external recipients whenever they try to share attachments to a chat involving clients on mobile. TRUE = show confirmation popup; FALSE = not show |
| Prompt content when sharing attachments with clients | STRING | [External Recipient Confirmation] Message to warn users & ask for their confirmation for sharing attachment with external recipients |
| Remind clients to delete files (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp File Transfer] Whether system should remind external clients to delete the file in native WeChat file transfer folder after sharing a file or not. TRUE = show reminder; FALSE = not show |
| Client onboarding on-behalf | BOOLEAN | [Client Onboarding On-behalf] Whether a user can initiate the client onboarding on behalf of another user or not. TRUE = allow; FALSE = not allow |
| Default User-Client role for onboarding on-behalf of another user | STRING | [Client Onboarding On-behalf] The user-client role that will be automatically used for the user when he initiates client onboarding on behalf of another user |
| Default User-Client role for onboarding on-behalf of oneself | STRING | [Client Onboarding On-behalf] The user-client role that will be automatically used for the user when another user initiates client onboarding on behalf of him/her |
| Include ethical groups for room conditions re-evaluation | STRING | [Room Conditions] List of Azure AD groups to monitor for continuous evaluation of room conditions |
| Username in User Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show username in User Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Client email in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client email in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Client phone number in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client phone number in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Username in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client username in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Privacy Policy link in User Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show Privacy Policy link in User Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Private contact | BOOLEAN | [Private Contact] To enable/disable private contact feature. If enabled |
| Max private contacts per user | STRING | [Private Contact] Configure the maximum number of private contacts allowed per user (not company) |
| User-Client role for private contacts | STRING| [Private Contact] Default user-client role applied at company level when inviting new private contact or assigning private contact to user|
| Verification link in welcome message | BOOLEAN | [Terms of Use] Whether user acceptance for Terms of Use should be enforced upon login. TRUE = show dialog to prompt acceptance; FALSE = not show. |
| Out-of-office (OOO) | BOOLEAN | [Out Of Office] Whether to enable Out Of Office feature at company level. TRUE = enable; FALSE = disable |
| Alternate contact for OOO | BOOLEAN | [Out Of Office] Whether to allow user to select an alternate contact to include in the automatic reply. TRUE = show; FALSE = hide |
| Max participants in a broadcast group | STRING | [Broadcast] Control number of maximum members allowed to add in a broadcast group |
| Prompt when sharing attachments with clients (web/desktop) | BOOLEAN | [External Recipient Confirmation] Whether to prompt user confirmation on external recipients whenever they try to share attachments to a chat involving clients on browser/desktop. TRUE = show confirmation popup; FALSE = not show |
| Prompt when sharing attachments with clients (mobile) | BOOLEAN | [External Recipient Confirmation] Whether to prompt user confirmation on external recipients whenever they try to share attachments to a chat involving clients on mobile. TRUE = show confirmation popup; FALSE = not show |
| Prompt content when sharing attachments with clients | STRING | [External Recipient Confirmation] Message to warn users & ask for their confirmation for sharing attachment with external recipients |
| Remind clients to delete files (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp File Transfer] Whether system should remind external clients to delete the file in native WeChat file transfer folder after sharing a file or not. TRUE = show reminder; FALSE = not show |
| Client onboarding on-behalf | BOOLEAN | [Client Onboarding On-behalf] Whether a user can initiate the client onboarding on behalf of another user or not. TRUE = allow; FALSE = not allow |
| Default User-Client role for onboarding on-behalf of another user | STRING | [Client Onboarding On-behalf] The user-client role that will be automatically used for the user when he initiates client onboarding on behalf of another user |
| Default User-Client role for onboarding on-behalf of oneself | STRING | [Client Onboarding On-behalf] The user-client role that will be automatically used for the user when another user initiates client onboarding on behalf of him/her |
| Include ethical groups for room conditions re-evaluation | STRING | [Room Conditions] List of Azure AD groups to monitor for continuous evaluation of room conditions |
| Username in User Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show username in User Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Client email in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client email in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Client phone number in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client phone number in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Username in Client Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show client username in Client Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Privacy Policy link in User Profile (WeChat MiniApp Governed) | BOOLEAN | [WeChat Miniapp] Whether to show Privacy Policy link in User Profile page in Miniapp or not. TRUE = show this info; FALSE = hide |
| Private contact | BOOLEAN | [Private Contact] To enable/disable private contact feature. If enabled |
| Max private contacts per user | STRING | [Private Contact] Configure the maximum number of private contacts allowed per user (not company) |
| User-Client role for private contacts | STRING | [Private Contact] Default user-client role applied at company level when inviting new private contact or assigning private contact to user |
| Username strategy | JSON_MAP | [Client Profile] Client code name auto-generation strategy |
| External company ID strategy | JSON_MAP | [External Company] External Company ID auto-generation strategy |
| Org Unit auto-assignment strategy | ENUM | [Organizational Unit] Define a strategy to auto assign Org Unit to client upon client’s invitation |
| OTP delivery method (WeChat MiniApp Governed) | ENUM | [WeChat MiniApp] Select how the OTP to be delivered to the client in the email onboarding flow |
| Send auto messages to chat rooms (WhatsApp Native) | JSON_MAP | [WhatsApp Native] To send automatic messages to archived chat rooms or not. |
| Restriction on invalid OTP attempts (WeChat MiniApp Governed) | JSON_MAP | [Wechat Miniapp] To enable restriction on invalid otp attempts or not. |
| Restriction on OTP attempts (WeChat MiniApp Governed) | JSON_MAP | [Wechat Miniapp] To enable restriction on resend otp attempts or not. |
| Restriction on phone number attempts (WeChat MiniApp Governed) | JSON_MAP | [Wechat Miniapp] To enable restriction on phone number otp attempts or not. |
| Onboarding guide on Leap Work mobile | BOOLEAN | [User Guide] Show the guidance for users on Leap Work application. |
| User quickstart guide on Leap Work web | BOOLEAN | [User Guide] Show the quickstart for users on Leap Work Web. |
| Text message character limit | NUMBER | The character limit of a text message user can send to a client. |
| User profile synchronization with Azure upon Teams SSO | BOOLEAN | Whether to enable synchronization between Azure and LeapXpert user feature configurations upon every Teams SSO event. TRUE = enable; FALSE = disable. |
| Block WhatsApp calls | BOOLEAN | [Android only] To block calls between WhatsApp numbers in WhatsApp application. |
| Block WhatsApp unlink actions | BOOLEAN | [Android only] To block users from unlinking FMOP devices in WhatsApp's Linked Devices section. |
| Message card style | ENUM | The card style that is displayed in Teams for all messages. ADAPTIVE_CARD = message with media such as channel logo & avatar; STANDARD_CARD = message displayed as plain text. |
| Reminder for 'Resume conversation' (WhatsApp Governed) | JSON_MAP | To send a reminder template message to WhatsApp clients to resume the conversation when being out of the 24h customer care window. TRUE = send reminders, FALSE = no reminder. |
| Prevent copying content | JSON_MAP | [Leap Work Mobile] To prevent users from copying and pasting contents from/to Leap Work Mobile or not. TRUE = prevent, FALSE = allow. |
| Data retention delay alert | BOOLEAN | Whether the data retention feature is enabled for this company. TRUE = enabled, FALSE = disabled. |
| Allow taking screenshots | BOOLEAN | [Leap Work Mobile] To allow users to take screenshots of Leap Work Mobile or not. TRUE = allow, FALSE = prevent. |
| Order of onboarding templates (SMS Governed) | ENUM | [SMS Governed] Sequential order to send onboarding templates to clients. |
| Send relink email (WhatsApp Native) | BOOLEAN | |
