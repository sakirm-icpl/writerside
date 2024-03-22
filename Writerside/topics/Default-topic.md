![logo.png](logo.png)
![logo_1.png]
# Invinsense Agent

The Invinsense Agent is a powerful security tool that brings together many popular open-source security programs into one package. It works on different operating systems and combines the features of Osquery, Sysmon, Wazuh, and antivirus software like Windows Defender for Windows and ClamAV for Linux. This means it can keep an eye on everything happening on your system, watch network activity, check files for changes, and look for malware, all to keep your devices safe.

Along with the Invinsense Agent, there's a central place for managing everything called the management console. This console lets administrators see what's going on with all the Invinsense Agents installed across the network in real-time. They can see if each tool is working correctly and quickly deal with any security issues or odd behavior. This setup makes it easier for organizations to watch over and control their computer systems, keeping everything running smoothly and securely.

1. Introduction

Welcome to the Invinsense Agent Installation, Upgrade, and Uninstallation Guide. This document provides step-by-step instructions for installing, upgrading, and uninstalling the Invinsense Agent software.
~~~~
2. Installation
   Installation Steps
   Follow these steps to install the Invinsense Agent:

2.1 Copy or Download InvinSetup.msi file on any directory

![InvinSetup_Property.png](InvinSetup_Property.png)

2.2 Open CMD as Administrator privileges where InvinSetup.msi file is present.

![cmd_path.png](cmd_path.png)

2.3 Run the Installation Command.	

`msiexec /i InvinSetup.msi /l*vx setup.log ApiUrl="<api_url:5001>" Groups="<groups>" TOKEN="<token>"`

Here ApiUrl is your Inivinsense-xdr Api url and Group is on which group you want to add this agent and TOKEN is authentication token for API connection.

![installation_command.png](installation_command.png)

2.3.1 Installation status.

![installation_statuspng](installation_status.png)

After Installation Invinsense you can see Invinsense 4.7.2 Tray will show on you machine.

![Tray_statuspng](Tray_status.png)

2.4 Check this machine is connected or not on our server.

2.4.1 Check machine hostname

![Installation_dashboard.png](Installation_dashboard.png)

Here You can see my machine is connected with my wazuh server.