```mermaid
graph LR
    classDef confidentiality fill:#9ad3bc,stroke:#333,stroke-width:2px,font-family:Arial,font-weight:bold;
    classDef principles fill:#f7dd72,stroke:#333,stroke-width:2px,font-family:Helvetica,font-weight:bold;
    classDef measures fill:#ffffff,stroke:#333,stroke-width:2px,font-family:Arial;
    classDef notes fill:#f29b9b,stroke:#333,stroke-width:2px,font-family:Verdana,font-style:italic;

    A[Confidentiality]
    B[Integrity]
    C[Availability]

    class A principles;
    class B principles;
    class C principles;

    A1[Encryption <br> Access Control<br>information classification<br>Authentication<br>User Training]
    B1[Backup Systems <br> Version Control<br>Checksums<br>Audit Trails]
    C1[Redundancy <br> Failover Systems<br> Disaster recovery plan]

    class A1,B1,C1 measures;

    A2[keeping information private and secure<br> protecting it from unauthorized access]
    B2[data remaining accurate, trustworthy<br> and consistent]
    C2[consistently accessible to<br> authorized parties]

    class A2,B2,C2 notes;

    A1 --> A
    B1 --> B
    C1 --> C

    A2 --> A
    B2 --> B
    C2 --> C

    A --> B
    B --> C
    C --> A