# h5 - Uryyb, Greb!

## x) Read and summarize

- € Schneier 2015: Applied Cryptography: Chapter 1: Foundations

 The chapter explains some key concepts about messages and encryption. The author defines the terms simply and establish a mathematical relationship.

 cryptography, "The art and science of keeping messages secure" (Schneier, 2015)
 
 plaintext M, the original message in plain text 
 
 encryption E, "The process of disguising a message in such a way as to hide its substance" (Schneier, 2015)
 
 ciphertext C, the encrypted message
 
 decryption D, "The process of turning ciphertext back into plaintext" (Schneier, 2015)

 Mathematically, we can express the following relation:

 E(M)=C  and    D(C)=M   so   D(E(M))=M

 It is important to note that the message can be "a stream of bits, a text file, a bitmap, a stream of digitized voice, a digital video image..." (Schneier, 2015)

 Cryptography is obviously important for confidentiality but also provides some benefits for:

 authentification => you can be certain of the identity of the sender

 integrity => you can be sure that the message was not changed while in transit

 nonrepudiation => "A sender should not be able to falsely deny later that he sent a message." (Schneier, 2015)

"A cryptographic algorithm, also called a cipher, is the mathematical function used for encryption and decryption." (Schneier, 2015)

Schneier gives 2 types of algorithms:

Restricted where the security is based on "keeping the way that algorithm works a secret". 

The second is based on a key "Modern cryptography solves this problem with a key, denoted by K. This key might be any one of a large number of values. 
The range of possible values of the key is called the keyspace. Both the encryption and decryption operations use this key 
(i.e., they are dependent on the key and this fact is denoted by the K subscript), so the functions now become:"

EK(M) = C   and   DK(C) = M   so   DK(EK(M)) = M
   
Some algorithms uses a different key for encryption/decrption. In this case we get the following:

EK1(M) = C   and DK2(C) = M   so   DK2(EK1 (M)) = M

All the security in based in the key, meaning that the algorithm can be "published and analysed".

Algorithms can be of 2 kinds, symmetric or Public-key. In a symmetric encryption, both the sender and rceiver use the same key. 
With the public key, the encryption public key is different than the decryption private key. So you can give your public key to anyone to send you encrypted data that only you can unlock.

"Cryptanalysis is the science of recovering the plaintext of a message without access to the key. Successful cryptanalysis may recover the plaintext or the key." (Schneier, 2015)

An attempted cryptanalysis is called an attack. There are 4 general types of cryptanalytic attacks. 

Ciphertext-only attack

Known-plaintext attack

Chosen-plaintext attack

Adaptive-chosen-plaintext attack


 

 
