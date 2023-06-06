---
title: Nessus Update
date: 2023-06-05 12:00:00 -0500
categories: [windows, security]
tags: [nessus,vulnerability,windows]
---

<img src="/assets/img/posts/nessus-update/nessus-update.jpg" alt="Nessus Update" style="height:400px; width:600px;" />

# Update Nessus Scanner (WIN10)

## Download the Latest Version of Nessus
* Navigate to = <https://www.tenable.com/downloads> 

## Launch the Trellix Desktop Application and disable Threat Prevention and Firewall settings 
* In the WIN10 taskbar, right click on the Trellix icon and click McAfee Endpoint Security
* On the top right, click the down arrow, click Administrator Log On and enter the password.
* Click on Threat Prevention, and uncheck the following boxes
  * Enable Access Protection
  * Enable Exploit Prevention
  * Enable On-Access Scan
  * Enable ScriptScan (scans scripts in browser only)	
    * Click Apply
* Click on Firewall, and uncheck the following boxes
  * Enable Firewall
    * Click Apply

## Install The Latest Version of Nessus on the Machine
* Navigate to where you saved the Nessus installation file and install the application.

## Confirm the Latest Version of Nessus is Installed
* Open a browser and navigate to <https://localhost:8834>
  * Nessus may take a while “compiling plugins” during the initial login
* Log into Nessus with the necessary credentials
* Click “settings” and the version should now reflect the 10.4.2 update.
  * If the version didn’t reflect the updated number, launch the Services application and restart the “Tenable Nessus” service, reboot and check again.

## Reboot the machine and the Trellix/McAfee Settings Will be Re-enabled

  _Congratulations. That's it!!! You have successfully updated the Nessus scanner._