```mermaid
classDiagram
    class StreamCiphers {
        +RC4
        +Salsa20/ChaCha
        +A5/1 and A5/2
    }

    class RC4 {
        +Used in SSL, WEP
        +Simple and fast
        +Known vulnerabilities
    }

    class Salsa20ChaCha {
        +High speed and security
        +Used in TLS, Google encryption
        +Designed by Daniel J. Bernstein
    }

    class A5_1_and_A5_2 {
        +Used in GSM networks
        +A5/1 stronger than A5/2
        +Considered insecure
    }

    StreamCiphers -- RC4
    StreamCiphers -- Salsa20ChaCha
    StreamCiphers -- A5_1_and_A5_2
