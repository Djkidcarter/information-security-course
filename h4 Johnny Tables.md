## h4 Johnny Tables

# x) Summaries

# Broken access control

Sitting at the first spot of the OWASP top 10, Broken access control is the most frequent app security risk.
It allows users to gain some privilleges that they are not supposed to have. For example, they can:

View sensitive data belonging to others.

Change or delete other people's files.

Perform "Admin" actions without being an admin.

To prevent it, it is recommended to follow these principles:

deny by default

The server must check permissions every single time.

check if a user is logged in; check if they actually own the specific data they are trying to access.

Disable directory listing

Monitor the logs and setup alerts
