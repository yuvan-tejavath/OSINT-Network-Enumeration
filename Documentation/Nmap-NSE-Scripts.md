# Nmap Scripting Engine (NSE) Observations

## Objective

Record the Nmap NSE and service-enumeration observations shown in the supplied two-page training PDF.

## Lab context

- Environment shown: Kali Linux / VMware lab
- Target shown: `192.168.93.1` (private lab address in the source screenshot)
- Nmap version displayed: `7.98`

## Observed port and service results

The scan output reports the host as up and shows these TCP ports as open:

| Port | State | Service label shown |
|---:|---|---|
| 135/tcp | open | msrpc |
| 139/tcp | open | netbios-ssn |
| 445/tcp | open | microsoft-ds |

The output also reports 997 TCP ports as not shown because they received no response in that scan. A VMware MAC address is visible in the original lab output and has intentionally been omitted from this public write-up.

## NSE observations

The supplied output shows:

- `smb-vuln-ms10-054`: `false`
- Other SMB-related checks returned negotiation/receive errors, including messages indicating that the script could not negotiate an SMB connection or receive bytes.

## Interpretation

An NSE script error is not a vulnerability finding. It means that the script did not complete its check successfully under the conditions of that scan. The `false` result applies only to the specific check and conditions shown; it does not establish that the host has no vulnerabilities.

Open ports identify reachable services, not confirmed vulnerabilities. Service ownership, patch level, configuration, and exposure should be assessed only within the authorized lab scope.

## Limitations

The supplied PDF contains terminal screenshots rather than a complete text export. The exact full NSE command line is not sufficiently legible in the source, so it is intentionally not reconstructed or guessed here.
