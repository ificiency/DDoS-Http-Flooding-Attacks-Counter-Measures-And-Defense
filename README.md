DISTRIBUTED DENIAL OF SERVICE (DDoS) SIMULATION AND MITIGATION


Overview

This project demonstrates Distributed Denial of Service (DDoS) attacks, specifically HTTP flooding at the application layer, and explores countermeasures. Using tools like High Orbit Ion Cannon (HOIC) for attacks and Anti-DDoS Guardian for defense, this simulation provides insights into the mechanisms of DDoS attacks and effective mitigation strategies.


Features

DDoS Simulation:
Simulates HTTP GET/POST flood attacks using HOIC on a virtualized environment.

Defense Mechanisms:
Implements mitigation strategies with Anti-DDoS Guardian, including IP blocking and traffic monitoring.

Traffic Analysis:
Captures and analyzes network traffic during attacks using Wireshark.

Performance Evaluation:
Demonstrates the impact of DDoS attacks on system performance and evaluates defense strategies.




Prerequisites

Virtualization tools (e.g., Oracle VirtualBox or VMware)

Virtual machines:
	Windows 11
	Windows Server 2019
	Windows Server 2022
	Parrot Security OS


Tools:
	High Orbit Ion Cannon (HOIC)
	Anti-DDoS Guardian (or similar)
	Wireshark



Installation

Set Up Virtual Machines:

	Install and configure the listed virtual machines on your virtualization platform.
	Ensure they are connected to the same virtual network.
	Install Required Tools:

Download and install HOIC on the Windows VMs.
	Install Anti-DDoS Guardian on the Windows 11 VM.
	Set up Wireshark on the Parrot Security VM.



Usage

   Simulate DDoS Attack:

	Launch HOIC on Windows VMs.
	Configure target IP (e.g., Parrot Security VM) and initiate the attack using the “Fire the Laser” button.


   Mitigate DDoS Attack:

	Start Anti-DDoS Guardian on the Windows 11 VM.
	Use its features to monitor traffic, block IPs, and control bandwidth to defend against incoming traffic.


   Analyze Traffic:

	Use Wireshark on the Parrot Security VM to capture packets during the attack.
	Analyze the traffic logs for insights into the attack and defense mechanisms.


Simulation Output

   DDoS Impact:
	Increased latency and eventual unresponsiveness of the targeted machine.


   Defense Results:
	Reduced malicious traffic and restored system responsiveness using Anti-DDoS Guardian.




Code Structure

This project focuses on practical demonstration; however, key steps and tools are structured as follows:

  HOIC Setup:
	Configurations for HTTP GET/POST flood attacks.

  Anti-DDoS Guardian:
	Defense configuration for traffic monitoring and mitigation.

  Wireshark:
	Traffic capture and analysis steps.


Example Output

  Wireshark Log:
	Captured logs showing high traffic volume during the attack.

  Anti-DDoS Guardian Log:
	Monitored traffic and blocked malicious IPs.



Example:

Action Taken: IP Blocked
Incoming Bytes: 1,234,567
Blocked Source IP: 192.168.1.100



Contributing

Contributions are welcome! Please follow these steps:

	Fork the repository.
	Create a new branch (git checkout -b feature-branch).
	Commit your changes (git commit -m "Add new feature").
	Push to the branch (git push origin feature-branch).
	Open a Pull Request.


License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Tools like HOIC, Anti-DDoS Guardian, and Wireshark for enabling this simulation.
The open-source community for providing resources and support.




