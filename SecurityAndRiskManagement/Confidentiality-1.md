```mermaid
graph LR
    A[Confidentiality in Information Security] --> B[Encryption]
    A --> C[Access Controls]
    
    B --> D[Data at Rest Encryption]
    B --> E[Data in Transit Encryption]
    B --> F[End-to-End Encryption]
    
    C --> G[User Authentication]
    C --> H[Least Privilege Principle]
    C --> I[Role-based Access Control RBAC]
    C --> J[Mandatory and Discretionary Access Control]
    C --> K[Audit Trails]
    C --> L[Time-based/Context-aware Access Controls]
    
    D --> M[Prevents Unauthorized Data Access at Rest]
    E --> N[Prevents Data Interception during Transit]
    F --> O[Prevents Unauthorized Data Access from Intermediaries]
    
    G --> P[Prevents Unauthorized System Access]
    H --> Q[Minimizes Unnecessary Data Exposure]
    I --> R[Limits Access Based on User Roles]
    J --> S[Enforces Organizational or Owner-defined Policies]
    K --> T[Detects and Deters Unauthorized Access]
    L --> U[Restricts Access Based on Context or Time]
    
    M --> V[Example Breach: Lost or Stolen Devices]
    N --> W[Example Breach: Man-in-the-Middle Attacks]
    O --> X[Example Breach: Intermediary Data Snooping]
    P --> Y[Example Breach: Unauthorized System Entry]
    Q --> Z[Example Breach: Excessive Permissions Exploitation]
    R --> AA[Example Breach: Role Elevation Attack]
    S --> AB[Example Breach: Policy Bypass or Misconfiguration]
    T --> AC[Example Breach: Unauthorized Access Detection Failure]
    U --> AD[Example Breach: Time-based Access Anomalies]
