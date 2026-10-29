# Findings and limitations

The following observations summarize the practical thesis results rather than presenting a new independent vulnerability disclosure.

## Availability and wireless behavior

The thesis reports successful interruption of wireless connectivity and video availability during deauthentication tests for each of the three cameras. The connection returned after the test was stopped. Traffic-stress testing also raised availability concerns; the thesis separately noted signs of defensive behavior on Reolink and Imou units under some probes.

**Interpretation:** Availability is a meaningful security property for surveillance systems. The experiments highlight the need to evaluate the wider wireless and network environment, not only device login settings.

## Network-service exposure

Nmap-based assessments compared accessible services and ports. The thesis described the tested JOOAN device as exposing more network functionality than the other units in the selected setup.

**Interpretation:** Exposed services increase the surface that must be reviewed. The research does not establish that every discovered port was remotely exploitable.

## Credential handling and video access

In a controlled JOOAN test, Wireshark captured account-related data during a management interaction. A weak password used in that experiment was recovered during an offline password-security test. The thesis also demonstrated access to the tested camera's video stream using known credentials and streaming information.

**Interpretation:** Credential protection, transport encryption and strong passwords are important. These observations are **specific to the documented JOOAN scenario** and should not be generalized to the other two cameras.

## Physical access and re-enrollment

For the tested devices, the thesis describes reset/re-enrollment scenarios involving physical access. This is an access-control and physical-security consideration, not evidence of a remote vulnerability by itself.

## Limits of the research

- Exactly **three** IoT cameras were assessed.
- Results reflect the setup, firmware/configuration and period of testing.
- No broader manufacturer or market-wide vulnerability prevalence can be inferred.
- No specific CVE attribution or responsible-disclosure case is claimed here.
- The repository intentionally omits raw captures and reproduction steps that could expose devices, identities or footage.

For mitigation steps, see [Security recommendations](recommendations.md).
