# Week 1 – Practical Evidence

## NetworkWalks Academy – Cybersecurity & Ethical Hacking Internship



## 1. Introduction

This folder contains screenshots and practical evidence collected during the Week 1 cybersecurity lab assignment.

The evidence is intended to demonstrate the Kali Linux environment, network configuration, connectivity testing, Nmap verification, and virtual machine snapshot creation.

## 2. Evidence and Verification

### 2.1 Kali Linux Environment

**Purpose:** Demonstrate that the Kali Linux virtual machine starts successfully and the desktop environment is accessible.



### 2.2 Network Interface and IP Address

**Command:**
```bash
ip a
```

**Purpose:** Identify the active network interface and verify its assigned IPv4 address.

**Expected configuration:**
- IP address: `10.0.0.2`
- Subnet mask: `/24`
- Gateway: `10.0.0.1`


### 2.3 Gateway Connectivity Test

**Command:**
```bash
ping -c 4 10.0.0.1
```

**Purpose:** Verify whether Kali Linux can communicate with the configured gateway.

**Expected result:** Successful ICMP echo replies from `10.0.0.1`.



### 2.4 External IP Connectivity Test

**Command:**
```bash
ping -c 4 8.8.8.8
```

**Purpose:** Test IP-level connectivity to an external destination.

**Expected result:** Successful replies from `8.8.8.8`, if ICMP traffic is permitted.



### 2.5 DNS Resolution Test

**Command:**
```bash
nslookup networkwalks.com
```

**Purpose:** Verify whether the configured DNS service can resolve a domain name into an IP address.

**Expected result:** A successful DNS response containing the resolved address.

**Evidence:** `dns-lookup.png`

### 2.6 Nmap Installation Verification

**Command:**
```bash
nmap --version
```

**Purpose:** Verify that Nmap is installed and identify its version.

**Expected result:** Nmap version information is displayed.

**Evidence:** `nmap-version.png`

*Note: Nmap testing should only be performed against systems you own or have explicit permission to assess.*

### 2.7 Virtual Machine Snapshot

**Purpose:** Demonstrate the creation of a recovery point for the virtual machine.


Update each status only after checking the corresponding screenshot or terminal output.



## 3. Conclusion

This evidence folder documents the practical activities performed during Week 1 of the NetworkWalks Academy Cybersecurity & Ethical Hacking internship. It provides a record of the lab environment, configuration steps, and verification results.
