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
