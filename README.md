# Palo Alto ML-Powered Next-Generation Firewall (NGFW) Lab
<img src="https://i.imgur.com/cPrSqHW.png" height="80%" alt="PA Firewall" />
## Overview
This lab explores the **Palo Alto ML-Powered Next-Generation Firewall (NGFW) capabilities** through the **Ultimate Test Drive (UTD) 4.3 Workshop**. It provides hands-on experience with **PAN-OS 11.1** and demonstrates the firewall’s advanced security features, including **application control, threat prevention, SSL decryption, policy optimization, and AI-powered security**.

## Lab Setup
The lab environment includes:
- **Palo Alto Networks NGFW (VM-Series)**
- **Student Desktop (Windows 10)**
- **Mobile PC (GlobalProtect Client)**
- **Various cloud services and SaaS applications**

## Objectives
- **Granular application control** using App-ID and sanctioned SaaS enforcement
- **Implement security policies** for applications running on non-standard ports
- **Policy Optimizer** to migrate port-based rules to application-based rules
- **Decryption policies** to inspect SSL/TLS traffic
- **Post-Quantum Computing (PQC) security** analysis and blocking
- **WildFire AI-driven malware protection** and real-time threat analysis
- **Advanced URL filtering** with ML-Powered analysis
- **GlobalProtect VPN configuration** for secure remote access
- **User-ID enforcement** for application access control
- **AIOps and automated security insights** for firewall monitoring

## Configuration Steps

### **1. Granular Control of Applications & SaaS Enforcement**
- Configure App-ID to identify OpenAI and ChatGPT applications
- Allow sanctioned SaaS applications while blocking unsanctioned ones

### **2. Secure Applications on Non-Standard Ports**
- Create security policies that restrict applications to their default ports
- Verify traffic enforcement via log analysis

### **3. Policy Optimizer for Rule Migration**
- Identify port-based rules and migrate them to App-ID-based rules
- Implement **enhanced security with application-default enforcement**

### **4. SSL/TLS Decryption & Inspection**
- Create decryption policies to inspect encrypted traffic
- Block malicious downloads hidden within SSL traffic

### **5. Post-Quantum Computing (PQC) Security**
- Detect and log PQC cipher usage in TLS 1.3 sessions
- Enforce policies to block unauthorized PQC encryption

### **6. AI-Powered Malware & Threat Protection (WildFire)**
- Configure **real-time WildFire analysis** for unknown threats
- Enable **Inline ML-Powered malware prevention** to block evasive threats

### **7. Advanced URL Filtering**
- Implement URL filtering policies to block phishing, malware, and C2 traffic
- Use **Inline ML-powered URL filtering** to detect emerging threats

### **8. GlobalProtect VPN for Secure Remote Access**
- Configure GlobalProtect Portal and Gateway for remote users
- Enforce security policies based on user identity and device health

### **9. User-ID & Identity-Based Access Control**
- Restrict application access based on user identity
- Enforce policies to enable SSH access for specific user groups

### **10. AIOps for Firewall Monitoring & Security Insights**
- Use **AI-driven analytics** for security posture assessment
- Automate threat detection and incident response

## **Verification & Testing**
### **1. Verify Security Policies & Logs**
```shell
show security policies
show session all
show traffic log
```

### **2. Check Application Visibility & Threat Detection**
```shell
show application usage
show threat log
```

### **3. Test SSL Decryption & URL Filtering**
```shell
show session decrypted
show url filtering logs
```

## **Repository Structure**
```
├── configs/
│   ├── PAN_NGFW_Config.txt   # Configuration for Palo Alto NGFW
│   ├── GlobalProtect_Config.txt   # Configuration for GlobalProtect VPN
├── README.md          # Documentation
├── screenshots/       # Screenshots of verification outputs
└── topology.png       # Network diagram
```

## **Conclusion**
This lab demonstrates the power of **Palo Alto ML-Powered NGFW** in securing modern networks against advanced threats. It provides hands-on experience with **AI-driven security, policy enforcement, SSL decryption, VPN, and AIOps monitoring**, making it a valuable resource for network and security professionals.

---
**Author:** Travis Johnson  
**Company:** 10Digit Solutions LLC  
**GitHub Repository:** [Add link when available]
