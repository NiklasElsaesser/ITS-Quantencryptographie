# ITS-Quantencryptographie

This Repository consits of only the Paper i´ve written as my Exam Projekt.

# Quanten Cryptographie
## Table of Contents
- [ITS-Quantencryptographie](#its-quantencryptographie)
- [Quanten Cryptographie](#quanten-cryptographie)
  - [Table of Contents](#table-of-contents)
  - [Introduction ](#introduction-)
  - [Methods ](#methods-)
    - [Symmetrical-Encryption ](#symmetrical-encryption-)
    - [Asymetrical Encryption ](#asymetrical-encryption-)
  - [Quanten Methods ](#quanten-methods-)
    - [Quantum-Parallelism ](#quantum-parallelism-)
    - [Shors-Algorithm ](#shors-algorithm-)
    - [Qubits ](#qubits-)
  - [Use Cases ](#use-cases-)
    - [Decryption ](#decryption-)
    - [Encryption ](#encryption-)
    - [Encryption Example ](#encryption-example-)
  - [Citations ](#citations-)

## Introduction <a name="introduction"></a>
When it is important to communicate securely over the internet, one has to ensure a encrypted method to transfer Data. This is done by encrypting the Data via various, usually mathematical based techniques. Now with the wider acces to Quanten Computers these conventional techniques can be decrpyted with new algorithms and additionally new quanten algorithms allow unbreakable encrpytion for data transfer.

Traditionell encryption methods as well as some type of quanten encryption methods are based on sharing two keys.

The widely used encryption techniques today are usually based on one hand the symmetrical techniques with, for example the "Advanced Encryption Standart" (AES) or the "Data Encryption Standard" (DES) and on the other hand the assymetrical techniques like the "RSA"-Procedure. Altough there is an ongoing struggle between encrypters and decrypters, the above listed techniques are still usable in real world scenarios. Although the symmetrical techniques have been cracked in theoretical cases. [4]

Now with the wider access to Quanten Computers a third technique enters the cryptographie landscape, Quanten cryptographie. This new technique differentiates between Quanten cryptographie and Post-Quanten cryptographie.

The term Quanten-Computer was first coined in 1985 by a british Physic David Deutsch. His assumptions regarding the operating principle are still valid today and are widely implemented. His **thoughts** were that a quanten computer had to work with so called "Qubits", like regular electronical computers these "Qubits" behave like a bits. Meaning beeing in astate of 1 and 0. But "Qubits" have the property of beeing in a superposition meaning a 1 and a 0 at the same time, opposing to regular computers, who can be either 1 or 0. The result of this is that  [4]

## Methods <a name="Methods"></a>

### Symmetrical-Encryption <a name="subparagraph2.1"></a>
The Vernam-Code is technically an absolut secure encryption algorithm, but in reality the randomly generated key is usually not completely random, which means a powerful computer can identify the rules after which the key is generated and reproduce set key. [1]

Furthermore the way to communicate the key between sender and receiver is usually not completely secure as well. Today any key can be intercepted with every conventional way of communication, i.e. wire-based and wireless. As a result the authenticity of a message is not garanteed, since the receiver can send messages to himself and make it look like they originated somewhere else.[1]

The Vernam

### Asymetrical Encryption <a name="subparagraph2.2"></a>
*explanation of asymmetrical oldschool codes*\
The most widely used and accepted types of encryption avoid the drawbacks of a secure key transmission and the authenticity by dedicating two different key to sender and receiver. The used technique is called *public key cryptographie* because the used encryption is publicly known. This technique is secure because it is impossible for todays most advacend computers to decrypt the keys. To decrypt the encrypted key, one just has to derive the decrpyted key from the encrypted one.[1]

Assymetrical encrypted procedures are based on the so called "trapdoor-function". It is easy to "enter" set function, but difficult to impossible to exit, meaning it is easy to multiply two prime numbers *p* and *q* to receive *n* (key) *n = p * q*. 
But it is difficult to calculate the arguments which led to the result, altough we know that a prime number is a produkt of a natural number we cant calculate *p* and *q* from *n*.[1]

In the field of algorithmical komplexitytheoriy to calculate *p* and *q* from *n* is a "NP-Problem with an exponential time of calculation". There hasent been any successfull approach to reduce the complexity.[1]

To enrypt a number it is only necessary to know product *n*, which means the sender makes *n* public and keeps the factors *p* and *q* hidden. Decrypting is only possible if one knows the prime numbers *p* and *q*.[1]

## Quanten Methods <a name="quanten-methods"></a>
### Quantum-Parallelism <a name="subparagraph3.1"></a>
Quantum-parallelism is a method to compute multiple calculations at once by having many conditions at the same time. In a Qubit register of size *m* a superpsoition can save the amount 2^*m* of *m* possible Qubits. A regular computer with a register of size *m* Bits can only save the amount of 2*m*.\
With quantum-parallelism, Shor´s Algorithm is able to calculate the prime factors. The calculation of a factorial number with a wordsize larger than 1024 Bit is nearly impossible for a regular computer.[1]

### Shors-Algorithm <a name="subparagraph3.2"></a>
Shor´s Algorithm on a quantum computer is able to decrypt every RSA encrypted message. It assumes that a number *n* can be factorized, if the modulfunction *f(x)= a^x mod n* for a number *a* < *n* can be calculated.[1]

[1]
Nach Definition bildet die Modulfunktion f die Menge der ganzen Zahlen Z auf die beschränkte Zahlenmenge Zn = {0, 1, ..., n − 1} ab. Für den Input 0, 1, ..., N − 1 des Quantenalgorithmus wird N in der Größenordnung n2 gewählt. Man geht also von einer Funktion f aus, mit der die Menge {0,1,...,N − 1} auf die Menge {0,1,...,n − 1} mit Periode p abgebildet wird, d. h. es gilt f(x + p) = f(x) für alle x aus {0, 1, ..., N − 1}. Der entsprechende unitäre Operator Uf von f bildet zwei Quan- tenregister |a⟩|b⟩ auf |a⟩|b ⨁ f(x)⟩ ab. Um die gewünschte Beschleunigung der Su- che nach Perioden der Modulfunktion zu erreichen, wird darauf die Quanten- Fourier-Transformation angesetzt.

```diff
- Seite 102, Picture of Gates from IBMQ[1]
```
[1]
Shors Algorithmus beruht also auf der Anwendung des Hadamard-Gatters, der unitären Transformation der Modulfunktion f(x) = ax mod n zur Faktorisie- rung von n und der Quanten-Fourier-Transformation. Insgesamt werden dazu Gatter in der Größenordnung von O((logn)3) benötigt. Die Rechenzeit des Quan- tenalgorithmus liegt in der Größenordnung von O(log log n · (logn)3) [21] Der klassische Teil von Shors Algorithmus (vgl. Abb. 6.3) verwendet nur Multiplika- tionen in der Größenordnung O(logn). Die Rechenzeit von Shors Algorithmus insgesamt zur Bestimmung eines echten Teilers der ganzen Zahl n beläuft sich daher auf die Größenordnung O(log log n · (logn)3) = O((logn)4). Der entschei- dende Schritt zur Beschleunigung der Periodenbestimmung ist die Fourier-Trans- formation, die in einen Quantenalgorithmus übersetzt wurde. Das ist zugleich der theoretische Durchbruch, das klassisch bisher nicht-polynomial lösbare Pro- bleme polynomial lösbar werden. Die Frage ist, ob Quantencomputer auch an- dere Probleme polynomial lösen können, die nicht von Quanten-Fourier-Trans- formationen abhängen.
### Qubits <a name="subparagraph3.3"></a>
```diff
- Seite 101[1]
```

## Use Cases <a name="use-cases"></a>
### Decryption <a name="subparagraph4.1"></a>
There are ways to decrpyt even the best RSA-Procedures, the algorithm used for this problem was discovered by Peter Shor in 1994. It solves the factorial problem in polynomial time.[1] A problem is in polynomial time solvable if a deterministic calculator can solve it in a time which does not grow stronger as a polynomial function.[5]

Shors algorithm uses the "Qauntenparallelismus" and can therefore decrypt factorial numbers from up to 1024 Bit´s. Which means as soon as a quanten computer with a big enough computing power exists, Shor´s alogrithm will be able to decrpyt any fomr of RSA and the data currently encrypted this way will be at risk.[1]

### Encryption <a name="subparagraph4.2"></a>
As previously described with conventional encryption, it is neccesary that the secret key won´t be stolen, for example by symmetric-key cryptographie during the transmission. If a quantum communication channel is used the participants Bob and Alice will know if a third party (Eve) intercepted the message (Bob, Alice and Eve are just placeholder protagonists).[6] Quantum communication networks are in development at multiple universities and companies, but none has left the development stage yet.[7]

The in the Example used protocoll uses the fact that the measurement of a qubit can change its state. If Alice sends Bob a message and Eve is listening and therefore measures the qubit before Bob does, the chance of a change in the state of the qubits increases. Therefore Bob will not receive the message i.e. the qubit Alice sent.[6]

For example, if Alice sends a qubit 0 in the X-basis and Bob measueres it in the X-basis, Bob measures 0. If Eve tries to measure the qubit now before Bob in the Z-basis before it reaches Bob, she will change the qubits state to either 0 or 1 and Bob will receive the initial 0 with a chance of only 5 %. Now Alice and Bob know Eve is evesdropping.[6]

To make tapping as hard as possible, the quantum key distribution protocol requires the following process enough times so an evesdropper can´t get away unnoticed. Which requires the following stepts:[6]
1. Alice generates a string of random bits, e.g.: 1000101011010100
2. Alice chooses a random basis for each bit: ZZXZXXXZXZXXXXXX
3. She keeps the two Values private.
4. Alice encodes each bit onto a string of qubits using the basis she chose, so each qubit is in one of the states |0⟩,|1⟩,|+⟩ or |-⟩, with the states chosen at random. The original qubit string looks like this:|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩,|0⟩ which is the message she sends to Bob.
5. Bob measures each qubit at a random basis, for example at: XZZZXZXZXZXZZZXZ He keeps the result of the measurement private.
6. Alice and Bob share the basis which they used for each qubit private. If Bob measured a qubit in the same basis as Alice prepared it in, the qubit becomes part of their shared secret key, if the qubit does not match its discarded.
7. Alice and Bob share a random sample of their keys and if the sample matches, they know (to a small error margin) that their transmission is succesfull.

### Encryption Example <a name="subparagraph4.3"></a>

The whole example is available as a jupyter notebook in binder here:[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/NiklasElsaesser/Quantum-Biscuit/HEAD?labpath=Quantum-Biscuit-Optimization.ipynb)

## Citations <a name="citations"></a>
[1] Mainzer, Klaus. "Quantencomputer: von der Quantenwelt zur Künstlichen Intelligenz", 2020. [Book]\
[2] Hughes, Ciaran; Isaacson, Joshua; Perry, Anastasia; Sun, Ranbel F.; Turner, Jessica. "Quantum Computing for the Quantum Curious", 2021. [Book]\
[3] Homeister, Matthias. "Quantum Computing verstehen: Grundlagen - Anwendungen - Perspektiven", 2022. [Book]\
[4] Schmeh, Klaus. "Codeknacker gegen Codemacher: die faszinierende Geschichte der Verschlüsselung", 2022. [Book]\
[5]Dwedney, A.K. "Der Turing Omnibuds", 1995.[Book]\
[6]The Jupyter Book Community,[Quantum Key Distribution](https://qiskit.org/textbook/ch-algorithms/quantum-key-distribution.html#1.-Introduction),2021.[Online]\
[7]van Loock, Peter.[Quantum communication research network launched](https://www.uni-mainz.de/presse/aktuell/14737_ENG_HTML.php),2021[Online]

