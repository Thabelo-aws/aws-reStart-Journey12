<h2>Troubleshooting a Network Issue (AWS)</h2>

<p>
In this hands-on AWS lab, I assumed the role of a Cloud Support Engineer and investigated a customer-reported networking issue affecting an Apache web server hosted on Amazon EC2. The customer was unable to ping the server or access its web page through a browser, requiring a systematic analysis of the AWS networking environment to identify and resolve the root cause.
</p>
<img width="249" height="225" alt="image" src="https://github.com/user-attachments/assets/118795cf-12e0-45da-bc38-4cdec04a31f9" />

<h3>Project Objectives</h3>
<ul>
    <li>Analyze a real-world customer networking scenario.</li>
    <li>Troubleshoot connectivity issues within an AWS Virtual Private Cloud (VPC).</li>
    <li>Validate EC2 instance accessibility and web server functionality.</li>
    <li>Identify and resolve security-related configuration errors.</li>
</ul>


<h3>Technologies & Services Used</h3>
<ul>
    <li>Amazon EC2</li>
    <li>Amazon VPC</li>
    <li>Security Groups</li>
    <li>Network ACLs (NACLs)</li>
    <li>Route Tables</li>
    <li>Internet Gateway</li>
    <li>Apache HTTP Server (httpd)</li>
    <li>Linux Command Line (SSH)</li>
</ul>

<h3>Key Activities</h3>
<ul>
    <li>Connected securely to an Amazon Linux EC2 instance using SSH.</li>
    <li>Verified the status of the Apache HTTP Server and started the httpd service.</li>
    <li>Tested web server accessibility using the instance's public IP address.</li>
    <li>Reviewed VPC components including subnets, route tables, internet gateways, network ACLs, and security groups.</li>
    <li>Performed network connectivity tests to validate internet access and server reachability.</li>
    <li>Analyzed inbound and outbound network traffic rules affecting the application.</li>
    <li>Identified a misconfigured Security Group that was blocking HTTP traffic to the Apache server.</li>
    <li>Updated the required security rules and verified successful connectivity.</li>
</ul>

<h3>Outcome</h3>
<p>
Successfully diagnosed and resolved the customer's networking issue by correcting Security Group configuration errors that prevented access to the Apache web server. After implementing the fix, the server became reachable via its public IP address and the Apache test page loaded successfully, restoring expected functionality.
</p>

<h3>Skills Demonstrated</h3>
<ul>
    <li>AWS Networking Troubleshooting</li>
    <li>Cloud Support Operations</li>
    <li>VPC Configuration Analysis</li>
    <li>Security Group Management</li>
    <li>Linux Administration</li>
    <li>SSH Connectivity</li>
    <li>Root Cause Analysis</li>
    <li>Web Server Troubleshooting</li>
</ul>
