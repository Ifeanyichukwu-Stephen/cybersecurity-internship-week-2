# cybersecurity-internship-week-2

# WEEK 2 CYBERSECURITY INTERNSHIP REPORT

## Footprinting, Reconnaissance and Local Network Scanning

**Organisation:** Networkwalks  
**Programme:** Cybersecurity Internship  
**Week:** 2  
**Operating System:** Kali Linux  
**Virtualisation Software:** Oracle VirtualBox  
**Tools Used:** WHOIS, WhatWeb, Nslookup, cURL, WAFW00F, Zenmap

---

## 1. Introduction

During the second week of my cybersecurity internship at Networkwalks, I gained practical experience in footprinting, reconnaissance, and local network scanning.

The activities focused on understanding how to gather information about a website using different reconnaissance tools and how to identify devices and services available on a local network using Zenmap.

These exercises helped me understand the importance of information gathering in cybersecurity assessments and how network discovery can provide useful information about the security of an environment.

## 2. Objectives

The main objectives of the week's activities were to:

- Understand the concept of footprinting and reconnaissance.
- Learn how to gather publicly available information about a domain.
- Identify technologies used by a website.
- Understand DNS resolution and HTTP response headers.
- Learn how to identify the presence of a Web Application Firewall.
- Install and become familiar with Zenmap.
- Perform a scan of an authorised local network.
- Understand how to identify active hosts, open ports, and detected services.
- Document findings from practical cybersecurity activities.

## 3. Footprinting and Reconnaissance

Footprinting is the process of collecting information about a target system, organisation, or domain. Reconnaissance is the information-gathering stage of a security assessment.

During this exercise, I used different tools available in Kali Linux to gather information about the domain:

**Target Domain:** `networkwalks.com`

### 3.1 WHOIS

**Command:**
```bash
whois networkwalks.com
```

**Description:**

WHOIS is a tool used to retrieve publicly available domain registration information. It can provide details such as the domain registrar, registration dates, name servers, and registrant information where available.

**Security Relevance:** Medium

**Importance:**

This information helps security professionals understand domain ownership and registration details. It can also provide useful background information during an initial security assessment.

### 3.2 WhatWeb

**Command:**
```bash
whatweb networkwalks.com
```

**Description:**

WhatWeb is a web technology identification tool. It helps identify technologies used by a website, including web servers, content management systems, frameworks, and other publicly detectable components.

**Security Relevance:** High

**Importance:**

Identifying the technologies used by a website helps security professionals understand its technology stack and determine which components may require further security review.

### 3.3 Nslookup

**Command:**
```bash
nslookup networkwalks.com
```

**Description:**

Nslookup is a DNS query tool used to retrieve information about domain names. It helps resolve a domain name into its corresponding IP address and obtain other DNS response information.

**Security Relevance:** High

**Importance:**

DNS information helps security professionals understand how a domain is mapped to network addresses and provides useful information during network reconnaissance.

### 3.4 cURL

**Command:**
```bash
curl -I https://networkwalks.com
```

**Description:**

cURL is a command-line tool used to communicate with web servers. The `-I` option sends an HTTP HEAD request and displays the response headers returned by the server.

**Security Relevance:** Medium

**Importance:**

HTTP response headers can provide information about server responses, status codes, redirects, and security-related configurations.

### 3.5 WAFW00F

**Command:**
```bash
wafw00f https://networkwalks.com
```

**Description:**

WAFW00F is a tool used to identify whether a website is protected by a Web Application Firewall (WAF). It may also identify the type or vendor of the firewall.

**Security Relevance:** High

**Importance:**

Understanding whether a Web Application Firewall is present helps security professionals understand the defensive technologies protecting a web application.

**Note:** WAF detection may not always be conclusive.

---

## 4. Local Network Scanning Using Zenmap

### 4.1 Introduction to Zenmap

Zenmap is the graphical user interface (GUI) for Nmap, a network discovery and security auditing tool.

It provides a visual interface that makes it easier to configure scans, monitor scan progress, and analyse network information.

During this exercise, I installed Zenmap and used it to perform a scan of my authorised local network.

