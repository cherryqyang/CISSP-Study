```mermaid
flowchart TD
    L7(Application Layer) -->|HTTP<br>FTP<br>SMTP| P7[Protocols]
    L7 -->|Malware<br>Phishing<br>Application vulnerabilities<br>DDoS attacks| T7[Threats]
    L7 -->|Data Message| D7[Data Unit]
    L7 -->|TLS/SSL<br>End-to-end encryption| E7[Encryption]
    L6(Presentation Layer) -->|SSL<br>TLS<br>MIME| P6[Protocols]
    L6 -->|Encryption attacks<br>MIME type attacks| T6[Threats]
    L6 -->|Data| D6[Data Unit]
    L6 -->|TLS/SSL<br>Encryption formats| E6[Encryption]
    L5(Session Layer) -->|NetBIOS<br>SSH<br>TLS| P5[Protocols]
    L5 -->|Session hijacking<br>Man-in-the-middle attacks<br>Session fixation| T5[Threats]
    L5 -->|Data| D5[Data Unit]
    L5 -->|SSH<br>TLS| E5[Encryption]
    L4(Transport Layer) -->|TCP<br>UDP| P4[Protocols]
    L4 -->|Session hijacking<br>SYN flooding<br>Port scanning| T4[Threats]
    L4 -->|Segment/Datagram| D4[Data Unit]
    L4 -->|TLS/SSL| E4[Encryption]
    L3(Network Layer) -->|IP<br>ICMP<br>ARP| P3[Protocols]
    L3 -->|IP spoofing<br>ICMP attacks<br>Routing attacks| T3[Threats]
    L3 -->|Packet| D3[Data Unit]
    L3 -->|IPsec| E3[Encryption]
    L2(Data Link Layer) -->|Ethernet<br>PPP<br>Switching| P2[Protocols]
    L2 -->|MAC spoofing<br>ARP spoofing<br>LAN switch attacks| T2[Threats]
    L2 -->|Frame| D2[Data Unit]
    L2 -->|MACsec| E2[Encryption]
    L1(Physical Layer) -->|Ethernet<br>USB<br>Bluetooth| P1[Protocols]
    L1 -->|Physical damage<br>Wiretapping<br>Eavesdropping<br>Interference| T1[Threats]
    L1 -->|Bit| D1[Data Unit]
    L1 -->|Physical security| E1[Encryption]

    classDef layer fill:#f9f,stroke:#333,stroke-width:4px;
    classDef protocol fill:#cfc,stroke:#333,stroke-width:2px;
    classDef threat fill:#ccf,stroke:#333,stroke-width:2px;
    classDef dataunit fill:#fcf,stroke:#333,stroke-width:2px;
    classDef encryption fill:#cff,stroke:#333,stroke-width:2px;
    class L1,L2,L3,L4,L5,L6,L7 layer;
    class P1,P2,P3,P4,P5,P6,P7 protocol;
    class T1,T2,T3,T4,T5,T6,T7 threat;
    class D1,D2,D3,D4,D5,D6,D7 dataunit;
    class E1,E2,E3,E4,E5,E6,E7 encryption;

    L7 --> L6
    L6 --> L5
    L5 --> L4
    L4 --> L3
    L3 --> L2
    L2 --> L1
