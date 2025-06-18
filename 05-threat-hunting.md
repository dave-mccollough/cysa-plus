# Threat Hunting

## Threat Modeling

- Identifiies and assess the possible threat actors and attack vectors that pose a risk to the security of an app, network, or other systems
- Threat modeling can be used agains corporate networks in general at a large scale
- How can an attack be performed
- What is the potential impact to CIA of data
- How likely is the risk to occur
- What mitigations are in place

- Adversary Capability
  - Formal classification of the resource and expertise available to a particular threat actor
    - Aquired and Augmented
    - Developed
    - Advanced
    - Integrated

- Attack Surface
  - The point at which a network or application received external connections or inputs/outputs that are potential vectors to be exploited by a threat actor
  - To determine attack surface, you need to inventory your assets
    - Network
    - Websites or cloud services
    - Custom software applications

- Attack Vector
  - The path a threat actor takes to gain unauthorized access to a system
    - Cyber
    - Human
    - Physical

- Likelihood
  - Chance of a threat being realized, typically expressed as a perecentage

- Impact
  - Cost of a security incident typically expressed in dollars

## Threat Hunting

- Cybersecurity technique designed to detect the presence of threats that have not been discovered by normal security monitoring
- Potenentially less disruptive than penetration testing
- Relies on tools developed for regular security monitoring and incident response
- Assume existing rules and configurations established in monitoring systems have failed

- Establishing a hypothesis
  - Dervived from threat modeling
  - Based on potential events with higher likelihood and impact

- Profiling threat actors and activiities
  - Creation of scenarios that show how a prospective attacker might attempt an intrusion and their objectives might be

- 1. Analyze Network Traffic
- 2. Analyze the executable process list
- 3. Identify how the malicious process was executed

- Threat hunting consumes a lot of time and resources, but can yield significant benefits, including
  - Improve detection capabilities
  - Integrate Intelligence
  - Reduce Attack Surface
  - Block Attack Vectors
  - Identify Critical Assets

## Open Source Intelligence

- Use of publicaly available information, plus the tools used to aggregate and search for it
- OSINT can allow any attacker to develop any number of strategies for comprising a target
- Publically available infomration
- Social Media
- Dating sites
- HTML code
- Metadata

## Google Hacking

- Open source intelligence technique that uses Google search operators to locate vulnerable web servers and applications

- Quotes
  - Specifies an exact phrase and makes search more precise
  - `"Joe Smith"`

- NOT
  - Excludes results that contain a word or quoted phrase
  - `CySA -Dion Training`
    - Returns all CySA results without Dion Training

- AND
  - Reqires both search terms
  - `Dave AND McCollough`

- OR
  - Requires either search term
  - `Dave OR McCollough`

- Scope
  - Selects the scope of the search, including
    - site
    - filetype
      - Search only for pdf files
      - `filetype:pdf`
    - related
    - allintitle
    - allinurl
    - allinanchor

- URL Modifiers

- Google Hacking Database (GHDB) [URL](https://www.exploit-db.com/google-hacking-database)
  - Provides search strings optimized for locating vulerable websites and services

- Shodan.io
  - Search engine optimzed to identify vulnerable internet attached devices

## Profiling Techniques

- Who works at a specific company
- Email Harvesting
  - OSINT technique used to gather email addresses from a domain
- Once a list of email addresses have been created, they can be used in social engineering attempts
- Tools
  - Pipl.com
  - Peekyou.com
  - Echosec.net

## Harvesting Techniques

- Uses OSINT to gather information about a domain

- whois
  - Public listing of all registered domains and their registered administrators

- DNS Zone Transfer
  - Method of replicating DNS databases across a set of DNS servers that is often used during the recon phase of an attack
  - If your DNS service is misconfigured, a DNS zone transfter could be allowed

## AbuselPDB

- Community driven database that keeps track of IP addresses reported for abusive behavior
- Enables organizations to take a proactive approch to cybersecurity
- Constally being updated with new information from a global community of users
- AbuseIPDB can be used to monitor logs for suspicious behaviors
- Data in AbuseIPDB is not considered to be 100% accurate - combine it with other security measures

## Deep Web and Dark Web

- Not easily accessible through traditional search engines

- Deep Web
  - Portion of internet not indexed by search engines
  - Can contain sensitive information not meant to be searchable by general public
    - Private databases
    - Subscription based websites
    - Other content not publically accessible
      - Medical and scientific research
      - University libraries
      - Government database

- Dark Web
  - Specifc part of the deep web that's used for illegal activity
    - Buying and selling drugs and weapons, personal information - credit card data

## Bug Bounty Hunting

- A way for companies to crowdsource security testing of their software services and applications to identify and address potential security issues
- Approach testing in a responsible and ethical mander
- Avoid causing harm, disruption to systems, applications or services
- Obtain necessary permissions and system for tracking, triaging and remediating vulnerabilities