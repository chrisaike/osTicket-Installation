# osTicket-Installation

<img src="https://i.imgur.com/D5vlFVD.png" />



<h2>Environments and Technologies Used:</h2>

  - Microsoft Azure Virtual Machines
  - Remote Desktop
  - Internet Information Service (IIS)
  - Windows 10 OS
  
  <h2>List of Prerequisites</h2>
  
- Web Server: Internet Information Services (IIS)
- PHP Version: 7.3 recommended
- MySQL Database: 5.0+

<h2>Steps For Installing osTicket:</h2>

- Create virtual machine(VM) with windows OS on microsoft azure cloud or in any environment.
<img src="https://i.imgur.com/L9I7wZt.png" />

<img src="https://i.imgur.com/s87CO2o.png" />

<img src="https://i.imgur.com/lAlRJP7.png" />

- Copy the public IP address of the VM
- Connect the vm via remote desktop using the public IP address
-	Enable Internet Information Services (IIS) on windows features

<img src="https://i.imgur.com/ejFdrvQ.png" />




-	Look for administrative tools to find IIS in the list.
-	Download and install web platform installer from the internet

<img src="https://i.imgur.com/GQYUeK6.png" />

-	Open the web platform just installed and add the prerequisites:
- MySQL 5.5, 
- PHP 5.5; 5.6.31; 
- 7.0.33(x86); 
- 7.1.29(x86); 
- 7.3.7(x86); 
- PHP Manager for IIS

<img src="https://i.imgur.com/VUwwb2D.png" />


<h2>NEXT:</h2>

- Click install to install all the above programs at once. The installer will require an administrative password (remember to save the password).

<h2>NEXT:</h2>

- After the installation, open the IIS and run it as an administrator—only necessary if you need to add the PHP manually (If some of the packages had failed to install).
- You will notice that some recommended extentions are not enabled. This is fix by adding these extensions manually.

<img src="https://i.imgur.com/T23e71O.png" />

- Open to PHP manager and enable the recommended extensions.

<img src="https://i.imgur.com/iWDzZBU.png" />

<h2>NEXT:</h2>

- Head over to osTicket website to download and install. After downloading the osTicket from its website, do the following:

-	Unzip the osTicket folder
-	Inside the zip folder(now unzipped), you will see two folders—scripts and upload folders.
-	Copy the upload folder and paste inside inetpub root directory(you will find this within the Local Disk(C) directory)
-	Open the inetpub directory, select www.root  and paste the upload folder inside it(www.root)
-	Rename the upload folder “osTicket”
-	Then return back to IIS dashboard and refresh.
-	You’ll notice the osTicket comes up below sites
-	With osTicket selected, go ahead and click on port 80 (at the right corner of the IIS windows).
-	osTicket installer page opens up and you will notice that some of the recommended extensions may not be enabled. We can fix this with the PHP manager…
-	Access the PHP manager within the IIS windows.
-	We can enable or disable extensions within the PHP manager. Enable all the recommended extensions.

<h2>NEXT:</h2>


NEXT: Create osTicket configure file:
-	Access the osTicket folder pasted in www.rootfolder and open to ost-sampleconfig.php
-	Copy and paste this file within same location and then rename the newly copied file with “osTicket-config”
-	Continue with the osTicket installation and fill out system settings, admin user, database(DB) settings (we need to create a database before filling out it information).
-	In this tutorial, we will HeidiSQL to create a DB and name it osTicket

<img src="https://i.imgur.com/mX9AMad.png" />
-	Fill out the information: 
- user = root
-	Password = the one used during installation stage
- osTicket is now installed and you will see a congratularoty screen displayed like below:

<img src="https://i.imgur.com/fqSWpO1.png" />

- You can now login to osTicket help desk:

<img src="https://i.imgur.com/cZQCqig.png" />

- Sample dashboard of help desk ticketing on osTicket:

<img src="https://i.imgur.com/jJFYhZk.png" />

<img src="https://i.imgur.com/oYBMWpi.png" />


<img src="https://i.imgur.com/Qs7K5cS.png" />



















