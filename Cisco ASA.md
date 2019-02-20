

# Cisco ASA 
### Adding New VPN Users
to add a new user to the VPN, do the following:

1.  ssh to ccadmin@10.50.1.1
2.  type en to enter enable mode. Enter the enable mode password (check with IT if you do not know the password).
3.  enter config mode by typing config t
4.  type the following command to add a new user
5.  **username %firstinital_lastname% password %unencrpted_password% privilege 15**
6.  replace %**firstinital_lastname**% and %**unencrpted_password**% to actual values.
7.  type exit to go back one level in the ASA.
8.  type  **write**  to save the change to NVRAM.
9.  Close the SSH session.
10.  Save the login and password into LastPass under  **Shared-IT-Employee-Logins**

### Email to User

%User%,

On your mac, do the following

1.  Go to  **System Preferences > Network**
2.  Click the  **+**  (plus) icon at the bottom of the list of interfaces on the left hand side
3.  From the  _Interfaces_  selector, choose  **VPN**.
4.  From the  _VPN Type_ selector, choose  **Cisco IPSec.**
5.  In the  _Server Address_  field, enter  _[vpn.poweron.com](http://vpn.poweron.com/)_
6.  In the  _Account Name_  field, enter  _username_
7.  In the  _Password_  field, enter  _password_
8.  Click on the  **Authentication Settings** button
9.  In the  _Shared Secret_  field, type  _Work@Home!_
10.  in the  _Group Name_  field, type  _remote_vpn_
11.  Click  **Ok**.
12.  Click  **Connect**

The VPN is always tricky to get working the first time you connect to it. Give me a call if you run into any connectivity issues
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyNTQyODU4NDRdfQ==
-->