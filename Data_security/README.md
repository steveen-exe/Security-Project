# Data Governance & Confidentiality for JFin Payments  
**Author:** Steven Reji George  

### 🏦 **Project Context**  
Secured sensitive financial data for *JFin Payments* (100K+ customers) through:  

### 🔐 **Data Classification**  
1. **Categories Defined**:  
   - **Confidential**: Customer PII, payment details (PCI-DSS).  
   - **Internal**: Employee records (GDPR).  
   - **Public**: Marketing materials.  

### 🛡️ **Security Controls**  
- **Disk Encryption**: RSA 2048-bit keys (screenshots provided).  
- **File Integrity**: SHA-256 hashing for critical files.  
- **VM Auditing**: Screenshots of:  
  - Password/Account Lockout Policies.  
  - Audit Policy configurations.  

### 📅 **Backup Strategy**  
| Data Type      | Backup Frequency | Retention Period |  
|----------------|------------------|------------------|  
| Confidential   | Real-time        | 1 year           |  
| Internal       | Daily            | 90 days          |  

### ⚖️ **Regulations Addressed**  
- GDPR, PCI-DSS, CCPA.  
