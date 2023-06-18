## Task 3: Analysing Malicious PDF's

- We use peepdf to begin a precursory analysis of a PDF file to determine the presence of Javascript.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/3df83565-925c-4a2f-8f19-037f655c51f1)

a) How many types of categories of "Suspicious elements" are there in "notsuspicious.pdf"

 ![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/a0649828-2725-4bdc-aafb-b5116dd3bdad)
 
 b) Use peepdf to extract the javascript from "notsuspicious.pdf". What is the flag?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/efa885a0-9fe2-4bfd-aebd-0485a3583da1)

c) How many types of categories of "Suspicious elements" are there in "advert.pdf"

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/03c04649-c1a8-48c7-8db0-6ffbb1c446e0)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9651ba00-2973-433d-bc8c-1b6b6ed08183)

d) Now use peepdf to extract the javascript from "advert.pdf". What is the value of "cName"?

- Now we analyse the given file using peedpdf and extract the Javascipt using 'extract js'.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1ad87047-40a4-4957-ab71-9c5648a95eb4)

- When we cat the extracted file we get

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/c71e0d65-8538-4dec-a3ff-68011457660c)

## Task 4: Analysing Malicious Microsoft Office Macros

- We can simply use REMnux's vmonkey which is a parser engine that is capable of analysing visual basic macros without executing.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/b2517dcf-de13-43b4-abeb-d2dcdf4d4898)

a)What is the name of the Macro for "DefinitelyALegitInvoice.doc"

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/4c93e6bd-49af-410f-aae6-7c0d5fd5eeec)

b) What is the URL the Macro in "Taxes2020.doc" would try to launch?

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f2ecfff9-5856-4b76-9079-d1f986d76952)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/ffa8ec70-74f4-47ef-9e77-bde2c53cee26)

## Task 6: How's Your Memory?

- In other scenarios, we would use the imageinfo plugin to help determine what profile is most suitable with the syntax of volatility -f Win7-Jigsaw.raw imageinfo.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9b85f616-8439-4e0c-b5b6-7ac9816460ac)

- This will take hours so we can see google Chrome within the process because the application was running at the time of the memory dump.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/f5f0ea80-7318-44d4-871a-6fcd885e47b1)

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/433cac41-d430-427d-93f2-be3307e44790)

- We can list the DLL's that "drpbx.exe" references with dlllist


![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/bddefd44-f79b-4dd8-a16a-ad76a1b7797c)

- This DLL is a Windows library that allows applications to use cryptography.

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/caf22f5e-39e6-40e6-8b36-c446365b9f09)


