# Identity Access Flow (Evidence-Based)

This diagram shows how identity is structured and how access is granted and proven.

```mermaid
flowchart LR
  U[Users] --> OU[OU Structure]
  OU --> G[Security Groups]
  G --> A[Resource / Role Access]
  A --> E[Evidence Pack (Screenshots/Logs)]

### 4) Commit it
- Scroll down
- Add a commit message like: **Add identity access flow diagram**
- Click **Commit new file**

---

## Add it to your README (so recruiters see it)

### 5) Open `README.md`
- Click `README.md` → click the **pencil icon** to edit

### 6) Add this small section anywhere near your screenshots/artifacts
```md
## Artifacts
- Identity Access Flow Diagram: docs/identity-access-flow.md
- Evidence Pack: images/slide1-ou-structure.png, images/slide2-rbac-assignment.png, images/slide3-rbac-enforcement.png

