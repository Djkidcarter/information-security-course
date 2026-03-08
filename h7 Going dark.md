# Going dark

## Summaries

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
