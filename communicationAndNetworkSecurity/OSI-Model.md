```mermaid
flowchart TD
    L7(Application Layer) -->|Protocols| P7[HTTP/S, TLS DNS, Telnet<br>SSH,FTP/S, LPD, SNMP<br>NFS, SMTP,POP3, IMAP, LDAP, DHCP]
    L7 -->|Threats| T7[Malware<br>Phishing<br>Application vulnerabilities<br>DDoS attacks]
    L7 -->|Network Container| D7[Prodocol Data Unit-PDU]
    L7 -->|TLS/SSL<br>End-to-end encryption| E7[Encryption]
    L7 -->|Devices| G7[Application Firewall]
    L7 -->|Functionality| H7[Interfacing user application,<br>network services, operating system<br> with the protocol stack ]

    L6(Presentation Layer) -->|Protocols| P6[SSL<br>TLS<br>MIME]
    L6 -->|Threats| T6[Encryption attacks<br>MIME type attacks]
    L6 -->|Network Container| D6[Prodocol Data Unit-PDU]
    L6 -->|TLS/SSL<br>Encryption formats| E6[Encryption]
    L6 -->|Functionality| H6[Transforming data received into <br> an understandable format ]

    L5(Session Layer) -->|Protocols | P5[NetBIOS&RPC<br>SSH<br>TLS]
    L5 -->|Threats| T5[Session hijacking<br>Man-in-the-middle attacks<br>Session fixation]
    L5 -->|Network Container| D5[Protocol Data Unit-PDU]
    L5 -->|SSH<br>TLS| E5[Encryption]
    L5 -->|Devices| F5[Circuit Proxy Firewall<br> Circuit Level gateway]
    L5 -->|Address| G5[How to address]
    L5 -->|Functionality| H5[Establishing, maintaining <br> terminating sessions]

    L4(Transport Layer) -->|Protocols| P4[TCP/UDP <br> SSL/TLS & BGP]
    L4 -->|Threats| T4[Session hijacking<br>SYN flooding<br>Port scanning]
    L4 -->|Network Container| D4[Segment--TCP<br>Datagram--UDP]
    L4 -->|TLS/SSL| E4[Encryption]
    L4 -->|Devices| G4[any device?]
    L4 -->|Address| F4[ports = Services]
    L4 -->|Functionality| H4[managing the integrity of a connection<br> controlling the session]
    

    L3(Network Layer) -->|Protocols | P3[ICMP-Ping, IPSec, IGMP]
    L3 -->|Threats | T3[IP spoofing<br>ICMP attacks<br>Routing attacks]
    L3 -->|Network Container|D3[Packet]
    L3 -->|IPsec| E3[Encryption]
    L3 -->|Address| F3[logical Address/IP Address]
    L3 -->|Devices| G3[Routers <br> Packet filtering Firewall]
    L3 -->|Functionality| H3[Adding routing and addressing <br>information to the data]

    L2(Data Link Layer) -->|Protocols| P2[802.x, ARP, PPTP<br> PPP, PAP<br> CHAP, EAP]
    L2 -->|Threats | T2[MAC spoofing<br>ARP spoofing<br>LAN switch attacks<br>Spanning tree attack]
    L2 -->|Network Container| D2[Frame]
    L2 -->|Encryption| E2[MACsec <br>WEP<br>WPA1/WPA2/WAP3]
    L2 -->|Devices| F2[Switches & Bridges]
    L2 -->|Address| G2[Mac Address--6bytes48bits<br>first 3bytes-OUI-vendor/manufacture]
    L2 -->|Functionality| H2[Formatting the received data<br>format into transmission format]

    L1(Physical Layer) -->|Protocols| P1[Ethernet<br>USB<br>Bluetooth<br>802.11<br>GSM/CDMA/5G<br>DSL]
    L1 -->|Threats| T1[Physical damage<br>Tampering<br>Wiretapping<br>Eavesdropping<br>Interference]
    L1 -->|Network Container| D1[Bit]
    L1 -->|Security| E1[Physical security]
    L1 -->|Devices| F1[Hubs, Repeaters<br> Concentrators]
    L1 -->|Functionality| H1[Contains device driver<br>telling the protocol how to use<br>the hardware for the transmission<br>or the reception of the bits]


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
