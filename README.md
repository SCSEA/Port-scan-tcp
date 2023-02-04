# Port-scan using tcp

Port Scanner using TCP scan

To establish a TCP connection, the host must perform a three-way handshake. Follow these steps to perform the action −

Step 1 − Packet with SYN flag set

In this step, the system that is trying to initiate a connection starts with a packet that has the SYN flag set.

Step 2 − Packet with SYN-ACK flag set

In this step, the target system returns a packet with SYN and ACK flag sets.

Step 3 − Packet with ACK flag set

At last, the initiating system will return a packet to the original target system with the ACK flag set.

Nevertheless, the question that arises here is if we can do port scanning using ICMP echo request and reply method (ping sweep scanner) then why do we need TCP scan? The main reason behind it is that suppose if we turn off the ICMP ECHO reply feature or using a firewall to ICMP packets then ping sweep scanner will not work and we need TCP scan.

# Installation

apt update && apt upgrade -y

pkg install git

pkg install python

pkg install python2

pkg install python3

git clone https://github.com/Yousuf9963/Port-scan-tcp.git

cd Port-scan-tcp

chmod +x *

python3 scan.py

Donation: https://www.buymeacoffee.com/junioprogrammer
