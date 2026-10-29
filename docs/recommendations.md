# Security recommendations

A defensive checklist based on the risk themes and recommendations discussed in the thesis.

| Risk area | Recommended safeguard |
|---|---|
| Default or weak credentials | Replace factory credentials immediately; use strong, unique passwords and secure storage practices |
| Unprotected management traffic | Prefer HTTPS/TLS or other protected management channels and verify device support |
| Unnecessary exposed services | Disable unused features and restrict network access to required services |
| Lateral movement | Put IoT cameras on an isolated network or VLAN, separate from critical and personal devices |
| Outdated firmware | Check manufacturer advisories and apply security updates promptly |
| Remote-access exposure | Minimize internet-facing services and review access permissions |
| Wireless disruption | Review wireless security posture and surveillance continuity requirements; avoid relying on Wi-Fi as a single point of availability for critical deployments |
| Physical reset/re-enrollment | Secure camera placement and restrict physical access to reset controls |
| Detection and recovery | Review logs where supported, monitor anomalous connectivity, and maintain a documented recovery procedure |

These are risk-reduction practices, not guarantees of protection against every attack. Their applicability depends on the particular product and deployment.
