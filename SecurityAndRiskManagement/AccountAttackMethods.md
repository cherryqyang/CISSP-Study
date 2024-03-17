```mermaid
flowchart LR
    classDef category fill:#f9f,stroke:#333,stroke-width:4px;
    classDef attack fill:#ccf,stroke:#333,stroke-width:2px;

    attacks[Cyber Attacks Against User Accounts]:::category
    credentialBased[Credential-Based Attacks]:::category
    socialEngineering[Social Engineering Attacks]:::category
    eavesdropping[Eavesdropping and Interception Attacks]:::category
    accountTakeover[Account Takeover and Fraud]:::category
    cryptographic[Cryptographic Attack]:::category

    attacks --> credentialBased
    attacks --> socialEngineering
    attacks --> eavesdropping
    attacks --> accountTakeover
    attacks --> cryptographic

    credentialStuffing[Credential Stuffing]:::attack
    bruteForce[Brute Force Attacks]:::attack
    dictionaryAttacks[Dictionary Attacks]:::attack

    credentialBased --> credentialStuffing
    credentialBased --> bruteForce
    credentialBased --> dictionaryAttacks

    phishing[Phishing]:::attack
    socialEngineeringAttack[Social Engineering]:::attack

    socialEngineering --> phishing
    socialEngineering --> socialEngineeringAttack

    keylogging[Keylogging]:::attack
    mitm[Man-in-the-Middle Attacks]:::attack
    sessionHijacking[Session Hijacking]:::attack

    eavesdropping --> keylogging
    eavesdropping --> mitm
    eavesdropping --> sessionHijacking

    simSwapping[SIM Swapping]:::attack
    rainbowTable[Rainbow Table Attacks]:::attack

    accountTakeover --> simSwapping
    accountTakeover --> rainbowTable

    birthdayAttack[Birthday Attack]:::attack

    cryptographic --> birthdayAttack
