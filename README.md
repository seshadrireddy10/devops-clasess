# devops-clasess 

# 🚀 Azure DevOps Workflow Architecture

This document describes the core services of the Azure DevOps suite and details how data and processes flow across the ecosystem.

## 🗺️ Service Ecosystem

```text
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Azure Boards  │    │   Azure Repos    │    │ Azure Pipelines │
│                 │    │                  │    │                 │
│ • Plan features │────│ • Store code     │────│ • Build apps    │
│ • Track bugs    │    │ • Code reviews   │    │ • Run tests     │
│ • Manage sprints│    │ • Branch policies│    │ • Deploy code   │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│ Azure Test Plans│    │ Azure Artifacts  │    │   Dashboards    │
│                 │    │                  │    │                 │
│ • Test planning │    │ • Package feeds  │    │ • Project views │
│ • Manual testing│◄───│ • Version control│───►│ • Team metrics  │
│ • Test reporting│    │ • Dependency mgmt│    │ • Build status  │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

### 🔄 Process Lifecycle
**Flow:** Plan → Code → Build → Test → Deploy → Monitor → Repeat

---

## 🛠️ Core Components Breakdown

1. **Azure Boards:** Used for Agile planning, tracking work items, Kanban boards, and sprint planning.
2. **Azure Repos:** Provides private Git repositories with pull requests and advanced branch management.
3. **Azure Pipelines:** Cloud-hosted CI/CD automation pipelines that integrate with any platform.
4. **Azure Test Plans:** Provides browser-based test management solutions for exploratory and manual testing.
5. **Azure Artifacts:** Integrates package management (npm, NuGet, Maven, Python) directly into pipelines.
