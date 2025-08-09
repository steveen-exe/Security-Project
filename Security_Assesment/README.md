# Windows & Linux Hardening for Regulatory Compliance  
**Author:** Steven Reji George  
**Date:** May 2025  

## 📜 Project Overview  
Conducted comprehensive compliance assessments and hardening for *Fed F1rst Control Systems* against industry standards (CMMC, NIST).  

## 🖥️ **Windows 10 Hardening**  
### Critical Fixes Implemented:  
✅ **Patch Management**  
- Enabled automatic Windows Updates  
- Installed missing security patches  

✅ **Security Policies**  
- Enforced strong password policy (12+ chars, complexity)  
```powershell
# Sample GPO command
Set-ADDefaultDomainPasswordPolicy -Identity domain.com -MinPasswordLength 12 -ComplexityEnabled $true
