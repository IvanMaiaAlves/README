## 🧑‍💻 Developer Profile & Philosophy

As an Identity & Access Management (IAM) and Security Engineer, my approach to development is rooted in three core principles: **Automation, Security-by-Design, and Operational Efficiency**. 

I build tools that bridge the gap between abstract security policies and concrete, automated enforcement. Instead of relying on manual checklists, I write code to treat infrastructure and compliance as data. This portfolio showcases production-ready logic built to solve real-world security bottlenecks, eliminate human error, and accelerate incident response.

---

## 🎯 How This Portfolio is Used Genuinely in the Enterprise

These projects are not just academic exercises; they replicate the core logic used by modern enterprise platforms (such as SailPoint, Saviynt, and SIEM tools) to safeguard cloud and on-premise environments:

# IAM & Cybersecurity Engineering Portfolio 🛡️

This repository centralizes a collection of automated tools, scripts, and architectures designed for **Identity and Access Management (IAM)**, **Identity Governance and Administration (IGA)**, **SecOps**, and **Privilege Management**.

The primary goal of this portfolio is to demonstrate the practical, scalable application of modern security pillars: Governance, Incident Response, Least Privilege, and Compliance Automation.

---

## 📁 Repository Structure (10-Project Roadmap)

### 📊 Phase 1: Governance, Logs & Base Automation
#### 1. `01_identity_governance` (IGA Audit Automation)
* **The Idea:** Automate access reviews by reconciling HR databases with cloud infrastructure data.
* **Features:** Detection of active accounts belonging to terminated employees (*Ghost Accounts*), unrotated access keys (*Stale Keys*), and conflicting high-privilege roles (*Segregation of Duties - SoD*).
* **Stack:** Python, Pandas, JSON, CSV.

#### 2. `02_auth_monitor` (Security Log Analysis & Brute Force Detection)
* **The Idea:** A lightweight SIEM-like log parser built for active monitoring and immediate threat containment.
* **Features:** Threshold-based brute force attack detection (`LOGIN_FAILED`) and automated IP extraction for firewall blocking rules.
* **Stack:** Native Python (File I/O, Exception Handling).

#### 3. `03_rbac_matrix_simulator` (Role-Based Access Control Engine)
* **The Idea:** A provisioning engine built strictly around the Principle of Least Privilege.
* **Features:** Map corporate roles via JSON matrices and mathematically assign exact permissions (AWS/Active Directory) based on job titles.
* **Stack:** Python, JSON Structuring.

---

### 🛡️ Phase 2: Privilege Management & Non-Human Identities (Coming Soon)
#### 4. `04_pam_just_in_time` (Privileged Access Management Simulator)
* **The Idea:** Simulate a modern credential vault/PAM tool with Just-In-Time (JIT) elevation and automated revocation.
* **Features:** Ephemeral credential generation with hardcoded Time-To-Live (TTL).

#### 5. `05_machine_identity_auditor` (Secret & Certificate Management)
* **The Idea:** Audit non-human identities, service accounts, API keys, and expiring certificates.
* **Features:** Automated configuration scan to mitigate secrets exposure and credential leaks.

#### 6. `06_abac_policy_validator` (Attribute-Based Access Control Policy Engine)
* **The Idea:** Validate dynamic access contexts based on environmental variables (business hours, geolocation, device compliance).

---

### 🚀 Phase 3: Cloud IAM, APIs & Advanced Governance (Coming Soon)
#### 7. `07_aws_iam_least_privilege_analyzer` (Cloud Security Assessment)
* **The Idea:** Analyze cloud IAM policies (AWS/Azure) to flag over-privileged identities and dangerous wildcard permissions (e.g., `"*.*"`).

#### 8. `08_oauth_api_gateway_monitor` (API Security)
* **The Idea:** Validate and monitor OAuth2 tokens and permission scopes across corporate APIs.

#### 9. `09_ciem_entitlement_reconciler` (Cloud Infrastructure Entitlement Management)
* **The Idea:** Map cross-cloud permissions to identify privilege creep across multi-tenant cloud environments.

#### 10. `10_iam_audit_dashboard` (Security Governance Metrics)
* **The Idea:** Consolidate audit artifacts into data metrics, generating high-level risk and IAM compliance KPIs.

---

## 🚀 How to Run Active Projects

### Prerequisites
Install the required libraries:
```bash
pip install pandas openpyxl
