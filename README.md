# 🛡️ Cybersecurity Audit Report: Botium Toys

## 📊 Executive Summary
* **Target System / Organization:** Botium Toys
* **Auditor:** Frederick D. Nixon III
* **Scope & Context:** Review of IT manager’s scope, goals, and risk assessment report, paired with an internal security controls and compliance audit.
* **Overall Risk Rating:** 🔴 **HIGH RISK** (Critical foundational controls are missing)

---

## 🔍 Audit Findings & Checklists

<details>
<summary><b>🛠️ 1. Security Controls Assessment</b></summary>

### Controls Checklist
- [ ] **Least Privilege** | *Type: Preventative* | ❌ **NO**
- [ ] **Disaster Recovery Plans** | *Type: Corrective* | ❌ **NO**
- [ ] **Password Policies** | *Type: Preventative* | ❌ **NO**
- [ ] **Separation of Duties** | *Type: Preventative* | ❌ **NO**
- [ ] **Firewall** | *Type: Preventative* |  **YES**
- [ ] **Intrusion Detection System (IDS)** | *Type: Detective* | ❌ **NO**
- [ ] **Backups** | *Type: Corrective* | ❌ **NO**
- [ ] **Antivirus Software** | *Type: Preventative* |  **YES**
- [ ] **Manual Monitoring, Maintenance & Intervention (Legacy Systems)** | *Type: Preventative* | ❌ **NO** *(Not complete)*
- [ ] **Encryption** | *Type: Deterrent* | ❌ **NO**
- [ ] **Password Management System** | *Type: Preventative* | ❌ **NO**
- [ ] **Locks (Offices, Storefront, Warehouse)** | *Type: Detective/Deterrent/Preventative* |  **YES**
- [ ] **Closed-Circuit Television (CCTV) Surveillance** | *Type: Preventative/Detective* |  **YES**
- [ ] **Fire Detection/Prevention (Fire Alarm, Sprinkler)** | *Type: Detective/Preventative* |  **YES**

### 📝 Control Gaps & Observations
* Physical security (locks, CCTV, fire tools) and basic perimeter network security (firewall, antivirus) are operational.
* Logical and administrative security measures are severely lacking across the board.
</details>

<details>
<summary><b>⚖️ 2. Regulatory Compliance Checklist</b></summary>

### 💳 Payment Card Industry Data Security Standard (PCI DSS)
* **Overall Adherence:** ❌ **NO**
- [ ] Only authorized users have access to customers’ credit card information. | *Access Control / Preventative* | ❌ **NO**
- [x] Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. |  **YES**
- [ ] Implement data encryption procedures to better secure credit card transaction touchpoints and data. | ❌ **NO**
- [ ] Adopt secure password management policies. | ❌ **NO**

### 🌍 General Data Protection Regulation (GDPR)
* **Overall Adherence:** ❌ **NO**
- [x] E.U. customers’ data is kept private/secured. |  **YES**
- [x] There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. |  **YES**
- [ ] Ensure data is properly classified and inventoried. | ❌ **NO**
- [ ] Enforce privacy policies, procedures, and processes to properly document and maintain data. | ❌ **NO**

### 🔒 System and Organizations Controls (SOC 1 / SOC 2)
* **Overall Adherence:** ❌ **NO**
- [ ] User access policies are established. | ❌ **NO**
- [ ] Sensitive data (PII/SPII) is confidential/private. | ❌ **NO**
- [ ] Data integrity ensures the data is consistent, complete, accurate, and has been validated. | ❌ **NO**
- [ ] Data is available to individuals authorized to access it. | ❌ **NO**
</details>

<details>
<summary><b>📝 3. Auditor Notes & Critical Findings</b></summary>

### Critical Vulnerability Summary
* **Identity & Access Management:** Least privilege, password policies, password management systems, and user access policies are completely non-existent. 
* **Data Exposure Risk:** While credit cards are stored securely, all employees have access to this information due to a complete lack of **separation of duty** policies.
* **Encryption Deficit:** No data encryption procedures are in place to secure sensitive information or transactional touchpoints.
* **Business Continuity Risk:** Disaster recovery plans and automated backups do not exist, putting the business at risk of permanent data loss.
* **Data Governance:** Data integrity framework has not been established; data classification and inventory protocols are missing.
</details>

---

## 🚀 Action Items & Remediation Plan

| ID | Required Action | Target Control / Compliance | Priority | Status |
| :--- | :--- | :--- | :--- | :--- |
| REM-01 | Enforce **Separation of Duties** & restrict credit card data access | PCI DSS / Access Control | 🔴 Critical | ⏳ Pending |
| REM-02 | Draft and enforce a formal **Password Policy** + deploy a password manager | PCI DSS / SOC | 🔴 Critical | ⏳ Pending |
| REM-03 | Implement data encryption for transactions and data-at-rest | PCI DSS / GDPR | 🔴 Critical | ⏳ Pending |
| REM-04 | Establish formal **User Access Policies** and least privilege models | SOC / IAM | 🟡 High | ⏳ Pending |
| REM-05 | Create **Disaster Recovery Plans** and activate automated data backups | Security Controls | 🟡 High | ⏳ Pending |
| REM-06 | Classify and inventory data; establish a data integrity validation process | GDPR / SOC | 🟢 Medium | ⏳ Pending |
