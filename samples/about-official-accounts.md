# Official Accounts

Official accounts are phone numbers registered with third-party services like **WhatsApp, WeChat, LINE, SMS, and more**.  

They are used when:  
- Employees communicate with clients without using personal phone numbers.  
- Company employees need to communicate with clients outside their country.  

There are two types of official accounts:  
1. **Official accounts for dedicated phone numbers** – dedicated for a user only.  
2. **Official accounts for shared pools** – many users share phone numbers.  

This article provides a definition, lists different types of official accounts, and explains their application on the LeapXpert platform.  

---

## Official Accounts for Dedicated Phone Numbers

An official account for dedicated phone numbers is provisioned to a **User** and dedicated for that User only.  
You can configure a dedicated phone number for a User to start a direct business conversation with clients.  

- From **LeapXpert version 1.22.1** onwards, you can configure dedicated phone numbers for **WhatsApp Governed integration**.  
- From **LeapXpert version 1.24.0** onwards, you can configure dedicated phone numbers for **SMS Governed integration**.  

This is an attempt towards our approach to the **Single Professional Identity**, in which users are expected to use the same phone number across all Governed channels and to have phone numbers dedicated to a User (instead of shared number pools).  

---

## Official Accounts for Shared Pool

With official accounts for shared pools, multiple users share access to official business accounts (**WhatsApp, WeChat, Telegram, etc.**) without needing individual logins for each account.  

- Official accounts are assigned to different **pools**, with each pool allocated to specific **organizational units (OUs)** and accessible to members of those OUs.  
- A pool consists of **primary** and **secondary** accounts.  

### Primary Account
- Used for prospects to contact the company.  
- Used to receive OTP from periodic verification.  

### Secondary Account
- Used for clients’ onboarding and communication.  

---

## Official Accounts Selection Process

When a client from the same organizational unit is invited to a channel, the system will follow these rules to select the official account for communication:  

### 1. Matching by Country Code
- The system checks the client’s country.  
- It looks for an official account in the pool with the same country code.  
- If a match is found, that account is used.  

### 2. Applying Fallback Rules (If No Match Found)

- **Geography Mapping Rule**  
  The system checks if the client’s country is mapped to a different country in the geography mapping rules.  
  If a mapping exists, the system finds a matching secondary official account and uses it.  

- **Default Region Rule**  
  If selected, the system assigns an official account from the default country set in the pool.  

- **Fallback Upward Rule**  
  If enabled, the system searches for an official account in higher-level OUs, using the same selection process.  

### 3. Error Handling
- If no suitable official account is found after all these steps, the system returns an error and terminates the communication.  

---

## Notes

- For **WhatsApp, SMS, iMessage**, in addition to primary official accounts, secondary official accounts are **required** to maintain conversations between clients and company employees.  
- **Secondary official accounts are not needed for WeChat Miniapp**; this channel uses **primary official accounts (email)** to facilitate communication.  
- For **Signal**, users use secondary accounts to communicate.  

---

## See Also

To understand the application of official accounts shared pools for each channel:  
- [Configure official account pools for WhatsApp and SMS Governed integration]()  
- [Configure official account pools for WeChat MiniApp Governed integration]()  
- [Configure official account pools for Signal Governed integration]()  
- [Configure official account pools for iMessage Governed integration (Preview version)]()  
- [Official account number recycling]()  
