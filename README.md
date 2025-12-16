# Active Directory Home Lab  
A hands-on identity management lab demonstrating user provisioning, Group Policy, MFA concepts, and core administrative workflows using Windows Server and Active Directory.

---

##  Overview  
This project recreates a small enterprise identity environment using a Windows Server domain controller and a Windows 10 client. It demonstrates how identity is created, managed, secured, and controlled in a real IT environment — similar to the workflows used in municipal and enterprise IT.

This lab reflects real experience from my IT internship, including user lifecycle management, MFA enforcement, and Zero Trust-aligned identity practices.

---

## Lab Architecture  
**Components:**
- Windows Server 2022 (Domain Controller)
- Windows 10 Client VM
- Active Directory Domain Services (AD DS)
- Organizational Units (OUs)
- Group Policy Objects (GPOs)
- User & Group Management
- MFA Conceptual Integration (Okta Verify / Azure AD)

**Network Setup:**
- Internal NAT network  
- Static IP for Domain Controller  
- DHCP for client machine  

---

##  dentity & Access Management Tasks  
### **1. Installed and configured Active Directory Domain Services**  
- Promoted server to Domain Controller  
- Created domain: `lab.local`  
- Configured DNS and domain trust settings  

### **2. Built Organizational Unit (OU) structure**  
- `Users`  
- `Admins`  
- `IT`  
- `HR`  
- `Workstations`  

### **3. Created user accounts and security groups**  
Examples:
- `jdoe` – Standard user  
- `asmith` – HR user  
- `gadmin` – IT admin  

Security groups:
- `HR-Group`  
- `IT-Admins`  
- `All-Employees`  

### **4. Implemented Group Policy Objects (GPOs)**  
- Password policy (complexity, expiration)  
- Account lockout policy  
- Desktop restrictions  
- Software installation policy  
- Login banner for security compliance  

---

## MFA & Zero Trust Concepts  
While MFA cannot be fully implemented inside a local AD-only lab, this project demonstrates:

### **How MFA works in enterprise identity**  
- Okta Verify / Microsoft Authenticator  
- Push notifications  
- Time-based one-time passwords (TOTP)  

### **Where MFA fits in the identity workflow**  
- Login → Authentication → MFA challenge → Access granted  

### **Zero Trust principles applied**  
- Never trust, always verify  
- Least-privilege access  
- Identity as the security perimeter  

---

## Troubleshooting & Administration  
Documented common admin tasks:
- Resetting passwords  
- Unlocking accounts  
- Forcing Group Policy updates  
- Joining devices to the domain  
- Checking replication  
- Reviewing event logs  

---

## Screenshots (Add These Later)  
Suggested screenshots to include:
- Server Manager AD DS installation  
- OU structure  
- User creation  
- GPO editor  
- Client machine domain join  

---

## Skills Demonstrated  
- Active Directory administration  
- Identity lifecycle management  
- Group Policy configuration  
- Windows Server management  
- Zero Trust & MFA concepts  
- Troubleshooting & documentation  

---

## Future Enhancements  
- Add Azure AD Connect  
- Add Okta integration demo  
- Add PowerShell automation scripts  
- Add Intune/Workspace ONE hybrid join example  

---

## Author  
**Gurveer**  
IT Support Intern | Managment Information Systems | Identity & Access | Cloud & Cybersecurity
