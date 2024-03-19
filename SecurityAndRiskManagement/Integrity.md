```mermaid
flowchart LR
    %% Define styles
    classDef importance fill:#ffcccc,color:#000;
    classDef measures fill:#ccffcc,color:#000;
    classDef threats fill:#ccccff,color:#000;
    classDef backup fill:#ffffcc,color:#000;
    classDef example fill:#ccffff,color:#000;

    subgraph Integrity_Importance ["Importance of Data Integrity"]
        direction LR
        Data_Consistency["Data Consistency"]
        Data_Accuracy["Data Accuracy"]
        Trustworthiness["Trustworthiness"]
    end

    subgraph Integrity_Ensuring_Measures ["Measures to Ensure Data Integrity"]
        direction LR
        Encryption["Encryption"]
        Secure_Protocols["Secure Transmission Protocols"]
        Hashing["Hashing"]
        Digital_Signatures["Digital Signatures"]
        Data_Integrity_Checks["Data Integrity Checks"]
        Access_Controls["Access Controls"]
        Monitoring["Monitoring & Alerts"]
        Endpoint_Security["Endpoint Security"]
        Regular_Audits["Regular Audits & Testing"]
    end

    subgraph Integrity_Threats ["Common Threats to Data Integrity"]
        direction LR
        Human_Errors["Human Errors"]
        Malware["Malware"]
        Hacking["Hacking & Unauthorized Access"]
        Insider_Threats["Insider Threats"]
        Data_Transfer_Errors["Data Transfer Errors"]
        Physical_Threats["Physical Threats"]
        Software_Bugs["Software Bugs & Glitches"]
        SQL_Injection["SQL Injection"]
        MitM_Attacks["MitM Attacks"]
    end

    subgraph Backup_Role ["Role of Backups in Data Integrity"]
        direction LR
        Recovery_Corruption["Recovery from Data Corruption"]
        Protection_Alterations["Protection Against Malicious Alterations"]
        Historical_Accuracy["Historical Accuracy"]
        Redundancy["Redundancy"]
        Audit_Compliance["Audit & Compliance"]
        Physical_Damage["Mitigating Physical Damage"]
        Business_Continuity["Ensuring Business Continuity"]
    end

    subgraph Example ["Example: Healthcare"]
        direction LR
        EHR_Integrity["EHR Data Integrity > Confidentiality"]
        Patient_Safety["Critical for Patient Safety"]
        Treatment_Accuracy["Ensures Treatment Accuracy"]
    end

    %% Apply styles
    class Integrity_Importance importance;
    class Integrity_Ensuring_Measures measures;
    class Integrity_Threats threats;
    class Backup_Role backup;
    class Example example;

    Integrity_Importance --> Integrity_Ensuring_Measures
    Integrity_Ensuring_Measures --> Integrity_Threats
    Integrity_Ensuring_Measures --> Backup_Role
    Backup_Role --> Example
