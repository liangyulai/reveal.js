Encryption & Cryptography

+++
# 密码学 Cryptography/Cryptology 

![Lorenz-SZ42](https://upload.wikimedia.org/wikipedia/commons/4/4d/Lorenz-SZ42-2.jpg)
> Cryptography or cryptology is the practice and study of techniques for secure communication in the presence of third parties called adversaries.

---

Britannica

> **密码学 Cryptology** (from the Greek kryptós, "hidden," and lógos, "word") is the science of secure (or, generally speaking, secret) communication. This security requires that legitimate users, a transmitter and a receiver, are able to transform information into a cipher by virtue of a key –that is, a piece of information known only to them. Although the cipher is inscrutable and often unforgeable to anyone without this secret key, the authorized receiver can either decrypt the cipher to recover the hidden information or verify that it was sent in all likelihood by someone possessing the key.


---

Britannica

> **密码编码学 Cryptography** was concerned initially with providing secrecy for written messages. Its principles apply equally well, however, to securing data flow between computers or to encrypting television signals. Today, the modern (mathematical) science of cryptology is not just a set of encryption mechanisms. It has since been applied to a broad range of aspects of modern life, including data and message integrity, electronic signatures, random numbers, secure key exchange, secure containers, electronic voting, and electronic money.

---

## Encryption terminology
* cipher: A synonym for the algorithm used in transforming plain text to ciphertext
* 明文 plaintext: message to be sent, in readable form
* 密文 ciphertext: message in coded form, unreadable without special information such as a key
* 加密 encrypt(encipher): turn plaintext into ciphertext
* 解密 decrypt(decipher): turn ciphertext back into plaintext
* 密码分析 cryptanalysis: cracking a code - attempting to decrypt without the required special information

---
## reference
* [Wikipedia: Cryptography](https://en.wikipedia.org/wiki/Cryptography)


---
## Cryptography Benefits

* 信息的机密性 Confidentiality
    Information can be made effectively unavailable or unreadable for unauthorized individuals, entities, and processes.
* 信息的认证性 Authentication
    The receiver of a message can verify the identity of the sender.
* 信息的完整性 Integrity
    Integrity ensures that data has not been altered or destroyed in an unauthorized manner.
* 信息的不可抵赖性（数字签名） Non-Repudiation
    The receiver can prove that the message he or she received is precisely what the sender sent; the sender will have no means to deny any part of his or her participation.

---
## 

* ATM Cards
* Computer paswords
* Electronic commerce

+++
## Symmetric Key Cryptography & Asymmetric Key Cryptography

* 对称密码 Symmetric Key Cryptography: 
    * 传统密码 Conventional cryptogrphy
    * 私钥密码 Secret-key cryptography
    * 公共密钥密码 Common-key cryptography
    * 共享密钥密码 Shared-key cryptography
    * 块密码 Block Cipher/流密码 Stream Cipher
    * DES(Data Enryption Standard), AES(Advanced Encryption Standard), RC4(Rivest Cipher), Blowfish
* 公钥密码 Asymmetric Key Cryptography(Public Key Cryptography)
    * Public Key for encrypt data, and Private Key is for decrypt the data
    * RSA(Rivest-Shamir-Adleman), DSA(Digital Signature Algorithm), Diffie-Helman

---
## 对称密码 Symmetric-key cryptography
* Stream ciphers
    * OTP
    * RC4
    * CSS
* Block ciphers
    * DES
    * 3DES
    * AES
    * Blowfish
    * Twofish

---
## 对称密码 Symmetric-key cryptography(1)
 
![Skytale](https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Skytale.png/800px-Skytale.png)

```
       | I | a | m | h | u |  |
     __| r | t | v | e | r |__| 
    |  | y | b | a | d | l |
    |  | y | H | E | L | P |
```
>   "I am hurt very badly HELP" ---> "IryyatbHmvaEhedLurlP"

[Cryptool online: Scytale](https://www.cryptool.org/en/cto-ciphers/scytale)

---
![ROT13](https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/ROT13_table_with_example.svg/1000px-ROT13_table_with_example.svg.png)
> ROT13 replaces each letter by its partner 13 characters further along the alphabet. For example, HELLO becomes URYYB (or, conversely, URYYB becomes HELLO again).

---
![Enigma machine](https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Enigma_%28crittografia%29_-_Museo_scienza_e_tecnologia_Milano.jpg/704px-Enigma_%28crittografia%29_-_Museo_scienza_e_tecnologia_Milano.jpg)
> Enigma was invented by the German engineer Arthur Scherbius at the end of World War I.
> Alan Turing (1912-1954) was a remarkable British cryptologist and mathematician of that time.


---
## Enigma machine

![](http://www.crypto-it.net/Images/simple_ciphers/rotor_machines/enigma_eng.png)

[Cryptool: Enigma](https://www.cryptool.org/en/cto-ciphers/enigma)

---
## 对称密码 Symmetric-key cryptography(2)
![Sigaba](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/SIGABA-patent.png/800px-SIGABA-patent.png)

>  ECM Mark II was a cipher machine used by the United States for message encryption from World War II until the 1950s. The machine was also known as the SIGABA or Converter M-134 by the Army, or CSP-888/889 by the Navy, and a modified Navy version was termed the CSP-2900. 

---
## 对称密码 Symmetric-key cryptography(3)

![Symmetric-key cryptography](https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/Symmetric_key_encryption.svg/1048px-Symmetric_key_encryption.svg.png)

---
![](https://dzone.com/storage/temp/7395837-symmetricencryption.png)

---
## 公钥密码 Public-key cryptography(1)

![Public-key cryptography](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/Public_key_encryption.svg/786px-Public_key_encryption.svg.png)

1. Bob encrypted a message with Alice's public key
2. Alice decrpyted Bob's message with her private key

---
## 公钥密码 Public-key cryptography(2)

![Public-key cryptography](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/Private_key_signing.png/250px-Private_key_signing.png)

![Public key](https://dzone.com/storage/temp/7395826-publickeyencryption.png)

1. Alice signs a message(not encrypted) with her private key. 
2. Bob can verify that Alice sent the message and that the message has not been modified.

---

> RSA was designed by Ron Rivest, Adi Shamir and Leonard Adleman in 1977. 
![RSA scheme](http://www.crypto-it.net/Images/rsa/rsa_scheme.png)

---
[Cryptool online: RSA](https://www.cryptool.org/en/cto-highlights/rsa-step-by-step)

+++
## 消息摘要和数字签名(Digital Signature)

---
## Simple diagram of the process of digital Signing and verification

![](https://cdn-images-1.medium.com/max/1400/1*UCn_xX0AOLxMKTb0xOeWfg.png)

---
![What is digital signature quora](https://dzone.com/storage/temp/7395825-digitalsignature.png)

---
![](https://www.camcert.gov.kh/wp-content/uploads/2017/12/digital-signatures-methodology.jpg)


+++
# 散列函数 Hash functions

* 高速的完整性鉴别
* 防止发送信息的一方否认曾经发送信息
* MD5, SHA

---
### MD5 

* 128bit

---
### SHA1/SHA2

* SHA-1(160bit), SHA-2(256/384/512bit)

---
### Message Authentication Code (MAC)

---

### Hash-Based Message Authentication Code (HMAC)



+++
# to be continue...

* SSL/TLS/OpenSSL
* HTTPS/SSH/SFTP
* PGP/OpenPGP/GnuPG(GPG)
* IKEv1/IKEv2
* IPsec
* X.509

+++

## reference 

[Portal: Cryptography](https://en.wikipedia.org/wiki/Portal:Cryptography)
[Outline of Cryptography](https://en.wikipedia.org/wiki/Outline_of_cryptography)
[Wikipedia: Encryption](https://en.wikipedia.org/wiki/Encryption)
[Cryptool](https://www.cryptool.org/images/ct1/presentations/CrypTool1-Presentation-en.pdf)
[Cryptography Visualization Software Downloads ](http://pages.mtu.edu/~shene/NSF-4/)
[Art of the Problem](https://www.youtube.com/user/ArtOfTheProblem)
[Crypto-IT](http://www.crypto-it.net/eng/index.html)