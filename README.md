<h1>Active Directory Lab</h1>

<h2>Description</h2>
This project demonstrates the setup of a basic Active Directory Domain Controller in a virtualized lab environment using Windows Server 2022 and Windows 10. The lab includes DNS, DHCP, and RAS features, with domain-joined client machines, simulating a small office IT infrastructure.
<br />

<h2>Network Setup</h2>

| MACHINE  | OS                        | IP ADDRESS      | ROLE                                | NICs             |
|----------|---------------------------|-----------------|-------------------------------------|------------------|
| THLDC    | Windows Server 2022 Eval  | 172.16.0.1      | Domain Controller, DNS, DHCP, RAS,  | NAT + Internal   |
| Client01 | Windows 10 Eval           | DHCP - assigned | Domin-joined Client                 | Internal only    |



<h2>System Workflow</h2>
@@ -29,11 +28,10 @@ This project demonstrates the setup of a basic Active Directory Domain Controlle
- <b>Windows Server 2022 (Evaluation)</b>
- <b>Windows 10 (Evaluation)</b>

<h2>Program walk-through:</h2>
<h2>Network Diagram:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="images/networkdiagram.png" height="80%" width="80%" >
<br />
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
