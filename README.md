# 🔐 **SOC Analyst Lab Project: TCP SYN Port Scan Investigation Using Wireshark Packet Analysis**

![Wireshark Logo](https://www.wireshark.org/assets/theme-2015/images/wslogo.svg)
![Nmap Logo](https://nmap.org/images/sitelogo.png)

## 📌 **Project Overview**

A hands-on cybersecurity lab project demonstrating **real-world SOC analyst skills** through detection and analysis of a TCP SYN port scan using **Wireshark**. This project simulates an actual security incident in a controlled environment, providing practical experience in network forensics, threat detection, and incident reporting.

## 🎯 **Project Objectives**

- ✅ **Simulate** a real-world reconnaissance attack (Nmap SYN Scan)
- ✅ **Detect** malicious network activity using Wireshark
- ✅ **Analyze** packet-level evidence of the attack
- ✅ **Document** findings in a professional incident report format
- ✅ **Develop** practical SOC skills for job readiness

## 🛠️ **Technologies & Tools Used**

| Tool | Purpose | Version |
|------|---------|---------|
| **Wireshark** | Network protocol analyzer | 4.2.0+ |
| **Nmap** | Network scanning (attacker tool) | 7.94+ |
| **VirtualBox/VMware** | Virtualization platform | Latest |
| **Kali Linux** | Attacker machine | 2024.1+ |
| **metasploitable Server** | Victim machine | 22.04 LTS |

## 🚀 **Getting Started**

### **Prerequisites**
- Basic understanding of networking (TCP/IP, ports, protocols)
- Virtualization software (VMware, VirtualBox, or Hyper-V)
- 8GB+ RAM recommended for running multiple VMs

### **Quick Start Guide**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/pathanfarhana/Wireshark-Network-Attack-Detection.git
   cd Wireshark-Network-Attack-Detection
   ```

2. **Set Up Your Lab Environment:**
   - Follow the [Lab Setup Guide](Documentation/Lab_Setup_Guide.md)
   - Configure three VMs with the following IPs:
     - Attacker: `192.168.0.179` (Kali Linux)
     - Victim: `192.168.0.170` (Ubuntu Server)
     - Monitor: `192.168.0.1` (Windows/Linux with Wireshark)

3. **Execute the Attack:**
   ```bash
   # On Kali Linux machine
   nmap -sS -p 1-1000 192.168.0.170
   ```

4. **Capture and Analyze Traffic:**
   - Start Wireshark on monitoring machine
   - Apply filter: `tcp.flags.syn == 1 and tcp.flags.ack == 0`
   - Analyze the captured packets

## 🔍 **Key Learning Outcomes**

### **Technical Skills Developed:**
1. **Network Traffic Analysis**
   - Packet capture and filtering
   - Protocol dissection (TCP/IP)
   - Anomaly detection in network flows

2. **Threat Detection**
   - Recognizing scan patterns
   - Identifying malicious behavior
   - Extracting Indicators of Compromise (IOCs)

3. **Forensic Analysis**
   - Evidence preservation
   - Timeline reconstruction
   - Attack vector identification

4. **Security Operations**
   - Incident response procedures
   - SOC report writing
   - Tool proficiency (Wireshark, Nmap)

### **Soft Skills Demonstrated:**
- Technical documentation
- Problem-solving methodology
- Attention to detail
- Clear communication of complex findings

## 📊 **Project Highlights**

### **What Makes This Project Valuable?**

| Feature | Benefit for Job Seekers |
|---------|-------------------------|
| **Real Attack Simulation** | Shows practical, not just theoretical knowledge |
| **Complete Documentation** | Demonstrates professional reporting skills |
| **Hands-on Tool Usage** | Proves proficiency with industry-standard tools |
| **End-to-End Process** | Shows understanding of full incident lifecycle |
| **Portfolio-Ready Output** | Provides tangible evidence of skills |

### **Skills Validated by This Project:**
- ✅ **Security+ Domain 1.0:** Threats, Attacks, and Vulnerabilities
- ✅ **Security+ Domain 4.0:** Architecture and Design
- ✅ **CySA+ Domain 2.0:** Vulnerability Management
- ✅ **NIST CSF:** Identify, Protect, Detect, Respond

## 📈 **Career Application**

### **For Entry-Level SOC Positions:**
This project demonstrates you can:
- Triage security alerts
- Perform initial incident investigation
- Use monitoring tools effectively
- Communicate findings to team members
- Follow established procedures

## 📚 **Learning Resources**

### **Reference Materials:**
- [Wireshark Official Documentation](https://www.wireshark.org/docs/)
- [Nmap Network Scanning Book](https://nmap.org/book/)
- [SANS Incident Response Posters](https://www.sans.org/posters/)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)

## 🤝 **Contributing**

This is a learning project! Feel free to:
- Fork and modify for your own learning
- Add additional attack scenarios
- Improve documentation
- Share your own analysis techniques

## 📄 **License**

This project is licensed under the MIT License - see the LICENSE file for details.

**Educational Use Only:** All techniques are demonstrated in controlled lab environments for educational purposes.

## 🌟 **Star This Project**

If you found this project helpful for your SOC analyst journey, please give it a star! ⭐

## 📞 **Connect With Me**

- **LinkedIn:** https://www.linkedin.com/in/pathan-farhana-659b95247
- **GitHub:** https://github.com/pathanfarhana

---

## 🏆 **Portfolio Ready**

This project is designed to be **interview-ready** and **portfolio-worthy**. Include it in your:
- GitHub portfolio
- Personal website
- LinkedIn projects section
- Resume as a "hands-on lab project"

**Remember:** Employers value practical skills. This project shows you can *do* the work, not just *talk* about it.

---

### ⏱️ **Time to Complete:** 4-8 hours
### **Difficulty Level:** Beginner to Intermediate
### **Target Audience:** Aspiring SOC Analysts, Cybersecurity Students, Career Changers

**Ready to start?** Check out the [Lab Setup Guide](Documentation/Lab_Setup_Guide.md)!

---

*"In cybersecurity, theory is important, but practice is everything. This project bridges that gap."*
