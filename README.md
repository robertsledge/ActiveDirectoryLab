# Active Directory Lab

I'll be building out an AD lab with VMs shortly in order to replicate certain attacks and recon methods.

I will add content as it becomes available.


================================


Server 2019 as Domain Controller

Settings as seen below. Keeping it friendly at 2 GB RAM, and deleted the floppy.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/1a.JPG)

NAT will be used throughout.

Used the 2019 Standard Evaluation (Desktop Experience) choice at setup.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/2.JPG)

Using the super secret password of Pa$$w0rd!

Here we go:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/3.JPG)

Rebooted and ready to log in:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/4.JPG)


More to come later tonight or tomorrow, including setting up our domain controller, adding users, and of course, attacking it with exploits. 

Talk soon. Have a great day!

================================

Client Machines

Client Machines will be Windows 10 Enterprise Eval isos

I upped the RAM to 4GB for the installs, but will be bringing it back to 2 so I can host both Clients, the Domain Controller, as well as my Kali attack machine on the same laptop without running into RAM issues (16 GB total on laptop).

Ok, let's log in with our super secret password (Pa$$w0rd!)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/6.JPG)

Netx, we will use our friend sysdm.cpl:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/7.JPG)

Let's rename our PC here:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/8.JPG)

Change the name, and then select 'Ok'.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/9.JPG)

And now a quick restart:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/10.JPG)

Ok, so - Every time you start Server 2019, you should have Server Manager pop up.

When it does, we want to select 'Manage', and then 'Add Roles and Features' at the top:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/11.JPG)

Select 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/12.JPG)

Select 'Next' again:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/13.JPG)

Select your server from the list and hit 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/14.JPG)

On this screen, we want to select 'Active Directory Domain Services', highlighted above.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/15.JPG)

When you click on 'Active Directory Domain Services', this box will appear next.

Click 'Add Features':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/16.JPG)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/17.JPG)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/18.JPG)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/19.JPG)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/20.JPG)

================================

================================

================================
