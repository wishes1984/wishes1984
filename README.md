%%{init: {'theme': 'neutral', 'fontFamily': 'Arial', 'gantt': {'barHeight': 20}}}%%
flowchart TD
    %% ========== INPUTS/DRIVERS ==========
    A[External Drivers\n<small>(Regulatory Pressures, e.g.,\nCarbon Tax Act, ISO 14001)</small>]
    B[Inbound Logistics\n<small>(Low-emission transport,\nRoute optimization)</small>]

    %% ========== CORE PILLARS ==========
    subgraph Core Pillars[" "]
        C[Compliance & Certification\n<small>(H6: β = 0.143**, p = 0.018)</small>]
        D[Green Logistics\n<small>(H7: β = 0.237***, p < 0.001)</small>]
    end

    %% ========== MEDIATOR ==========
    E[Environmental Sustainability\n<small>(ES)</small>]

    %% ========== OUTPUTS ==========
    F[Productivity\n<small>(H9: β = 0.461***)</small>]
    G[Quality\n<small>(H10: β = 0.593***)</small>]
    H[Innovation\n<small>(H11: β = 0.442***)</small>]
    I[Customer Relationships\n<small>(H13: β = 0.317***)</small>]

    %% ========== INSIGNIFICANT PATHS (GREYED OUT) ==========
    J[Technology Adoption\n<small>(H2: β = -0.032, p = 0.661)</small>]:::insignificant
    K[Top Management Support\n<small>(H3: β = 0.081, p = 0.321)</small>]:::insignificant
    L[Supplier Relationships\n<small>(H12: β = 0.076, p = 0.182)</small>]:::insignificant

    %% ========== ARROW CONNECTIONS ==========
    A --> C
    B --> D
    C --> E
    D --> E
    E --> F
    E --> G
    E --> H
    E --> I

    %% ========== GREYED-OUT INSIGNIFICANT PATHS ==========
    J -.-> E
    K -.-> E
    E -.-> L

    %% ========== STYLING ==========
    classDef significant fill:#e6f3ff,stroke:#0066cc,stroke-width:2px
    classDef insignificant fill:#f0f0f0,stroke:#999,stroke-dasharray:3
    class A,B,C,D,E,F,G,H,I significant
    class J,K,L insignificant
