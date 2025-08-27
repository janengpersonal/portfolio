# Telegram Native integration functionalities

This document highlights features that are currently supported in Telegram Native channels in the latest version of the LeapXpert Platform.

**Icon:**
- ✅ Supported  
- ❌ Currently not supported  
- ⚠️ Supported but with known issue/limitation  
- N/A – Not available due to channel limitations  

---

## Captured events

### Messaging functionalities

| Feature / Function        | Telegram                                                                 |
|---------------------------|--------------------------------------------------------------------------|
| Text                      | ✅ Supported                                                             |
| Image                     | ✅ Supported                                                             |
| Audio + voice note        | ✅ Supported                                                             |
| Video from gallery        | ✅ Supported                                                             |
| Video from camera         | ⚠️ Supported but with known issue/limitation. <br>*In Android, LeapXpert cannot capture videos if sent directly from the camera, or with compression.*<br> **Workaround:** Send via File option or *Send without compression*. |
| File                      | ✅ Supported                                                             |
| Emoji messages            | ✅ Supported                                                             |
| GIF                       | ✅ Supported                                                             |
| Sticker                   | ⚠️ Supported but with known issue/limitation. <br>Dynamic stickers are displayed in raw files. |
| Location                  | ⚠️ Captured but displays [Unsupported content].                          |
| Contact card              | ⚠️ Captured but displays [Unsupported content].                          |
| Poll                      | ⚠️ Captured but displays [Unsupported content].                          |
| Voice/video call event    | ❌ Currently not supported                                                |
| Template message          | N/A                                                                      |
| Edited messages           | ✅ Supported                                                             |
| Replied messages          | ✅ Supported                                                             |
| Forwarded messages        | ✅ Supported                                                             |
| Recalled messages         | N/A                                                                      |
| Deleted messages          | ✅ Supported                                                             |
| Reaction                  | ✅ Supported                                                             |
| New contact joins Telegram| ⚠️ Captured but displays [Unsupported content].                          |
| Delete chat room          | ⚠️ Captured as Deleted for the new contact event.                        |
| Chats archived in Telegram| ❌ Currently not supported                                                |

---

### Group chats

| Feature                   | Telegram  |
|----------------------------|-----------|
| Create group               | ✅ Supported |
| Get added to a group       | ✅ Supported |
| Leave group                | ✅ Supported |
| Get removed from a group   | ✅ Supported |
| Add/Remove member          | ✅ Supported |
| Update group name          | ✅ Supported |
| Update group avatar        | ✅ Supported |
| Promote/Dismiss admin      | ✅ Supported |
| Create broadcast groups    | N/A       |
| Group invite               | N/A       |

---

### Generic

| Feature                                                                 | Telegram  |
|--------------------------------------------------------------------------|-----------|
| [Leap Work web/mobile] Display channel integration status in client tab | ✅ Supported |

>**Note:** Excessively large files will be blocked and recorded in the Archiving Export and Audit log. File types include pdf, video, audio...etc. The default limitation is currently **100 MB**.  

---

## Supported features

### Onboarding/Offboarding activities

Feature                                                   | Telegram |
-----------------------------------------------------------|----------|
 Audit log                                                        | ✅ Supported 
| Activate messaging identity  (Leap Work web/mobile)                             | ✅ Supported |
Deactivate messaging identity (Leap Work web/mobile)                            | ✅ Supported |
Promote/Demote Client to AM (Leap Work web/mobile)                               | ✅ Supported |
Separate one-to-one chats between AM & Client after promotion (Leap Work web/mobile)  | N/A   |
Terminate session in Telegram after deactivation (Leap Work web/mobile)          | N/A      |
 Update status after the session gets terminated in Telegram (Leap Work web/mobile)  | N/A    |
Create Clients after importing messages/adding to a group (Leap Work web/mobile)  | ⚠️ Captured event as Update client profiles. |
Auto-assign client to AM after creation (Leap Work web/mobile)                  | N/A      |
Display Business or Personal account (Leap Work web/mobile)                       | N/A      |
Last status change time (Leap Work web/mobile)                                   | N/A      |
White-labeling (Leap Work web/mobile)                                            | N/A      |
Activate messaging identity  (Org Admin portal)                             | ✅ Supported |
Deactivate messaging identity  (Org Admin portal)                          | ✅ Supported |

---

## Notification features

| Feature                                                                                  | Telegram | Audit log |
|------------------------------------------------------------------------------------------|----------|-----------|
| Send email notifications when activating/deactivating messaging identity                 | N/A      | —         |
| Send notifications & disclaimers to chat rooms when archiving starts/stops               | N/A      | —         |
| Send native app notifications when message violates Data Leakage Prevention policy       | N/A      | —         |
| Send native app notifications when room conditions are violated                          | N/A      | —         |
| Send notifications on Leap Work web/mobile when a message violates DLP policy            | ✅ Supported <br>*Note: DLP doesn’t block but only warns. Does not ignore Unsupported content.* | — |
| Send notifications on Leap Work web/mobile when room conditions are violated             | ✅ Supported <br>*Note: Room condition doesn’t block but only warns the poisoned room.* | — |
