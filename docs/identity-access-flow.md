# Identity Access Flow (Evidence-Based)

This diagram shows how identity is structured and how access is granted and proven.

```mermaid
flowchart LR
  U[Users] --> OU[OU Structure]
  OU --> G[Security Groups]
  G --> A[Resource / Role Access]
  A --> E[Evidence Pack (Screenshots/Logs)]
