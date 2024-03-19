```mermaid
graph LR
    style A fill:#f9f,stroke:#333,stroke-width:4px
    A[CISSP law regulations and standars] --> B[Laws & Regulations]
    A --> C[Standards]
    style B fill:#ccf,stroke:#333,stroke-width:2px
    style C fill:#cfc,stroke:#333,stroke-width:2px

    B --> GLBA[GLBA]
    style GLBA fill:#fcf,stroke:#333,stroke-width:1px
    GLBA --> GLBA_Desc["Gramm-Leach-Bliley Act: Requires financial institutions to protect customer information"]
    style GLBA_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> SOX[SOX]
    style SOX fill:#fcf,stroke:#333,stroke-width:1px
    SOX --> SOX_Desc["Sarbanes-Oxley Act: Protects investors by improving the accuracy of corporate disclosures"]
    style SOX_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> HIPAA[HIPAA]
    style HIPAA fill:#fcf,stroke:#333,stroke-width:1px
    HIPAA --> HIPAA_Desc["Health Insurance Portability and Accountability Act: Protects personal health information"]
    style HIPAA_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> FERPA[FERPA]
    style FERPA fill:#fcf,stroke:#333,stroke-width:1px
    FERPA --> FERPA_Desc["Family Educational Rights and Privacy Act: Protects the privacy of student education records"]
    style FERPA_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> FISMA[FISMA]
    style FISMA fill:#fcf,stroke:#333,stroke-width:1px
    FISMA --> FISMA_Desc["Federal Information Security Management Act: Requires federal agencies to protect government information"]
    style FISMA_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> PCI_DSS[PCI DSS]
    style PCI_DSS fill:#fcf,stroke:#333,stroke-width:1px
    PCI_DSS --> PCI_DSS_Desc["Payment Card Industry Data Security Standard: Ensures secure credit card transactions"]
    style PCI_DSS_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> GISRA[GISRA]
    style GISRA fill:#fcf,stroke:#333,stroke-width:1px
    GISRA --> GISRA_Desc["Government Information Security Reform Act: Required agencies to implement information security protections<br>superseded by FISMA"]
    style GISRA_Desc fill:#fff,stroke:#333,stroke-width:1px

    B --> GDPR[GDPR]
    style GDPR fill:#fcf,stroke:#333,stroke-width:1px
    GDPR --> GDPR_Desc["General Data Protection Regulation: Protects the data privacy of EU citizens"]
    style GDPR_Desc fill:#fff,stroke:#333,stroke-width:1px

    C --> ISO_IEC_27001[ISO/IEC 27001]
    style ISO_IEC_27001 fill:#cff,stroke:#333,stroke-width:1px
    ISO_IEC_27001 --> ISO_IEC_27001_Desc["International standard for information security management systems"]
    style ISO_IEC_27001_Desc fill:#fff,stroke:#333,stroke-width:1px

    C --> NIST[NIST Frameworks]
    style NIST fill:#cff,stroke:#333,stroke-width:1px
    NIST --> NIST_Desc["National Institute of Standards and Technology Frameworks: Provides cybersecurity guidelines"]
    style NIST_Desc fill:#fff,stroke:#333,stroke-width:1px

    C --> COBIT[COBIT]
    style COBIT fill:#cff,stroke:#333,stroke-width:1px
    COBIT --> COBIT_Desc["Control Objectives for Information and Related Technologies: IT management and governance framework"]
    style COBIT_Desc fill:#fff,stroke:#333,stroke-width:1px

