# Network Packet Analyzer

**Overview**

This Python script is designed to sniff packets on a network interface for a specified duration, analyze the packets, and display the results in a tabular format. It utilizes the Scapy library for packet manipulation and the tabulate library for generating tables.

**Packet Analysis**

The script is structured to analyze packets of various protocols, including TCP, UDP, ICMP, and DNS. Upon sniffing a packet, the script determines its type and extracts relevant information such as source and destination IP addresses, source and destination ports, and payload. It then categorizes the packets based on their protocol and stores the analyzed information in a list.

**Packet Sniffing**

The sniff_packets function continuously sniffs packets for a specified duration using Scapy's sniff function. It calls the process_packet function for each packet sniffed.

**User Interaction**

The script prompts the user to input the duration for packet sniffing. It validates the input to ensure it is a positive number. After the specified duration, it displays the analyzed packets in a table format.

**Requirements**

The script requires Python 3.x along with the following libraries:

+ Scapy: A powerful packet manipulation tool.
+ tabulate: A Python library for generating tables from tabular data.

**Install the required dependencies:**

Use pip to install the required Python dependencies
+ Scapy: `pip install scapy`
+ tabulate: `pip install tabulate`
+ If you're using Windows, you need to install **Npcap** for Scapy to function properly. You can download the Npcap installer from the Npcap website and follow the installation instructions.
