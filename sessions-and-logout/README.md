# Session Management

A session is created in an application after a user successfully authenticates with it, this user data is stored on its server and used to track if the user is currently logged into the application, along with passing the active or inactive session details to other views/pages that are accessible within the app to maintain security and consistency.

Active sessions terminate depending on app configuration, some common options are below:

* `The user clicks logout.`

* `The user changes their password or performs a security-sensitive action.`

* `The session times out due to inactivity.`

* `The session reaches its maximum lifetime as set in its app configuration.`

* `The user signs in on another device`

# Terminating a session via logout
