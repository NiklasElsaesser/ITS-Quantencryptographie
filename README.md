# ITS-Quantencryptographie

This Repository consits of only the Paper i´ve written as my Exam Projekt.

# Quanten Cryptographie
## Table of Contents
1. [Introduction](#Introduction)
2. [Methods](#Methods)
3. [Third Example](#third-example)

## Introduction <a name="Introduction"></a>
When it is important to communicate securely over the internet, one has to ensure a encrypted method to transfer Data. This is done by encrypting the Data via various, usually mathematical based techniques. Now with the wider acces to Quanten Computers these conventional techniques can be decrpyted with new algorithms and additionally new quanten algorithms allow unbreakable encrpytion for data transfer.

Traditionell encryption methods as well as some type of quanten encryption methods are based on sharing two keys.

The widely used encryption techniques today are usually based on one hand the symmetrical techniques with, for example the "Advanced Encryption Standart" (AES) or the "Data Encryption Standard" (DES) and on the other hand the assymetrical techniques like the "RSA"-Procedure. Altough there is an ongoing struggle between encrypters and decrypters, the above listed techniques are still usable in real world scenarios. Although the symmetrical techniques have been cracked in theoretical cases. [4]

### Symmetrical-Encryption
The Vernam-Code is technically an absolut secure encryption algorithm, but in reality the randomly generated key is usually not completely random, which means a powerful computer can identify the rules after which the key is generated and reproduce set key. [1]

Furthermore the way to communicate the key between sender and receiver is usually not completely secure as well. Today any key can be intercepted with every conventional way of communication, i.e. wire-based and wireless. As a result the authenticity of a message is not garanteed, since the receiver can send messages to himself and make it look like they originated somewhere else.[1]

*explanation of symmetrical oldschool codes* [1]\
The Vernam

### RSA-Procedure (Assymetrical Encryption)\
*explanation of asymmetrical oldschool codes*\
The most widely used and accepted types of encryption avoid the drawbacks of a secure key transmission and the authenticity by dedicating two different key to sender and receiver. The used technique is called *public key cryptographie* because the used encryption is publicly known. This technique is secure because it is impossible for todays most advacend computers to decrypt the keys. To decrypt the encrypted key, one just has to derive the decrpyted key from the encrypted one.[1]

Assymetrical encrypted procedures are based on the so called "trapdoor-function". It is easy to "enter" set function, but difficult to impossible to exit, meaning it is easy to multiply two prime numbers *p* and *q* to receive *n* (key) *n = p * q*. 
But it is difficult to calculate the arguments which led to the result, altough we know that a prime number is a produkt of a natural number we cant calculate *p* and *q* from *n*.\
**bspl bild einfügen bzw. latex formel o.ä.**[1]

In the field of algorithmical komplexitytheoriy to calculate *p* and *q* from *n* is a "NP-Problem with an exponential time of calculation". There hasent been any successfull approach to reduce the complexity.[1]

To enrypt a number it is only necessary to know product *n*, which means the sender makes *n* public and keeps the factors *p* and *q* hidden. Decrypting is only possible if one knows the prime numbers *p* and *q*.[1]

#### Euclid´s Algorithm


Now with the wider access to Quanten Computers a third technique enters the cryptographie landscape, Quanten cryptographie. This new technique differentiates between Quanten cryptographie and Post-Quanten cryptographie.

The term Quanten-Computer was first coined in 1985 by a british Physic David Deutsch. His assumptions regarding the operating principle are still valid today and are widely implemented. His **thoughts** were that a quanten computer had to work with so called "Qubits", like regular electronical computers these "Qubits" behave like a bits. Meaning beeing in astate of 1 and 0. But "Qubits" have the property of beeing in a superposition meaning a 1 and a 0 at the same time, opposing to regular computers, who can be either 1 or 0. The result of this is that  [4]

## Methods <a name="Methods"></a>


## Use Cases
### Decryption


### Encryption


### Encryption Example


## Citations
[1] Mainzer, Klaus. "Quantencomputer: von der Quantenwelt zur Künstlichen Intelligenz", 2020. [Book]\
[2] Hughes, Ciaran; Isaacson, Joshua; Perry, Anastasia; Sun, Ranbel F.; Turner, Jessica. "Quantum Computing for the Quantum Curious", 2021. [Book]\
[3] Homeister, Matthias. "Quantum Computing verstehen: Grundlagen - Anwendungen - Perspektiven", 2022. [Book]\
[4] Schmeh, Klaus. "Codeknacker gegen Codemacher: die faszinierende Geschichte der Verschlüsselung", 2022. [Book]\

