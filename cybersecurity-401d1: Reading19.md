The STRIDE Security Threat Model has six areas of focus:

Spoofing
Tampering
Repudiation
Information Disclosure
Denial of Service
Elevation of Privilege

Spoofing

When you provide access to your systems or data, you need to authenticate every request. The security of your systems depends upon trust in the other party’s identity. A threat to this trust is spoofing — when someone claims to be a person or system they are not.

Single key: many APIs use a single API Key to authenticate requests to their service. The value is static, though it can typically be deleted and regenerated in a user interface. Anyone who obtains the key would have access to the systems that trust it indefinitely.

Access token: similar to the single key, an access token is one value that authenticates a request. However, the access is usually limited in some way, often only usable for a short period. Anyone with an access token would only have minimal usage before needing additional credentials to generate another token.

Signatures: in contrast to the other two methods, signature-based authentication uses encryption, which requires private keys. Each request is signed using a shared secret that you can verify. To spoof a signature, the attacker would need access to the sender's private key.
These are just a few common examples of spoofing. The important thing to consider is what mechanism you’re using to communicate identity and how you know the identity can be trusted. Look to common methods and conventions, such as open source libraries, to ensure your systems are secure and not vulnerable to spoofing attacks.

Tampering

Even if you feel confident in your authentication security, trust must extend to all systems you touch. When you retrieve data from a system, for example, you should feel confident that it’s reliable. Data is especially susceptible to threats of tampering, but physical machines or hardware may also be vulnerable.

Repudiation

Secure systems should build in non-repudiation mechanisms, such that the data source and the data itself can be trusted. For this reason, repudiation is intertwined with other elements of the STRIDE framework. For example, tampered logs or a spoofed account both could lead to the user denying wrongdoing.

Information Disclosure

Significant data breaches have made headlines in recent years. Passwords, payment details, and other personal data can be expensive disclosures. At a minimum, customers have to be notified and high profile incidents have extended consequences.

Denial Of Service

Another security threat from the technical news, a denial of service makes a system unreachable by exploiting resources so they can’t be used for legitimate purposes. In networking, this can mean overloading a system with incoming requests, making it impossible for users to connect.

Elevation Of Privilege

The final area of the STRIDE framework could be the most threatening. Where spoofing is focused on authentication, elevation of privilege is related to authorization. In other words, the attacker not only claimed to be a valid user, but one with an expanded role.


