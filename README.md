# Description
The script listens for network packets on a specified network interface, displaying relevant details such as source and destination IPs, protocol types, and ports for TCP and UDP packets. It also provides a preview of each packet's payload for deeper inspection.

Note: Running a packet sniffer may require administrative privileges. Ensure you have permission to capture packets on any network to avoid legal issues.

# Features
IP Layer Information: Shows source and destination IP addresses and protocol type.
TCP/UDP Layer Information: Displays source and destination ports for TCP and UDP packets.
ICMP Detection: Detects and displays ICMP packet details.
Payload Preview: Shows the first 20 bytes of the payload (if available) for quick inspection.

# Usage
1. Installation: Make sure scapy is installed: pip install scapy
2. Running the Script: Save the Script: Save this code as packet_sniffer.py.
Run: Use sudo for permissions, especially on Linux/MacOS: sudo python packet_sniffer.py
Specify Network Interface (Optional): To target a specific interface, pass it to sniff() like this: sniff(iface="eth0", prn=packet_callback, filter="ip", store=False)
Filter by Protocol: Use filter="tcp" or filter="udp" to capture only specific protocols: sniff(prn=packet_callback, filter="tcp", store=False)
3. Stopping the Script: Press Ctrl + C in the terminal to stop capturing packets.

# Contribution
Contributions are welcome! Feel free to open issues or submit pull requests to improve this script or add new features.
