## Task 2: Windows Domains
-  The main idea behind a domain is to centralise the administration of common components of a Windows computer network in a single repository called Active Directory (AD).
-  The server that runs the Active Directory services is known as a Domain Controller (DC).
### The main advantages of having a configured Windows domain are:
- **Centralised identity management:** All users across the network can be configured from Active Directory with minimum effort.
- **Managing security policies:** You can configure security policies directly from Active Directory and apply them to users and computers across the network as needed.

a) In a Windows domain, credentials are stored in a centralised repository called...
- Active Directory

b) The server in charge of running the Active Directory services is called...
- Domain Controller

## Task 3: Active Directory
### Users
- Users are one of the most common object types in Active Directory.
- Users are one of the objects known as security principals, meaning that they can be authenticated by the domain and can be assigned privileges over resources like files or printers.
### Machines
- Machines are another type of object within Active Directory; for every computer that joins the Active Directory domain, a machine object will be created.
- Machines are also considered "security principals" and are assigned an account just as any regular user.

- **OUs**: They are handy for applying policies to users and computers, which include specific configurations that pertain to sets of users depending on their particular role in the enterprise. Remember, a user can only be a member of a single OU at a time, as it wouldn't make sense to try to apply two different sets of policies to a single user.
- **Security Groups**: They are used to grant permissions over resources. For example, you will use groups if you want to allow some users to access a shared folder or network printer.

a) Which group normally administrates all computers and resources in a domain?
- Domain Admins

b) What would be the name of the machine account associated with a machine named TOM-PC?
- TOM-PC$

c) Suppose our company creates a new department for Quality Assurance. What type of containers should we use to group all Quality Assurance users so that policies can be applied consistently to them?
- Organizational units

## Task 4: Managing Users in AD
### Delegation
- One of the nice things you can do in AD is to give specific users some control over some OUs.
- This process is known as delegation and allows you to grant users specific privileges to perform advanced tasks on OUs without needing a Domain Administrator to step in.

