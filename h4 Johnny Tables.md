## h4 Johnny Tables

# x) Summaries

# Broken access control

Sitting at the first spot of the OWASP top 10, Broken access control is the most frequent app security risk.
It allows users to gain some privilleges that they are not supposed to have. For example, they can:

- View sensitive data belonging to others.

- Change or delete other people's files.

- Perform "Admin" actions without being an admin.

To prevent it, it is recommended to follow these principles:

- deny by default

- The server must check permissions every single time.

- check if a user is logged in; check if they actually own the specific data they are trying to access.

- Disable directory listing

- Monitor the logs and setup alerts

# Security misconfiguration

Number 2 of the latest OWASP Top 10. It happens when the configuration of the security has not been done or has been incorrectly. 
This can creates backdoors for attackers. It is often the result of a human error.

It may happen in many ways (ex: default/weak passwords, misconfiguration of a security setting on your public cloud account, etc)

To prevent it, you should:

-  environments should all be configured identically, with different credentials used in each environment. This process should be automated to minimize the effort required to set up a new secure environment.

-  A minimal platform without any unnecessary features

-  change the default passwords and disable default accounts.

-  Ensure the website only shows generic error messages to users. Keep the detailed technical logs hidden on the server for developers only.

