# Scope and methodology

## Purpose

The study examined the security implications of deploying network-connected consumer surveillance cameras in a home-like setting. It focused on communications, authentication, streaming, device availability and practical safeguards.

## Test scope

- **Devices:** Reolink E Series E320, JOOAN A2R-U, Imou Ranger 2C.
- **Setting:** Controlled academic lab with local network and personally accessible test equipment.
- **Equipment:** An end-user workstation, a Kali Linux testing machine/virtual environment, a wireless network adapter and the cameras.
- **Approach:** Asset inventory, examination of network/protocol characteristics, service discovery, controlled security testing, observation of behavior, reporting and mitigation analysis.

## Test categories

1. **Asset and service inventory:** Identify connected components and visible network services.
2. **Traffic and protocol inspection:** Review how the tested systems communicate and which security properties are relevant to video surveillance.
3. **Availability testing:** Observe disruption to connectivity and streaming under laboratory conditions.
4. **Authentication and credential assessment:** Evaluate whether observed data handling creates risks; limit password testing to authorized lab materials.
5. **Stream access assessment:** Evaluate access-control implications without distributing credentials or stream URLs.
6. **Physical-access scenario:** Assess how device reset/reassignment changes the threat model.
7. **Threat/risk framing:** Discuss STRIDE categories and the DREAD model to organize risks and mitigations.

## Important distinctions

- This was **not** a statistically representative survey of consumer cameras.
- A service appearing in a network scan is not, by itself, confirmation of a vulnerability.
- A successful laboratory disruption does not imply that persistent access was gained.
- Device characteristics and results may depend on firmware version, configuration and wireless/network environment.
- The thesis discusses STRIDE and DREAD as assessment frameworks; this repository does **not** claim to contain a complete numeric DREAD scoring dataset.

## Reproducibility and publication

To avoid distributing potentially harmful procedures or sensitive lab data, this public portfolio does not include executable attack instructions, source packet captures, access tokens, password hashes, BSSIDs, RTSP links, or device identifiers. Interested reviewers can discuss research methods and validation at a conceptual level.
