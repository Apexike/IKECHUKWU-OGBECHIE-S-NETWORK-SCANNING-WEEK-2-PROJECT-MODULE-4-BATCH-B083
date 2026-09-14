# IKECHUKWU-OGBECHIE-S-NETWORK-SCANNING-WEEK-2-PROJECT-MODULE-4-BATCH-B083
LIABILITY DISCLAIMER:

This project is solely for educational purpose and for no other intent.

DESCRIPTION:

theHarvester (Kali) is a passive OSINT tool that gathers public info—emails, subdomains, hostnames, IPs—via search engines, DNS, Shodan, VirusTotal. Zenmap (Nmap GUI) actively scans targets for live hosts, open ports, services, and OS fingerprints. Only use on systems you own or are authorized to test.

TOOLS USED:

Kali linux(theHarvester and Zenmap)

NETWORK SCANNING WITH theHarvester:

Scanning with theHarvester

theHarvester is a passive OSINT (Open Source Intelligence) tool built into Kali Linux, used to gather publicly available information about a target domain or organization — without directly interacting with their systems.

What it collects:

	•	Email addresses
	•	Subdomains and hostnames
	•	Employee names
	•	IP addresses
	•	Related URLs

NETWORK SCANNING WITH Zenmap:

Zenmap is the official GUI for Nmap, used to scan networks and identify live hosts, open ports, running services, and operating systems.
Steps:

	1.	Launch Zenmap on Kali Linux
	2.	Enter the target IP address, hostname, or range in the “Target” field
	3.	Select a scan profile (e.g., “Intense scan,” “Quick scan,” “Ping scan”) from the dropdown
	4.	Click Scan to begin

Output:

	•	Nmap Output tab — raw scan results and command used
	•	Ports/Hosts tab — list of open/closed/filtered ports and detected services
	•	Topology tab — visual network map of discovered hosts
	•	Host Details tab — OS guesses, MAC address, uptime, etc.
  Zenmap should only be used against systems you own or have explicit written permission to test — unauthorized scanning can be illegal.

Risk Analysis: theHarvester

Risk level: Low


- Passive reconnaissance — no direct connection made to the target's systems
- Only pulls from public sources (search engines, DNS, Shodan, VirusTotal, etc.)
- Target typically cannot detect it's being scanned, since no packets are sent to their infrastructure


  Residual risks:

  
- Can still expose sensitive info (employee emails, subdomains) useful to an attacker for phishing or further recon
- Findings could unintentionally reveal misconfigurations (e.g., forgotten subdomains) if shared improperly
- API keys used for sources like Shodan/Hunter.io could be exposed if the tool or config is mishandle.
 
    

Risk Analysis: Zenmap (Nmap)

Risk level: Medium–High
- Active scanning — sends packets directly to the target, so it can be detected/logged by firewalls, IDS/IPS
- Intense scans (-A, -T4) are noisy and easily flagged as suspicious activity


  Residual risks:
  
- Can trigger security alerts or lockouts on the target network
- Aggressive timing settings may cause service disruption on fragile/legacy systems
- Running against systems without authorization is illegal (unauthorized access/computer misuse laws)
- Results (open ports, services, OS) reveal exploitable attack surface if leaked


Mitigations for both:
 
- Always get explicit written authorization before scanning
- Use scoped, minimal scans first (e.g., ping scan before intense scan) to reduce network impact
- Store and share findings securely — treat results as sensitive data
- Log activity for accountability during authorized engagements


Conclusion:

theHarvester and Zenmap serve complementary roles in the reconnaissance phase of a security assessment. theHarvester provides low-risk, passive intelligence by gathering publicly exposed information — emails, subdomains, and hosts — without ever touching the target's systems. Zenmap, by contrast, delivers deeper, more actionable insight through active scanning, revealing live hosts, open ports, and running services, but carries greater risk of detection and potential disruption. Used together, they give a well-rounded view of a target's attack surface: theHarvester maps what's publicly visible, while Zenmap confirms what's actually reachable and exploitable. As with any reconnaissance activity, both tools must be used strictly within authorized scope, with findings handled responsibly and securely. When applied correctly, they form a solid foundation for identifying vulnerabilities before they can be exploited by malicious actors.

PHOTO SAMPLES:

<img width="1920" height="923" alt="theharvester" src="https://github.com/user-attachments/assets/8c947d8d-a8a7-449f-8e8c-da1d7dce3742" />
<img width="1920" height="923" alt="theharvesr2" src="https://github.com/user-attachments/assets/e946a9ab-1a26-46a1-acf4-7f4370113425" />
<img width="1920" height="923" alt="3" src="https://github.com/user-attachments/assets/288b343a-1d5e-429f-b839-a09e601bd20b" />
<img width="1920" height="923" alt="ping Target" src="https://github.com/user-attachments/assets/264e5b1b-93d6-44e4-a78d-4876551d33e7" />
<img width="1920" height="923" alt="Zenmap scanning" src="https://github.com/user-attachments/assets/22e4498f-e230-4c79-a2f1-33663d3e0df1" />
<img width="1920" height="923" alt="topography" src="https://github.com/user-attachments/assets/c570a68d-5f0d-4ad8-87e6-cd8bae570030" />

LINKEDIN:
 www.linkedin.com/in/ikechukwu-ogbechie-286380239

 REPORT:

 <img width="1206" height="1079" alt="e8aa303b-4bb1-4d2b-8c88-50ad0b811834" src="https://github.com/user-attachments/assets/6afe9c68-1265-45d4-bb6d-d69c14e2d05a" />



