```mermaid
graph TD
    A[Dose (800 mg)] --> B[Blood Compartment]
    B[Blood Compartment] -->|ka: Absorption Rate Constant| C[Body Compartment]
    B[Blood Compartment] -->|k12: Rate Constant from Blood to Brain| D[Brain Compartment]
    D[Brain Compartment] -->|k21: Rate Constant from Brain to Blood| B[Blood Compartment]
    B[Blood Compartment] -->|k10: Elimination Rate Constant| E[Elimination]

    subgraph Parameters
        F[Body Weight (80 kg)]
        G[Volume of Distribution (0.14 L/kg)]
        H[Clearance (0.01 L/h/kg)]
        I[ka: Absorption Rate Constant (1 1/h)]
        J[k12: Rate Constant from Blood to Brain (0.2 1/h)]
        K[k21: Rate Constant from Brain to Blood (0.1 1/h)]
        L[k10: Elimination Rate Constant (0.01 1/h)]
    end
```
