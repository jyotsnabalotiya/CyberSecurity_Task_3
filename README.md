# CyberSecurity_Task_3

## Task: Perform a Basic Vulnerability Scan on Your PC
### Tool Used: Nessus


## Objective

Perform a vulnerability assessment on my local computer using Nessus Essentials, a free vulnerability scanner, to identify common security issues and risks.

## Procedure/ Commands used

### Step 1
''' sudo dpkg -i Nessus-10.9.2-ubuntu1604_amd64.deb '''
This command uses dpkg (Debian package manager) to install the Nessus package on the system. Make sure the filename matches the version you downloaded.
- image1.png

### Step 2
''' sudo systemctl start nessusd '''
This command starts the Nessus service, which runs the vulnerability scanner in the background and allows you to access the Nessus web interface.
- image2.png

### Step 3
''' sudo systemctl enable nessusd '''
This command configures the system to start the Nessus service automatically every time the computer boots up.
- image3.png

### Step 4
''' sudo systemctl status nessusd '''
This command shows the current status of the Nessus service, indicating whether it is active (running), inactive, or if there are any errors.
- image4.png

### Step 5
https://localhost:8834 (open this in your browser)
This URL opens the Nessus web interface on your local machine where you can complete setup, configure scans, and view results.
Note: The connection is secure (HTTPS), so your browser may show a security warning due to a self-signed certificate — you can safely proceed.
- image5.png

### Step 6
Host Discovery Scan Page
In the Nessus web interface, the Host Discovery Scan page allows you to perform a quick scan to identify live hosts on your network or your local machine. This scan checks which devices are online and responsive, helping to map your network before a full vulnerability assessment.
       You can set the target IP address or hostname here (e.g., localhost or your local IP).
       This scan is useful for detecting active systems and basic open ports.
       It runs faster than a full vulnerability scan and helps in identifying what’s reachable.
- image6.jpeg

### Step 7
Nessus Basic Network Scan Results
Basic Network Scan performed using Tenable Nessus Essentials on the host 192.168.60.3. The scan completed successfully, revealing vulnerabilities categorized by severity using the CVSS v3.0 base scoring system.
-- Scan Details:
                Policy: Basic Network Scan
                Status: Completed
                Scanner: Local Scanner
                Start Time: 12:21 AM
                End Time: 1:07 AM
                Duration: ~1 hour

-- Vulnerability Summary:
                Critical: 2
                High: 4
                Medium: 7
                Low: 80
                Info: Additional informational findings
The vulnerability distribution is visualized in a pie chart, allowing quick identification of the most severe security risks. These findings highlight the importance of remediation steps to reduce potential attack surfaces and improve the overall security posture of the scanned host.
- image7.jpeg

## Conclusion
Performing a basic vulnerability scan on my local PC using Nessus Essentials helped identify several security weaknesses and potential risks. The scan provided detailed insights into critical and high-severity vulnerabilities that could be exploited if left unaddressed. By reviewing the results, I gained a better understanding of the security posture of my system and identified practical mitigation steps to improve it.
Regular vulnerability scanning is essential for maintaining system security and protecting against emerging threats. Tools like Nessus Essentials make it accessible to users by providing comprehensive scanning capabilities for free. Moving forward, I plan to apply the recommended fixes and schedule periodic scans to ensure my system remains secure.




