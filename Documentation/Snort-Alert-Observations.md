# Snort Alert Observations

## Objective

Summarize the network-alert screenshot supplied in `Nmap Detect.pdf`.

## Tool and environment shown

- Snort network intrusion detection
- Windows virtual machine shown in the monitoring environment

## Alert labels visible in the screenshot

The screenshot contains alert entries labelled as:

- UDP port scan detected
- ICMP ping detected
- TCP session without three-way handshake

## Interpretation

These alerts indicate that Snort generated detections matching configured rules or signatures. An alert is an investigative lead, not proof by itself of malicious activity. Analysts should correlate timestamps, source/destination addresses, packet details, rule identifiers, and surrounding traffic before classifying an event.

## SOC triage checklist

1. Confirm the alert timestamp and sensor.
2. Identify source and destination hosts within the authorized environment.
3. Review packet/flow context and related alerts.
4. Determine whether the activity matches an approved scan or expected lab test.
5. Record evidence, impact, and confidence.
6. Escalate or contain only according to the organization's incident-response procedure.

## Evidence limitation

The public repository does not include the original screenshot because it contains network identifiers and detailed traffic data that should be sanitized and approved before disclosure.
