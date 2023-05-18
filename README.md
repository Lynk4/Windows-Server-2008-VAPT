# Windows Server 2008 VAPT Report

REPORT BY - CHANDRA KANT BAURI
---

Target IP - 192.168.43.177

|    CRITICAL   | HIGH          | MEDIUM|
| ------------- |:-------------:| -----:|
|       3       |       1       |     1 |

***Host Information***

Netbios Name: WIN-KAVQ59H6PK1

MAC Address: XXXXXXXXXXX

OS: Microsoft Windows Server 2008 Enterprise Service Pack 1

Nmap Scan:


<img width="452" alt="image" src="https://github.com/Lynk4/Windows-Server-2008-VAPT/assets/44930131/4d1c030e-27b0-4ab4-b937-dfb96d8b727e">


---
Vulnerabilities :

| No. | Severity | Vulnerability                                                                                                                                                                                   | Count |
|-----|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
| 1.  | Critical | MS09-050: Microsoft Windows SMB2 _Smb2ValidateProviderCallback() Vulnerability (975497) (EDUCATEDSCHOLAR) (uncredentialed check)                                                                | 1     |
| 2.  | Critical | MS11-030: Vulnerability in DNS Resolution Could Allow Remote Code Execution (2509553) (remote check)                                                                                            | 1     |
| 3.  | Critical | Unsupported Windows OS (remote)                                                                                                                                                                 | 1     |
| 4.  | High     | MS17-010: Security Update for Microsoft Windows SMB Server (4013389) (ETERNALBLUE) (ETERNALCHAMPION) (ETERNALROMANCE) (ETERNALSYNERGY) (WannaCry) (EternalRocks) (Petya) (uncredentialed check) | 1     |
| 5.  | Medium   | SMB Signing not required                                                                                                                                                                        | 1     |


***

### 1. 40887 - MS09-050: Microsoft Windows SMB2 _Smb2ValidateProviderCallback() Vulnerability (975497) (EDUCATEDSCHOLAR) (uncredentialed check)


Description:


The remote host is running a version of Microsoft Windows Vista or Windows Server 2008 that contains a vulnerability in its SMBv2 implementation. An attacker can exploit this flaw to disable the remote host or to execute arbitrary code on it.


EDUCATEDSCHOLAR is one of multiple Equation Group vulnerabilities and exploits disclosed on 2017/04/14 by a group known as the Shadow Brokers.


Exploitable With


Metasploit (MS09-050 Microsoft SRV2.SYS SMB Negotiate ProcessID Function Table Dereference)


Port: 445/tcp


POC:


<img width="452" alt="image" src="https://github.com/Lynk4/Windows-Server-2008-VAPT/assets/44930131/9c8183bf-f30f-4b94-9542-43084b0c5247">



<img width="452" alt="image" src="https://github.com/Lynk4/Windows-Server-2008-VAPT/assets/44930131/18e55748-72d7-4741-b2f0-d56f4c4571cb">


Note - After 180 second it will trigger the exploit and you will get a shell connection from windows server of the root user(System32).


CVSS v3.0 Base Score


Solution:


Microsoft has released a patch for Windows Vista and Windows Server 2008.


***


### 2. MS11-030: Vulnerability in DNS Resolution Could Allow Remote Code Execution (2509553) (remote check)








