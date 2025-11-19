# BUGEMA UNIVERSITY  
**DEPARTMENT OF COMPUTING & INFORMATICS**  
**IT Project Management – Assignment Solution**  
**Date: 31 October 2025**

---

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
**(Preferred by the Project Manager)**

```mermaid
graph TD
    Start[Start] --> A & B & C
    A[A<br>Dur=2] --> D[D<br>Dur=4]
    B[B<br>Dur=3] --> E[E<br>Dur=5]
    B --> F[F<br>Dur=6]
    C[C<br>Dur=3] --> G[G<br>Dur=6]
    D --> H[H<br>Dur=7]
    E --> H
    G --> I[I<br>Dur=8]
    H --> J[J<br>Dur=3]
    F --> J
    I --> J
    J --> Finish[Finish]

    classDef activity fill:#bbdefb,stroke:#1565c0,stroke-width:2px,color:black,radius:10px;
    class A,B,C,D,E,F,G,H,I,J activity