```mermaid
graph LR;
    A[Cryptographic Modes of Operation] --> B[ECB Electronic Codebook]
    A --> C[CBC Cipher Block Chaining]
    A --> D[CFB Cipher Feedback]
    A --> E[OFB Output Feedback]
    A --> F[CTR Counter]
    A --> G[GCM Galois/Counter Mode]
   

    B --> J["ECB: Encrypts each block independently, revealing patterns."]
    C --> K["CBC: XORs each block with the previous ciphertext block."]
    D --> L["CFB: Makes a block cipher into a self-synchronizing stream cipher."]
    E --> M["OFB: Makes a block cipher into a synchronous stream cipher."]
    F --> N["CTR: Turns a block cipher into a stream cipher using a counter."]
    G --> O["GCM: Provides both encryption and authentication, using CTR mode for encryption and adding a data integrity check."]
 