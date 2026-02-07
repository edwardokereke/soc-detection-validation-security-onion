# soc-detection-validation-security-onion
SOC detection validation lab using Security Onion, Zeek, and Suricata
# SOC Detection Validation Lab – Security Onion

## Objective
Validate Security Onion detections by generating controlled traffic and correlating Zeek connection logs with Suricata alerts.

## Environment
- Security Onion 2.4
- Kali Linux (traffic generator)
- VMware Workstation
- Zeek, Suricata, Elastic

## Methodology
1. Generated network traffic using Nmap and FTP from Kali Linux
2. Observed connection metadata in Zeek (`zeek.conn`)
3. Reviewed Suricata alerts triggered by scanning behavior
4. Correlated alerts with Zeek logs by time, IP, and protocol
5. Classified alerts based on SOC triage standards

## Findings
- Zeek successfully logged all connection attempts
- Suricata generated informational alerts for reconnaissance activity
- Traffic matched expected lab behavior
- No malicious activity confirmed

## Analyst Conclusion
This activity was classified as **Benign / Expected Lab Traffic**.  
No escalation or remediation required.

## Skills Demonstrated
- SOC alert triage
- Zeek & Suricata correlation
- Network traffic analysis
- False positive validation
- Security Onion Hunt usage
