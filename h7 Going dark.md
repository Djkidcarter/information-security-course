# Going dark

## x) Summaries

- https://www.eff.org/deeplinks/2014/07/7-things-you-should-know-about-tor

This article lists 7 things you should know about the TOR browser. The first point explains that TOR is still effective. The author affirms that the browser has " probably not been broken at a cryptographic level". In some specific situations, the NSA have managed to compromised individual users, mainly due to user misconfiguration. They also exploited some vulnerabilities in Firefox, but this was patched quickly. TOR also explained that if someone wanted to track you, they could monitor both sides of the connection. " Its design does assume that at least one side of the connection isn't being monitored by whomever you're trying to stay private from."

Secondly, it seems to have a general misconception that TOR is "only used by criminals and pedophiles". It is obviously not true. Activists and journalists, for example, use the service to preserve their anonimity. It is also explained that some families use it to protect their children and preserve their privacy. The military also use TOR for communicating and planning.

Thirdly, there is an other belief that TOR was created by the military so it must have a backdoor they can use. Even though, the browser was funded by the US navy, it has been proved by security experts that there are no backdoors in place and since the project is open source, anyone can look at the code and confirm it.

Next, you cannot be prosecuted for running a TOR relay (as long as you do not do anything illegal of course!). The authors of this article are, as a matter of fact, running one so they are credible when making this statement.

Then, there is a belief that the browser is difficult to use. That is simply not the case. You can download a bundle that comes pre configured for safe use. There is also an other way to use, Tails which "is a live operating system that runs on a DVD or thumb drive. Tails routes your entire Internet connection through Tor. And when you shut it down, Tails “forgets” everything that was done while it was running".

At the number 6 spot, people tend to believe that TOR is very slow. It is said here that the developers have worked hard to increase the speed and mentioned that the more relays they have, the faster the network will be.

Lastly, TOR is of course not perfect and can "destroy your own anonymity" if used incorrectly.


- Shavers & Bair 2016: Hiding Behind the Keyboard: The Tor Browser

TOR is free and easy to use browser allowing a person to hide their IP address in order  to stay anonymous when surfing the web or sending emails. Initially developed by the US government, TOR is a browser that allow to keep private conversations private. As many things, it can be used properly or to do something illegal. It is also important to note that, the open source service does not belong to anyone and "For that reason alone, Tor receives worldwide input from privacy motivated experts to ensure it remains relevant and effective".

So, how does it work concretely? It directs the route of a user's traffic through random relays, hence the name of the onion router. Like an onion, it is made up of different layers. With every relay, "a layer of encryption is peeled off as it goes through the Tor nodes to its final destination."

<img width="671" height="409" alt="image" src="https://github.com/user-attachments/assets/d3f840ee-edfb-4f83-92aa-5861783e4e2a" />

The relays are ran by volunteers and anyone can do it by configuring a server to become one. It is said in this book that "there are over 750,000 users of Tor using over 6000 relays worldwide".

TOR is a portable application and do not require an installation, an extraction of the file is simply needed to run.

TOR hides the user's true IP address by replacing it with the IP address of the exit node. This is obviously good to protect anonimity but can also be used by criminals to commit illegal actions.

It is extremely difficult to track users of TOR, and the FBI has succeeded once in a dismantlement of a child pornography server. But this was due to a vulnerability that got patched quickly. The major weakness of the service remains the user as they can misconfigure the browser, like allowing geolocation request or install plugins that can bypass the TOR proxy to reveal the true IP address.

## a) Install TOR browser and access TOR network (.onion addresses)

Being a complete beginner, I was a bit unsure how to complete this part of the homework safely so I have done some research first. It was recommended to take a snapshot of the virtual machine should anything happened, I could always revert to this version. I have named the snapshot pre-darknet homework as shown in the following picture.

<img width="1919" height="297" alt="image" src="https://github.com/user-attachments/assets/dcedcd28-1309-4b6c-8391-d38d57f2d633" />

Then, I switched on my virtual machine and accessed the terminal. As usual, the first thing to do is to update Debian to make sure I have the latest security patches.

<img width="804" height="231" alt="image" src="https://github.com/user-attachments/assets/892da344-22bc-4f06-a6e2-294ed8809f42" />

Then I opened my browser and typed the following address https://www.torproject.org/download/

<img width="829" height="240" alt="image" src="https://github.com/user-attachments/assets/631fdd02-cbaf-4d65-91d9-f17604725842" />

<img width="931" height="880" alt="image" src="https://github.com/user-attachments/assets/9dc267dc-67c9-4dbc-94b4-c9a29adc4f98" />

I hit the download for Linux button.

