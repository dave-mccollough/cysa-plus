# Clasifying Threats

## Threat Classification

- Known Threats
  - Can be identified using basic signature or pattern matching
    - Malware
      - Software intentionally designed to cause damage to a computer, server, client or computer network
    - Documented Exploits
      - Software, data, or a sequence of commands that takes advantage of a vulnerability to cause unintended behavior or gain unauthorized access to sensative data
    
- Unknown THreat
  - Threat that cannot be identified using basic signature or pattern matching
    - Zero day exploits
      - Unkown exploit that exppses a vulnerabiltiy in software or hardware
      - Can cause problems before being identified
    - Obfuscated malware code
      - Malicious code that has been compressed, encrypted or encoded to limit the ability to analyze it
    - Behavior based detection
      - Malware detection method that evaluates an object based on its intended actions before it actually executes the behavior
    - Recycled Threats
      - Combining or modifying existing exploit code to create new threats
      - Not easily identified by automatic scanning
    - Known Unknowns
      - Malware classification that contains obfuscation techniques that circumvent signature matching and detection
    - Unknown Unknowns
      - Malware tha contains new attack vectors and exploits

## Threat Actors

- Individuals or groups that want to do harm to networks, hardware, software, or steal secure data

- Script Kiddie
  - Uses other peoples tools for their attacks
  - Do not have skills to make their own tools
  - Often don't understand what their doing
- Insider Threat
  - Individuals who have authorized access to an organizations network, policies, procedures and business practices
  - Intentional or unintentional harm
- Competitor
  - Business attempting to conduct syber expionage against another organization
- Organized Crime
  - Hacking for computer fraud for financial gains
- Hactivist
  - Politically minded hacker
  - Targets governments or individuals to advance their political ideaology
- Nation State
  - Group of hackers with capabiltiy, organization and funding
  - Intent to hack system or network
  - Conducts highly covert hacks over long periods of time
  - Typically affiliated with a government
- APT (Advance Persistent Threat)
  - Hacker that establishes a long term presence on a network to gain sensitive information
  - Harvest sensative data, intelectual property and other sensitive information
- Supply Chain Threats

## Malware

- Types of Malware
  - Commodity
    - Malicious software applications
    - Available for sale
    - Easy to obtain and use 
  - Targeted
    - Developed or deployed with a specific target in mind
  - Zero Day
    - Vulnerability that is discovered or exploited before a vendor can patch or fix
    - Mostly used for high value attacks
  - APT (Advance Persistent Threat)
    - Hackers ability to obtain, maintain and diversify access to network systems using exploits and malware
    - Considered a known unkown threat
    - Usually targe financial, healthcare and governments to get PII datasets
  - Command and Control
    - Infrastructure of hosts and services 
    - Used to direct, distribute and control malware over botnets
  - Persistence
    - Ability of a threat actor to maintain covert access to a target or network

## Threat Research

- Repuational Threat Research
  - Reputational Data 
    - Blacklists of known threat sources including malware signatures, IP address ranges and DNS domains
- Indicator of Comprimise (IoC)
  - Residual sign that an asset or network has been attacked or is under attack
  - Unauthorized softare or files
  - Suspicious Emails
  - Suspicious registry and file system changes
  - Unknown port or protocol usage
- Indicator or Attack (IoA)
  - Evidence of an ongoing intrusion attack
- Behavioral Threat Research
  - Correlation of IoC into attack patterns
- Tactics, Techniques and Procedures (TTP)
  - Behavior patterns used in cyberattacks and adversary actions
  - DDoS
  - Virus or worms
  - Network Reconnaissance
  - ATP
  - Data Exfiltration
- Port Hopping
  - ATP C2 application uses any port to communiate with, and jump between different ports
- Fast Flux DNS
  - Rapid changes in IP addres associated with a domain
- Data Exfiltration
  - Unauthorized transfer of data from a computer or device

## Attack Frameworks

- These models can be used individually or combined
- Lockheed Martin Kill Chain
  - Describes the stages a threat actor progresses a network intrusion
  - Older framework
  - Used to identify a defensive course of accation the counter the progress of an attack at each stage
  - 7 Step method
    - 1. Reconnaissance
      - Attacker determines what methods to use to complete the phases of the attack
      - Starts with passive information gathering and then moves into active scanning
    - 2. Weaponization
      - Attacker couples payload code to enable access with exploit code 
      - Attacer will use a vulneratbility to execute on a target system
    - 3. Delivery
      - Attacker identifies a vector to transmit the weaponized code to the targe enviornment
    - 4. Exploitation
      - Weaponzied code is executed on the target system
    - 5. Installation
      - Weaponized code runs a remote access tool to achieve persistence on the target system
    - 6. Command and Control (C2)
      - Weaponized code establishes an outbound channel to remote server
      - Remove can be used to control the remote access tool possiblky downloading additional tools to progress the attack
    - 7. Actions on objectives
      - Attacker uses the access achieved to collect information from target systems and transfer to remote system or other goals/motives

- MITRE ATT&CK Framework
  - Knowledge based that lists and explains specific advesary tactics, techiques and common knowledge or procedures
  - Pre-ATT&CK tactics matrix aligns with the reconnaissance and weaponization phases of the Kill Chain

- Diamond Model of Intrusion Analysis
  - Framework for analyzing cybersecurity incidents and intrusions by exploring the relationship between four core features
    - Advesary
    - Capability 
    - Infrastructure
    - Victim

## Indicator Management

- Structured Threat Information eXpression(STIX)
  - Standard terminology for IoCs and indicating relationships between them
  - Included as part of the OASIS Cyber Threat Intelligence (CTI) network
  - Expressed as JSON
- Trusted Automated eXchange of Indicator Information (TAXII)
  - Protocol for supplying codified infomration to automate incident detecion and analysis
  - Subscribers obtain updates to their data for their analysis tools using TAXII
- OpenIOC
  - Framework by Mandian that uses XML formated files for supplying codified information to automate incident detection and analysis
- Malware Information Sharing Project (MISP)
  - Server platform for cyber threat intelligence
  - Propietary format
  - Support OpenIOC definitions
  - Can import/export STIX over TAXII