### 4.2 Objectives of the Network Scan

The objectives of this activity were to:

- Discover devices connected to the local network.
- Identify active hosts.
- Examine open, closed, and filtered ports.
- Identify services running on discovered devices where possible.
- Understand how network scanning supports security assessments.

### 4.3 Tool Used

**Tool:** Zenmap  
**Underlying scanning engine:** Nmap  
**Environment:** Kali Linux

### 4.4 Scanning Procedure

The following steps were carried out:

1. Installed and opened Zenmap on Kali Linux.
2. Identified the local network range authorised for testing.
3. Entered the target network range into Zenmap.
4. Selected an appropriate scan profile.
5. Started the network scan.
6. Monitored the scanning process.
7. Reviewed the scan results using the Nmap Output and Ports/Hosts sections.
8. Examined the discovered hosts and available port information.
9. Recorded the results for documentation.

### 4.5 Understanding the Scan Results

During network scanning, the following terms are important:

| Term | Meaning |
|---|---|
| Host Discovery | Identifying devices that respond to network discovery probes. |
| Open Port | A port where an application is accepting connections. |
| Closed Port | A port where no application is listening, although the host responds. |
| Filtered Port | A port whose state cannot be determined because filtering or network conditions prevent a clear response. |
| Service Detection | Identifying the service associated with an open port. |
| Version Detection | Attempting to identify the software version providing a service. |

### 4.6 Network Scan Findings

**Note:** Complete this section with the actual results displayed by Zenmap.

| Information | Result |


### 4.8 Security Importance of Network Scanning

Network scanning is an important part of cybersecurity because it helps security professionals understand the devices and services available within a network.

It can help identify:

- Unrecognised devices connected to a network.
- Services that may require security review.
- Unnecessary exposed ports.
- Network visibility and filtering behaviour.
- Systems that may require further assessment.

An open port does not automatically mean that a system is vulnerable. Further investigation is required to determine whether a service presents a security risk.

---

## 5. Challenges and Observations

During the practical exercises, I gained experience working with different command-line reconnaissance tools and the Zenmap graphical interface.

The activities also helped me understand that the accuracy of network scan results can depend on network configuration, firewall settings, virtual machine networking mode, and the selected scan profile.

One important lesson was the need to analyse tool outputs carefully rather than making assumptions based on detected information.

## 6. Skills and Knowledge Acquired

At the end of the week's activities, I gained practical knowledge in the following areas:

- Domain information gathering using WHOIS.
- Website technology identification using WhatWeb.
- DNS lookup and resolution using Nslookup.
- HTTP response header inspection using cURL.
- Web Application Firewall detection using WAFW00F.
- Installation and use of Zenmap.
- Local network discovery and scanning.
- Identification of active hosts and network ports.
- Basic interpretation of network scan results.
- Cybersecurity documentation and reporting.

## 7. Conclusion

Week 2 of my cybersecurity internship at Networkwalks provided valuable practical experience in footprinting, reconnaissance, and local network scanning.

I learned how different tools can be used to gather information about a domain, examine web technologies, query DNS information, inspect HTTP response headers, and check for Web Application Firewall protection.

I also gained practical experience using Zenmap to scan an authorised local network and understand how network discovery helps identify active hosts, open ports, and available services.

These activities strengthened my understanding of the information-gathering stage of cybersecurity assessments and provided a foundation for more advanced network security and vulnerability assessment exercises.

---

## 8. Evidence and Screenshots



- WHOIS
- WhatWeb command output.
- Nslookup command output.
- cURL HTTP response headers.
- WAFW00F detection output.
- Zenmap network scan screenshot.
- Zenmap Ports/Hosts results.
- Zenmap Nmap Output screenshot.



---

## 9. Author

**Role:** Cybersecurity Intern  
**Organisation:** Networkwalks  
**Focus:** Footprinting, Reconnaissance and Network Scanning

---

**Disclaimer:** All scanning activities should be performed only on systems and networks that you own or have explicit permission to assess. Sensitive network information should be removed before publishing this report publicly.
