ARP(Address Resoltion Protocol) is a process in which a user sends a broadcast address, asking for a MAC Address from a specific IP address. Then the user with the specific IP address sends it MAC Address as its response. Then the former user updates the IP in the ARP Cache.

1) Perform Password stealing (over plaintext) using ARP Cache Poisoning attacks.
- ARP Cache Poisoning is a process in which an attacker intervens in between the arp transfer and spoofs the identity of the user the requested IP Address.It also sends the attackers MAC address to the requested user which causes it to update the attackers MAC in ARP Cache.
- Once the attacker's MAC address is associated with the IP address of the target device, the attacker can intercept network traffic, including passwords transmitted in plaintext.

![image](https://user-images.githubusercontent.com/65653010/227773728-ac69474c-3ead-4ffa-a6ce-76fc30a1d21f.png)

