# Awesome Incident Response with stars

> A curated list of tools and resources for security incident response, aimed to help security analysts and [DFIR](http://www.acronymfinder.com/Digital-Forensics%2c-Incident-Response-%28DFIR%29.html) teams.

Digital Forensics and Incident Response (DFIR) teams are groups of people in an organization responsible for managing the response to a security incident, including gathering evidence of the incident, remediating its effects, and implementing controls to prevent the incident from recurring in the future.

## Contents

* [Adversary Emulation](#adversary-emulation)
* [All-In-One Tools](#all-in-one-tools)
* [Books](#books)
* [Communities](#communities)
* [Disk Image Creation Tools](#disk-image-creation-tools)
* [Evidence Collection](#evidence-collection)
* [Incident Management](#incident-management)
* [Knowledge Bases](#knowledge-bases)
* [Linux Distributions](#linux-distributions)
* [Linux Evidence Collection](#linux-evidence-collection)
* [Log Analysis Tools](#log-analysis-tools)
* [Memory Analysis Tools](#memory-analysis-tools)
* [Memory Imaging Tools](#memory-imaging-tools)
* [OSX Evidence Collection](#osx-evidence-collection)
* [Other Lists](#other-lists)
* [Other Tools](#other-tools)
* [Playbooks](#playbooks)
* [Process Dump Tools](#process-dump-tools)
* [Sandboxing/Reversing Tools](#sandboxingreversing-tools)
* [Scanner Tools](#scanner-tools)
* [Timeline Tools](#timeline-tools)
* [Videos](#videos)
* [Windows Evidence Collection](#windows-evidence-collection)

## IR Tools Collection

### Adversary Emulation

* [Atomic Red Team (ART)](https://github.com/redcanaryco/atomic-red-team) ⭐ 12,486 | 🐛 33 | 🌐 C | 📅 2026-08-31 - Small and highly portable detection tests mapped to the MITRE ATT\&CK Framework.
* [Caldera](https://github.com/mitre/caldera) ⭐ 7,237 | 🐛 71 | 🌐 Python | 📅 2026-08-27 - Automated adversary emulation system that performs post-compromise adversarial behavior within Windows Enterprise networks. It generates plans during operation using a planning system and a pre-configured adversary model based on the Adversarial Tactics, Techniques & Common Knowledge (ATT\&CK™) project.
* [APTSimulator](https://github.com/NextronSystems/APTSimulator) ⭐ 2,765 | 🐛 4 | 🌐 Batchfile | 📅 2025-09-23 - Windows Batch script that uses a set of tools and output files to make a system look as if it was compromised.
* [Network Flight Simulator](https://github.com/alphasoc/flightsim) ⭐ 1,363 | 🐛 24 | 🌐 Go | 📅 2024-04-04 - Lightweight utility used to generate malicious network traffic and help security teams to evaluate security controls and network visibility.
* [RedHunt-OS](https://github.com/redhuntlabs/RedHunt-OS) ⭐ 1,319 | 🐛 7 | 📅 2025-01-22 - Virtual machine for adversary emulation and threat hunting.
* [Metta](https://github.com/uber-common/metta) ⭐ 1,146 | 🐛 13 | 🌐 Python | 📅 2019-04-01 - Information security preparedness tool to do adversarial simulation.
* [Red Team Automation (RTA)](https://github.com/endgameinc/RTA) ⭐ 1,097 | 🐛 7 | 🌐 Python | 📅 2019-05-01 - RTA provides a framework of scripts designed to allow blue teams to test their detection capabilities against malicious tradecraft, modeled after MITRE ATT\&CK.
* [DumpsterFire](https://github.com/TryCatchHCF/DumpsterFire) ⭐ 1,040 | 🐛 5 | 🌐 Python | 📅 2020-05-27 - Modular, menu-driven, cross-platform tool for building repeatable, time-delayed, distributed security events. Easily create custom event chains for Blue Team drills and sensor /   alert mapping. Red Teams can create decoy incidents, distractions, and lures to support and scale their operations.
* [AutoTTP](https://github.com/jymcheong/AutoTTP) ⭐ 262 | 🐛 0 | 🌐 Python | 📅 2023-05-26 - Automated Tactics Techniques & Procedures. Re-running complex sequences manually for regression tests, product evaluations, generate data for researchers.

### All-In-One Tools

* [Flare](https://github.com/fireeye/flare-vm) ⭐ 8,996 | 🐛 28 | 🌐 PowerShell | 📅 2026-06-23 - A fully customizable, Windows-based security distribution for malware analysis, incident response, penetration testing.
* [Fleetdm](https://github.com/fleetdm/fleet) ⭐ 6,812 | 🐛 3,458 | 🌐 Go | 📅 2026-09-04 - State of the art host monitoring platform tailored for security experts. Leveraging Facebook's battle-tested osquery project, Fleetdm delivers continuous updates, features and fast answers to big questions.
* [GRR Rapid Response](https://github.com/google/grr) ⭐ 5,089 | 🐛 191 | 🌐 Python | 📅 2026-05-12 - Incident response framework focused on remote live forensics. It consists of a python agent (client) that is installed on target systems, and a python server infrastructure that can manage and talk to the agent. Besides the included Python API client, [PowerGRR](https://github.com/swisscom/PowerGRR) ⭐ 57 | 🐛 1 | 🌐 PowerShell | 📅 2022-03-18 provides an API client library in PowerShell working on Windows, Linux and macOS for GRR automation and scripting.
* [Velociraptor](https://github.com/Velocidex/velociraptor) ⭐ 4,234 | 🐛 74 | 🌐 Go | 📅 2026-09-04 - Endpoint visibility and collection tool
* [MozDef](https://github.com/mozilla/MozDef) ⚠️ Archived - Automates the security incident handling process and facilitate the real-time activities of incident handlers.
* [Matano](https://github.com/matanolabs/matano) ⭐ 1,694 | 🐛 55 | 🌐 Rust | 📅 2025-01-08: Open source serverless security lake platform on AWS that lets you ingest, store, and analyze petabytes of security data into an Apache Iceberg data lake and run realtime Python detections as code.
* [IRIS](https://github.com/dfir-iris/iris-web) ⭐ 1,558 | 🐛 431 | 🌐 Python | 📅 2026-08-24 - IRIS is a web collaborative platform for incident response analysts allowing to share investigations at a technical level.
* [Dissect](https://github.com/fox-it/dissect) ⭐ 1,151 | 🐛 10 | 📅 2026-02-25 - Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group).
* [Kuiper](https://github.com/DFIRKuiper/Kuiper) ⭐ 905 | 🐛 12 | 🌐 JavaScript | 📅 2024-10-12 - Digital Forensics Investigation Platform
* [Zentral](https://github.com/zentralopensource/zentral) ⭐ 879 | 🐛 39 | 🌐 Python | 📅 2026-09-04 - Combines osquery's powerful endpoint inventory features with a flexible notification and action framework. This enables one to identify and react to changes on OS X and Linux clients.
* [CimSweep](https://github.com/PowerShellMafia/CimSweep) ⭐ 657 | 🐛 2 | 🌐 PowerShell | 📅 2019-08-19 - Suite of CIM/WMI-based tools that enable the ability to perform incident response and hunting operations remotely across all versions of Windows.
* [Doorman](https://github.com/mwielgoszewski/doorman) ⭐ 622 | 🐛 29 | 🌐 Python | 📅 2022-12-08 - osquery fleet manager that allows remote management of osquery configurations retrieved by nodes. It takes advantage of osquery's TLS configuration, logger, and distributed read/write endpoints, to give administrators visibility across a fleet of devices with minimal overhead and intrusiveness.
* [nightHawk](https://github.com/biggiesmallsAG/nightHawkResponse) ⭐ 608 | 🐛 23 | 🌐 Go | 📅 2019-11-20 - Application built for asynchronous forensic data presentation using ElasticSearch as the backend. It's designed to ingest Redline collections.
* [SOC Multi-tool](https://github.com/zdhenard42/SOC-Multitool) ⭐ 422 | 🐛 0 | 🌐 JavaScript | 📅 2025-05-13 - A powerful and user-friendly browser extension that streamlines investigations for security professionals.
* [Cynative](https://github.com/cynative/cynative) ⭐ 196 | 🐛 18 | 🌐 Go | 📅 2026-09-04 - Deep research agent for your infra - sandboxed, read-only, covers AWS, GCP, Azure, K8s, GitHub and GitLab.
* [VanGuard](https://github.com/ridgelinecyberdefence/vanguard) ⭐ 154 | 🐛 0 | 🌐 Go | 📅 2026-07-28 - Cross-platform incident response toolkit with 28 pre-built use cases in a single zero-install binary. Collects memory, disk, network, and cloud artifacts with automated timeline generation.
* [CIRTkit](https://github.com/byt3smith/CIRTKit) ⭐ 153 | 🐛 0 | 🌐 Python | 📅 2017-04-17 - CIRTKit is not just a collection of tools, but also a framework to aid in the ongoing unification of Incident Response and Forensics investigation processes.
* [MutableSecurity](https://github.com/MutableSecurity/mutablesecurity) ⚠️ Archived - CLI program for automating the setup, configuration, and use of cybersecurity solutions.
* [Belkasoft Evidence Center](https://belkasoft.com/ec) -  The toolkit will quickly extract digital evidence from multiple sources by analyzing hard drives, drive images, memory dumps, iOS, Blackberry and Android backups, UFED, JTAG and chip-off dumps.
* [Cyber Triage](http://www.cybertriage.com) - Cyber Triage collects and analyzes host data to determine if it is compromised. It's scoring system and recommendation engine allow you to quickly focus on the important artifacts. It can import data from its collection tool, disk images, and other collectors (such as KAPE). It can run on an examiner's desktop or in a server model. Developed by Sleuth Kit Labs, which also makes Autopsy.
* [Falcon Orchestrator](https://github.com/CrowdStrike/falcon-orchestrator) - Extendable Windows-based application that provides workflow automation, case management and security response functionality.
* [Limacharlie](https://www.limacharlie.io/) - Endpoint security platform composed of a collection of small projects all working together that gives you a cross-platform (Windows, OSX, Linux, Android and iOS) low-level environment for managing and pushing additional modules into memory to extend its functionality.
* [Open Computer Forensics Architecture](http://sourceforge.net/projects/ocfa/) - Another popular distributed open-source computer forensics framework. This framework was built on Linux platform and uses postgreSQL database for storing data.
* [osquery](https://osquery.io/) - Easily ask questions about your Linux and macOS infrastructure using a SQL-like query language; the provided *incident-response pack* helps you detect and respond to breaches.
* [Redline](https://www.fireeye.com/services/freeware/redline.html) - Provides host investigative capabilities to users to find signs of malicious activity through memory and file analysis, and the development of a threat assessment profile.
* [The Sleuth Kit & Autopsy](http://www.sleuthkit.org) - Unix and Windows based tool which helps in forensic analysis of computers. It comes with various tools which helps in digital forensics. These tools help in analyzing disk images, performing in-depth analysis of file systems, and various other things.
* [TheHive](https://thehive-project.org/) - Scalable 3-in-1 open source and free solution designed to make life easier for SOCs, CSIRTs, CERTs and any information security practitioner dealing with security incidents that need to be investigated and acted upon swiftly.
* [X-Ways Forensics](http://www.x-ways.net/forensics/) - Forensics tool for Disk cloning and imaging. It can be used to find deleted files and disk analysis.

### Books

* [Applied Incident Response](https://www.amazon.com/Applied-Incident-Response-Steve-Anson/dp/1119560268/) - Steve Anson's book on Incident Response.
* [Art of Memory Forensics](https://www.amazon.com/Art-Memory-Forensics-Detecting-Malware/dp/1118825098/) - Detecting Malware and Threats in Windows, Linux, and Mac Memory.
* [Crafting the InfoSec Playbook: Security Monitoring and Incident Response Master Plan](https://www.amazon.com/Crafting-InfoSec-Playbook-Security-Monitoring/dp/1491949406) - by Jeff Bollinger, Brandon Enright and Matthew Valites.
* [Digital Forensics and Incident Response: Incident response techniques and procedures to respond to modern cyber threats](https://www.amazon.com/Digital-Forensics-Incident-Response-techniques/dp/183864900X) - by Gerard Johansen.
* [Introduction to DFIR](https://medium.com/@sroberts/introduction-to-dfir-d35d5de4c180/) - By Scott J. Roberts.
* [Incident Response & Computer Forensics, Third Edition](https://www.amazon.com/Incident-Response-Computer-Forensics-Third/dp/0071798684/) - The definitive guide to incident response.
* [Incident Response Techniques for Ransomware Attacks](https://www.amazon.com/Incident-Response-Techniques-Ransomware-Attacks/dp/180324044X) - A great guide to build an incident response strategy for ransomware attacks. By Oleg Skulkin.
* [Incident Response with Threat Intelligence](https://www.amazon.com/Incident-response-Threat-Intelligence-intelligence-based/dp/1801072957) - Great reference to build an incident response plan based also on Threat Intelligence. By Roberto Martinez.
* [Intelligence-Driven Incident Response](https://www.amazon.com/Intelligence-Driven-Incident-Response-Outwitting-Adversary-ebook-dp-B074ZRN5T7/dp/B074ZRN5T7) - By Scott J. Roberts, Rebekah Brown.
* [Operator Handbook: Red Team + OSINT + Blue Team Reference](https://www.amazon.com/Operator-Handbook-Team-OSINT-Reference/dp/B085RR67H5/) - Great reference for incident responders.
* [Practical Memory Forensics](https://www.amazon.com/Practical-Memory-Forensics-Jumpstart-effective/dp/1801070334) - The definitive guide to practice memory forensics. By Svetlana Ostrovskaya and Oleg Skulkin.
* [The Practice of Network Security Monitoring: Understanding Incident Detection and Response](http://www.amazon.com/gp/product/1593275099) - Richard Bejtlich's book on IR.

### Communities

* [Digital Forensics Discord Server](https://discordapp.com/invite/JUqe9Ek) - Community of 8,000+ working professionals from Law Enforcement, Private Sector, and Forensic Vendors. Additionally, plenty of students and hobbyists! Guide [here](https://aboutdfir.com/a-beginners-guide-to-the-digital-forensics-discord-server/).
* [Slack DFIR channel](https://dfircommunity.slack.com) - Slack DFIR Communitiy channel - [Signup here](https://start.paloaltonetworks.com/join-our-slack-community).

### Disk Image Creation Tools

* [Bitscout](https://github.com/vitaly-kamluk/bitscout) ⭐ 479 | 🐛 0 | 🌐 Shell | 📅 2025-03-21 - Bitscout by Vitaly Kamluk helps you build your fully-trusted customizable LiveCD/LiveUSB image to be used for remote digital forensics (or perhaps any other task of your choice). It is meant to be transparent and monitorable by the owner of the system, forensically sound, customizable and compact.
* [AccessData FTK Imager](http://accessdata.com/product-download/?/support/adownloads#FTKImager) - Forensics tool whose main purpose is to preview recoverable data from a disk of any kind. FTK Imager can also acquire live memory and paging file on 32bit and 64bit systems.
* [GetData Forensic Imager](http://www.forensicimager.com/) - Windows based program that will acquire, convert, or verify a forensic image in one of the following common forensic file formats.
* [Guymager](http://guymager.sourceforge.net) - Free forensic imager for media acquisition on Linux.
* [Magnet ACQUIRE](https://www.magnetforensics.com/magnet-acquire/) - ACQUIRE by Magnet Forensics allows various types of disk acquisitions to be performed on Windows, Linux, and OS X as well as mobile operating systems.

### Evidence Collection

* [UAC](https://github.com/tclahr/uac) ⭐ 1,443 | 🐛 10 | 🌐 Shell | 📅 2026-09-03 - UAC (Unix-like Artifacts Collector) is a Live Response collection script for Incident Response that makes use of native binaries and tools to automate the collection of AIX, Android, ESXi, FreeBSD, Linux, macOS, NetBSD, NetScaler, OpenBSD and Solaris systems artifacts.
* [bulk\_extractor](https://github.com/simsong/bulk_extractor) ⭐ 1,418 | 🐛 67 | 🌐 C++ | 📅 2026-09-01 - Computer forensics tool that scans a disk image, a file, or a directory of files and extracts useful information without parsing the file system or file system structures. Because of ignoring the file system structure, the program distinguishes itself in terms of speed and thoroughness.
* [Forensic Artifacts](https://github.com/ForensicArtifacts/artifacts) ⭐ 1,271 | 🐛 44 | 🌐 Python | 📅 2026-07-31 - Digital Forensics Artifact Repository
* [CyLR](https://github.com/orlikoski/CyLR) ⭐ 734 | 🐛 21 | 🌐 C# | 📅 2022-06-01 - The CyLR tool collects forensic artifacts from hosts with NTFS file systems quickly, securely and minimizes impact to the host.
* [ir-rescue](https://github.com/diogo-fernan/ir-rescue) ⭐ 487 | 🐛 4 | 🌐 Batchfile | 📅 2021-02-21 - Windows Batch script and a Unix Bash script to comprehensively collect host forensic data during incident response.
* [Cold Disk Quick Response](https://github.com/rough007/CDQR) ⭐ 345 | 🐛 5 | 🌐 Python | 📅 2022-06-25 - Streamlined list of parsers to quickly analyze a forensic image file (`dd`, E01, `.vmdk`, etc) and output nine reports.
* [artifactcollector](https://github.com/forensicanalysis/artifactcollector) ⚠️ Archived - The artifactcollector project provides a software that collects forensic artifacts on systems.
* [Margarita Shotgun](https://github.com/ThreatResponse/margaritashotgun) ⭐ 253 | 🐛 13 | 🌐 Python | 📅 2020-09-22 - Command line utility (that works with or without Amazon EC2 instances) to parallelize remote memory acquisition.
* [Acquire](https://github.com/fox-it/acquire) ⭐ 122 | 🐛 54 | 🌐 Python | 📅 2026-08-12 - Acquire is a tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container. This makes Acquire an excellent tool to, among others, speedup the process of digital forensic triage. It uses [Dissect](https://github.com/fox-it/dissect) ⭐ 1,151 | 🐛 10 | 📅 2026-02-25 to gather that information from the raw disk, if possible.
* [SPECTR3](https://github.com/alpine-sec/SPECTR3) ⭐ 44 | 🐛 0 | 🌐 C# | 📅 2024-10-25 - Acquire, triage and investigate remote evidence via portable iSCSI readonly access
* [Live Response Collection](https://www.brimorlabs.com/tools/) - Automated tool that collects volatile data from Windows, OSX, and \*nix based operating systems.

### Incident Management

* [Shuffle](https://github.com/frikky/Shuffle) ⭐ 2,424 | 🐛 491 | 🌐 JavaScript | 📅 2026-09-04 - A general purpose security automation platform focused on accessibility.
* [Fast Incident Response (FIR)](https://github.com/certsocietegenerale/FIR/) ⭐ 2,033 | 🐛 14 | 🌐 JavaScript | 📅 2026-08-31 - Cybersecurity incident management platform designed with agility and speed in mind. It allows for easy creation, tracking, and reporting of cybersecurity incidents and is useful for CSIRTs, CERTs and SOCs alike.
* [DFIRTrack](https://github.com/dfirtrack/dfirtrack) ⭐ 538 | 🐛 7 | 🌐 Python | 📅 2026-01-13 - Incident Response tracking application handling one or more incidents via cases and tasks with a lot of affected systems and artifacts.
* [Catalyst](https://github.com/SecurityBrewery/catalyst) ⚠️ Archived - A free SOAR system that helps to automate alert handling and incident response processes.
* [threat\_note](https://github.com/defpoint/threat_note) ⚠️ Archived - Lightweight investigation notebook that allows security researchers the ability to register and retrieve indicators related to their research.
* [DFTimewolf](https://github.com/log2timeline/dftimewolf) ⭐ 353 | 🐛 4 | 🌐 Python | 📅 2026-09-03 - A framework for orchestrating forensic collection, processing and data export.
* [Sandia Cyber Omni Tracker (SCOT)](https://github.com/sandialabs/scot) ⭐ 254 | 🐛 12 | 🌐 JavaScript | 📅 2024-11-04 - Incident Response collaboration and knowledge capture tool focused on flexibility and ease of use. Our goal is to add value to the incident response process without burdening the user.
* [CyberCPR](https://www.cybercpr.com) - Community and commercial incident management tool with Need-to-Know built in to support GDPR compliance while handling sensitive incidents.
* [Cyphon](https://medevel.com/cyphon/) - Cyphon eliminates the headaches of incident management by streamlining a multitude of related tasks through a single platform. It receives, processes and triages events to provide an all-encompassing solution for your analytic workflow — aggregating data, bundling and prioritizing alerts, and empowering analysts to investigate and document incidents.
* [CORTEX XSOAR](https://www.paloaltonetworks.com/cortex/xsoar) - Paloalto security orchestration, automation and response platform with full Incident lifecycle management and many integrations to enhance automations.
* [RTIR](https://www.bestpractical.com/rtir/) - Request Tracker for Incident Response (RTIR) is the premier open source incident handling system targeted for computer security teams. We worked with over a dozen CERT and CSIRT teams around the world to help you handle the ever-increasing volume of incident reports. RTIR builds on all the features of Request Tracker.
* [Zenduty](https://www.zenduty.com) - Zenduty is a novel incident management platform providing end-to-end incident alerting, on-call management and response orchestration, giving teams greater control and automation over the incident management lifecycle.

### Knowledge Bases

* [Windows Events Attack Samples](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES) ⭐ 2,622 | 🐛 5 | 🌐 HTML | 📅 2023-01-24 - Windows Events Attack Samples
* [Windows Registry Knowledge Base](https://github.com/libyal/winreg-kb) ⭐ 203 | 🐛 5 | 🌐 Python | 📅 2026-07-30 - Windows Registry Knowledge Base
* [Digital Forensics Artifact Knowledge Base](https://github.com/ForensicArtifacts/artifacts-kb) ⭐ 90 | 🐛 1 | 🌐 Python | 📅 2026-05-16 - Digital Forensics Artifact Knowledge Base

### Linux Distributions

* [Security Onion](https://github.com/Security-Onion-Solutions/security-onion) ⚠️ Archived - Special Linux distro aimed at network security monitoring featuring advanced analysis tools.
* [CCF-VM](https://github.com/rough007/CCF-VM) ⭐ 519 | 🐛 5 | 🌐 Shell | 📅 2022-10-21 - CyLR CDQR Forensics Virtual Machine (CCF-VM): An all-in-one solution to parsing collected data, making it easily searchable with built-in common searches, enable searching of single and multiple hosts simultaneously.
* [NullSec Linux](https://github.com/bad-antics/nullsec-linux) ⭐ 82 | 🐛 2 | 🌐 Shell | 📅 2026-04-17 - Security-focused Linux distribution with 140+ pre-installed forensic and offensive security tools, custom hardened kernel, and integrated incident response workflows.
* [The Appliance for Digital Investigation and Analysis (ADIA)](https://forensics.cert.org/#ADIA) - VMware-based appliance used for digital investigation and acquisition and is built entirely from public domain software. Among the tools contained in ADIA are Autopsy, the Sleuth Kit, the Digital Forensics Framework, log2timeline, Xplico, and Wireshark. Most of the system maintenance uses Webmin. It is designed for small-to-medium sized digital investigations and acquisitions. The appliance runs under Linux, Windows, and Mac OS. Both i386 (32-bit) and x86\_64 (64-bit) versions are available.
* [Computer Aided Investigative Environment (CAINE)](http://www.caine-live.net/index.html) - Contains numerous tools that help investigators during their analysis, including forensic evidence collection.
* [NST - Network Security Toolkit](https://sourceforge.net/projects/nst/files/latest/download?source=files) - Linux distribution that includes a vast collection of best-of-breed open source network security applications useful to the network security professional.
* [PALADIN](https://sumuri.com/software/paladin/) - Modified Linux distribution to perform various forensics task in a forensically sound manner. It comes with many open source forensics tools included.
* [SANS Investigative Forensic Toolkit (SIFT) Workstation](http://digital-forensics.sans.org/community/downloads) - Demonstrates that advanced incident response capabilities and deep dive digital forensic techniques to intrusions can be accomplished using cutting-edge open-source tools that are freely available and frequently updated.

### Linux Evidence Collection

* [MAGNET DumpIt](https://github.com/MagnetForensics/dumpit-linux) ⭐ 249 | 🐛 3 | 🌐 Rust | 📅 2023-11-21 - Fast memory acquisition open source tool for Linux written in Rust. Generate full memory crash dumps of Linux machines.
* [FastIR Collector Linux](https://github.com/SekoiaLab/Fastir_Collector_Linux) ⭐ 177 | 🐛 1 | 🌐 Python | 📅 2021-01-26 - FastIR for Linux collects different artifacts on live Linux and records the results in CSV files.

### Log Analysis Tools

* [Sigma](https://github.com/SigmaHQ/sigma) ⭐ 10,979 | 🐛 196 | 🌐 Python | 📅 2026-09-03 - Generic signature format for SIEM systems already containing an extensive ruleset.
* [Chainsaw](https://github.com/countercept/chainsaw) ⭐ 3,654 | 🐛 4 | 🌐 Rust | 📅 2026-08-25 - Chainsaw provides a powerful ‘first-response’ capability to quickly identify threats within Windows event logs.
* [Hayabusa](https://github.com/Yamato-Security/hayabusa) ⭐ 3,335 | 🐛 19 | 🌐 Rust | 📅 2026-09-04 - Hayabusa is a Windows event log fast forensics timeline generator and threat hunting tool created by the Yamato Security group in Japan.
* [LogonTracer](https://github.com/JPCERTCC/LogonTracer) ⭐ 3,230 | 🐛 21 | 🌐 Python | 📅 2026-08-02 - Tool to investigate malicious Windows logon by visualizing and analyzing Windows event log.
* [StreamAlert](https://github.com/airbnb/streamalert) ⭐ 2,890 | 🐛 90 | 🌐 Python | 📅 2023-10-23 - Serverless, real-time log data analysis framework, capable of ingesting custom data sources and triggering alerts using user-defined logic.
* [APT Hunter](https://github.com/ahmedkhlief/APT-Hunter) ⭐ 1,419 | 🐛 10 | 🌐 Python | 📅 2024-11-07 - APT-Hunter is Threat Hunting tool for windows event logs.
* [Zircolite](https://github.com/wagga40/Zircolite) ⭐ 851 | 🐛 0 | 🌐 Python | 📅 2026-08-24 - A standalone and fast SIGMA-based detection tool for EVTX or JSON.
* [SysmonSearch](https://github.com/JPCERTCC/SysmonSearch) ⭐ 433 | 🐛 15 | 🌐 JavaScript | 📅 2023-12-22 - SysmonSearch makes Windows event log analysis more effective and less time consuming by aggregation of event logs.
* [Lorg](https://github.com/jensvoid/lorg) ⭐ 215 | 🐛 6 | 🌐 HTML | 📅 2019-02-22 - Tool for advanced HTTPD logfile security analysis and forensics.
* [AppCompatProcessor](https://github.com/mbevilacqua/appcompatprocessor) ⭐ 214 | 🐛 6 | 🌐 Python | 📅 2021-09-15 - AppCompatProcessor has been designed to extract additional value from enterprise-wide AppCompat / AmCache data beyond the classic stacking and grepping techniques.
* [Logdissect](https://github.com/dogoncouch/logdissect) ⭐ 161 | 🐛 3 | 🌐 Python | 📅 2024-08-07 - CLI utility and Python API for analyzing log files and other data.
* [WELA](https://github.com/Yamato-Security/WELA) ⭐ 120 | 🐛 6 | 🌐 PowerShell | 📅 2026-09-03 - Windows Event Log Analyzer aims to be the Swiss Army knife for Windows event logs.
* [NullSec LogReaper](https://github.com/bad-antics/nullsec-logreaper) ⭐ 82 | 🐛 6 | 🌐 C | 📅 2026-04-16 - High-speed log analysis and forensics tool with multi-format parsing, pattern matching, timeline reconstruction and anomaly detection for incident response.
* [Event Log Explorer](https://eventlogxp.com/) - Tool developed to quickly analyze log files and other data.
* [Event Log Observer](https://lizard-labs.com/event_log_observer.aspx) - View, analyze and monitor events recorded in Microsoft Windows event logs with this GUI tool.
* [Kaspersky CyberTrace](https://support.kaspersky.com/13850) - Threat intelligence fusion and analysis tool that integrates threat data feeds with SIEM solutions. Users can immediately leverage threat intelligence for security monitoring and incident report (IR) activities in the workflow of their existing security operations.
* [Log Parser Lizard](https://lizard-labs.com/log_parser_lizard.aspx) - Execute SQL queries against structured log data: server logs, Windows Events, file system, Active Directory, log4net logs, comma/tab separated text, XML or JSON files. Also provides a GUI to Microsoft LogParser 2.2 with powerful UI elements: syntax editor, data grid, chart, pivot table, dashboard, query manager and more.

### Memory Analysis Tools

* [Volatility](https://github.com/volatilityfoundation/volatility) ⚠️ Archived - Advanced memory forensics framework.
* [Volatility 3](https://github.com/volatilityfoundation/volatility3) ⭐ 4,375 | 🐛 135 | 🌐 Python | 📅 2026-08-19 - The volatile memory extraction framework (successor of Volatility)
* \[MemProcFS] (<https://github.com/ufrisk/MemProcFS> ⭐ 4,317 | 🐛 9 | 🌐 C | 📅 2026-08-25) - MemProcFS is an easy and convenient way of viewing physical memory as files in a virtual file system.
* [LiME](https://github.com/504ensicsLabs/LiME) ⭐ 2,031 | 🐛 35 | 🌐 C | 📅 2026-04-05 - Loadable Kernel Module (LKM), which allows the acquisition of volatile memory from Linux and Linux-based devices, formerly called DMD.
* [AVML](https://github.com/microsoft/avml) ⭐ 1,119 | 🐛 5 | 🌐 Rust | 📅 2026-08-19 - A portable volatile memory acquisition tool for Linux.
* [MalConfScan](https://github.com/JPCERTCC/MalConfScan) ⭐ 498 | 🐛 4 | 🌐 Python | 📅 2023-12-22 - MalConfScan is a Volatility plugin extracts configuration data of known malware. Volatility is an open-source memory forensics framework for incident response and malware analysis. This tool searches for malware in memory images and dumps configuration data. In addition, this tool has a function to list strings to which malicious code refers.
* [inVtero.net](https://github.com/ShaneK2/inVtero.net) ⭐ 296 | 🐛 2 | 🌐 C# | 📅 2023-09-30 - Advanced memory analysis for Windows x64 with nested hypervisor support.
* [Orochi](https://github.com/LDO-CERT/orochi) ⭐ 275 | 🐛 92 | 🌐 JavaScript | 📅 2026-09-04 - Orochi is an open source framework for collaborative forensic memory dump analysis.
* [VolatilityBot](https://github.com/mkorman90/VolatilityBot) ⭐ 268 | 🐛 1 | 🌐 Python | 📅 2021-06-15 - Automation tool for researchers cuts all the guesswork and manual tasks out of the binary extraction phase, or to help the investigator in the first steps of performing a memory analysis investigation.
* [Evolve](https://github.com/JamesHabben/evolve) ⭐ 258 | 🐛 12 | 🌐 JavaScript | 📅 2017-11-21 - Web interface for the Volatility Memory Forensics Framework.
* [VolDiff](https://github.com/aim4r/VolDiff) ⚠️ Archived - Malware Memory Footprint Analysis based on Volatility.
* [Memoryze](https://www.fireeye.com/services/freeware/memoryze.html) - Free memory forensic software that helps incident responders find evil in live memory. Memoryze can acquire and/or analyze memory images, and on live systems, can include the paging file in its analysis.
* [Memoryze for Mac](https://www.fireeye.com/services/freeware/memoryze.html) - Memoryze for Mac is Memoryze but then for Macs. A lower number of features, however.
* [Rekall](http://www.rekall-forensic.com/) - Open source tool (and library) for the extraction of digital artifacts from volatile memory (RAM) samples.
* [WindowsSCOPE](http://www.windowsscope.com/windowsscope-cyber-forensics/) - Memory forensics and reverse engineering tool used for analyzing volatile memory offering the capability of analyzing the Windows kernel, drivers, DLLs, and virtual and physical memory.

### Memory Imaging Tools

* [Linux Memory Grabber](https://github.com/halpomeranz/lmg/) ⭐ 275 | 🐛 1 | 🌐 Shell | 📅 2020-02-01 - Script for dumping Linux memory and creating Volatility profiles.
* [Belkasoft Live RAM Capturer](http://belkasoft.com/ram-capturer) - Tiny free forensic tool to reliably extract the entire content of the computer’s volatile memory – even if protected by an active anti-debugging or anti-dumping system.
* [MAGNET DumpIt](https://www.magnetforensics.com/resources/magnet-dumpit-for-windows) - Fast memory acquisition tool for Windows (x86, x64, ARM64). Generate full memory crash dumps of Windows machines.
* [Magnet RAM Capture](https://www.magnetforensics.com/free-tool-magnet-ram-capture/) - Free imaging tool designed to capture the physical memory of a suspect’s computer. Supports recent versions of Windows.
* [OSForensics](http://www.osforensics.com/) - Tool to acquire live memory on 32-bit and 64-bit systems. A dump of an individual process’s memory space or physical memory dump can be done.

### OSX Evidence Collection

* [OSX Auditor](https://github.com/jipegit/OSXAuditor) ⭐ 3,133 | 🐛 8 | 🌐 JavaScript | 📅 2020-07-27 - Free Mac OS X computer forensics tool.
* [OSX Collector](https://github.com/yelp/osxcollector) ⚠️ Archived - OSX Auditor offshoot for live response.
* [macOS Artifact Parsing Tool (mac\_apt)](https://github.com/ydkhatri/mac_apt) ⭐ 1,081 | 🐛 8 | 🌐 Python | 📅 2026-08-21 - Plugin based forensics framework for quick mac triage that works on live machines, disk images or individual artifact files.
* [Knockknock](https://objective-see.com/products/knockknock.html) - Displays persistent items(scripts, commands, binaries, etc.) that are set to execute automatically on OSX.
* [The ESF Playground](https://themittenmac.com/the-esf-playground/) - A tool to view the events in Apple Endpoint Security Framework (ESF) in real time.

### Other Lists

* [Awesome Forensics](https://github.com/cugu/awesome-forensics) ⭐ 5,174 | 🐛 10 | 📅 2026-08-23 - A curated list of awesome forensic analysis tools and resources.
* [Didier Stevens Suite](https://github.com/DidierStevens/DidierStevensSuite) ⭐ 2,531 | 🐛 13 | 🌐 Python | 📅 2026-07-30 - Tool collection
* [List of various Security APIs](https://github.com/deralexxx/security-apis) ⭐ 990 | 🐛 3 | 📅 2026-09-01 - Collective list of public JSON APIs for use in security.
* [Awesome Event IDs](https://github.com/stuhli/awesome-event-ids) ⭐ 663 | 🐛 0 | 📅 2024-06-19 - Collection of Event ID resources useful for Digital Forensics and Incident Response.
* [Eric Zimmerman Tools](https://ericzimmerman.github.io/) - An updated list of forensic tools created by Eric Zimmerman, an instructor for SANS institute.

### Other Tools

* [sysmon-config](https://github.com/SwiftOnSecurity/sysmon-config) ⭐ 5,636 | 🐛 82 | 📅 2024-07-03 - Sysmon configuration file template with default high-quality event tracing
* [HELK](https://github.com/Cyb3rWard0g/HELK) ⭐ 3,931 | 🐛 60 | 🌐 Jupyter Notebook | 📅 2024-06-01 - Threat Hunting platform.
* [sysmon-modular](https://github.com/olafhartong/sysmon-modular) ⭐ 3,126 | 🐛 49 | 🌐 PowerShell | 📅 2026-08-31 - A repository of sysmon configuration modules
* [Stenographer](https://github.com/google/stenographer) ⚠️ Archived - Packet capture solution which aims to quickly spool all packets to disk, then provide simple, fast access to subsets of those packets. It stores as much history as it possible, managing disk usage, and deleting when disk limits are hit. It's ideal for capturing the traffic just before and during an incident, without the need explicit need to store all of the network traffic.
* [Kansa](https://github.com/davehull/Kansa/) ⭐ 1,661 | 🐛 46 | 🌐 PowerShell | 📅 2022-11-22 - Modular incident response framework in PowerShell.
* [Hindsight](https://github.com/obsidianforensics/hindsight) ⭐ 1,501 | 🐛 9 | 🌐 Python | 📅 2026-09-04 - Internet history forensics for Google Chrome/Chromium.
* [Raccine](https://github.com/Neo23x0/Raccine) ⭐ 983 | 🐛 21 | 🌐 C++ | 📅 2023-11-08 - A Simple Ransomware Protection
* [Munin](https://github.com/Neo23x0/munin) ⭐ 852 | 🐛 27 | 🌐 Python | 📅 2025-03-21 - Online hash checker for VirusTotal and other services.
* [Diffy](https://github.com/Netflix-Skunkworks/diffy) ⭐ 629 | 🐛 3 | 🌐 Python | 📅 2024-01-11 - DFIR tool developed by Netflix's SIRT that allows an investigator to quickly scope a compromise across cloud instances (Linux instances on AWS, currently) during an incident and efficiently triaging those instances for followup actions by showing differences against a baseline.
* [MFT Browser](https://github.com/kacos2000/MFT_Browser) ⭐ 332 | 🐛 0 | 🌐 PowerShell | 📅 2024-10-07 - MFT directory tree reconstruction & record info.
* [Hostintel](https://github.com/keithjjones/hostintel) ⭐ 274 | 🐛 1 | 🌐 Python | 📅 2021-04-13 - Pull intelligence per host.
* [rastrea2r](https://github.com/rastrea2r/rastrea2r) ⭐ 238 | 🐛 8 | 🌐 Python | 📅 2021-08-01 - Allows one to scan disks and memory for IOCs using YARA on Windows, Linux and OS X.
* [imagemounter](https://github.com/ralphje/imagemounter) ⭐ 127 | 🐛 6 | 🌐 Python | 📅 2023-02-09 - Command line utility and Python package to ease the (un)mounting of forensic disk images.
* [Fileintel](https://github.com/keithjjones/fileintel) ⭐ 123 | 🐛 0 | 🌐 Python | 📅 2020-12-04 - Pull intelligence per file hash.
* [PowerSponse](https://github.com/swisscom/PowerSponse) ⭐ 40 | 🐛 10 | 🌐 PowerShell | 📅 2022-03-18 - PowerSponse is a PowerShell module focused on targeted containment and remediation during security incident response.
* [traceroute-circl](https://github.com/CIRCL/traceroute-circl) ⭐ 40 | 🐛 2 | 🌐 Perl | 📅 2024-10-09 - Extended traceroute to support the activities of CSIRT (or CERT) operators. Usually CSIRT team have to handle incidents based on IP addresses received. Created by Computer Emergency Response Center Luxembourg.
* [PyaraScanner](https://github.com/nogoodconfig/pyarascanner) ⭐ 27 | 🐛 0 | 🌐 Python | 📅 2018-06-03 - Very simple multi-threaded many-rules to many-files YARA scanning Python script for malware zoos and IR.
* [domfind](https://github.com/diogo-fernan/domfind) ⭐ 25 | 🐛 0 | 🌐 Python | 📅 2019-05-18 - Python DNS crawler for finding identical domain names under different TLDs.
* [Cortex](https://thehive-project.org) - Cortex allows you to analyze observables such as IP and email addresses, URLs, domain names, files or hashes one by one or in bulk mode using a Web interface. Analysts can also automate these operations using its REST API.
* [Crits](https://crits.github.io/) - Web-based tool which combines an analytic engine with a cyber threat database.
* [IPASIS](https://ipasis.com/) - Real-time IP reputation and email validation API for investigating suspicious interactions. Returns an Interaction Trust Score (0-100) combining VPN/proxy/Tor detection with email risk assessment in a single API call.
* [RaQet](https://raqet.github.io/) - Unconventional remote acquisition and triaging tool that allows triage a disk of a remote computer (client) that is restarted with a purposely built forensic operating system.
* [Stalk](https://www.percona.com/doc/percona-toolkit/2.2/pt-stalk.html) - Collect forensic data about MySQL when problems occur.
* [Scout2](https://nccgroup.github.io/Scout2/) - Security tool that lets Amazon Web Services administrators assess their environment's security posture.
* [sqhunter](https://github.com/0x4d31/sqhunter) - Threat hunter based on osquery and Salt Open (SaltStack) that can issue ad-hoc or distributed queries without the need for osquery's tls plugin. sqhunter allows you to query open network sockets and check them against threat intelligence sources.
* [X-Ray 2.0](https://www.raymond.cc/blog/xray/) - Windows utility (poorly maintained or no longer maintained) to submit virus samples to AV vendors.

### Playbooks

* [ThreatHunter-Playbook](https://github.com/OTRF/ThreatHunter-Playbook) ⭐ 4,652 | 🐛 6 | 🌐 Python | 📅 2026-01-12 - Playbook to aid the development of techniques and hypothesis for hunting campaigns.
* [IRM](https://github.com/certsocietegenerale/IRM) ⭐ 1,141 | 🐛 0 | 📅 2025-04-11 - Incident Response Methodologies by CERT Societe Generale.
* [AWS Incident Response Runbook Samples](https://github.com/aws-samples/aws-incident-response-runbooks/tree/0d9a1c0f7ad68fb2c1b2d86be8914f2069492e21) ⭐ 1,106 | 🐛 1 | 📅 2026-08-28 - AWS IR Runbook Samples meant to be customized per each entity using them. The three samples are: "DoS or DDoS attack", "credential leakage", and "unintended access to an Amazon S3 bucket".
* [PagerDuty Incident Response Documentation](https://response.pagerduty.com/) - Documents that describe parts of the PagerDuty Incident Response process. It provides information not only on preparing for an incident, but also what to do during and after. Source is available on [GitHub](https://github.com/PagerDuty/incident-response-docs) ⭐ 1,050 | 🐛 3 | 🌐 Dockerfile | 📅 2026-07-02.
* [Counteractive Playbooks](https://github.com/counteractive/incident-response-plan-template/tree/master/playbooks) ⭐ 803 | 🐛 5 | 🌐 Makefile | 📅 2024-05-07 - Counteractive PLaybooks collection.
* [Phantom Community Playbooks](https://github.com/phantomcyber/playbooks) ⭐ 552 | 🐛 17 | 🌐 Python | 📅 2026-09-01 - Phantom Community Playbooks for Splunk but also customizable for other use.
* [GuardSIght Playbook Battle Cards](https://github.com/guardsight/gsvsoc_cirt-playbook-battle-cards) ⭐ 435 | 🐛 0 | 📅 2024-05-10 - A collection of Cyber Incident Response Playbook Battle Cards

### Process Dump Tools

* [Microsoft ProcDump](https://docs.microsoft.com/en-us/sysinternals/downloads/procdump) - Dumps any running Win32 processes memory image on the fly.
* [PMDump](http://www.ntsecurity.nu/toolbox/pmdump/) - Tool that lets you dump the memory contents of a process to a file without stopping the process.

### Sandboxing/Reversing Tools

* [Ghidra](https://github.com/NationalSecurityAgency/ghidra) ⭐ 74,376 | 🐛 1,937 | 🌐 Java | 📅 2026-09-02 - Software Reverse Engineering Framework.
* [Radare2](https://github.com/radareorg/radare2) ⭐ 24,739 | 🐛 829 | 🌐 C | 📅 2026-09-04 - Reverse engineering framework and command-line toolset.
* [Cutter](https://github.com/rizinorg/cutter) ⭐ 19,669 | 🐛 493 | 🌐 C++ | 📅 2026-08-22 - Free and Open Source Reverse Engineering Platform powered by rizin.
* [CAPA](https://github.com/mandiant/capa) ⭐ 6,170 | 🐛 298 | 🌐 Python | 📅 2026-09-01 - detects capabilities in executable files. You run it against a PE, ELF, .NET module, or shellcode file and it tells you what it thinks the program can do.
* [Cuckoo](https://github.com/cuckoosandbox/cuckoo) ⚠️ Archived - Open Source Highly configurable sandboxing tool.
* [Rizin](https://github.com/rizinorg/rizin) ⭐ 3,852 | 🐛 553 | 🌐 C | 📅 2026-09-04 - UNIX-like reverse engineering framework and command-line toolset
* [CAPEv2](https://github.com/kevoreilly/CAPEv2) ⭐ 3,471 | 🐛 63 | 🌐 Python | 📅 2026-09-03 - Malware Configuration And Payload Extraction.
* [Viper](https://github.com/viper-framework/viper) ⚠️ Archived - Python based binary analysis and management framework, that works well with Cuckoo and YARA.
* [StringSifter](https://github.com/fireeye/stringsifter) ⭐ 762 | 🐛 12 | 🌐 Python | 📅 2026-07-24 - A machine learning tool that ranks strings based on their relevance for malware analysis.
* [Cuckoo-modified](https://github.com/spender-sandbox/cuckoo-modified) ⭐ 406 | 🐛 173 | 🌐 Python | 📅 2017-11-21 - Heavily modified Cuckoo fork developed by community.
* [Mastiff](https://github.com/KoreLogicSecurity/mastiff) ⚠️ Archived - Static analysis framework that automates the process of extracting key characteristics from a number of different file formats.
* [Visualize\_Logs](https://github.com/keithjjones/visualize_logs) ⭐ 146 | 🐛 3 | 🌐 HTML | 📅 2022-12-27 - Open source visualization library and command line tools for logs (Cuckoo, Procmon, more to come).
* [Cuckoo-modified-api](https://github.com/keithjjones/cuckoo-modified-api) ⭐ 23 | 🐛 0 | 🌐 Python | 📅 2016-10-31 - Python library to control a cuckoo-modified sandbox.
* [Any Run](https://app.any.run/) - Interactive online malware analysis service for dynamic and static research of most types of threats using any environment.
* [Hybrid-Analysis](https://www.hybrid-analysis.com/) - Free powerful online sandbox by CrowdStrike.
* [Intezer](https://analyze.intezer.com/#/) - Intezer Analyze dives into Windows binaries to detect micro-code similarities to known threats, in order to provide accurate yet easy-to-understand results.
* [Joe Sandbox (Community)](https://www.joesandbox.com/) - Joe Sandbox detects and analyzes potential malicious files and URLs on Windows, Android, Mac OS, Linux, and iOS for suspicious activities; providing comprehensive and detailed analysis reports.
* [Metadefender Cloud](https://www.metadefender.com) - Free threat intelligence platform providing multiscanning, data sanitization and vulnerability assessment of files.
* [Reverse.IT](https://www.reverse.it/) - Alternative domain for the Hybrid-Analysis tool provided by CrowdStrike.
* [Threat.Zone](https://app.threat.zone) - Cloud based threat analysis platform which include sandbox, CDR and interactive analysis for researchers.
* [Valkyrie Comodo](https://valkyrie.comodo.com) - Valkyrie uses run-time behavior and hundreds of features from a file to perform analysis.
* [Virustotal](https://www.virustotal.com) - Free online service that analyzes files and URLs enabling the identification of viruses, worms, trojans and other kinds of malicious content detected by antivirus engines and website scanners.
* [Yomi](https://yomi.yoroi.company) - Free MultiSandbox managed and hosted by Yoroi.

### Scanner Tools

* [LOKI](https://github.com/Neo23x0/Loki) ⭐ 3,788 | 🐛 18 | 🌐 Python | 📅 2026-01-12 - Free IR scanner for scanning endpoint with yara rules and other indicators(IOCs).
* [Fenrir](https://github.com/Neo23x0/Fenrir) ⭐ 776 | 🐛 1 | 🌐 Shell | 📅 2022-02-12 - Simple IOC scanner. It allows scanning any Linux/Unix/OSX system for IOCs in plain bash. Created by the creators of THOR and LOKI.
* [Spyre](https://github.com/spyre-project/spyre) ⭐ 181 | 🐛 13 | 🌐 Go | 📅 2026-03-17 - Simple YARA-based IOC scanner written in Go

### Timeline Tools

* [Timesketch](https://github.com/google/timesketch) ⭐ 3,406 | 🐛 217 | 🌐 Python | 📅 2026-09-03 - Open source tool for collaborative forensic timeline analysis.
* [Plaso](https://github.com/log2timeline/plaso) ⭐ 2,148 | 🐛 276 | 🌐 Python | 📅 2026-08-28 -  a Python-based backend engine for the tool log2timeline.
* [Aurora Incident Response](https://github.com/cyb3rfox/Aurora-Incident-Response) ⭐ 1,077 | 🐛 41 | 🌐 JavaScript | 📅 2023-10-05 - Platform developed to build easily a detailed timeline of an incident.
* [Morgue](https://github.com/etsy/morgue) ⚠️ Archived - PHP Web app by Etsy for managing postmortems.
* [Highlighter](https://www.fireeye.com/services/freeware/highlighter.html) - Free Tool available from Fire/Mandiant that will depict log/text file that can highlight areas on the graphic, that corresponded to a key word or phrase. Good for time lining an infection and what was done post compromise.

### Videos

* [The Future of Incident Response](https://www.youtube.com/watch?v=bDcx4UNpKNc) - Presented by Bruce Schneier at OWASP AppSecUSA 2015.

### Windows Evidence Collection

* [LOKI](https://github.com/Neo23x0/Loki) ⭐ 3,788 | 🐛 18 | 🌐 Python | 📅 2026-01-12 - Free IR scanner for scanning endpoint with yara rules and other indicators(IOCs).
* [Fibratus](https://github.com/rabbitstack/fibratus) ⭐ 2,539 | 🐛 42 | 🌐 Go | 📅 2026-09-01 - Tool for exploration and tracing of the Windows kernel.
* [PowerForensics](https://github.com/Invoke-IR/PowerForensics) ⭐ 1,444 | 🐛 64 | 🌐 C# | 📅 2023-11-16 - Live disk forensics platform, using PowerShell.
* [RegRipper](https://github.com/keydet89/RegRipper3.0) ⭐ 716 | 🐛 9 | 🌐 Perl | 📅 2026-05-27 - Open source tool, written in Perl, for extracting/parsing information (keys, values, data) from the Registry and presenting it for analysis.
* [FastIR Collector](https://github.com/SekoiaLab/Fastir_Collector) ⭐ 521 | 🐛 11 | 🌐 Python | 📅 2021-01-26 - Tool that collects different artifacts on live Windows systems and records the results in csv files. With the analyses of these artifacts, an early compromise can be detected.
* [PSRecon](https://github.com/gfoss/PSRecon/) ⭐ 495 | 🐛 4 | 🌐 PowerShell | 📅 2017-07-29 - PSRecon gathers data from a remote Windows host using PowerShell (v2 or later), organizes the data into folders, hashes all extracted data, hashes PowerShell and various system properties, and sends the data off to the security team. The data can be pushed to a share, sent over email, or retained locally.
* [MEERKAT](https://github.com/TonyPhipps/Meerkat) ⭐ 483 | 🐛 0 | 🌐 PowerShell | 📅 2024-11-15 - PowerShell-based triage and threat hunting for Windows.
* [DFIR ORC](https://dfir-orc.github.io/) - DFIR ORC is a collection of specialized tools dedicated to reliably parse and collect critical artifacts such as the MFT, registry hives or event logs. DFIR ORC collects data, but does not analyze it: it is not meant to triage machines. It provides a forensically relevant snapshot of machines running Microsoft Windows. The code can be found on [GitHub](https://github.com/DFIR-ORC/dfir-orc) ⭐ 447 | 🐛 10 | 🌐 C++ | 📅 2026-07-29.
* [Hoarder](https://github.com/muteb/Hoarder) ⭐ 216 | 🐛 3 | 🌐 Python | 📅 2020-10-19 - Collecting the most valuable artifacts for forensics or incident response investigations.
* [AChoir](https://github.com/OMENScan/AChoir) ⭐ 193 | 🐛 1 | 🌐 C++ | 📅 2022-06-20 - Framework/scripting tool to standardize and simplify the process of scripting live acquisition utilities for Windows.
* [Invoke-LiveResponse](https://github.com/mgreen27/Invoke-LiveResponse) ⭐ 150 | 🐛 0 | 🌐 PowerShell | 📅 2022-02-22 -  Invoke-LiveResponse is a live response tool for targeted collection.
* [IRTriage](https://github.com/AJMartel/IRTriage) ⭐ 138 | 🐛 0 | 🌐 AutoIt | 📅 2016-04-21 - Incident Response Triage - Windows Evidence Collection for Forensic Analysis.
* [Panorama](https://github.com/AlmCo/Panorama) ⭐ 41 | 🐛 1 | 🌐 Python | 📅 2017-02-11 - Fast incident overview on live Windows systems.
* [Crowd Response](http://www.crowdstrike.com/community-tools/) - Lightweight Windows console application designed to aid in the gathering of system information for incident response and security engagements. It features numerous modules and output formats.
* [Cyber Triage](http://www.cybertriage.com) - Cyber Triage has a lightweight collection tool that is free to use. It collects source files (such as registry hives and event logs), but also parses them on the live host so that it can also collect the executables that the startup items, scheduled, tasks, etc. refer to. It's output is a JSON file that can be imported into the free version of Cyber Triage. Cyber Triage is made by Sleuth Kit Labs, which also makes Autopsy.
* [IREC](https://binalyze.com/products/irec-free/) - All-in-one IR Evidence Collector which captures RAM Image, $MFT, EventLogs, WMI Scripts, Registry Hives, System Restore Points and much more. It is FREE, lightning fast and easy to use.
* [IOC Finder](https://www.fireeye.com/services/freeware/ioc-finder.html) - Free tool from Mandiant for collecting host system data and reporting the presence of Indicators of Compromise (IOCs). Support for Windows only. No longer maintained. Only fully supported up to Windows 7 / Windows Server 2008 R2.
* [KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape) - Kroll Artifact Parser and Extractor (KAPE) by Eric Zimmerman. A triage tool that finds the most prevalent digital artifacts and then parses them quickly. Great and thorough when time is of the essence.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-04._
