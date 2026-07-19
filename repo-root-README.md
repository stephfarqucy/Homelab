# Homelab Security Projects

A collection of hands-on security projects built on a self-hosted Proxmox VE home lab, documenting real deployment, attack simulation, and remediation work — including the troubleshooting encountered along the way.

## Projects

### [Wazuh SIEM Deployment](./wazuh-siem-lab/README.md)
Deployed a self-hosted Wazuh SIEM, onboarded a monitored endpoint, and validated the full detection pipeline end-to-end using simulated attack traffic. Includes a detailed incident log covering infrastructure failures diagnosed and resolved along the way — an invalid IP cascading through multiple config files, a missing dependency causing silent failures, and more.

**Skills demonstrated:** SIEM deployment, Linux/Proxmox administration, systematic root-cause troubleshooting

---

### Active Directory Attack Lab & Remediation
A two-part project simulating a real Kerberoasting attack against a deliberately vulnerable Active Directory service account, then closing the vulnerability and proving the fix.

- **[Part 1: Attack Lab](./ad-attack-lab/AD-attack-lab-README.md)** — Building the domain, the vulnerable service account, and executing the attack (confirmed via Windows Security event logs).
- **[Part 2: GPO Hardening & Remediation](./ad-attack-lab/GPO-hardening-README.md)** — Enforcing AES-only Kerberos encryption via Group Policy, then re-running the identical attack to verify it fails.

**Skills demonstrated:** Active Directory/Windows Server administration, Kerberos internals, MITRE ATT&CK technique execution (T1558.003), Group Policy hardening, attack/remediation verification methodology

---

## About

Built while pursuing a graduate certificate in Information Systems Security at the University at Albany, with a focus on incident response and security tooling. These projects were built to gain hands-on experience beyond coursework, targeting SOC Analyst / detection & response roles.
