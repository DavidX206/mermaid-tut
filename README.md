graph TD
    %% Nodes
    A[1. Patient arrives<br><small>Walk-in or EMS</small>]
    B[2. Registration<br><small>Clerk records demographics</small>]
    C[3. Vital signs<br><small>Nurse records — paper first</small>]
    D{4. Triage level<br>ESI Assessment}
    E1[ESI Level 1]
    E2[ESI Level 2]
    E3[ESI Level 3]
    F[5. Care area assignment]
    G[6. Consultant disposition]

    %% Connections
    A --> B
    B --> C
    C --> D
    
    D --> E1
    D --> E2
    D --> E3
    
    E1 --> F
    E2 --> F
    E3 --> F
    
    F --> G

    %% Styling
    style D fill:#f9f,stroke:#333,stroke-width:2px
    style E1 fill:#ffcccb,stroke:#333
    style E2 fill:#ffe5b4,stroke:#333
    style E3 fill:#ffffcc,stroke:#333
