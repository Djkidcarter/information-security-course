# h4 Johnny Tables ###

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

To prevent it, it is recommended to follow these principles:

-  environments should all be configured identically, with different credentials used in each environment. This process should be automated to minimize the effort required to set up a new secure environment.

-  A minimal platform without any unnecessary features

-  change the default passwords and disable default accounts.

-  Ensure the website only shows generic error messages to users. Keep the detailed technical logs hidden on the server for developers only.

#  Vulnerable and Outdated Components

Apps are made from a patchwork of pre-made libraries and if any of these have a known bug, the whole app is infected and attackers can figure out how to exploit it.

To prevent it, it is recommended to follow these principles:

- monitor your libraries and delete what you don't use.

- get components from official sources over secure links.

- using tools like versions, OWASP Dependency Check, retire.js. Automate the process with SCA software composition analysis.

# Injection

It happens when an attacker inject some command to be executed by the database. The database is tricked and the attacker can access the data.
Some of the more common injections are SQL, NoSQL, OS command, Object Relational Mapping (ORM), LDAP, and Expression Language (EL) or Object Graph Navigation Library (OGNL) injection.

To prevent it, it is recommended to follow these principles:

- Use Parameterized Queries. Instead of building a command string manually, use templates where the data is plugged in safely. This tells the database to treat this input strictly as a name, never as a command.

- Use positive server-side input validation

- use safe APIs

# Exploits of a Mom

This is a humouristic webcomic related to SQL injection. A mother receives a phone call from her son's school asking her to verify his name. "Is your son's name Robert'); DROP TABLE Students;--?"
The mother replied positively. The scholl had lost all the student records for the year. And the mother to advice the school on sanitizing the database inputs.


# a) Webgoat

First, I updated all linux software with the following command.

<img width="793" height="460" alt="image" src="https://github.com/user-attachments/assets/990279a2-ef24-4473-8724-99a8441a307e" />

Then I entered the command $ sudo apt-get install openjdk-21-jre as the debian version I use, 13.3 will only work with the 21-jre instead of the 17-jre

<img width="787" height="242" alt="image" src="https://github.com/user-attachments/assets/5ae9b47a-236f-4693-a315-919510710d0a" />

My java version is 

<img width="816" height="103" alt="image" src="https://github.com/user-attachments/assets/050ee8a6-988f-4930-b0fb-790ebadba7c4" />

Then I installed a firewall and enabled it.

<img width="652" height="115" alt="image" src="https://github.com/user-attachments/assets/243e6aeb-027c-42b6-bd45-446338f2fb30" />

<img width="505" height="57" alt="image" src="https://github.com/user-attachments/assets/da1a5dfa-d24a-4c54-a3b2-86a5d6c64247" />

Next, I had to install wget

<img width="847" height="322" alt="image" src="https://github.com/user-attachments/assets/d60c964d-497a-4c80-b501-7d85b2d8f00e" />

i tried the command $ wget https://github.com/WebGoat/WebGoat/releases/download/v2023.4/webgoat-2023.4.jar
But I got an error 404.

I visited the github repo to get the correct version.

<img width="1111" height="287" alt="image" src="https://github.com/user-attachments/assets/7b41e2ca-f200-49de-b358-43da49c6a22f" />

Then I ran the command 

<img width="1567" height="392" alt="image" src="https://github.com/user-attachments/assets/885cf26d-329b-4a8d-b145-acb1d10a3e2e" />

and managed to get to the webgoat.

<img width="640" height="471" alt="image" src="https://github.com/user-attachments/assets/457b6422-dc7f-4f3b-ace3-16e564b4df02" />

# b) Solving webgoat 2023.4

<img width="1557" height="537" alt="image" src="https://github.com/user-attachments/assets/26d6e19a-f2ac-472c-a334-6d63bcd30e54" />

I opened the dev tools by pressing f12 and followed the instructions.

<img width="692" height="293" alt="image" src="https://github.com/user-attachments/assets/8c565821-b09e-49ba-99bf-5ef8c39f9228" />

I have managed to find the network number.

<img width="610" height="313" alt="image" src="https://github.com/user-attachments/assets/9303826e-4ce2-4b1b-90e1-c74351e225d7" />

# c) Update all OS and application on Linux

Everything was already up to date.

<img width="678" height="223" alt="image" src="https://github.com/user-attachments/assets/1e020994-687e-49af-a417-15fadf0d699d" />

# d) SQLZoo

- 0 SELECT basics

<img width="802" height="436" alt="image" src="https://github.com/user-attachments/assets/c3274318-7a85-41b2-b006-3de77e60c817" />

<img width="838" height="523" alt="image" src="https://github.com/user-attachments/assets/2c6065ad-ac46-49f8-8c4b-a1f15f7402c0" />

<img width="840" height="488" alt="image" src="https://github.com/user-attachments/assets/2295c19c-0bf6-4e9f-ad68-d20263991499" />

- 2 SELECT from World: First two subtasks:

<img width="1204" height="519" alt="image" src="https://github.com/user-attachments/assets/7fc5e624-0cd0-4563-adac-344fdc876e46" />

<img width="826" height="449" alt="image" src="https://github.com/user-attachments/assets/9e3fb012-e50f-419b-af33-9979cf3229cc" />

# e) Portswigger Labs

<img width="833" height="354" alt="image" src="https://github.com/user-attachments/assets/8852d9bb-f0bd-4012-8d60-7b310bae79b2" />

Since the SQL statement is SELECT * FROM products WHERE category = 'Gifts' AND released = 1
and that we want to see unreleased items, we need to find a way to get rid of "AND released = 1" by injecting something before
OR 1=1--

<img width="1112" height="223" alt="image" src="https://github.com/user-attachments/assets/44a4fc6f-308f-428f-a99b-ca759e3beaed" />
