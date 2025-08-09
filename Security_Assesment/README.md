### **2. Compliance Assessment**  
**Location:** `2-Compliance-Assessment/README.md`  
```markdown
# Windows & Linux Hardening for Regulatory Compliance  
**Author:** Steven Reji George  
**Date:** May 2025  

### 📜 **Project Scope**  
Conducted compliance assessments for *Fed F1rst Control Systems* against industry standards (CMMC, NIST). Hardened Windows 10 and macOS systems, and audited Linux servers.  

### ✅ **Windows 10 Hardening**  
1. **Critical Fixes**:  
   - Enabled Windows Defender Firewall.  
   - Enforced password policy (min. 12 chars + complexity).  
   - Disabled Remote Registry service.  
2. **Automation**: Configured auto-updates via GPO.  

### 🍏 **macOS Hardening**  
- Enabled FileVault encryption.  
- Restricted app installations to App Store only (Gatekeeper).  

### 🐧 **Linux Compliance**  
- Verified:  
  - AIDE installation (file integrity).  
  - Disabled insecure services (TFTP, CUPS).  
  - Enabled iptables (firewall).  

### 📊 **Evidence**  
- Screenshots of:  
  - Security Policy Editor (`gpedit.msc`).  
  - Linux command outputs (`systemctl is-enabled tftp`).  

### 🔗 **Policy Templates**  
- Included `Email Policy` and `BYOD Policy` PDFs.  

---
