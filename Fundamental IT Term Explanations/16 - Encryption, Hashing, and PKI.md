# 16. Encryption, Hashing, and PKI

[[00 - Overview|← Overview]]

**Related Security+ material:** [[1.4 - Public Key Infrastructure]] · [[1.4 - Hashing and Digital Signatures]] · [[1.4 - Encryption Technologies]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Plaintext** | Data in readable, original form. | Meet at 0900. | Plaintext exposure reveals information directly. |
| **Ciphertext** | Data transformed into an unreadable form through encryption. | Random-looking characters produced from a message. | Ciphertext should remain unreadable without the correct key. |
| [[1.4 - Encryption Technologies\|Encryption]] | Transforming readable data into ciphertext using an algorithm and key. | BitLocker encrypts a laptop drive. | Encryption protects confidentiality. |
| **Decryption** | Transforming ciphertext back into readable data with the correct key. | A user unlocks an encrypted drive. | Strong access controls must protect decryption keys. |
| **Cryptographic key** | A value used by an encryption or signing algorithm. | An AES key encrypts a file. | Key compromise can defeat otherwise strong encryption. |
| **Symmetric encryption** | Encryption that uses the same secret key to encrypt and decrypt data. | AES encrypts a hard drive. | It works quickly but requires secure key sharing. |
| **Asymmetric encryption** | Encryption that uses a mathematically linked public key and private key. | RSA protects a small secret during a secure connection. | It supports secure key exchange and digital signatures. |
| [[1.4 - Public Key Infrastructure\|Public key]] | The shareable half of an asymmetric key pair. | Anyone can use it to encrypt data for the owner. | Sharing the public key does not reveal the private key. |
| **Private key** | The secret half of an asymmetric key pair. | A web server uses it during TLS authentication. | Private-key theft allows impersonation or decryption. |
| **AES** | A widely used symmetric encryption algorithm. | Encrypting files, drives, and VPN traffic. | Security+ treats AES as a strong modern choice. |
| **RSA** | A common asymmetric algorithm used for encryption and signatures. | A certificate contains an RSA public key. | Weak key sizes or poor implementation reduce security. |
| **ECC** | Asymmetric cryptography that provides strong security with smaller keys. | Mobile devices use elliptic-curve certificates. | Smaller keys improve performance and efficiency. |
| [[1.4 - Key Exchange\|Key exchange]] | A process that allows parties to establish a shared secret securely. | A browser and server create a TLS session key. | Secure key exchange prevents eavesdroppers from learning the key. |
| **Diffie-Hellman** | A method that lets two parties establish a shared secret over an untrusted network. | A VPN creates a shared encryption key. | Ephemeral versions support forward secrecy. |
| **Hash** | A fixed-length fingerprint generated from data. | A file produces a SHA-256 value. | Hashes help detect changes and store passwords safely. |
| [[1.4 - Hashing and Digital Signatures\|Hashing]] | A one-way process that converts data into a fixed-length digest. | Hashing a downloaded installer. | Hashing supports integrity but does not hide data like encryption. |
| **SHA-256** | A widely used cryptographic hash algorithm. | Verifying that a file matches the publisher’s checksum. | It provides stronger integrity protection than outdated hashes. |
| **MD5** | An older hash algorithm with known collision weaknesses. | Legacy file checksums. | It should not protect security-sensitive integrity. |
| **SHA-1** | An older hash algorithm with known collision weaknesses. | Legacy certificates or repositories. | Modern systems should use stronger alternatives. |
| **Salt** | Random data added to a password before hashing it. | Two identical passwords produce different stored hashes. | Salts defeat precomputed rainbow-table attacks. |
| **Key stretching** | Repeatedly processing a password to make each guessing attempt slower. | PBKDF2 performs many hash rounds. | It increases the cost of offline password cracking. |
| [[1.4 - Hashing and Digital Signatures\|Digital signature]] | A value created with a private key that proves origin and detects changes. | A software vendor signs an installer. | Signatures provide integrity, authenticity, and non-repudiation. |
| **Digital certificate** | An electronic document linking an identity to a public key. | A website certificate identifies example.com. | Certificates support trusted encrypted connections. |
| **PKI** | The people, policies, systems, and technology used to manage certificates and public keys. | An organization issues certificates to users and servers. | PKI provides scalable trust and identity verification. |
| **Certificate authority** | A trusted organization or system that issues and signs certificates. | DigiCert or an internal enterprise CA. | Trust in certificates depends on the CA. |
| **Root CA** | The highest-level trusted CA whose certificate normally signs intermediate CAs. | A browser contains trusted root certificates. | Root CA compromise can undermine the entire trust chain. |
| **Intermediate CA** | A CA signed by a root CA that issues certificates to users or systems. | An intermediate signs a website certificate. | It protects the root CA from routine exposure. |
| **Certificate chain** | The linked path from an end certificate through intermediate CAs to a trusted root CA. | Website certificate → intermediate CA → root CA. | Clients validate the entire chain before trusting a certificate. |
| **CSR** | A request containing identity information and a public key sent to a CA for certificate issuance. | A web administrator requests a new TLS certificate. | Protecting the associated private key remains critical. |
| **CRL** | A published list of certificates that a CA has revoked. | A browser checks whether a certificate appears on the list. | Revocation prevents continued trust in compromised certificates. |
| **OCSP** | A protocol that asks a CA whether one certificate remains valid. | A browser checks a website certificate in real time. | It provides faster status checks than downloading a full CRL. |
| **Self-signed certificate** | A certificate signed by its own private key instead of a trusted CA. | A lab server generates its own certificate. | Clients cannot automatically trust the claimed identity. |
| **Wildcard certificate** | A certificate that covers multiple hosts under one domain. | *.example.com covers mail.example.com and vpn.example.com. | Compromise can affect many covered services. |
| **Certificate pinning** | An application accepts only a specific certificate or public key. | A mobile app rejects unexpected certificates. | It helps resist fraudulent CAs and interception. |
| **Perfect forward secrecy** | A design where compromise of a long-term private key does not reveal older session data. | Ephemeral Diffie-Hellman creates new keys for each session. | It limits damage after future key theft. |
| [[1.2 - Non-repudiation\|Non-repudiation]] | Evidence that makes it difficult for someone to deny performing an action. | A verified digital signature proves who signed a document. | It supports accountability and legal confidence. |
| [[1.4 - Obfuscation\|Obfuscation]] | Making data or code harder to understand without truly encrypting it. | Renaming variables in JavaScript. | Obfuscation slows analysis but does not provide strong confidentiality. |
| **Encoding** | Changing data into another format for compatibility, not secrecy. | Base64 converts binary data into text characters. | Attackers may hide content in encoding, but anyone can decode it. |

---
[[00 - Overview|← Overview]]
