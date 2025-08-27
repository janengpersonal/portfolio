# Signal Governed integration functionalities

This document highlights features that are currently supported in Signal Governed channels in the latest version of the LeapXpert communication platform.  

| Icon | Description |
|------|-------------|
| ✅| Support |
| ❌| Currently not supported |
| ⚠️| Supported but with known issue/limitation | 
| N/A | Not available due to channel limitations|

---

## Captured events for direct chat

| Functions | Supported? | Audit log |
|-----------|-------------|-----------|
 Text |  ✅ |✅ |
Image + video from gallery | ✅ |✅  |
Audio + voice note |✅  | ✅ |
Photo + video from camera | ✅ |✅  |
Sticker | ❌ | ❌ |
GIF |✅  | ✅ |
Location | ✅ | ✅ |
Poll | ❌ |  ❌ |
Office files | ✅ | ✅ |
Contact card | ❌  |  ❌ |
Voice/video call event | N/A | N/A |
Template message | N/A | N/A |
Edited messages |  ❌ | ❌  |
Replied messages |⚠️The replied message is captured as a normal message without quoted text. | ✅ |
Forwarded messages |⚠️ The forward message is captured as a normal message without quoted text. | ✅ |
 Unsend messages | N/A | N/A |
 Deleted messages | ❌  |  ❌ |
Reaction |  ❌ |  ❌ |
Delete chat room | ❌  | ❌  |
Archive chats |  ❌ |  ❌ |
Text | ✅ | ✅ |
Image | ✅ | ✅ |
Audio/Voice note | ✅ | ✅ |
Video | ✅ | ✅ |
File | ✅ | ✅ |
Replied messages |⚠️ Only support replied with text. The replied message is captured as a normal message without quoted text. | ✅ |
Forward messages |⚠️ The forward message is captured as a normal message without quoted text. | ✅ |
Message template | N/A | N/A |
Workflow | N/A | N/A |
Message delivery status |⚠️ Only capture the Delivered status. |⚠️ Only capture the Delivered status. |

---

## Captured events for group chat

| Features | Functions | Supported? | Audit log |
|----------|-----------|-------------|-----------|
| Group chats | Send files to a group | ⚠️There is no indicator of the file sender in a group chat. Some file types might not go through. | ✅ |
| Group chats | Send text messages to a group |✅  | ✅|
| Group chats | [System message] Joiner/Leaver notification |  ❌ | ❌  |

---

## Other features

| Features | Functions | Supported? | Audit log |
|----------|-----------|-------------|-----------|
| Data Leakage Prevention (DLP) | DLP warning for messages from Clients |  ❌ |  ❌ |
| DLP | DLP warning for messages from Users |  ❌ | ✅ |
| DLP  | DLP block for messages from Clients |  ❌ |  ❌ |
| DLP | DLP block for messages from Users | ✅ | ✅ |
| Room conditions | Set poisoned rooms |  ❌ |  ❌ |
