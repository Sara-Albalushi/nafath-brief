Version: NAFATH-V1
Your track: Cybersecurity

Overview


A national digital login service connects citizens to government services through one account. Software standards help the service verify identities and control access to protected resources. Artificial intelligence can identify unusual login patterns, but its decisions must be tested for accuracy, fairness, privacy, and security. Mobile applications must request sensitive permissions appropriately and protect information stored on devices. Networking technologies help secure communication and protect certain parts of users’ online activity. Cybersecurity controls reduce the risk of account theft, phishing, and unauthorized access. Data protection practices ensure that citizens’ personal information is collected and handled responsibly under applicable laws. These six fields work together to make the service secure, reliable, accessible, and trustworthy for citizens.


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

Cybersecurity

Data

Misconception in My Track

Open Question
