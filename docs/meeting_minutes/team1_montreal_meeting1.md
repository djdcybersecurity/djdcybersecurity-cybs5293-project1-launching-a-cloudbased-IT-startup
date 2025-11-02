# Team 1 – Montreal, Canada  
## Cloud Service Usage Plan – Meeting Minutes  
**Date:** November 2, 2025  
**Meeting Duration:** 1 hour  
**Meeting Method:** Microsoft Teams  

---

### 🧑‍💻 Attendees
- Daren (Project Lead / Systems Architect)  
- [Add other team members here]  

---

### 🏢 Overview of the Startup
**Startup Name:** Aurora Ledger  
**Headquarters:** Montreal, Canada  
**Business Type:** Fintech Cloud Platform  

Aurora Ledger focuses on providing secure financial data processing, compliance automation, and API-based banking tools for small and medium-sized financial institutions. The company leverages Canada’s strong data privacy framework and regional data centers for cloud service reliability.

---

### 🎯 Discussion Topics

#### 1. Business Objective
The team agreed to design a **cloud-based Fintech service** that offers:
- Encrypted financial data storage and analytics.
- Automated compliance verification (FINTRAC, PCI DSS).
- Developer-friendly API access for integration with banking systems.

#### 2. Service Models
The team will evaluate two cloud service models:

| Model | Description | Tools/Environment |
|--------|--------------|------------------|
| **PaaS (Platform as a Service)** | Build and host the Aurora Ledger transaction engine using Proxmox VE virtual machines. | Proxmox VE, Ubuntu Server, MySQL, Node.js |
| **SaaS (Software as a Service)** | Deploy a pre-built financial management suite using a TurnKey Linux LXC container. | TurnKey Linux, Docker, LocalStack (for AWS simulation) |

#### 3. Cloud Architecture Goals
- Ensure **data encryption** in transit and at rest.  
- Implement **load balancing** and **redundancy** for high availability.  
- Enable **automated backup & recovery**.  
- Maintain **compliance** with Canadian and U.S. financial standards.

#### 4. Security Strategy (Initial Plan)
- **IAM**: Role-based access and MFA for all users.  
- **Network Security**: Virtual Private Cloud (VPC) segmentation and firewalls.  
- **Data Security**: End-to-end encryption and secure object storage.  
- **Monitoring**: Intrusion detection and log analysis.  
- **Testing**: LocalStack environment for simulated AWS security validation.

---

### 💰 Cost Considerations (to be analyzed in detail)
- Estimate Proxmox VM hosting vs. TurnKey SaaS container deployment.  
- Factor in compute, bandwidth, and object storage.  
- Compare scalability costs between models.  

---

### ✅ Action Items
| Task | Assigned To | Due Date |
|------|--------------|----------|
| Draft concept overview document | Daren | ✅ Completed |
| Begin PaaS and SaaS environment setup | Team 1 | Nov 4, 2025 |
| Complete cost analysis report | Daren | Nov 9, 2025 |
| Review final deliverables | All team members | Nov 10, 2025 |

---

### 🗓️ Next Meeting
**Date:** November 6, 2025  
**Agenda:**  
- Review cost analysis progress  
- Confirm architecture diagram  
- Prepare for submission phase  

---

**Prepared by:**  
Daren – Project Lead  
**CYBS 5293 – Project 1: Launching a Cloud-Based IT Startup**
