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
<li>Diagnosed DNS resolution failures using dig and system logs</li>
<li>Verified reverse DNS lookups using PTR records</li>
 <li>Troubleshot network connectivity and interface issues using ip and ping</li>
 <li>Flushed DNS cache using resolvectl to validate changes</li>
 <li>Managed DNS and system services using systemctl</li>
 <li>Performed end-to-end connectivity testing between Linux server and Windows client</li>
</ul>





<h2>Screenshots</h2>
