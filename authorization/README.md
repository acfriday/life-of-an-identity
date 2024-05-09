# Authorizing an Identity to Access Internal Resources

After the creation of an account, it's commonly necessary to provide privileges that will allow it to interact with internal resources. If an attempt to access private data is performed by a requester lacking proper permissions there is usually a specific error message that will be returned to the requester to identify this to them. Using the principle of least privilege admins can assign a role that suits an identity's needs and assign those to authorize access to any desired internal resource.

## API Registered on Entra ID

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/8d789408-fd02-4336-bb26-cfb2b31f924b)

The `UserManagementRestAPI` identity belongs to an API that will be attempting to list a user from the Microsoft Entra ID tenant where it's registered to verify the user is present in the organization, after this the API will delete that user from the organization. When attempting to perform this action before that is done this error is returned.

## Example - Permissions Error When Querying The User

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/07721dbd-91fc-492a-b89c-308068919ad7)

To authorize this action the principle of least privilege will be followed to provide the necessary permissions needed to list and delete users in the organization for the application type API.

### Adding Proper Permissions To Authorize The API

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/1908b16a-4b0b-495a-9f21-00fca24b5241)

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/34a92860-bad8-4b6c-808d-9bff093bf25c)

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/0ba55206-bc44-46cc-8cc5-683e964f60ff)

## Example - Re-Attempting To List The Desired User

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/99e0eb0f-8bf2-4d61-9c64-a2819e2fff23)

## Example - Deleting The User Account

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/9727f4b7-72c7-42dd-8bd4-e69c4671ca75)

This request returns a `204 No Content` response code. We'll list the user again since this doesn't return data to confirm account deletion.

## Example - List The User's Account Again To Confirm It's No Longer Active In The Organization

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/4b34a365-1a9c-47a2-8f4b-af64739c5e4c)
