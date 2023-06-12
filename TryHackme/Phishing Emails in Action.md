## Task-2: Cancel your PayPal order

Here are some quick observations about this email sample:

- This is an unusual email recipient address. This is not the email address associated with the Yahoo account. 
- This mismatch should immediately stand out. The sender's details (service@paypal.com) don't match the sender's email address (gibberish@sultanbogor.com). 
- The subject line hints that you made a purchase or a transaction of some sort. If you don't recall this account, then it will grab your attention. This social engineering tactic is to prompt you to interact with the email with haste. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/9890f9e0-5d3b-47c2-a188-8e432d01cba9)

- The body of the message consistes of a button which shows 'cancel the order'. This message is shown as if it is sent from paypal service.
 
![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/14c118c9-5295-4068-b68b-2e7213dc6907)
- Now if we inspect the Page Source of the page we see that the nbutton redirects us to such a link

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/66cad3d2-b705-4620-bbb4-3a7332910ff0)

- Such a link can be identified as flaw or can be checked by using various online tools

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/1667e859-e2a3-4fcb-8634-d1f0ab13bd1b)


a) What phrase does the gibberish sender email start with?
- noreply

## Task-3: Track your package

Here are some quick observations about this email sample:

- The email is tailored to appear that it's sent from a mail distribution center of some sort. 
- The subject line adds to the pretense with a 'tracking number.' 
- The link in the email body matches the subject line. 

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/6d7ffb95-2352-4514-a519-dc578fcd2d04)

- Now let us inspect the pagesource

![image](https://github.com/Akhilkj123/Cyber-Security/assets/65653010/83cabe4f-1225-4474-b121-072d94df864e)

- The link is poinitng to some other website and also a image file is present in it. A single tracking pixel is embedded in the email, usually (but not always) hidden within an image or a link. When the email is opened, code within the pixel sends the info back to the company’s server. 
- Yahoo automatically blocked the images in this email. Many email providers do the same.

a) What is the root domain for each URL? Defang the URL. 
- devret[.]xyz
