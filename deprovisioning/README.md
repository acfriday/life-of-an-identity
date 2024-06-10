# Deprovisioning Digital Identities

Deprovisioning is the act of removing a user's access to internal applications when an identity needs to be offboarded entirely from an organization, or temporarily disabled for various reasons with one common reason being an investigation into actions performed by the account until the owner can be cleared of any wrongdoing. Deprovisioning is a critical security process designed to ensure sensitive internal resources are protected from future access, and account data is properly discarded excluding any data required for future auditing.

## Deleting a User Account In Microsoft Entra ID
* When a user is deleted they no longer appear on the `All users` page. The user will be available on the `Deleted users` page for the next 30 days where they can be restored during that time window if needed. Any licenses tied to the user will be made available for other users in the organization after account deletion.

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/96addc7d-d943-4f93-a91c-aaa23837933d)

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/19ce38b7-7a84-46f1-9f18-a761e537b16d)

### Disabling a User Account In Microsoft Entra ID
* Disabling an account provides a flexible and secure way to manage user access. This option supports security investigations, compliance requirements, temporary suspensions, risk mitigation during policy changes, and the preservation of historical data without removing the account from the identity platform so it can be quickly reused or reinstated if needed.

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/688aefe4-0483-45cd-bbc0-63b860fc5049)

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/f671cb66-9973-4f18-ba2f-bb5e5d6e662c)
