# Pyramid of Pain

![](https://i.ibb.co/QYWXRSh/pop2.png)

## Hash Values (Trivial)

Some of the most common hashing algorithms:   

-   **MD5 (Message Digest, defined by [RFC 1321](https://www.ietf.org/rfc/rfc1321.txt)****)** - was designed by Ron Rivest in 1992 and is a widely used cryptographic hash function with a 128-bit hash value. MD5 hashes are **NOT** considered **cryptographically secure**. In 2011, the IETF published RFC 6151, ["Updated Security Considerations for the MD5 Message-Digest and the HMAC-MD5 Algorithms](https://datatracker.ietf.org/doc/html/rfc6151)," which mentioned a number of attacks against MD5 hashes, including the hash collision.
-   SHA-1 (Secure Hash Algorithm 1, defined by [RFC 3174](https://tools.ietf.org/html/rfc3174)) - was invented by United States National Security Agency in 1995. When data is fed to SHA-1 Hashing Algorithm, SHA-1 takes an input and produces a 160-bit hash value string as a 40 digit hexadecimal number. [NIST deprecated the use of SHA-1 in 2011](https://csrc.nist.gov/news/2017/research-results-on-sha-1-collisions) and banned its use for digital signatures at the end of 2013 based on it being susceptible to brute-force attacks. Instead, NIST recommends migrating from SHA-1 to stronger hash algorithms in the SHA-2 and SHA-3 families.
-   **The SHA-2 (Secure Hash Algorithm 2)** - SHA-2 Hashing Algorithm was designed by The National Institute of Standards and Technology (NIST) and the National Security Agency (NSA) in 2001 to replace SHA-1. SHA-2 has many variants, and arguably the most common is SHA-256. The SHA-256 algorithm returns a hash value of 256-bits as a 64 digit hexadecimal number.

A hash is not considered to be cryptographically secure if two files have the same hash value or digest.

Security professionals usually use the hash values to gain insight into a specific malware sample, a malicious or a suspicious file, and as a way to uniquely identify and reference the malicious artifact.

It is really easy to spot a malicious file if we have the hash in our arsenal. However, as an attacker, it’s trivial to modify a file by even a single bit, which would produce a different hash value.

## IP Address (Easy)

From a defense standpoint, knowledge of the IP addresses an adversary uses can be valuable. A common defense tactic is to block, drop, or deny inbound requests from IP addresses on your parameter or external firewall. This tactic is often not bulletproof as it’s trivial for an experienced adversary to recover simply by using a new public IP address.

Fast Flux is a DNS technique used by botnets to hide phishing, web proxying, malware delivery, and malware communication activities behind compromised hosts acting as proxies. The purpose of using the Fast Flux network is to make the communication between malware and its command and control server (C&C) challenging to be discovered by security professionals. 

So, the primary concept of a Fast Flux network is having multiple IP addresses associated with a domain name, which is constantly changing. Palo Alto created a great fictional scenario to explain Fast Flux: ["](https://unit42.paloaltonetworks.com/fast-flux-101/)[Fast Flux 101: How Cybercriminals Improve the Resilience of Their Infrastructure to Evade Detection and Law Enforcement Takedowns"](https://unit42.paloaltonetworks.com/fast-flux-101/)


## Domain Names (Simple)

