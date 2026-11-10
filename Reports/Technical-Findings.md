# Technical Findings Summary

This report consolidates observations from the three training PDFs supplied for portfolio preparation.

| Area | Source-supported observation | Limitation |
|---|---|---|
| Subdomain enumeration | An Amass screenshot displays `Found 84`. | The complete target list is not reproduced; results require validation and authorization review. |
| theHarvester | One run reports no IPs, emails, hosts, or people. | A no-result response is not proof that no assets exist. |
| Sublist3r | A run ends with a Python traceback during DNSdumpster-related processing. | This run is not treated as a successful complete enumeration. |
| Nmap / NSE | Lab host `192.168.93.1` is shown with TCP 135, 139, and 445 open. | Screenshot-based result; one scan snapshot only. |
| SMB NSE checks | `smb-vuln-ms10-054` reports `false`; other checks show SMB negotiation/receive errors. | Errors are inconclusive and do not prove secure or vulnerable status. |
| Snort | Screenshot shows UDP port-scan, ICMP ping, and TCP handshake-related alert labels. | Alert labels alone do not establish malicious intent. |

## Overall learning outcomes

- Exposure to passive and active reconnaissance tools.
- Familiarity with subdomain discovery and DNS-related data sources.
- Understanding of host, port, and service enumeration output.
- Awareness of NSE script limitations and inconclusive results.
- Introduction to interpreting IDS alerts and the need for contextual triage.

## Publication note

This is a sanitized summary, not a replacement for the original internship submissions. Original PDFs, screenshots, target names, network identifiers, and any company/client information should remain private unless the relevant owner has explicitly approved public disclosure.
