# Authenticating Digital Identities

To access resources in your organization that are not publicly available, an entity will need to provide credentials. These credentials are the personal identifiers that were used to register an account for said entity in your org. Once provided, these credentials will be validated against the target account's currently stored personal identifiers that were taken during its registration.

The full process of authentication could require the receipt of various personal identifiers tied to the previously registered account. With those requirements usually being something the entity ***is***, ***knows***, or ***has***. A fingerprint for example would be something the user is. A password would be something the user knows. And a time-based two-factor authentication code can be something the user has.

When a user has a previously registered account in a Microsoft ID tenant, that user can user input their credentials and authenticate with the Microsoft tenant. When the requirements are only something the user both ***knows*** and ***has***, authentication would look like the below:

## Example - Authenticating with a Microsoft Entra ID Tenant

#### *Username/Email* - **`Something the user knows`**

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/d64fe33c-2603-47e0-b56f-790f90b73a78)


#### *Password* - **`Something the user knows`**

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/f832bb9f-f4df-4699-8750-8a8a03fbd09c)


#### *2FA Code* - **`Something the user has`**

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/c44f6910-0ce5-4b09-a0f3-62bd5ca429bf)

## **Post-Authentication Success**

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/6de214d1-449f-4216-9d21-b69719db2fb5)




