# Active-Directory

## Description

Designed an active directory home lab by running it as a service on windows server 2022 and further configuring the server to function as a domain controller. Hosted and configured a splunk server on ubuntu server platform to allow for enterprise level SIEM features over the web. Installed Sysmon on host machine to ingest host's telemetry for retrieval on splunk server dashboard for further analysis. The goal behind this home lab project is to gain exposure and familiarity with common tools used in the cybersecurity industry and also to simulate a scenario where tools and services used in the industry can be safegaurded from malicious events through log analysis and threat detection.

## System Design
![AD_Diagram](https://github.com/Akbram98/Active-Directory/blob/main/AD_Diagram.png)

##### Title: Diagram above showing the design of system components and interactions for this active directory project

## Getting Started

This project wouldn't be possible without the many cybersecurity projects and information sessions posted by the popular youtuber: [MyDFIR](https://www.youtube.com/@MyDFIR). If you are like me, a person who wants to gain relevant skills in the field of cybersecurity and also to have a clear view of the path necessary for a career in SOC, then be sure to check out his youtube channel as he provides many resources to help you. If you would like to build out a project just like this one, be sure to watch and follow along with the project series that was posted by him: [ACTIVE DIRECTORY PROJECT](https://www.youtube.com/watch?v=5OessbOgyEo&t=1s).

## Prerequisites
 - [Install Virtual Box](https://www.virtualbox.org/)

## Learning outcomes
  - Installed and configured a splunk server using the ubuntu server platform
  - Installed and configured Windows Server 2022 to run as a domain controller with active directory services
  - Configured hosts to send application, security and application event logs to the splunk server via Splunk Forwarder
  - Configured hosts to send Sysmon event logs to the splunk server via Splunk Forwarder
  - Setup an attacking machine via Kali Linux which performs a brute-force attack using crowbar to gain user credentials
  - Enabled RDP on target machine to prepare for a malicious attack simulation through remote login attempts
  - Analysed event logs on splunk server after the brute-force attack to observe what kind of telemetry was generated
  - Installed Atomic Redteam to test TTPs provided by MITRE ATT&CK against the current system, and observed what telemetry this generated on splunk server
  - Practiced System Design using Draw.io to provide a graphical overview of the systems and interaction between components
