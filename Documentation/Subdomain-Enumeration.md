# Subdomain Enumeration

## Objective

Document the subdomain-discovery and reconnaissance exercise shown in the supplied training record.

## Tools visible in the record

- Amass
- theHarvester
- Sublist3r
- DNS-related enumeration sources

## Observations recorded

- One screenshot displays a subdomain-enumeration result list under an example-style domain label.
- An Amass run in the supplied material displays the message **“Found 84”** during the exercise.
- A theHarvester run displays no IPs, emails, hosts, or people for the domain queried in that particular run.
- A later Sublist3r run ends with a Python traceback involving its DNSdumpster-related processing. The run should be treated as an unsuccessful/partially completed execution rather than a confirmed enumeration result.

## Interpretation

Different OSINT tools rely on different data sources and collection methods, so their results may differ. A tool returning no records does not prove that no subdomains or related assets exist. Likewise, a displayed count should be validated, deduplicated, and checked before being treated as a final asset inventory.

## Suggested validation workflow

1. Confirm the assessment scope and written authorization.
2. Record the exact tool name and version used during the test.
3. Save raw output locally and remove secrets or identifying data before sharing.
4. Deduplicate discovered names.
5. Resolve candidate names and validate only assets within the approved scope.
6. Record tool errors and limitations alongside successful results.

## Evidence and limitations

This write-up is based on the supplied five-page PDF. Raw screenshots and target names are not included in this public version because the screenshots contain domain identifiers that should be reviewed and authorized before publication. The source material does not provide a complete, clean, reproducible command transcript for every tool, so commands have not been invented here.
