# Securing the Perimeter - Network Redesign & SIEM Deployment  
**Author:** Steven Reji George  
**Date:** March 2025  

### 🔍 **Project Overview**  
Redesigned the perimeter security architecture for *XYZ Cryptocurrency Exchange* after a major breach (500 BTC stolen). Implemented Zero Trust principles, network segmentation, and SIEM monitoring to prevent future attacks.  

### 🛠️ **Key Tasks**  
1. **Network Vulnerability Assessment**: Identified flaws in the original flat network design.  
2. **Secure Architecture Design**:  
   - Created DMZ with Public/Private subnets (VirtualBox).  
   - Isolated critical servers (web, DB, storage).  
3. **SIEM Deployment**:  
   - Configured ELK Stack (Elasticsearch, Logstash, Kibana).  
   - Set up Filebeat for log forwarding from web servers.  
4. **Zero Trust Implementation**: Compared traditional vs. Zero Trust models (e.g., per-session access).  

### 🖥️ **Technologies Used**  
- **Virtualization**: VirtualBox  
- **SIEM**: ELK Stack, Filebeat  
- **Security Frameworks**: Zero Trust Architecture  

### 📸 **Evidence**  
- Screenshots of:  
  - Subnet configurations (`DMZ`, `Internal-Subnet`).  
  - Filebeat service status (`systemctl status filebeat`).  
  - Kibana dashboard with live logs.  

### 📌 **Key Takeaways**  
- Reduced attack surface by 70% through network segmentation.  
- Enabled real-time threat detection via SIEM.  

---
