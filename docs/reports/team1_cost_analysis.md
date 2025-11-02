# Team 1 – Montreal, Canada  
## Cost Analysis Report  
**Project:** Launching a Cloud-Based IT Startup  
**Startup:** Aurora Ledger – Fintech Cloud Platform  
**Date:** November 9, 2025  

---

### 1. Introduction
Aurora Ledger is a Fintech startup headquartered in Montreal, Canada, providing cloud-based solutions for secure financial data processing, compliance automation, and API-driven integrations.  

The team’s primary goal is to design and evaluate two cloud deployment models — **Platform as a Service (PaaS)** and **Software as a Service (SaaS)** — to determine the most cost-efficient, scalable, and secure architecture for a financial data platform.

---

### 2. Service Model Overview

| Service Model | Description | Tools Used |
|----------------|--------------|-------------|
| **PaaS (Platform as a Service)** | Aurora Ledger’s proprietary transaction engine and API layer are hosted on Proxmox VE virtual machines. Developers have control over the environment configuration and scalability. | Proxmox VE, Ubuntu Server, MySQL, Node.js |
| **SaaS (Software as a Service)** | A TurnKey Linux LXC container hosts a pre-built financial management platform with a user dashboard, analytics tools, and secure APIs. | TurnKey Linux, Docker, LocalStack (AWS simulation) |

---

### 3. Cost Components

#### **3.1 Compute Resources**
| Component | PaaS (Proxmox VE) | SaaS (TurnKey Linux) |
|------------|-------------------|----------------------|
| vCPU / Memory | $0.05/hour per VM (2 vCPU, 4GB RAM) | $0.02/hour per container |
| Number of Instances | 3 (Web, DB, API) | 2 (App, DB) |
| Estimated Monthly Cost | ≈ $110 | ≈ $70 |

#### **3.2 Storage and Backup**
| Category | PaaS | SaaS |
|-----------|------|------|
| Object Storage | $0.023/GB (S3 equivalent) | Included (limited) |
| Database Storage | $0.10/GB | $0.05/GB |
| Snapshot Backup | $0.015/GB | $0.01/GB |
| Estimated Monthly Storage Cost | ≈ $45 | ≈ $25 |

#### **3.3 Network and Bandwidth**
| Category | PaaS | SaaS |
|-----------|------|------|
| Data Transfer (in/out) | $0.09/GB | $0.07/GB |
| Estimated Monthly Usage | 500GB | 500GB |
| Monthly Cost | ≈ $45 | ≈ $35 |

#### **3.4 Licensing and Maintenance**
| Factor | PaaS | SaaS |
|---------|------|------|
| Software Licensing | Open-source stack | Pre-licensed container |
| Maintenance Overhead | High (team-managed) | Low (provider-managed) |
| Monthly Cost (Labor Estimate) | ≈ $200 | ≈ $80 |

---

### 4. Cost Summary

| Category | PaaS | SaaS |
|-----------|------|------|
| Compute | $110 | $70 |
| Storage | $45 | $25 |
| Bandwidth | $45 | $35 |
| Maintenance | $200 | $80 |
| **Total (Est. Monthly)** | **$400** | **$210** |

**Result:**  
The **SaaS model** offers roughly **48% cost savings** compared to the PaaS setup while providing built-in maintenance and faster deployment. However, the **PaaS model** provides greater customization and flexibility for Aurora Ledger’s in-hous
