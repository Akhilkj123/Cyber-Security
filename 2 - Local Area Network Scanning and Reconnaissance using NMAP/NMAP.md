1) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.
- A subnet is a portion of a larger network that has been divided into smaller, more manageable sections. It is a way of dividing a network into smaller parts for better management and security. A subnet has its own unique IP address range, and devices within that range can communicate with each other directly without having to go through a router.
![image](https://user-images.githubusercontent.com/65653010/226183010-3d91bb16-2353-48af-acc7-889811aa4c24.png)



2) What is a firewall and mention its types. Use the NMAP command to detect that a firewall protects the host.
- A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. 
- Its primary function is to prevent unauthorized access to or from a private network while allowing authorized communication.
- Types of firewalls:
- Packet filtering firewalls
- Stateful inspection firewalls
- Proxy firewalls
![image](https://user-images.githubusercontent.com/65653010/226183166-0b4a49e9-769e-4959-a74e-c8e9fd301b9e.png)
![image](https://user-images.githubusercontent.com/65653010/226261588-b1b85771-167e-45f7-b1fa-b577a8282af9.png)



3)  Use the NMAP command to scan a network and determine which devices are up and running.

![image](https://user-images.githubusercontent.com/65653010/226183268-48a64bd6-49d0-4015-a82a-d6aff6cfc888.png)
![image](https://user-images.githubusercontent.com/65653010/226261855-d31f4c67-31f0-4425-a8bf-8e2587e6fd91.png)

4)  What are vertical and horizontal scanning?
- Horizontal scanning: This is the process of drawing each horizontal line of an image on the screen from left to right. The display hardware first draws the top line of the image, then the second line below it, and so on until the entire image is displayed.
- Vertical scanning: This technique is used in interlaced video formats, where the image is split into two fields, with one field consisting of odd-numbered lines and the other field consisting of even-numbered lines. 

5) Use the NMAP command to scan multiple hosts.
![image](https://user-images.githubusercontent.com/65653010/226183413-fbacde48-4c6f-45f5-b26c-e14b42c6f734.png)
![image](https://user-images.githubusercontent.com/65653010/226262283-85ac7fb8-c159-44d8-ad64-f073d924b816.png)


6) Use NMAP commands to export the output in XML format.
  
![image](https://user-images.githubusercontent.com/65653010/226183953-a5fd5034-cd2c-46f8-9ec6-3a68eb7b1ef3.png)

  
7) Use the NMAP command to get OS information about a host. 
  
  ![image](https://user-images.githubusercontent.com/65653010/226184067-abe934ee-2531-4f55-bbdd-4021f06323fe.png)
![image](https://user-images.githubusercontent.com/65653010/226262688-4ec5618a-f035-465a-aba8-aef859c74ba6.png)

8) Explain ping sweeping and Perform ping sweeping using Nmap.
 - Ping sweeping is a technique used to scan a network and identify which IP addresses are currently in use. 
 - It involves sending ICMP echo requests (pings) to each IP address on the network and analyzing the response to determine if the IP address is active and responsive. 
  - This can be useful for identifying active hosts on a network and identifying potential targets for further scanning or analysis.
![image](https://user-images.githubusercontent.com/65653010/226184238-871c4453-3627-4567-9851-1d5084fb07a1.png)
![image](https://user-images.githubusercontent.com/65653010/226261855-d31f4c67-31f0-4425-a8bf-8e2587e6fd91.png)


9) What is a web application firewall? How do you use Nmap to detect a WAF? Perform WAF fingerprint detection using NMAP
- A web application firewall (WAF) is a type of firewall that is specifically designed to protect web applications from various types of attacks, such as cross-site scripting (XSS), SQL injection, and other vulnerabilities. It analyzes HTTP traffic between a web application and the Internet and filters out any malicious requests before they can reach the web server.
 ![image](https://user-images.githubusercontent.com/65653010/226184409-70e22f4d-f757-40e1-a742-4988e0129882.png)
![image](https://user-images.githubusercontent.com/65653010/226264273-707f8dfb-b90f-41fc-9c09-f457d7e382ce.png)

10) What is EXIF data?  Try to find EXIF data of images on a website using NMAP NSE.
- EXIF stands for Exchangeable Image File Format, and it is a metadata format that is embedded in image files captured by digital cameras and other devices that capture digital images.
- EXIF data contains various information about the image, such as the camera settings used to capture the image, the date and time the image was captured, the GPS coordinates of where the image was captured, and other technical information.
  ![image](https://user-images.githubusercontent.com/65653010/226184571-86ff29cb-53f4-4335-9f3c-f68dc5e2e4f4.png)
![image](https://user-images.githubusercontent.com/65653010/226266591-d339814f-a4e3-426b-9d30-42840c2a6e12.png)


11) Use NMAP NSE to find all subdomains of the website. 
  ![image](https://user-images.githubusercontent.com/65653010/226184764-a3cca821-2ba1-48ad-a10f-6cc8254b5672.png)
  ![image](https://user-images.githubusercontent.com/65653010/226269477-6e65a444-1b17-483a-a408-1ba56df4300d.png)


12) Perform a vulnerability scan on the target host using NMAP NSE.
  ![image](https://user-images.githubusercontent.com/65653010/226185238-2faa5a92-8c01-4bb4-942c-d425714f971f.png)
![image](https://user-images.githubusercontent.com/65653010/226270295-750e2368-efde-4f89-977d-34327a7f9d96.png)

