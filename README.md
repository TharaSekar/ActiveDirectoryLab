<h1>Active Directory Home Lab</h1>


<h2>Description</h2>
This project demonstrates the setup of a basic Active Directory Domain Controller in a virtualized lab environment using Windows Server 2022 and Windows 10. The lab includes DNS, DHCP, and RAS features, with domain-joined client machines, simulating a small office IT infrastructure.
<br />

<h2>Network Setup</h2>
| Machine&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| OS&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| IP Address&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Role&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| NICs&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
<br />
|---------------|-------------------------|------------------|-----------------------------------------|------------------|
<br />
| DC&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Windows Server 2022&nbsp;| 172.16.0.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Domain Controller, DNS, DHCP, RAS&nbsp;| NAT + Internal |
<br />
| Client01&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Windows 10 Eval&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| DHCP-assigned&nbsp;| Domain-joined Client&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Internal only&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
  

<h2>System Workflow</h2>

- The DC uses a static IP on the internal network (e.g., 172.16.0.1)
- The client connects to the DC via internal network only
- The DC connects to the internet via NAT and shares it to the client using RAS
- DHCP is used to assign IPs to clients
- DNS on the DC resolves domain-related names

- <h2>Tools Used</h2>

- <b>VirtualBox (hosted on Windows 11)</b>
- <b>Windows Server 2022 (Evaluation)</b>
- <b>Windows 10 (Evaluation)</b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
