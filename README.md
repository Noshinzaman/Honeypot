# Honeypot
# Honeypot Assignment

**Time spent:** **5** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

 I deployed MHN in an UBUNTU 14.04 instance using Google Cloud Services with the following honeypots: shockpot, Dionaea, snort, suricata, p0f, elastichoney.
The setup:

    create a gcloud account and a project
    in the cloud launcher, select Ubuntu Trusty (14, because the newer versions don't work)
    allow HTTP traffic and all ports
    in Compute Engine, select the VM instance and open SSH in a separate browser window
    in the opened window, install MHN by executing the following commands: sudo apt-get update sudo apt-get install git -y $ cd /opt $ sudo git clone https://github.com/RedolentSun/mhn.git $ cd mhn $ sudo ./install.sh
    whenever prompted, answer n or blank


<img src="https://user-images.githubusercontent.com/89932088/143962231-46113e5f-7e60-4a66-b872-63350f435351.gif">

### Dionaea Honeypot Deployment (Required)

 Demonstration:

    I used nmap to scan the networknmap
    An example of the data captured by the honeypot (example: IDS logs including IP, request paths, alerts triggered) 
<img src="https://user-images.githubusercontent.com/89932088/143962376-9725bcf2-1779-482b-800e-f05f33f997b2.gif">
<img src="https://user-images.githubusercontent.com/89932088/143962445-b04bc807-6933-4b11-b91e-7f826780abc4.gif">

### Database Backup (Required) 


    Additional attack demos/writeups
    Captured malicious payload (see above)
    Enhanced logging of exploit post-exploit activity (example: attacker-initiated commands captured and logged)
    
    https://github.com/Noshinzaman/Honeypot/blob/main/session.JSON
    

### Deploying Additional Honeypot(s) (Optional)

#### X Honeypot

    HTTPS enabled (self-signed SSL cert)
    A web application with both authenticated and unauthenticated footprint
    Database back-end
    Custom exploits (example: intentionally added SQLI vulnerabilities)
    Custom traps (example: modified version of known vulnerability to prevent full exploitation)
    Custom IDS alert (example: email sent when footprinting detected)
    Custom incident response (example: IDS alert triggers added firewall rule to block an IP)





