```mermaid
flowchart LR
    classDef dataProtection fill:#f9d5e5,stroke:#b548c6,stroke-width:2px;
    classDef ipProtection fill:#fefbd8,stroke:#b58946,stroke-width:2px;
    classDef ethics fill:#d0f4de,stroke:#3c9d9b,stroke-width:2px;
    classDef forensics fill:#f7cac9,stroke:#f7786b,stroke-width:2px;
    classDef standards fill:#b5ead7,stroke:#96c9dc,stroke-width:2px;
    classDef laws fill:#c5cbe3,stroke:#6b5b95,stroke-width:2px;
    classDef incidentResponse fill:#ffef96,stroke:#ffcc5c,stroke-width:2px;
    
    A[CISSP Compliance and Legal Issues] --> B[Data Protection Laws]
    A --> C[IP Protections]
    A --> D[Professional Ethics]
    A --> E[Digital Forensics]
    A --> F[Standards and Frameworks]
    A --> G[Relevant Laws]
    A --> H[Incident Response]
    
    B --> B1[GDPR]
    B --> B2[PCI DSS]
    B --> B3[US-EU Privacy Shield Invalidated]
    B --> B4[CFAA]
    B --> B5[HIPAA]
    class B,B1,B2,B3,B4,B5 dataProtection;
    
    C --> C1[Copyright for Software]
    C --> C2[Trade Secrets for Processes/Algorithms]
    C --> C3[Patents for Unique Functionalities]
    class C,C1,C2,C3 ipProtection;
    
    D --> D1[Code of Ethics Purpose]
    D --> D2[Ensuring Trust and Professionalism]
    class D,D1,D2 ethics;
    
    E --> E1[Chain of Custody Importance]
    E --> E2[E-discovery Process]
    E --> E3[Role of InfoSec in E-discovery]
    class E,E1,E1A,E1B,E2,E2A,E2B,E2C,E3,E3A,E3B,E3C forensics;
    
    F --> F1[ISO 27001]
    class F,F1 standards;
    
    G --> G1[Employment Law]
    class G,G1 laws;
    
    H --> H1[Incident Response Process]
    class H,H1,H1A,H1B,H1C,H1D incidentResponse;
    
    E1 --> E1A[Ensuring Integrity and Authenticity]
    E1 --> E1B[Legal Admissibility]
    
    E2 --> E2A[Identification and Preservation]
    E2 --> E2B[Collection and Analysis]
    E2 --> E2C[Review and Production]
    
    E3 --> E3A[Securing Data]
    E3 --> E3B[Providing Expertise]
    E3 --> E3C[Ensuring Compliance]
    
    H1 --> H1A[Preparation]
    H1 --> H1B[Detection and Analysis]
    H1 --> H1C[Containment, Eradication, and Recovery]
    H1 --> H1D[Post-Incident Activity]