<img width="491" height="134" alt="image" src="https://github.com/user-attachments/assets/2ec75fd2-d128-43fd-86ee-e6ae5ed61d5b" />

When the dowload finished, i right clicked on the .tar.xz file and selected "extract here".

<img width="764" height="519" alt="image" src="https://github.com/user-attachments/assets/2067184f-a827-4ce5-aed7-c4d3bd4fc432" />

Next, I selected start-tor-browser.desktop and clicked on extract.

<img width="601" height="304" alt="image" src="https://github.com/user-attachments/assets/de005520-775e-4609-ba9a-a364d06ad889" />

<img width="269" height="241" alt="image" src="https://github.com/user-attachments/assets/bf5a5c81-7f95-446a-ae2f-853a59f3ee71" />

Then, I was able to start the launcher.

<img width="862" height="610" alt="image" src="https://github.com/user-attachments/assets/770afcc8-161f-406f-90e3-738f7f39c878" />

I hit the connect button.

<img width="763" height="282" alt="image" src="https://github.com/user-attachments/assets/0783bfe8-fb45-451f-ba2e-f1da84ebafca" />

<img width="793" height="588" alt="image" src="https://github.com/user-attachments/assets/192a9f6f-97d6-4883-9c16-45c8e621bd13" />

First thing, I changed the security settings to the safest option as show in the following picture and restarted the browser.

<img width="794" height="782" alt="image" src="https://github.com/user-attachments/assets/657205c6-cdad-4dc5-b9cc-b16acf602d00" />

## b) Browse TOR network, find, take screenshots and comment

- search engine for onion sites

For the search engine, TOR is recommending "Ahmia" as abuse material is not allowed.

<img width="769" height="586" alt="image" src="https://github.com/user-attachments/assets/ce6759f0-370e-40a2-94cd-dd1840caeb0f" />

<img width="804" height="712" alt="image" src="https://github.com/user-attachments/assets/0729f134-65b4-49cb-a7c4-0f2c8c5f1363" />

The service seems to work like a traditional search engine except that is giving only .onion sites.

<img width="794" height="717" alt="image" src="https://github.com/user-attachments/assets/2001fe9e-56a1-400b-b587-e95d4b88117a" />

I clicked on the first link and it seems that I have accessed a black marketplace.

<img width="796" height="789" alt="image" src="https://github.com/user-attachments/assets/86a3c821-16a7-4d33-916d-58eefd1b1dd9" />

It is actually insane that you can buy credit cards details, ATM skimmers or counterfeit money from this site.

<img width="787" height="623" alt="image" src="https://github.com/user-attachments/assets/5644afda-28d3-4526-929b-adaa3d3b239b" />

Next, I decided to visit the Abacus marketplace as it was recommended by Gemini.

<img width="681" height="314" alt="image" src="https://github.com/user-attachments/assets/98e2f637-7a6d-4688-b947-87ea6067d957" />

<img width="439" height="202" alt="image" src="https://github.com/user-attachments/assets/3ad7f05a-06e4-4c85-b071-7071288cfdc3" />

It looks like this onion site is inactive as I got stuck there for minutes until I decided to move on.

<img width="760" height="532" alt="image" src="https://github.com/user-attachments/assets/7086a30a-bb8d-4cc3-986a-0b0d8605a771" />

For the forum, I chose "Dread" as it is apparently the Reddit of the dark web.

<img width="791" height="717" alt="image" src="https://github.com/user-attachments/assets/8079e91a-0ed2-43dc-a136-6b96321686ee" />

Being a reddit user, it is true that the interface shares some similarities.

<img width="798" height="775" alt="image" src="https://github.com/user-attachments/assets/128b5a66-5edc-4438-908f-fad217eb1def" />

<img width="795" height="734" alt="image" src="https://github.com/user-attachments/assets/6eb818f7-c53c-45c6-95ca-04eea2d20f92" />

For the last part of the assignment, let's now visit a well known organization. We have been told by Tero that the CIA has a site on the dark net. Let's see if we can find it.

<img width="789" height="713" alt="image" src="https://github.com/user-attachments/assets/7d9d23ee-3f97-462b-b653-4b5b7fcdc7ca" />

<img width="782" height="414" alt="image" src="https://github.com/user-attachments/assets/a4ff9742-cb34-44e3-8e71-cf27a550efae" />

This looks like the correct site when you can apparently contact the, also report some information or even apply.

<img width="780" height="402" alt="image" src="https://github.com/user-attachments/assets/75c17e8b-fe27-4d0e-b97a-e3971092d411" />

<img width="748" height="567" alt="image" src="https://github.com/user-attachments/assets/101d4695-dbc1-4fa7-a565-9a02f08ef1ca" />
