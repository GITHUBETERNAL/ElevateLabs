# ElevateLabs
Daily Tasks of Elevate labs
: daily tasks are in their respective folder


Interview Questions:
############################################################################################################
Task 1:

1.What is an open port?
Ans: An open port is a network port on a device that is configured to accept incoming traffic from connections. It indicates that a service or an application is actively listening for traffic.

2.How does Nmap perform a TCP SYN scan?
Ans: Nmap sends TCP packets with SYN flag set to the target ports. Target reolies determine port state:
  - SYN-ACK recieved : port is open. Nmap sends RST to avoid full hand shake.
  - RST recieved : port is closed.
  - No response or ICMP unrechable : port is filtered.
No full TCP handshake occurs. Scan remains stealthy.

3.What risks are associated with open ports?
Ans:  - Unauthorized access: Open ports expose services that maybe  exploitable.
      - Vulnerability exposure: Services with known flaws can be targated.
      - Reconnaissance: Attacker enumerate open ports to plan intrusions.
      - Malware entry: Open ports can be entry points for worms, trojans etc.
      - Denial-of-Service: Services on opne ports may be overwhelmed.
      - Lateral movement: Compromised ports facilitate internal network traversal.

4.Explain the difference between TCP and UDP scanning.
Ans:  - TCP scanning performs connection-oriented checks. It may complete or simulate handshakes, eg. SYN scan. It detects service relibility but is slower and more detectable.
      - UDP scanning sends datagrams without handshake. If no ICMP unrechable is returned, port may be open. Less reliable, slower due to lack of acknowledgements and often blocked by firewalls.

5.How can open ports be secured?
Ans:  - Close unused ports via firewwall or service configuration.
      - Use host-based and network firewalls to restrict access.
      - Apply service-specific access control, eg. IP whitelisting.
      - Implement intrusion detection/prevention systems.
      - Use port knocking or VPNs for controlled access.
      - Regularly patch exposes services.
      - Monitor with port scanning tools to detect unauthorized changes.
      
6.What is a firewall's role regarding ports?
Ans:  - Close unused ports via firewall or service configuration.
      - use host-based  and netweok firewalls to restrict access.
      - Apply service-specific access control, eg. IP whitelisting.
      - Implement intrusion detection/prevention syetem.
      - Use port knocking or VPNs for controlled access.
      - Regularly patch exposed services.
      - Monitor with port scanning tools to detect unauthorized changes.
  
7.What is a port scan and why do attackers perform it?
Ans:  - A port scan is the systematioc probing of a target system's network ports to identify which are open, closed or filterd. Attackers perform it to:
      - Discoveractive services and applications.
      - Identify vulnerabilities tied to specific port.
      - Map the attack surface of a network or host.
      - Enumerate operating systems and service versions.
      - Prepare for targated exploitation or lateral movement.
      
8.How does Wireshark complement port scanning?
Ans: - Wireshark captures and analyzes packer level traffic. It completements port scanning by: 
      - verifying scan behaviour, eg., SYN, RST, ICMP responses.
      - Detecting scan signatures and patterns.
      - Monitoring target responses in real time.
      - Validating firewall and intrusion detection reactions.
      - Revealing unintended service leaks or misconfigured responses.

############################################################################################################
Task 2

1. 
