# ABC
## This is for testing
With LeapXpert platform, admins can send email instructions directly to assigned Users to help them self-onboard their iMessage accounts for message archiving. 
From version 2.3.2 onwards, users who use Managed Apple ID federated with Okta can self-onboard iMessage accounts. Users can verify their accounts with two authentication methods:
Password only
Password and Okta Verify - Push notification
This guide explains how to self-onboard with Okta using email, password, without the need to use Okta Verify app.
For self-onboarding with Okta using email, and password only, see Self-Onboarding iMessage Native for Managed Apple ID with Okta (Email and Password Only authentication method)
Important:
- Admins cannot access the Mac that has been issued to users for self-onboarding. 
- Admins can no longer activate iMessage native on behalf of users who are assigned to self-onboard. To learn more about onboarding iMessage Native on-behalf of users, see: Configure iMessage Native integration in Organization Admin on the OS level.
Before you start
For admins
Ensure the Managed Apple ID login authentication methods are supported.
Have following permissions:
View list of corporate phone number provisionings.
Edit corporate phone number provisioning.
Activate user’s messaging identities (AM users & admins).
Deactivate user’s messaging identity (AM users & admins).
Request Mac machines set up exclusively for self-onboarding.
Enable iMessage Native self-onboarding on the Org Admin portal (Company Settings > Feature Configurations > com.leapxpert.imessage_native.self-onboarding).
For AM users
Double-check Apple ID details.
Set up iCloud for Messages, Keychain and Contacts. For more information, check Prepare your iPhone and iMessage account: A step-by-step guide.
Use desktop browser for self-onboarding (highly recommended).
Note: Those practices ensure a frictionless self-onboarding process.
