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


---

## 📚 References

**Amazon Web Services (AWS). (2024).** *Overview of Cloud Computing with AWS.*  
[https://aws.amazon.com/what-is-cloud-computing/](https://aws.amazon.com/what-is-cloud-computing/)  
> **Description:** This source provides foundational information about cloud computing models — **IaaS**, **PaaS**, and **SaaS** — and helps validate Aurora Ledger’s cloud service design. It supports the comparison between service models by explaining scalability, cost, and infrastructure flexibility from an industry leader’s perspective.

---

**Proxmox Server Solutions GmbH. (2024).** *Proxmox VE Documentation.*  
[https://www.proxmox.com/en/proxmox-ve](https://www.proxmox.com/en/proxmox-ve)  
> **Description:** The official documentation for Proxmox VE supports the project’s **PaaS implementation** choice. It describes how Proxmox’s virtualization technology enhances resource management, scalability, and secure multi-tenant deployment — all key components of Aurora Ledger’s architecture.

---

**TurnKey Linux. (2024).** *TurnKey GNU/Linux Appliance Library.*  
[https://www.turnkeylinux.org/](https://www.turnkeylinux.org/)  
> **Description:** This library provides pre-configured, lightweight Linux containers suitable for **SaaS environments**. It supports Aurora Ledger’s approach to rapid deployment, reduced maintenance, and streamlined scalability through container-based application delivery.

---

**National Institute of Standards and Technology (NIST). (2023).** *NIST SP 800-145: The NIST Definition of Cloud Computing.*  
[https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf)  
> **Description:** The NIST publication is the authoritative source defining cloud computing models and their characteristics. It reinforces Aurora Ledger’s technical framework and ensures that terminology and architectural references align with globally recognized standards.

---

**Wazuh, Inc. (2024).** *Wazuh Security Platform Documentation.*  
[https://documentation.wazuh.com/](https://documentation.wazuh.com/)  
> **Description:** Wazuh is an open-source SIEM and XDR platform. This documentation supports Aurora Ledger’s **security monitoring plan**, detailing features like intrusion detection, log analysis, and real-time alerting, which strengthen the project’s multi-layered cybersecurity strategy.

---

**Payment Card Industry Security Standards Council (PCI SSC). (2024).** *PCI DSS v4.0 Requirements and Security Assessment Procedures.*  
[https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/)  
> **Description:** PCI DSS v4.0 outlines data protection and encryption standards for financial institutions. It supports Aurora Ledger’s implementation of **AES-256 encryption**, **TLS 1.3**, and **multi-factor authentication**, ensuring compliance with financial data handling regulations.

---

**FINTRAC (Financial Transactions and Reports Analysis Centre of Canada). (2024).** *Compliance Program Guidance for Financial Institutions.*  
[https://www.fintrac-canafe.gc.ca/](https://www.fintrac-canafe.gc.ca/)  
> **Description:** FINTRAC provides Canadian compliance and anti-money laundering guidelines. It strengthens Aurora Ledger’s focus on **regulatory compliance automation**, confirming alignment with national standards for secure and lawful financial operations.

---

### 🧩 Summary

These references collectively enhance the credibility of Aurora Ledger’s project by:  
- Validating **technical architecture decisions** (AWS, Proxmox, TurnKey Linux).  
- Reinforcing **security and compliance standards** (PCI DSS, FINTRAC, Wazuh).  
- Ensuring **alignment with authoritative definitions** and global frameworks (NIST).  
- Supporting the **academic and professional legitimacy** of the cost and scalability analysis.



---

**Prepared by:**  
**Team 1 – Montreal, Canada**  
Daren Diaz, Conner Culpepper, Conner Tunnell, Hunter Hammontree, Wesley White
*CYBS 5293 – Launching a Cloud-Based IT Startup*



