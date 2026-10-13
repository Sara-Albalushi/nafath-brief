Version: NAFATH-V1
Your track: Cybersecurity

Overview


A national digital login service connects citizens to government services through one account. Software standards help the service verify identities and control access to protected resources. Artificial intelligence can identify unusual login patterns, but its decisions must be tested for accuracy, fairness, privacy, and security. Mobile applications must request sensitive permissions appropriately and protect information stored on devices. Networking technologies help secure communication and protect certain parts of users’ online activity. Data protection practices ensure that citizens’ personal information is collected and handled responsibly under applicable laws. Cybersecurity controls, especially phishing-resistant authentication, help protect citizens’ accounts from phishing attacks and unauthorized access.



Software


OAuth 2.0 and OpenID Connect serve different purposes in a national login service. OAuth 2.0 allows applications to obtain limited access to protected resources. OpenID Connect adds an identity layer to OAuth 2.0, enabling applications to verify a user's identity. Therefore, OAuth 2.0 is designed for delegated access, while OpenID Connect is designed for user authentication.


Resource: OpenID Connect Core 1.0 - https://openid.net/specs/openid-connect-core-1_0.html


AI

Before launching an AI model to flag suspicious logins, the authority should identify potential risks and define clear responsibilities. Using the NIST AI Risk Management Framework, it should map the system’s context and possible impacts, measure its accuracy, security, privacy, and bias, and manage identified risks. The model should be tested before deployment, monitored continuously, and updated or disabled if it produces unsafe or unreliable results.


Resource: AI Risk Management Framework - NIST - https://airc.nist.gov/airmf-resources/airmf/5-sec-core/


Mobile

Android uses runtime permissions to protect sensitive user data. An application should request permission when the user uses a feature that needs access, such as the camera or location. It should explain why the permission is needed and check whether access has been granted. If the user denies permission, the app should respect the decision and continue working where possible.


Resource: Request runtime permissions - Android Developers - https://developer.android.com/training/permissions/requesting


Networking


DNS over HTTPS (DoH) sends DNS queries and responses over HTTPS, encrypting them during transmission. For the national login service, DoH can help protect citizens' DNS queries from network observers and reduce interference with DNS traffic. However, it does not hide all online activity, such as the destination IP address, and the DoH provider may still see the queries. Therefore, DoH improves DNS privacy but is not a complete privacy or security solution.


Resource: RFC 8484 - DNS Queries over HTTPS (DoH) - https://www.rfc-editor.org/rfc/rfc8484


Cybersecurity


Phishing-resistant authentication helps protect the national login service from fake websites that try to steal citizens’ credentials. CISA identifies FIDO/WebAuthn as a widely available phishing-resistant method, using security keys or authenticators built into devices. PKI-based methods, such as smart cards, can also provide phishing-resistant MFA. However, text and email codes are not generally phishing-resistant because attackers may steal or relay them. The service should prioritize phishing-resistant methods to reduce account takeover risks.


Resource: Implementing Phishing-Resistant MFA - CISA - https://www.cisa.gov/sites/default/files/2023-01/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf


Data


Oman’s Personal Data Protection Law (Royal Decree 6/2022, as amended in 2026) sets rules for processing personal data. However, it excludes processing by government administrative units when carrying out their legally assigned duties. Such authorities must follow the applicable government personal data protection policy. The login service should explain why citizens’ data is collected, protect stored information, restrict its use to authorized purposes, and follow the applicable rules for data rights and breach reporting.


Resource: Personal Data Protection Policy for Units of the State Administrative Apparatus - MTCIT Oman - https://www.mtcit.gov.om/library-3/legislations-policies-8/policies-73/personal-data-protection-policy-for-units-of-the-state-administrative-apparatus-1342


Misconception in My Track


A common misconception is that all multi-factor authentication (MFA) methods provide equal protection against phishing. In reality, attackers may steal or relay codes sent by text or email, so these methods are not generally phishing-resistant. CISA identifies FIDO/WebAuthn as a widely available phishing-resistant method and also describes PKI-based MFA, such as smart cards. This shows that using more than one authentication factor does not automatically prevent phishing. The CISA resource supports this correction under the heading “Phishing-Resistant MFA Implementations,” particularly the “FIDO/WebAuthn Authentication” and “PKI-based MFA” sections.


Open Question


How can the authority make phishing-resistant authentication accessible to citizens using different phones and devices, while keeping account recovery secure?


