# Vitual Private Network (VPN)
<p align="center">
<img src="https://github.com/user-attachments/assets/148ea37f-12b6-4db2-9a6d-dd2d9df49395" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Prerequisites and Installation</h1>
In this section, we will set up a Virtual Private Network (VPN) by first creating a virtual machine in Microsoft Azure, then configuring the necessary network settings to establish secure remote connections within a network infrastructure .<br />

<h2>Environments and Technologies Used</h2>

- Proton VPN (Virtual Private Network)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 11 Pro</b> (22H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locating local personal IP address
- STEP 2 - Setting up Virtual Machine using Azure
- STEP 3 - Locating IP through Virtual Machine (France)
- STEP 4 - Connecting to VPN (Virtual Private Network) Through Virtual Machine
- STEP 5 - Locating IP Through VPN (Netherlands)

<h2>Installation Steps</h2>

STEP 1 - Locate your personal IP address by going to "www.whatismyipaddress.com" and it will show your local IP address. Use my example posted (EXAMPLE 1A) as a reference.

EXAMPLE 1A
<p>
<img <img width="1820" height="809" alt="VPN 1" src="https://github.com/user-attachments/assets/5b352c4b-9f75-45bd-8699-30956443324e" />

</p>
<p>

Now we will set up our virtual machine in Microsoft Azure. 
  
</p>
<br />

STEP 2 - In order to create a virtual machine, we must first create a Resource Group. After the Resource Group has been created type Virtual Machines into the search bar. Next click "Create" followed by Virtual Machine tab to began creating one. See Example 2A below as a reference guide. 

EXAMPLE 2A
<p>
<img <img width="1653" height="773" alt="VPN 2" src="https://github.com/user-attachments/assets/9b1eb6f1-78f4-4900-b438-2a88e1a10a79" />

</p>
<p>

Create the Virtual Machine on EXAMPLE 2B by listing "VPN-Test" as the Resource group and listing “FranceVM” as the Virtual machine name. Ensure the other items are selected as shown in EXAMPLE 2B & 2C.

EXAMPLE 2B
<p>
<img <img width="1064" height="710" alt="VPN 3" src="https://github.com/user-attachments/assets/a835454e-0eb7-42e0-bbc6-02e604544308" />

</p>
<p>

For the Username and Password you can create your credentials.
  
</p>
<br />

EXAMPLE 2C
<p>
<img <img width="935" height="694" alt="VPN 4" src="https://github.com/user-attachments/assets/db6a4961-269d-42e3-b8eb-ac29f4ef68fa" />

</p>
<p>

Select the tab that says "Networking" (Basics -> Disks -> Networking) towards the top of the page and view EXAMPLE 2D inputs to match. 
  
</p>
<br />

EXAMPLE 2D
<p>
<img <img width="1029" height="822" alt="VPN 5" src="https://github.com/user-attachments/assets/978161fc-9de6-43b7-a7ea-b520ff2cadc1" />

</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. You will receive a follow-up notification that says "deployment in progress" so be prepared to wait for about 2-3 minutes for it to complete.
  
</p>
<br />

Once Deployment is completed we can click on our Virtual Machine to open it. There we will discover our VM'S Public IP address and other information as shown in EXAMPLE 2E

EXAMPLE 2E

<p>
<img <img width="1661" height="783" alt="VPN 6" src="https://github.com/user-attachments/assets/edca9eb6-e2d6-485c-9507-982c80dc8f6f" />

</p>
<p>


STEP 3 – Log Into the VM and Find IP Address
<p>
Since we have set up our Virtual Machine we can now connect to it using Remote Desktop (shown in EXAMPLE 3A). Input the IP address our VM generated (refer back to EXAMPLE 2E for help) as the Computer and then type in the Username + Password (refer back to EXAMPLE 2C for help). After logging into Remote Desktop, open the web browser and look up www.whatismyipaddress.com once again (EXAMPLE 3B).

  
</p>
<br />
EXAMPLE 3A
<p>
<img <img width="599" height="371" alt="VPN 7" src="https://github.com/user-attachments/assets/38946338-4184-4359-92f9-49bd763123ea" />

</p>
<p>

  
</p>
<br />

EXAMPLE 3B
<p>
<img <img width="1799" height="682" alt="VPN 8" src="https://github.com/user-attachments/assets/26221819-21df-4349-8b82-52804cb097aa" />

</p>
<p>

When we look up the IP address for this VM through www.whatismyipaddress.com we now see that it's showing Amazon.com as our Internet Service Provider (ISP) and our location has changed to France (EXAMPLE 3C).
  
</p>
<br />

EXAMPLE 3C
<p>
<img <img width="1799" height="682" alt="VPN 8" src="https://github.com/user-attachments/assets/95a8852b-8e39-4e9b-87d8-b4d4117bfc01" />

</p>
<p>

STEP 4 – Connecting to the VPN (Free Version)

Using the local computer (not Remote Desktop) go to www.protonvpn.com and create a free account. DO NOT you use the VM unless you understand French because that is what will be displayed on your browser. After the logging into your account, copy the URL from Proton VPN's website (EXAMPLE 4A) and paste it into to the VM web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>
<img <img width="1408" height="937" alt="VPN 10" src="https://github.com/user-attachments/assets/98ae99f3-3bb0-49fb-9506-35fbe010a5a8" />

</p>
<p>

Now scroll down the and select the “Downloads" tab. Here we will choose which OS we want to download our VPN. In our case “Windows” is the correct one (as shown in EXAMPLE 4B). Once the download completes the application is now installed so we will log in using the credentials created to set up the free account.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img <img width="1625" height="944" alt="VPN 11" src="https://github.com/user-attachments/assets/f0621ae7-378e-4438-81bc-15ad52799e18" />

</p>
<p>

Connect to the VPN through the installed app. We see that the Netherlands was selected as the fastest free server. EXAMPLE 4C below shows the VPN being connected to an IP in the Netherlands. 
  
</p>
<br />

EXAMPLE 4C
<p>
<img <img width="1713" height="966" alt="VPN 12" src="https://github.com/user-attachments/assets/30bac208-db22-45aa-8216-d4f52477df45" />

</p>
<p>

Finally we will look at the IP again using the VM browser now that we have connected the VPN to the Netherlands. The website www.whatismyipaddress.com shows yet another IP address change using the VPN from the Netherlands. I must say this is quite fascinating!
  
</p>
<br />

EXAMPLE 4D
<p>
<img <img width="1708" height="745" alt="VPN 13" src="https://github.com/user-attachments/assets/8a0c7180-f46e-4b68-a092-7a8acb1c4854" />

</p>
<p>

Looking at this exercise we see that 3 different IP addresses were utilized just from our local computer to connect to the internet.
Home IP (USA): 99.47.77.196,
Virtual Machine IP (France): 98.66.162.170,
Virtual Machine IP VPN (Netherlands) 80.79.7.127

  
</p>
<br />
