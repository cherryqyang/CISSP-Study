```mermaid
graph LR 
%% "Application Security Verification Standard overview"
    AV1("Security Architecture, Design and Threat Modeling")
    AV0("Security Design and Threat Modeling")
    SSDLC("Secure Software Development Lifecycle")
    ThreatModeling("Threat Modeling")
    UserStories("User Stories and Security Requirements")
    SecureArchDesign("Secure Architecture and Design Review")
    AV2["Authentication Architecture"]
    AV1 --> AV2
    AV3["Session Management Architecture"]
    AV1 --> AV3
    AV4["Access Control Architecture"]
    AV1 --> AV4
    AV5["Validation, Sanitization and Encoding Architecture"]
    AV1 --> AV5
    AV6["Stored Cryptography Architecture"]
    AV1 --> AV6
    AV7["Error Handling, Logging and Auditing Architecture"]
    AV1 --> AV7
    AV8["Data Protection Architecture"]
    AV1 --> AV8
    AV9["Communication Architecture"]
    AV1 --> AV9
    AV10["Malicious Code Architecture"]
    AV1 --> AV10
    AV11["Business Logic Architecture"]
    AV1 --> AV11
    AV12["Secure File Upload Architecture"]
    AV1 --> AV12
    AV13["API and Web Service Architecture"]
    AV1 --> AV13
    AV14["Configuration Architecture"]
    AV1 --> AV14

    AV0 --> SSDLC
    AV0 --> ThreatModeling
    AV0 --> UserStories
    AV0 --> SecureArchDesign
