<div align="center">

# 🚀 Power Platform ALM Pipelines

**Automated build, test, and deployment pipelines for Power Platform solutions.**

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white)
![Power Platform](https://img.shields.io/badge/Power_Platform-742774?style=for-the-badge&logo=powerapps&logoColor=white)
![Status](https://img.shields.io/badge/Status-Growing-success?style=for-the-badge)

</div>

---

## ✨ What's Inside

| 📁 Folder | 📝 Contents |
|---|---|
| `github-actions/` | Workflows for export, import, and deploy |
| `azure-devops/` | YAML pipelines using Power Platform Build Tools |
| `docs/` | ALM guides, environment strategy, diagrams |

## 🔄 Deployment Flow

```mermaid
flowchart LR
    A[Dev: unmanaged] --> B[Export and unpack]
    B --> C[Commit to Git]
    C --> D[Build: managed solution]
    D --> E[Test]
    E --> F[Prod]
```

## 🧭 Core Practices

- 📦 Develop **unmanaged** in Dev, deploy **managed** to Test and Prod
- 🔐 Use **service principals**, never personal accounts
- ⚙️ Use **environment variables** and **connection references**
- 🧪 Gate Prod behind approvals

## 🗺️ Roadmap

- [x] Create repository
- [ ] Solution export and unpack workflow
- [ ] Build managed solution workflow
- [ ] Dev → Test → Prod deployment pipeline
- [ ] Environment variables and connection references guide
- [ ] Approval gates for Prod

> 🔒 All pipelines are sanitized: no secrets, tenant IDs, or client data.

---

<div align="center">

Built by **[Bharadwaj Vemula](https://github.com/bharadwaj-vemula)** · Microsoft Power Platform Developer

</div>
