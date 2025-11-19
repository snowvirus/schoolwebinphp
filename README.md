# schoolwebinphp

# BUGEMA UNIVERSITY  
**DEPARTMENT OF COMPUTING & INFORMATICS**  
**IT Project Management – Assignment Solution**  
**Date: 31/10/2025**

## Given Data

| Activity | Duration | Immediate Predecessors |
|----------|----------|------------------------|
| A        | 2        | –                      |
| B        | 3        | –                      |
| C        | 3        | –                      |
| D        | 4        | A                      |
| E        | 5        | B                      |
| F        | 6        | B                      |
| G        | 6        | C                      |
| H        | 7        | D, E                   |
| I        | 8        | G                      |
| J        | 3        | H, F, I                |

---

### a) Network Diagram – Activity on Node (AoN)

```mermaid
graph TD
    Start --> A & B & C
    A --> D
    B --> E & F
    C --> G
    D --> H
    E --> H
    G --> I
    H --> J
    F --> J
    I --> J
    J --> Finish

    A[A(2)]:::act
    B[B(3)]:::act
    C[C(3)]:::act
    D[D(4)]:::act
    E[E(5)]:::act
    F[F(6)]:::act
    G[G(6)]:::act
    H[H(7)]:::act
    I[I(8)]:::act
    J[J(3)]:::act

    classDef act fill:#e1f5fe,stroke:#333,stroke-width:2px;