Enterprise Network Security with FortiGate

Course Final Project — A complete enterprise network security implementation using FortiGate firewalls, covering topology design, policy configuration, VPN tunnels, and traffic monitoring.



## Project Overview

This project demonstrates the design and configuration of an enterprise-grade network security infrastructure using a FortiGate firewall running FortiOS. All configurations were performed via the CLI and are documented here for reproducibility.

### What's Covered

 Network Topology - Multi-zone design: LAN, DMZ, WAN 

 Firewall Policies - Zone-based rules 

 VPN - Site-to-site VPN 

 Monitoring - Traffic logs, event logs, threat reports 

Logging  - Logging with Splunk 


## Repository Structure

/Assets
   
   Topology.png
   
  /Assets/Screenshots
  
	    ├── dashboard.png

        ├── policies.png

        ├── vpn-status.png

        ├── traffic-logs.png

        ├── cli-config.png

        └── security-profiles.png
  /Assets/Configs
	
      ├── FG1.conf

      ├── FG2.conf



IP addressing Scheme 

Site 1 Subnet - 192.168.10.0/24 

	FG1 Internal IP – 192.168.10.99
	FG1 Wan2 IP – 10.0.0.1 - Used for One Side of Tunnel
	
Site 2 Subnet –192.168.20.0/24 

 	FG2 Internal IP– 192.168.20.99 
	FG2 Wan2 IP - 10.0.0.2 - Used for Other Side of Tunnel 


Host Machine 1 – 192.168.10.110 

	Server 1 Running on HM1 – 192.168.10.111 
	Splunk Logging – 192.168.10.110 - Splunk running on HM1 

Host Machine 2 – 192.168.20.110

	Server 2 Running on HM2 – 192.168.20.111 


Attacker Kali – 192.168.10.20 - Attacking the Firewall FG1 as the gateway 


## Author

Emmett Tuck — Computer Information Systems Administration — BCIT — 2026

---

*All configurations are for educational purposes. Do not apply to production environments without review.*
