# Active-Directory

## Description

This project involves the creation and configuration of an Active Directory home lab, utilizing Windows Server 2022 as a domain controller. The lab setup includes:

- **Windows Server 2022**: Configured to run Active Directory services and function as a domain controller.
- **Splunk Server**: Deployed on an Ubuntu Server platform to provide enterprise-level Security Information and Event Management (SIEM) capabilities accessible over the web.
- **Sysmon Installation**: Installed on the host machine to collect telemetry data, which is then ingested and visualized on the Splunk server dashboard for detailed analysis.
The primary objective of this project is to gain practical experience with key cybersecurity tools and techniques. By simulating real-world scenarios, the project demonstrates how industry-standard tools and services can be protected against malicious activities through effective log analysis and threat detection.

## Getting Started

This project wouldn't be possible without the many cybersecurity projects and information sessions posted by the popular youtuber: [MyDFIR](https://www.youtube.com/@MyDFIR). If you are like me, a person who wants to gain relevant skills in the field of cybersecurity and also to have a clear view of the path necessary for a career in SOC, then be sure to check out his youtube channel as he provides many resources to help you. If you would like to build out a project just like this one, be sure to watch and follow along with the project series that was posted by him: [ACTIVE DIRECTORY PROJECT](https://www.youtube.com/watch?v=5OessbOgyEo&t=1s).

## System Design
![AD_Diagram](https://github.com/Akbram98/Active-Directory/blob/main/AD_Diagram.png)

##### Title: Diagram above shows the design of system components and interactions for this active directory project

## Project Setup Phase 1 - Virtual Box VM setup

![Virtual Box Setup](https://github.com/Akbram98/Active-Directory/blob/main/VBox_Setup.png)

### Setup Prerequisites
 - [Install Virtual Box](https://www.virtualbox.org/)
 - [Download Windows 10 msi using Windows installation media](https://www.microsoft.com/en-ca/software-download/windows10)
 - [Download Windows Server 2022 msi](https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022)
 - [Download Ubuntu server msi](https://ubuntu.com/download/server)
 - [Download Kali Linux prebuilt VM](https://www.kali.org/get-kali/#kali-virtual-machines)

## Project Setup Phase 2 - Target Machine

![Target Machine Diagram](https://github.com/Akbram98/Active-Directory/blob/main/TargetMachine_Diagram.png)

### Setup Prerequisites
- [Download Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Download Splunk Universal Forwarder Installer](https://www.splunk.com/en_us/products/splunk-enterprise.html)
- [Download sysmonconfig.xml file](https://github.com/olafhartong/sysmon-modular/blob/master/sysmonconfig.xml)

## Project Setup Phase 3 - Servers and Attacking machine

![Server and Attack Machine diagram](https://github.com/Akbram98/Active-Directory/blob/main/Servers%26AttackMachine_Diagram.png)

### Setup Prerequisites
- [Download sysmonconfig.xml file in Windows Server 2022 machine](https://github.com/olafhartong/sysmon-modular/blob/master/sysmonconfig.xml)
- [Download Sysmon in Windows Server 2022 machine](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Download Splunk Universal Forwarder Installer in Windows Server 2022 machine](https://www.splunk.com/en_us/products/splunk-enterprise.html)
   
## Learning outcomes
- Installed and configured a Splunk server on an Ubuntu platform to centralize log management and analysis.
- Set up and configured Windows Server 2022 as a domain controller with Active Directory services.
- Configured hosts to forward application, security, and system event logs to the Splunk server using Splunk Forwarder.
- Enabled Sysmon on hosts and configured them to send event logs to the Splunk server via Splunk Forwarder.
- Deployed a Kali Linux machine to conduct a brute-force attack using Crowbar to simulate credential theft.
- Enabled Remote Desktop Protocol (RDP) on target machines to simulate and analyze remote login attack scenarios.
- Analyzed event logs on the Splunk server post-attack to identify and interpret telemetry data.
- Implemented Atomic Red Team to test MITRE ATT&CK Tactics, Techniques, and Procedures (TTPs), and analyzed the resulting telemetry on the Splunk server.
- Practiced system design using Draw.io to create graphical representations of system architecture and component interactions.

