```mermaid
graph TD
    B2CCustomer[B2C Customer - Browser]
    AngularFrontend[Angular Frontend]
    ApplicationServer[Application Server]
    Google[Google - Out of Scope]
    B2CCustomer -->|Data Flow| AngularFrontend
    AngularFrontend -->|Data Flow| ApplicationServer
    ApplicationServer -->|Data Flow| Google

    classDef inScope fill:#f9f,stroke:#333,stroke-width:2px;
    classDef outScope fill:#bbb,stroke:#333,stroke-width:2px,dasharray: 5, 5;
    class B2CCustomer,AngularFrontend,ApplicationServer inScope;
    class Google outScope;
