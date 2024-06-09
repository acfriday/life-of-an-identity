# Session Management

A session is created in an application after a user successfully authenticates with it, this user data is stored on its server and used to track if the user is currently logged into the application, along with passing the active or inactive session details to other views/pages that are accessible within the app to maintain security and consistency.

Active sessions terminate depending on app configuration, some common options are below:

* `The user clicks logout.`

* `The user changes their password or performs a security-sensitive action.`

* `The session times out due to inactivity.`

* `The session reaches its maximum lifetime as set in its app configuration.`

* `The user signs in on another device`

## Example - Session lifetime with Microsoft Entra ID

After successfully authenticating with Microsoft the  `Keep me signed in (KMSI) process is initiated with the user:

![image](https://github.com/acfriday/life-of-an-identity/assets/82184168/66b7d955-fd77-44c0-a2fc-a887dfee2602)

If `Yes` is selected for the `Stay signed in?` prompt, Azure generates a persistent authentication cookie and uses the persistent cookie to extend the user session and revokes the cookie only after the user logs out.

# Session Timeout and Logout

Session Timeout and Session Logout are two distinct mechanisms that serve different purposes. Here's a breakdown of their configuration differences below:

* ### Session Timeout
  A session timeout revolves around the two primary concepts of lifetime expiration and user inactivity. User inactivity is acknowledged by the application after a user hasn't 
  performed any actions in the application for a predetermined time. This inactivity will automatically trigger the session's termination unless actions are performed beforehand. 
  Lifetime expiration on the other hand is an explicitly set maximum duration a user session is allowed to remain active, regardless of any user activity, when this time is 
  reached their session will be terminated.

* ### Session Logout

  A session logout is an explicit request made by an end-user, admin, or system user to the application they're authenticated with to signal their desire for their current 
  session to be terminated. This manual process focuses on preventing access to the user's account and requires re-authentication before being granted access again.
