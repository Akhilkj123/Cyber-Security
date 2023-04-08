**1.  Learn the basic working of Wi-Fi and its types with various types of attacks on it.**
- **Wi-Fi** is a wireless technology that enables devices to connect to the internet or communicate with each other without the need for physical cables. It works by using radio waves to transmit and receive data between devices and a wireless access point (WAP) or wireless router.
   Some common types of attacks on Wi-Fi networks:
-  **Rogue Access Points:** Attackers can create rogue access points to trick users into connecting to them instead of the legitimate access point. Once connected, the attacker can intercept sensitive information such as login credentials or inject malware.
- **Password Cracking:** Attackers can use password cracking tools to guess or brute-force passwords to gain access to Wi-Fi networks.
- **Denial-of-Service (DoS) Attacks:** In a DoS attack, the attacker floods the Wi-Fi network with traffic to overload it, causing it to crash or become unavailable to legitimate users.
**Eavesdropping:** Attackers can use tools to monitor Wi-Fi traffic to intercept and steal sensitive information such as login credentials or credit card details.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 
**2. Perform Wi-Fi fingerprinting using Wigile, Inssider, and Kismet.**
- **Wiggle** - Wiggle is a network scanning tool that can be found in Kali Linux. It is a tool that helps in the detection and discovery of wireless networks. 


![image](https://user-images.githubusercontent.com/65653010/230719514-a0f32306-3ca3-4218-95e7-b3e427b0656c.png)

- **Inssider** - Inssider is a wireless network scanner tool that can be found in Kali Linux. It allows users to scan and analyze wireless networks in the vicinity, displaying information such as the network's name, signal strength, and encryption method.

![image](https://user-images.githubusercontent.com/65653010/230718774-19056bc7-bd5b-4dea-83c6-09b615e34175.png)

![image](https://user-images.githubusercontent.com/65653010/230718790-787ed1cb-b656-42f7-9aba-bba0a697933e.png)

- **Kismet** - Kismet is a popular open-source wireless network detector, sniffer, and intrusion detection system that is included in the Kali Linux operating system. It is used for finding and analyzing wireless network traffic, identifying Wi-Fi networks, detecting wireless devices, and analyzing wireless protocols.
- Start monitor-mode wlan0: airmon-ng start wlan0

![image](https://user-images.githubusercontent.com/65653010/230620620-9d51c71a-d128-4865-8c40-0abd98cb9723.png)

- Start kismet using: kismet -c wlan0

![image](https://user-images.githubusercontent.com/65653010/230624975-f0a7bd91-ae89-47b5-ae00-0bc44097b7d7.png)

- Result of the Wi-fi hotspots scanned using kismet

![image](https://user-images.githubusercontent.com/65653010/230625372-a3dbb08f-8b3d-468a-96b5-65dffb9e9f85.png)
![image](https://user-images.githubusercontent.com/65653010/230625623-f5001a31-e435-43c5-a3d2-726bfa4c7495.png)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 

 **3. Create an Access point with any Wi-Fi encryption standard and start testingthe security of that connectionusing any Wi-Fi security testing tools,which should include (Aircrack-Ng, Wifite, not limited). Try to capture the 4-wayhandshake using these methods.**
 - Start monitor-mode wlan0: airmon-ng start wlan0

![image](https://user-images.githubusercontent.com/65653010/230620620-9d51c71a-d128-4865-8c40-0abd98cb9723.png)

- Let us monitor the network using: airodump-ng wlan0

![image](https://user-images.githubusercontent.com/65653010/230626001-affa1361-9162-4ff2-8722-d04d9129b206.png)

- Select a certain network using SSID : airodump-ng --bssid (bssid of the certain network) -c (channel) --write (name of file) wlan0

![image](https://user-images.githubusercontent.com/65653010/230626832-7fe857b1-51ec-47ce-bf71-13e43227d94b.png)

- Captured the 4-way handshake using Wireshark

![image](https://user-images.githubusercontent.com/65653010/230719476-ed6b56b3-3302-4a9b-99ee-eac4d2bf8860.png)


**4. After capturing the required filesfortesting, usedictionarygeneration and password cracking tools to crack the Wi-Fi password.** 

 a. You must use an existing word file to crack the password.
 
 b. Also you have to create your dictionaryfilefor cracking the passwords.
 
c. Keep 3 different types of passwords for your Wi-Fi to test it. Simple, medium,and complex passwords can be used for testing. Simple can be a dictionary word, medium can be of dictionary word with some numbers, and complex can be generated from any password generator on  line.

- Now trying to crack the tough password 

![image](https://user-images.githubusercontent.com/65653010/230719269-f8b8aa29-b45a-4006-9b39-7b1cd45d5e1f.png)

- Now trying to crack the easy password

![image](https://user-images.githubusercontent.com/65653010/230719408-f6383d6e-3dbe-40de-bd8d-08f6bbaec9bb.png)

**6. Learn the protocol level working of WPA3 and how it differs from WPA2**

 **WPA3** is the latest version of the Wi-Fi Protected Access (WPA) security protocol used in wireless networks. It was designed to address the weaknesses found in the previous versions, WPA and WPA2. The WPA3 protocol operates on a higher level of the OSI model, specifically at the data link layer (layer 2) and network layer (layer 3). The protocol provides more robust encryption and authentication mechanisms to protect wireless networks from attacks and unauthorized access.
- Authentication: The WPA3 protocol uses a new authentication mechanism called Simultaneous Authentication of Equals (SAE), also known as Dragonfly. 
- Encryption: WPA3 uses a new encryption algorithm called the 256-bit Galois/Counter Mode Protocol (GCMP-256) for data encryption. 
- Brute-Force Protection: WPA3 also includes brute-force protection, which makes it more difficult for attackers to guess the passphrase through a brute-force attack. 

- **WPA3** is the next generation of WPA and has better security features. It protects against weak passwords that can be cracked relatively easily via guessing.
- 128-bit encryption in WPA3-Personal mode (192-bit in WPA3-Enterprise) and forward secrecy. WPA3 also replaces the Pre-Shared Key (PSK) exchange with Simultaneous Authentication of Equals, a more secure way to do initial key exchange
