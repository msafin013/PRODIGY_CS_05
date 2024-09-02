 Packet Sniffer Tool

 Overview

This packet sniffer tool is designed for educational and research purposes. It allows users to capture and analyze network packets in real-time, providing insight into network protocols, traffic patterns, and network security concepts.

 Features

- Capture network packets on specified network interfaces.
- Display source and destination IP addresses.
- Identify protocols (TCP, UDP, etc.) used in packets.
- Display source and destination port numbers.
- Analyze and display packet payload data.

 Requirements

 System Requirements

   Operating System: Linux distribution (e.g., Ubuntu, Debian, Fedora).
   Network Interface: Access to a network interface (e.g., eth0, wlan0).

 Software Requirements

- Python: Version 3.6 or later.
- Libraries:
  - scapy for packet manipulation.
  - pyshark (optional) for advanced packet analysis.
  - tshark for command-line packet analysis with pyshark.

 Installing Dependencies

Run the following commands to install the necessary dependencies:

bash
sudo apt-get update
sudo apt-get install python3 python3-pip
pip3 install scapy
pip3 install pyshark   Optional, for advanced analysis
sudo apt-get install tshark   Required if using Pyshark


 Usage

 Cloning the Repository

Clone the repository to your local machine:

bash
git clone https://github.com/your-username/packet-sniffer-tool.git
cd packet-sniffer-tool


 Running the Tool

To run the packet sniffer tool, execute it with root privileges:

bash
sudo python3 packet_sniffer.py


 Output

The tool will capture and display the following information for each packet:

- Source IP Address
- Destination IP Address
- Protocol (e.g., TCP, UDP)
- Source and Destination Ports (if applicable)
- Payload Data

 Stopping the Tool

Press Ctrl+C to stop the packet sniffer.

 Filtering Traffic

Modify the script to filter specific traffic types (e.g., only TCP traffic):

python
sniff(filter="tcp", prn=packet_callback, store=0)


 Ethical Considerations

This tool is intended for educational purposes only. Please use it responsibly and legally:

- Authorized Networks Only: Use this tool only on networks you own or have explicit permission to monitor.
- Respect Privacy: Do not intercept private communications without consent.
- No Malicious Use: Avoid using this tool for unauthorized access or data theft.

 Educational Usage

This tool is perfect for:

- Learning network protocols and packet analysis.
- Debugging network issues.
- Exploring cybersecurity concepts in a controlled environment.
                                                                
