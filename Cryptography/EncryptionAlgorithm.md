```mermaid
classDiagram
    class Symmetric {
        +AES
        +DES
        +3DES
        +Blowfish/Twofish
    }
    class Asymmetric {
        +RSA
        +ECC
        +Diffie-Hellman
    }
    class Hash {
        +MD5
        +SHA-1
        +SHA-2
        +SHA-3
    }

    class AES {
        +Block cipher
        +Key sizes: 128, 192, 256 bits
    }
    class DES {
        +Block cipher
        +56-bit key
        +Vulnerable
    }
    class 3DES {
        +Block cipher
        +Key lengths: 112, 168 bits
        +More secure than DES
    }
    class BlowfishTwofish {
        +Block cipher
        +Key sizes: up to 448/256 bits
    }
    class RSA {
        +Large prime factorization
        +Key sizes: 1024 to 4096 bits
    }
    class ECC {
        +Elliptic curves
        +Smaller key sizes, efficient
    }
    class DiffieHellman {
        +Key exchange
        +Susceptible to MITM if not secured
    }
    class MD5 {
        +128-bit hash
        +Broken and vulnerable
    }
    class SHA-1 {
        +160-bit hash
        +Vulnerabilities demonstrated
    }
    class SHA-2 {
        +Variants: SHA-224, SHA-256, SHA-384, SHA-512
        +Considered secure
    }
    class SHA-3 {
        +Different foundation from SHA-2
        +Considered secure
    }

    Symmetric -- AES
    Symmetric -- DES
    Symmetric -- 3DES
    Symmetric -- BlowfishTwofish: Blowfish/Twofish
    Asymmetric -- RSA
    Asymmetric -- ECC
    Asymmetric -- DiffieHellman: Diffie-Hellman
    Hash -- MD5
    Hash -- SHA-1
    Hash -- SHA-2
    Hash -- SHA-3
