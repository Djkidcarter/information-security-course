# h6 February2026!

## x) Summaries

- Schneier 2015: Applied Cryptography: 2.3 One-Way Functions

One way functions are an important part of public key cryptography. They are easy to compute but very difficult to reverse.
The author gives the analogy of the plate as a good example of a one way function. It is easy to break a plate into lots of small pieces
but it is very hard to put those pieces back together to reconstruct the plate.

Mathematicians did not proved that one way functions exist. We just use functions that are so difficult to crack that they might as well be one way.
One way functions cannot be used for encryption as is. No one could decrypt it. We need something else, a trapdoor one way function.
It contains the secret instruction on how to reverse the process. The author gives this time a watch analogy. It is easy to take all the components of a watch apart.
It is incredibly difficult to put back together but if you have access to the instruction, the task becomes a lot easier.

- Schneier 2015: Applied Cryptography: 2.4 One-Way Hash Functions

One way hash functions have many names: compression function, contraction function, message digest, fingerprint, cryptographic checksum, message integrity check (MIC), and manipulation detection code (MDC).
A one way hash function turns a variable-length input string (called a pre-image) and converts it to a fixed-length (generally smaller) output string (called a hash value). Also, it is important to note that even a small change in the imput will give a completely different hash.

A good hash function is collision free, meaning that it is nearly impossible to find 2 different files that gives the exact same hash. The process for the hash function is public knowledge as everyone knows how the math works, so the security comes from the math being impossible to reverse.
Hash functions can be great to maintain integrity as the hashes can be compared to ensure that files have not been tampered with.
A message authentication code (MAC) is a hash function that needs a secret key. A person with the key can then verify the hash value.

## Install HashCat

First thing first, I started my virtual machine and updated Linux with the following command.

<img width="807" height="246" alt="image" src="https://github.com/user-attachments/assets/7530e601-1215-4d12-9eb8-34b04ac1de3c" />

Next, we need to install HashCat using the command sudo apt-get -y install hashid hashcat wget

<img width="787" height="268" alt="image" src="https://github.com/user-attachments/assets/4eeb0dca-7a37-4d04-86b1-45cc46356bdd" />

Then we need to create a directory to store our solved hashes.

<img width="433" height="59" alt="image" src="https://github.com/user-attachments/assets/4fb86022-8248-4360-a512-faac0c2faf32" />

The next step require us to download a dictionary. Rockyou is  presented as the most popular and it has over 14M words. Let's download it from the GitHub repository with the following command.

<img width="803" height="439" alt="image" src="https://github.com/user-attachments/assets/177f8f2a-c236-4761-9795-d6896a0cde0c" />

Next, we need to extract the file with the following command.

<img width="565" height="70" alt="image" src="https://github.com/user-attachments/assets/b4073614-afbd-443c-a3ff-4282d106f4c3" />

We can then enter the command ls to make sure the file is present in the directory.

<img width="570" height="101" alt="image" src="https://github.com/user-attachments/assets/8348703f-931a-440d-893b-47702313c475" />

Let's check that the file was extracted correctly and see how many words are available.

<img width="483" height="64" alt="image" src="https://github.com/user-attachments/assets/e709359b-7882-4015-872a-677810622bf2" />

We can see that we have 14344391 words.
We can now identifi the hash type with the following command.

<img width="763" height="409" alt="image" src="https://github.com/user-attachments/assets/e09071c2-6eeb-431e-a819-7ac0255a9060" />

It is now time to crack the hash.

<img width="808" height="208" alt="image" src="https://github.com/user-attachments/assets/97d398ea-a200-4392-833a-dd9134d43a73" />

<img width="792" height="458" alt="image" src="https://github.com/user-attachments/assets/2583322e-f16b-4033-9c6d-69abdb42bef8" />

Next, we enter the following command to see the password in plain text.

<img width="405" height="62" alt="image" src="https://github.com/user-attachments/assets/a70dfd64-2088-4f0d-aa7b-4c45b52d19a8" />

The password is "disobey".
