```mermaid
graph LR
    classDef routingSwitching fill:#8EC1DA,stroke:#333,stroke-width:2px;
    classDef security fill:#F6B26B,stroke:#333,stroke-width:2px;
    classDef connectivity fill:#93C47D,stroke:#333,stroke-width:2px;
    classDef monitoring fill:#B4A7D6,stroke:#333,stroke-width:2px;
    
    NSD["Network/Security Devices"]:::security

    subgraph  RSD ["Routing and Switching Devices"]
        router(Router\nLayer 3- Network)
        switch(Switch\nLayer 2 - DataLink)
        dns(DNS\nLayer 7 -- Application)
        dhcp(DHCP\nLayer 7 -- Application)
    end

    subgraph SD ["Security Devices\n"]
        firewall(Static Packet-Filtering Firewall\nLayer3--Network \n Layer4--Transport)
        firewall1(Circuit-Level Firewall\nLayer5--Session)
        firewall2(Next-generation Firewall\nLayer2 Datalink -- Layer7 Application)
        ids_ips("IDS/IPS\nLayer 3 Network -7 Application")
        dlp(Data Loss Prevention\nLayer 7 -- Application)
        nac(Network Access Control\nayer2 Datalink - Layer7 Applicatio)
        proxy(Proxy Server\nLayer 7--Application )
    end

    subgraph CED ["Connectivity Enhancement Devices\n"]
        vpn(VPN Appliance\nLayers 2-3)
        wap(Wireless Access Points\nLayer 1-2)
        lb(Load Balancer\nLayers 4-7)
    end

    subgraph NMMD["Network Monitoring and Management Devices\n"]
        nms(Network Management Systems\nLayers 2-7)
        probe("Network Probes/Analyzers\nLayers 1-7")
    end

    NSD-->RSD
    NSD-->SD
    NSD-->CED
    NSD-->NMMD
    
    class router,switch,dns,dhcp routingSwitching;
    class firewall,firewall1,firewall2,ids_ips,dlp,nac,proxy security;
    class vpn,wap,lb connectivity;
    class nms,probe monitoring;
