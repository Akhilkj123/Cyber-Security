**ARP(Address Resoltion Protocol)** is a process in which a user sends a broadcast address, asking for a MAC Address from a specific IP address. Then the user with the specific IP address sends it MAC Address as its response. Then the former user updates the IP in the ARP Cache.

**1) Perform Password stealing (over plaintext) using ARP Cache Poisoning attacks.**
- **ARP Cache Poisoning** is a process in which an attacker intervens in between the arp transfer and spoofs the identity of the user the requested IP Address.It also sends the attackers MAC address to the requested user which causes it to update the attackers MAC in ARP Cache.
- Once the attacker's MAC address is associated with the IP address of the target device, the attacker can intercept network traffic, including passwords transmitted in plaintext.
- Ettercap is a tool used to perform ARP cache poisoning attack which will capture the password and display it in plaintext in its logs.
![image](https://user-images.githubusercontent.com/65653010/227773728-ac69474c-3ead-4ffa-a6ce-76fc30a1d21f.png)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**2) Perform Denial of Service (DoS) attacks using ARP Cache Poisoning attacks.**
- In DoS attack, the attacker sends large number of fake ARP messages to the victim, each with a different MAC Address. This floods the ARP cache of the target device with invalid entries, effectively overwhelming it and causing it to drop legitimate traffic. The result is that the targeted device becomes unavailable, effectively denying service to legitimate users.
![image](https://user-images.githubusercontent.com/65653010/227775269-47c9b34a-b5ce-4fa3-ba07-0fe439c15542.png)
- The result is that the targeted device becomes unavailable, effectively denying service to legitimate users.
![image](https://user-images.githubusercontent.com/65653010/227775284-3224daac-af9d-46d4-84de-eeb1ff9c7b83.png)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**3) Perform DNS Spoofing attack using ARP Cache Poisoning attacks.** 
- In DNS attack, the attacker uses the ARP Cache Poisoning method to redirect the DNS request made by the user to a site preferred by the attacker. 
- When the user sends a DNS request, the attacker which performed the ARP Poisoning on the user redirects the DNS request to a DNS request created by the attacker which causes the user to open a site preferred by the user.
- Using ettercap, we can do DNS Spoofing using ARP Poisoning.
![image](https://user-images.githubusercontent.com/65653010/227776384-56f860d7-60b9-4511-92fe-48eae765e8e3.png)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**4) Invoke ‘sslstrip tool’ for stealing passwordsfrom any machine that is connected toa LAN by stripping the HTTPSconnection.** 
- When a user attempts to connect to a secure website using SSLstrip, the tool will intercept the request and alter it so that it appears to be a request for an unsecured HTTP connection.
-  This will cause the user's browser to communicate with the website over an unencrypted connection, rather than the secure HTTPS connection it intended to use. 
-  This can allow an attacker to intercept and read any data being transmitted between the user's browser and the website, including sensitive information such as login credentials and credit card details.
-  Now using Ettercap we will add the ip of the victim to attackers list.
![image](https://user-images.githubusercontent.com/65653010/227987258-c8a273c9-8026-443e-acb3-f3a03dbd801f.png)
- When the attacker uses Ettercap to do SSLstrip, the secured version of the site get cancelled and the site gets blocked.
![image](https://user-images.githubusercontent.com/65653010/227987427-1833420c-b3eb-4860-b1c2-1eb903ba8f5e.png)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**5) Use arp_cop and scan_poisoner plugins to learn about the detection of ARP attacks.**

