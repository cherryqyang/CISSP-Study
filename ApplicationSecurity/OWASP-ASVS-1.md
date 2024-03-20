```mermaid
graph TD
AV1["Architecture, Design and Threat Modeling"]
AV2["Authentication"]
AV1 --> AV2
AV3["Session Management"]
AV2 --> AV3
AV4["Access Control"]
AV3 --> AV4
AV5["Validation, Sanitization and Encoding"]
AV4 --> AV5
AV6["Stored Cryptography"]
AV5 --> AV6
AV7["Error Handling and Logging"]
AV6 --> AV7
AV8["Data Protection"]
AV7 --> AV8
AV9["Communication"]
AV8 --> AV9
AV10["Malicious Code"]
AV9 --> AV10
AV11["Business Logic"]
AV10 --> AV11
AV12["Files and Resources"]
AV11 --> AV12
AV13["API and Web Service"]
AV12 --> AV13
AV14["Configuration"]
AV13 --> AV14
