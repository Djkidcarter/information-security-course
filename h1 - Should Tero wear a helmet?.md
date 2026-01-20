## Threat modeling

The article is about a group of security experts providing some guidelines and a philosophy for threat modeling. 
Their definition of the term is “analyzing representations of a system to highlight concerns about security and privacy characteristics.”
It asks 4 simple questions:
•	What are we working on?
•	What can go wrong?
•	What are we going to do about it?
•	Did we do a good enough job?
The article carries on with why threat modelling is important and who should do it.
The manifesto follows a similar format to the Agile manifesto.
Next, they explained that they have a set of values and principles. 
For example, they value “people and collaboration over processes” and they follow the principle that the “outcomes of threat modeling are meaningful when they are of value to stakeholders.”
Finally, the article lists some beneficial patterns like having a systematic approach and some anti patterns which would inhibit threat modeling like having a tendency to overfocus.

## Videos 

The playlist of YouTube video is a crash course on threat modeling by Adam Shostack. It explains the goal and insists on the 4 important questions we need to ask ourselves.
What are we working on?
What can go wrong?
What are we gonna do about it?
Did we do a good job?
Adam gives a few tips to get better at threat modeling like sketching or making diagrams as well as having honest discussions to get a common understanding. The author is talking about threat modeling as a journey more than 1 job delivery.
There are some structures in place to help mitigate the risks like STRIDE.
Spoofing
Tampering
Repudiation
Information disclosure
Denial of service
Elevation of privileges
What are we going to do about it? Adam explains that the work needs to be tracked and that “the solutions need to be variable, one constant”. There are many ways to respond to a threat, but you need a clear plan. 
In his last episode, Adam explains that to answer the question, did we do a good job? You need to ask the question, would you recommend threat modeling to a colleague? If not, you probably did not do a good job. 

## Threat Modeling Cheat sheet

The article is a cheat sheet about the OWASP threat modeling. The 4 questions remain the same.
What are we working on?
It is important to understand what we are building and see where it might be vulnerable. Data flow diagram can help to map the system.
What can go wrong?
We need to identify the ways an attacker could make some damage. STRIDE (Spoofing, Tampering, Repudiation, Information disclosure, Denial of service, Elevation of privileges) can help with that by imposing some structure
What are we gonna do about it?
Decide on the response by mitigating, eliminating, transferring or accepting the threat.
Did we do a good job?
Review your work and make sure the issue is fixed
Ideally, threat modeling needs to be started during the design phase and is an ongoing process.
On the cloud, the author explains that there is a shared responsibility. It is therefore important to know what the provider handle and what are your responsibilities.


## EP 135: The D.R. Incident, Darknet Diaries Podcast

The episode tells the story of Omar Avilez who helped the Dominican Republic in 2022 fight against cyber attacks. 
After seeing Costa Rica get hacked, Omar started checking his own government’s computers for dangers. During his investigation, he found a spying tool that had been hidden for nearly a year.
His team ended up fighting three different groups at once, some criminals after money, Hacktivists and foreign spies.
They stopped a major ransomware attack from locking their systems and manage to clear the spies out of their network.
The main takeaways from this episode are that cybersecurity is not about having a perfect and permanent protection but making it the most painful for the attackers. 
The chances are if it is too “annoying” the attackers won’t bother. Sometimes, you might find a spying tool by accident when working on something not related.
These tools can remain undetected for months. Also, the role of collaboration between country was important in this story. 
The Dominican Republic was better prepared thanks to Costa Rica which got hacked previously.

## Security hygiene

# For the average Joe:

Be careful with phishing emails
Be careful when downloading software malware, trojan
Have a strong password and change it regularly
Do not use the same password for all sites

# For the companies

Be careful with phishing emails
Have a strong password and change it regularly
Have done a threat modeling of their systems
Document issues and fixes
Have a disaster recovery plan in place
Train their employees on safe practices

## Make belief boogie man

Our company ITloop buys used smartphones, fix them and resell them via an app.
  
# What are we working on ?
  
Our key assets are:
Customer data
Database of the phones
We need to ensure that we do not sell stolen phones and get our data hacked to keep getting paid. Our customer interacts with us through the app.
  
# What can go wrong?
  
With STRIDE, for example:
Hackers can access our system and change prices  tampering (medium risk)
Hacker could steal our customer data  information disclosure (high risk)
Customer says he has not received a phone  repudiation (low risk)
Our main threats are hackers who could access our system. We need to keep our infrastructure intact if we want to ensure business continuity.

# What are we going to do about it?

We have to make sure that our code has no vulnerabilities so no hackers can enter our system.
We need to buy a shipping insurance if a phone gets lost.

# Did we do a good enough job?

Daily security audits are in place and the team is continuing to update our threat modeling strategy.


## Sources

https://www.threatmodelingmanifesto.org/
https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf
https://darknetdiaries.com/episode/135/ 



