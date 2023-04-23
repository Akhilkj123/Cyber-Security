1.Create anIPsec-basedVPN with the help of the Strongswan tool. 

a. Configure it with IKE version 1, perform the pen-testing procedures,and make it to IKE version 2 and follow the same. Add your observations to the report. 

b. Configure your PSK to your own key phrase,then try to crack it offline. Then followthe same by creating a random auto-generatedPSK and try the same. 
- Inside /etc/ipsec.conf this lines must be added with the given IP's
![image](https://user-images.githubusercontent.com/65653010/233831754-4a03f1e0-0939-493f-9731-462a5f8c0f3d.png)
- Inside /etc/ipsec.secrets passkey line must be added.
![image](https://user-images.githubusercontent.com/65653010/233831887-5b3c843b-4bcc-45c6-b846-eb8e5ecb0a27.png)
- Now start the ipsec service
![image](https://user-images.githubusercontent.com/65653010/233831977-a3a119c8-86f3-495e-b997-da643297fdac.png)
- Now let us check the connectivity by pinging and capturing it with wireshark
![image](https://user-images.githubusercontent.com/65653010/233832236-639eadcf-b42b-4caf-8b5e-9297712de15e.png)
- Now when scanned using NMAP with port 500
![image](https://user-images.githubusercontent.com/65653010/233832314-ad13cc11-6b93-41cb-8ba2-0df48863dd41.png)
