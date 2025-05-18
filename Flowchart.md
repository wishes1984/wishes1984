mermaid
flowchart TD
    A[External Drivers\nRegulations] --> C[Compliance & Certification\nH6: β=0.143**]
    B[Inbound Logistics] --> D[Green Logistics\nH7: β=0.237***]
    C --> E[Environmental Sustainability]
    D --> E
    E --> F[Productivity\nH9: β=0.461***]
    E --> G[Quality\nH10: β=0.593***]
    E --> H[Innovation\nH11: β=0.442***]
    E --> I[Customer Relationships\nH13: β=0.317***]
    
    J[Technology Adoption\nH2: β=-0.032] -.-> E
    K[Top Management\nH3: β=0.081] -.-> E
    E -.-> L[Supplier Relationships\nH12: β=0.076]
    
    style A,B,C,D,E,F,G,H,I stroke:#0066cc,stroke-width:2px
    style J,K,L stroke:#999,stroke-dasharray:3

