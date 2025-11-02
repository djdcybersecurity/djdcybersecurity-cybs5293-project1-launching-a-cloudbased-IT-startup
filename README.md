# CYBS 5293 – Project 1: Launching a Cloud-Based IT Startup  
**Team 1 – Montreal, Canada**  
**Startup:** Aurora Ledger  
**Instructor:** Dr. Sungbo Jung
**Date:** November 2025  

---

## 🏢 Company Overview
**Aurora Ledger** is a Canadian Fintech cloud startup headquartered in **Montreal, QC**, specializing in secure financial data processing, compliance automation, and API-based banking integrations.  
Our mission is to enable small and medium-sized financial institutions to modernize their operations through cloud-native, scalable, and regulatory-compliant solutions.

---

## 🎯 Project Goals
1. **Design a secure and scalable cloud architecture** using modern service models: **Bare Metal, IaaS, PaaS, and SaaS**.  
2. **Compare costs** between at least two models to determine efficiency and scalability.  
3. **Develop a comprehensive security strategy** aligned with best practices for the chosen models.

---

## 💼 Business Objective
Aurora Ledger falls under the **“Free to Choose”** business objective category.  
Our focus: deliver a **Fintech Cloud Platform** for secure financial data processing and compliance automation through both **PaaS** and **SaaS** implementations.

---

## ☁️ Cloud Service Models

| Service Model | Description | Example Tools / Environment |
|---------------|--------------|-----------------------------|
| **PaaS (Platform as a Service)** | Aurora Ledger’s transaction engine and API gateway are deployed on **Proxmox VE VMs** running Ubuntu Server, MySQL, and Node.js. This setup provides flexibility, scalability, and developer control. | Proxmox VE, Ubuntu Server, MySQL, Node.js |
| **SaaS (Software as a Service)** | A **TurnKey Linux LXC container** hosts a pre-built financial management suite that clients access via secure web dashboards and APIs. | TurnKey Linux, Docker, LocalStack (AWS simulation) |
| **IaaS (Infrastructure as a Service)** | Future expansion may involve virtualized infrastructure such as AWS EC2 instances or Azure VMs to provide elastic scaling for analytics workloads. | AWS EC2, S3, VPC |
| **Bare Metal** | Dedicated physical servers could be used in high-compliance environments requiring full isolation and direct hardware control. | On-premise Dell/HP servers + Proxmox bare-metal nodes |

---

## 🔒 Security Strategy
Aurora Ledger implements a **multi-layered cloud security framework**:
- **IAM & MFA:** Role-based access and multi-factor authentication for all accounts.  
- **Data Protection:** AES-256 encryption at rest + TLS 1.3 in transit.  
- **Network Security:** Segmented VPCs, firewalls, and secure API gateways.  
- **Monitoring & Logging:** Centralized log analysis (Wazuh) and intrusion detection.  
- **Compliance:** Aligned with PCI DSS, FINTRAC, and SOC 2 Type II standards.

---

## 💰 Cost Analysis Summary

| Category | PaaS | SaaS |
|-----------|------|------|
| Compute | $110 | $70 |
| Storage | $45 | $25 |
| Bandwidth | $45 | $35 |
| Maintenance / Labor | $200 | $80 |
| **Total (Est. Monthly)** | **$400** | **$210** |

**Result:** The SaaS model provides roughly **48% cost savings**, while PaaS offers greater flexibility and long-term scalability.

---

## ⚙️ Scalability and Expansion Plan
- **Short-Term:** Launch SaaS prototype using TurnKey Linux containers on LocalStack.  
- **Mid-Term:** Deploy hybrid model (SaaS + custom PaaS API engine).  
- **Long-Term:** Integrate IaaS for global scalability and compliance-driven Bare Metal nodes.

---

## 🧱 Architecture Overview
![Aurora Ledger Cloud Architecture](assets/diagrams/aurora_ledger_cloud_architecture.png)

### Architecture Highlights
- Dual-layer design separating **PaaS** and **SaaS** components.  
- Centralized encrypted data storage and object storage backend.  
- IAM authentication gateway for all API access.  
- AWS LocalStack integration for testing and deployment simulation.  
- Monitoring and alerting for compliance and uptime.

---

## 🧾 Deliverables

| Deliverable | File Path | Status |
|--------------|-----------|--------|
| **Concept Overview Document** | `docs/team1_concept_overview.md` | ✅ Completed |
| **Meeting Minutes** | `docs/meeting_minutes/team1_montreal_meeting1.md` | ✅ Completed |
| **Cost Analysis Report** | `docs/reports/team1_cost_analysis.md` | ✅ Completed |
| **Cloud Architecture Diagram** | `assets/diagrams/aurora_ledger_cloud_architecture.png` | ✅ Completed |

---

## 📈 Progress Status
| Category | Completion |
|-----------|-------------|
| Meeting Minutes | ✅ 100% |
| Cost Analysis Report | ✅ 100% |
| Cloud Model Coverage (Bare Metal + IaaS added) | ✅ 100% |
| Security & Architecture | ✅ 100% |
| Repo Organization / Documentation | ✅ 100% |

**Overall Project Completion:** ✅ **100% – Ready for Submission**

---

**Prepared by:**  
**Team 1 – Montreal, Canada**  
Daren (Lead / Systems Architect) • [Add other team members]  
*CYBS 5293 – Launching a Cloud-Based IT Startup*

