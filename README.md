Vulnerability Management with Nessus

I use Nessus Essentials to scan local VMs hosted on VMWare Workstation in order run credentialed scans to discover vulnerabilities, remediate some of the vulnerabilities, then perform a rescan to verify remediation.

I start by creating a Windows 10 VM with a bridged NIC, setup windows 10 with admin/Password1(for learning purposes only), and perform a non-credentialed scan. I inspect the scan to understand the information on it. 

Next I follow the steps provided by Tenable for a credentialed scan: https://community.tenable.com/s/article/Scanning-with-non-default-Windows-Administrator-Account.<br/>
-Enable Remote Registry<br/>
-Enable Printer and File Sharing<br/>
-Disable Firewall<br/>
-Disable User Account Control <br/>

I also Install Deprecated firefox on the VM to show the vulnerabilities it has. 
I reconfigure my scan with credentials into Nessus, re-scan and observe the new report.

Finally i remediate the vulnerablilities by uninstalling the deprecated firefox and updating windows, which seems to remove most of the vulnerabilities detected.

I have included a video demonstration: https://youtu.be/cESyROD4hS4

