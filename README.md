# AWS-Cloud-Networking-Lab
This project demonstrates the deployment and administration of a segmented AWS cloud networking environment using Amazon EC2, VPC networking, Bastion host architecture, Linux administration, and Apache web services.
<h2>Description</h2>

The lab simulates a basic enterprise-style infrastructure model featuring:</p>
<ul>
<li> Public Bastion host</li>
<li>Private internal App Server</li>
 <li>Security Group-based access controls</li>
 <li>SSH key authentication</li>
   <li>Apache web hosting</li>
   <li>Internal-only server management</li>
</ul>

<b>Technologies Used</b>
<ul>
<li>Amazon Web Services (AWS)</li>
<li>Amazon EC2</li>
 <li>VPC Networking</li>
 <li>Security Groups</li>
<li>Amazon Linux 2023</li>
 <li>Apache HTTP Server</li>
 <li>SSH/PEM Key Authentication</li>
 <li>Linux Networking Tools</li>
</ul>

<h2>Architecture</h2>
<p><b>Public Bastion Host</b></p>
<ul>
<li>Public IPv4 enabled</li>
<li>Used as administrative entry point </li>
 <li>Accessible from external internet via SSH</li>
</ul>

<p><b>Private App Server</b></p>
<ul>
<li>Private IPv4 only</li>
<li>No public internet exposure</li>
 <li>Accessible only through Bastion host</li>
</ul>

<b>Key Skills Demonstrated</b>
<ul>
<li>Cloud infrastructure deployment</li>
<li>Linux server administration</li>
 <li>SSH remote management</li>
 <li>Security Group configuration</li>
 <li>Bastion host implementation</li>
 <li>Public/private subnet architecture</li>
 <li>Apache web server deployment</li>
 <li>Internal VPC communication</li>
 <li>Troubleshooting network connectivity</li>
</ul>

<b>Validations Performed</b>
<ul>
<li>Verified SSH connectivity from local workstation to Bastion host</li>
<li>Validated private server access through Bastion architecture</li>
 <li>Confirmed internal VPC routing functionality</li>
 <li>Tested outbound internet access and DNS resolution</li>
 <li>Configured and validated Apache web server availability</li>
 <li>Implemented Security Group referencing for secure administrative access</li>
</ul>

<b>Example Linux Commands Used</b>
<ul>
<li>ip addr</li>
<li>ip route</li>
 <li>ping 8.8.8.8</li>
 <li>curl ifconfig.me</li>
 <li>systemctl status httpd</li>
 <li>ss -tulnp</li>
  <li>ssh -i CloudLab-Key.pem ec2-user@10.0.3.17</li>
</ul>

## Architecture Diagram

```text
                    Internet
                        │
                        │
                Public SSH Access
                        │
                        ▼
        ┌──────────────────────────┐
        │   CloudLab-Bastion       │
        │   Public EC2 Instance    │
        │   Public IP + Private IP │
        └──────────────────────────┘
                        │
                 Internal SSH
                        │
                        ▼
        ┌──────────────────────────┐
        │      App-Server          │
        │   Private EC2 Instance   │
        │   Private IP Only        │
        └──────────────────────────┘
```
<h2>Screenshots</h2>

<p align="center">
Bastion EC2 Details: <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/Bastion_Instance%20.png" height="80%" width="80%" 
<br />
<br />
AppServer Private IP:  <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/App_Server_Details(private_IP).png" height="80%" width="80%" 
<br />
<br />
Apache Browser Page: <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/Apache_Web_Server.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Security Group Rules:  <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/Security_Group_Rules.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Bastion SSH Into App Server: <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/Bastion_to_AppServer_SSH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Linux Networking Commands:  <br/>
<img src="https://github.com/jasons559/AWS-Cloud-Networking-Lab/blob/main/images/Terminal_Validation.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


</p>
