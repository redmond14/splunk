## This lab is designed for security practitioners to gain hands-on experience. The goal is to utilize both vendor-provided and open-source security tools and applications.

### Part One: Basic Environment Setup
- Set up Splunk to serve as your central log management system.
- Configure Firewall Interfaces, routing, NAT, IPS policies etc.
- Ensure that firewall logs are being sent to and properly parsed by Splunk. Firepower integration via eStreamer to Splunk. 

### Part Two: Integration with Other Systems
- Configure Splunk to collect and analyze logs from both Windows and Linux endpoints.
- Use Sysmon for enhanced visibility into endpoint activities.
- Utilize the Atomic Red Team tool (Offensive tool) to generate logs and test your defenses.
- Purple Team Activity Tracking leveraging Vectr, an open-source tool, to document and track purple team activities.

### Part Three: Proactive Threat Hunting
- This section focuses on more advanced Threat Hunting
- Use Zeek to analyze pre-recorded PCAP files for beaconing activity.

### Part Four: Cyber Deception
Cyber deception is a highly effective yet underutilized concept in security. Many organizations overlook its potential, despite its ability to detect unusual behavior with minimal investment. Since adversaries typically do not anticipate deception tactics, strategically placing traps throughout the network can significantly enhance security.