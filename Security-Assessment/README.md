
# Security Assessment Framework  
**Steven Reji George** | *Security Analyst | CBS-041*  
[![OWASP](https://img.shields.io/badge/OWASP%20ZAP-Enabled-red)](https://owasp.org/www-project-zap/) 
[![NIST](https://img.shields.io/badge/NIST%20SP-800--115-compliant-blue)](https://csrc.nist.gov/publications/detail/sp/800-115/final)

## 🔍 Assessment Overview
**Objective**: Identify and remediate vulnerabilities across:  
- Network infrastructure  
- Application security  
- Compliance controls  
- Data protection mechanisms  

**Methodology**:  
```mermaid
graph TD
    A[Reconnaissance] --> B[Vulnerability Scanning]
    B --> C[Penetration Testing]
    C --> D[Compliance Audit]
    D --> E[Remediation Plan]

## 🛡️ Key Assessment Areas

| Area              | Tool       | Target           | Critical Findings     |
|-------------------|------------|------------------|-----------------------|
| Network Security  | Nmap       | 192.168.1.0/24   | 3 open RDP ports      |
|                   | Wireshark  | DMZ traffic      | Unencrypted FTP       |
|                   | Nessus     | All hosts        | CVE-2023-1234         |

---

## 2. Compliance Checks

| Standard  | Controls Assessed | Pass Rate |
|-----------|-------------------|-----------|
| PCI-DSS   | 12/12              | 92%       |
| GDPR      | 8/10               | 80%       |

---

## 3. 📊 Risk Matrix

| Vulnerability         | CVSS | Impact   | Likelihood | Status         |
|-----------------------|------|----------|------------|----------------|
| Unpatched WS2019      | 9.1  | Critical | High       | 🟡 Mitigating  |
| Weak Password Policy  | 7.5  | High     | Medium     | 🔴 Open        |

---

## 4. 🛠️ Remediation Roadmap

### Immediate Actions (0–7 days)
- Patch critical CVEs (`KB5034441`)
- Disable legacy protocols (FTP, SMBv1)

### Mid-Term (8–30 days)
```powershell
# Enforce LAPS for local admin passwords
Set-AdmfPasswordPolicy -Identity "Default Domain Policy" -MinPasswordLength 14
