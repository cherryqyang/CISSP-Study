```mermaid
graph TD
    A[SDLC Stages] --> B[Requirements Gathering]
    A --> C[Design Phase]
    A --> D[Development Phase]
    A --> E[Testing Phase]
    A --> F[Deployment and Maintenance]

    B --> G[Identify Security Objectives]
    C --> H[Conduct Threat Modeling]
    D --> I[Implement Security Controls]
    E --> J[Test for Threats and Vulnerabilities]
    F --> K[Revisit Threat Modeling for Changes]

    H --> L[Threat Identification]
    H --> M[Risk Assessment]
    H --> N[Countermeasure Definition]

    L --> O[Document Identified Threats]
    M --> P[Document Risk Levels]
    N --> Q[Plan for Countermeasures]

    O --> R[Threat Documentation]
    P --> S[Risk Analysis Documentation]
    Q --> T[Countermeasure Implementation Plan]
