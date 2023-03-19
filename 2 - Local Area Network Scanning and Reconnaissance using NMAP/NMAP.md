1) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.
- A subnet is a portion of a larger network that has been divided into smaller, more manageable sections. It is a way of dividing a network into smaller parts for better management and security. A subnet has its own unique IP address range, and devices within that range can communicate with each other directly without having to go through a router.
![image](https://user-images.githubusercontent.com/65653010/226177912-22816ab9-ce20-46bf-a5c7-ff2da073d033.png)


2) What is a firewall and mention its types. Use the NMAP command to detect that a firewall protects the host.
- A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. 
- Its primary function is to prevent unauthorized access to or from a private network while allowing authorized communication.
- Types of firewalls:
- Packet filtering firewalls
- Stateful inspection firewalls
- Proxy firewalls

![image](https://user-images.githubusercontent.com/65653010/226178206-acb09fac-97e4-4c81-a4f9-bb4e0fc0f099.png)


3)  Use the NMAP command to scan a network and determine which devices are up and running.

![image](https://user-images.githubusercontent.com/65653010/226178371-58faea30-add8-44d9-875d-a8f439f6e852.png)

4)  What are vertical and horizontal scanning?
- Horizontal scanning: This is the process of drawing each horizontal line of an image on the screen from left to right. The display hardware first draws the top line of the image, then the second line below it, and so on until the entire image is displayed.
- Vertical scanning: This technique is used in interlaced video formats, where the image is split into two fields, with one field consisting of odd-numbered lines and the other field consisting of even-numbered lines. 

5) Use the NMAP command to scan multiple hosts.

 nmap <target1> <target2> <target3> ...

7) Use NMAP commands to export the output in XML format.
  
  ![image](https://user-images.githubusercontent.com/65653010/226178813-8a83855a-ae52-4fdd-94d7-79970ab7f16b.png)

  
8) Use the NMAP command to get OS information about a host. 
  
  ![image](https://user-images.githubusercontent.com/65653010/226178928-ec2d77c2-f1b3-4b22-9e51-926622545f69.png)

9) Explain ping sweeping and Perform ping sweeping using Nmap.
 - Ping sweeping is a technique used to scan a network and identify which IP addresses are currently in use. 
 - It involves sending ICMP echo requests (pings) to each IP address on the network and analyzing the response to determine if the IP address is active and responsive. 
  - This can be useful for identifying active hosts on a network and identifying potential targets for further scanning or analysis.
  ![image](https://user-images.githubusercontent.com/65653010/226179087-40accdf5-0d3d-437c-bd6b-0862f814e321.png)

10) What is a web application firewall? How do you use Nmap to detect a WAF? Perform WAF fingerprint detection using NMAP
- A web application firewall (WAF) is a type of firewall that is specifically designed to protect web applications from various types of attacks, such as cross-site scripting (XSS), SQL injection, and other vulnerabilities. It analyzes HTTP traffic between a web application and the Internet and filters out any malicious requests before they can reach the web server.
  ![image](https://user-images.githubusercontent.com/65653010/226179159-47ca9c75-cc0e-4936-b05a-b51de0886e4e.png)

11) What is EXIF data?  Try to find EXIF data of images on a website using NMAP NSE.
- EXIF stands for Exchangeable Image File Format, and it is a metadata format that is embedded in image files captured by digital cameras and other devices that capture digital images.
- EXIF data contains various information about the image, such as the camera settings used to capture the image, the date and time the image was captured, the GPS coordinates of where the image was captured, and other technical information.
  ![image](https://user-images.githubusercontent.com/65653010/226179272-3a46bcf7-5815-4701-bf78-f37f1cbc59e5.png)


11) Use NMAP NSE to find all subdomains of the website. 
  ![image](https://user-images.githubusercontent.com/65653010/226179363-b5083631-0386-4f8c-b62b-8d2485b860cf.png)

12) Perform a vulnerability scan on the target host using NMAP NSE.
  ![image](https://user-images.githubusercontent.com/65653010/226179612-a5885ed7-5f94-4eb0-a01a-3300c37cf3fa.png)

