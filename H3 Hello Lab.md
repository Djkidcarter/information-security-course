* **Summary** Karvinen 2021: Install Debian on Virtualbox - Updated 2024

  The article is a step by step guide on how to install Debian Linux on a virtual machine using VirtualBox.
  First you need to dowload the Debian ISO file and install VirtualBox. Then you need to create a virtual machine, install the system and reboot.
  Finally, after logging in there are some commands to enter in the terminal to check for the latest software update and increase the resolution.

* **Summary** Karvinen 2020: Command Line Basics Revisited

  The article is a compilation of useful commands to know when using a Linux CLI.
  It explains how to move and look around.

  *pwd* *ls* *cd* *..* *less*

  It shows how to manipulate files.

  *nano* *mkdir* *mv* *cp* *rm*

  Then the article explains that everything in Linux is organised under the root directory and lists some important directories.

  */home/* */etc/* */var/log/*

  It gives some administrative commands *sudo apt-get update* to install software update.

  Lastly, the author shows a way to access SSH remotely. *ssh tero@example.com*

* **Can't fish**

  When pinging 1.1.1.1 on the Linux terminal, I received replies only when I was connected to the internet.
  The replies of the ping stop instantly when switching off my Wi-Fi showing that packets don't go through when the networking is disabled.
  
  <img width="825" height="522" alt="image" src="https://github.com/user-attachments/assets/910a992b-f777-4289-9787-6c0bce747d60" />

*  **Local only**
  
In the terminal of the virtual machine, I first ran the command *sudo apt- install nmap* to install nmap.
Then I disable the network and enterred the command *sudo nmap -A localhost* and got the following:
  
<img width="1478" height="420" alt="image" src="https://github.com/user-attachments/assets/faa4e7cf-b395-42c3-af5e-66a26c81498a" />

To analyze the latest command:

sudo runs the command with admin permissions. nmap is the software used for mapping the network. -A enables the aggressive detection and localhost is the target.

* **Daemon scan**

  First, I entered the command *nmap localhost*. I can see that there is only port 631 opened.

  Then I send the command *sudo apt-get install apache2* to install Apache 2 and ran again a port scan and got the following.

 <img width="723" height="332" alt="image" src="https://github.com/user-attachments/assets/986f8db9-d6d8-4e71-8f27-39fb89b8c9a9" />

 It shows this time 2 ports open, 631 and 80.

 * **Over the wire**

   *level 0*
   
    <img width="578" height="39" alt="image" src="https://github.com/user-attachments/assets/07ff11e7-8b36-4c15-8d76-e11de84b31ce" />
    
    password is bandit0

   *level 1*
   
   <img width="995" height="199" alt="image" src="https://github.com/user-attachments/assets/0a3785db-e8eb-4885-9037-51e712457cfe" />

*level 2*

    <img width="327" height="69" alt="image" src="https://github.com/user-attachments/assets/c600a0b8-0387-4436-a0b7-f91801b95cc3" />

*level 3*

<img width="504" height="63" alt="image" src="https://github.com/user-attachments/assets/8298568c-0130-4ddb-bfbc-8ce7b9eff506" />

*level 4*

<img width="447" height="115" alt="image" src="https://github.com/user-attachments/assets/25f19a38-a779-40aa-a731-7d21554301df" />


I asked gemini for clues for the level 3 and 4.



