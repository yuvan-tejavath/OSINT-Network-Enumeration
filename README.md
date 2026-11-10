# OSINT & Network Enumeration Lab

A portfolio write-up based on practical cybersecurity training exercises covering subdomain discovery, DNS/reconnaissance tooling, Nmap host and service scanning, Nmap Scripting Engine (NSE) checks, and network-alert observation in Snort.

> **Scope and evidence note:** This repository is a cleaned, public-safe summary of the supplied training PDFs. Target identifiers and raw screenshots have intentionally not been republished. The source material includes third-party domain references and lab network details. Add screenshots or raw outputs only after confirming you are authorized to disclose them and removing sensitive identifiers.

## Topics covered

- [Subdomain enumeration](Documentation/Subdomain-Enumeration.md)
- [Nmap host and service detection](Documentation/Nmap-Scanning.md)
- [Nmap NSE and SMB script observations](Documentation/Nmap-NSE-Scripts.md)
- [Snort alert observations](Documentation/Snort-Alert-Observations.md)
- [Consolidated findings](Reports/Technical-Findings.md)

## Tools shown in the supplied training material

- Kali Linux
- Amass
- theHarvester
- Sublist3r
- Nmap / Nmap Scripting Engine
- Snort

## Key observations from the training records

- The subdomain-enumeration exercise displayed a result count of **84**. The source screenshots also show a Sublist3r execution ending in a Python traceback; this is recorded as a tool execution issue, not as a successful result.
- The Nmap NSE exercise reported a lab host at `192.168.93.1` with TCP ports `135`, `139`, and `445` open. The service labels shown were `msrpc`, `netbios-ssn`, and `microsoft-ds`.
- SMB-related NSE output included a result of `false` for `smb-vuln-ms10-054` and negotiation/receive errors for other SMB checks. These errors do **not** establish that a host is vulnerable or secure.
- The Snort screenshot contains alerts labelled as UDP port-scan and ICMP ping detection, plus a TCP session-without-three-way-handshake alert.

## Responsible-use statement

All scanning and testing must be limited to systems you own or have explicit written permission to assess. Do not use these techniques against public systems without authorization. Do not commit credentials, API keys, personal data, private reports, or confidential internship material.

## Author

Yuvan Tejavath — Cybersecurity learner / aspiring SOC Analyst.
