# Compliance Assessment & System Hardening  
**Steven Reji George** | *Completed: May 2025*  
[![Compliance](https://img.shields.io/badge/CMMC-Level%203-blue)](https://www.acq.osd.mil/cmmc/) 
[![NIST](https://img.shields.io/badge/NIST%20SP-800--171-compliant-green)](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)

## 📋 Project Overview
Conducted enterprise-wide security hardening for **Fed F1rst Control Systems**, achieving:
- 100% compliance on 14 critical Windows 10 controls
- 94% compliance on 16 Linux CIS benchmarks
- Developed enforceable BYOD and email security policies

## 🖥️ System Hardening Matrix

### Windows 10 Hardening
| Control | Implementation | Verification | Status |
|---------|---------------|-------------|--------|
| Patch Management | Configured auto-updates | `Get-WindowsUpdateLog` | ✅ |
| BitLocker | Enabled full-disk encryption | `manage-bde -status C:` | ✅ |
| Password Policy | 12+ chars, complexity | `secedit /export /cfg gpresult.txt` | ✅ |
| Firewall | Enabled all profiles | `netsh advfirewall show allprofiles` | ✅ |

### macOS Hardening
```bash
# 1. Enable FileVault
sudo fdesetup enable

# 2. Configure Firewall
sudo /usr/libexec/ApplicationFirewall/socketfilterfw \
  --setglobalstate on \
  --setstealthmode on

Linux Hardening (CIS v2.0.0)
bash
# Verify critical controls
sudo systemctl is-enabled tftp.socket  # Should return 'disabled'
sudo aide --check                      # File integrity check
sudo grep '^max_log_file' /etc/audit/auditd.conf  # Log rotation config
📜 Security Policies
Email Policy Highlights
Authentication: Enforced SPF/DKIM/DMARC

Training: Mandatory phishing simulation quarterly

Reporting: 24-hour incident response SLA


