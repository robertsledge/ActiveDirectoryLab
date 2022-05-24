# Active Directory Lab - Domain Controller Setup







Here we go. We'll be using Server 2019 as our Domain Controller.

Settings as seen below. Keeping it friendly at 2 GB RAM, and deleted the floppy.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/1a.JPG)

NAT will be used throughout.

Used the 2019 Standard Evaluation (Desktop Experience) choice at setup.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/2.JPG)

Using the super secret password of Pa$$w0rd!

Here we go:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/3.JPG)

Rebooted and ready to log in:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/4.JPG)


More to come later tonight or tomorrow, including setting up our domain controller, adding users, and of course, attacking it with exploits. 

Talk soon. Have a great day!

================================


I upped the RAM to 4GB for the installs, but will be bringing it back to 2 so I can host both Clients, the Domain Controller, as well as my Kali attack machine on the same laptop without running into RAM issues (16 GB total on laptop).

Ok, let's log in with our super secret password (Pa$$w0rd!)

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/6.JPG)

Netx, we will use our friend sysdm.cpl:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/7.JPG)

Let's rename our PC here:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/8.JPG)

Change the name, and then select 'Ok'.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/9.JPG)

And now a quick restart:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/10.JPG)

Ok, so - Every time you start Server 2019, you should have Server Manager pop up.

When it does, we want to select 'Manage', and then 'Add Roles and Features' at the top:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/11.JPG)

Select 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/12.JPG)

Select 'Next' again:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/13.JPG)

Select your server from the list and hit 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/14.JPG)

On this screen, we want to select 'Active Directory Domain Services', highlighted above.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/15.JPG)

When you click on 'Active Directory Domain Services', this box will appear next.

Click 'Add Features':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/16.JPG)

Click 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/17.JPG)

Click 'Next'again:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/18.JPG)

Click 'Next' one more time:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/19.JPG)

Click 'Install':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/20.JPG)

Once your install is done, you can click on the Notification at the top: 

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/21.JPG)

And then select 'Promote this server to a domain controller'.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/22.JPG)

On the following screen, select 'Add a new forest' and name your domain. 

I named mine 'ExampleDomain.local':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/23.JPG)

On this next screen, enter a password (this time we again used the super secret password of Pa$$w0rd!), and hit 'Next':

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/24.JPG)

You can simply hit 'Next' here as well:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/25.JPG)

Now this screen might take a moment to come up.

Once it does, your domain name should be auto-populated in 'NETBIOS domain name' the box.

When it does, hit 'Next'.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/26.JPG)

We can simply hit 'Next' here as well:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/27.JPG)

Select 'Next' one more time (if all your install options look correct), and the server will go through a series of prerequisite checks.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/28.JPG)

Once everything passes the prerequisite checks, you can hit 'Install'...

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/29.JPG)

The server will reboot on its own.

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/30.JPG)

Now we log in with our SUPER SECRET Pa$$w0rd!...

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/31.JPG)

For verification, we can cehck our user account info and see that we are logged in as the Administrator Account on our new domain:

![alt text](https://github.com/robertsledge/ActiveDirectoryLab/blob/main/media/32.JPG)


Congraulations! You are the Admin of your Domain Controller! 

If you've gotten this far on your own, AWESOME!

If you have to go back and Google a few things, that's fine too.

Next lesson: Setting up Client Machines - Coming up!




