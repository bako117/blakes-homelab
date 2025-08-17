#At-Home SOC 
##Summary
**First Started:** August 2025

**End-Date:** Still ongoing

**Overview:** This project acts as a homebase for my at-home SOC. It is designed to ingest data and monitor security in my home network environment. It simulates how a SOC ingests, parses, and analyzes logs from different environment components. The focus is on hands-on security monitoring, SIEM customization, and developing a repeatable workflow that mirrors enterprise SOC environments.

**Goal/Idea:** Create a SOC in my home network with these goals in mind:
- Learn how to install and configure security tools accross my environment
- Engineer alerts to trigger based off of log data ingested
- Make my home network stronger and more resistant to threats
- Utilize automation and create workflows to reduce any analysis time

##Skills Learned
- Security Tool Deployment
- Detection Creation
- Log Ingestion Development
  
##Sub-Project Table
Creating an at-home SOC is unfortunately not as simple as downloading a single piece of software and hitting run. This project has me constantly learning and required many separate work sessions to get my SOC into it's current state. Below are all the lab writeups related to this project. 
| Project | Tools Utilized | Summary | Date Started |
|---|---|---|---|
| [Creating a Splunk App For PiHole](pihole-ta.md) | - Splunk Enterprise | Designing a Splunk TA for properly ingesting Splunk logs, then validating and creating dashboards utilizing newly formatted data | 8/15/25 |
| [Setting Up Splunk Enterprise](splunk-setup.md) | - VMWare<br>- Linux<br>- Splunk Enterprise | Setting up a server to run Splunk Enterprise and ingesting pihole logs | 8/11/25 |
| [Pi-hole Deployment](pihole.md) | - Raspberry PI<br>- Pihole<br>- Linux | Setup DNS filtering across the network through the use of pihole | 8/3/25 |
