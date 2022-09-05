# Windows-Endless-Nightmare </p>

Problem #1. VMware </br>
There are 2 host versions, ESXi is for "Native/No HostOS" like Proxmox: </br>
Fusion Player 12.1.2 for OSX Catalina </br>
Workstation Player 12 for Windows. </p>

VMware installs some tools v11 that cannot be uninstalled. </p>

Problem #2.  </br>
if you have a MacPro4,1/5,1 2009/2010=2012 </br>
The Bootcamp HDD can be used as a Virtual Machine directly, without Importing the HDD OS to a Real Virtual Machine. </br>
Works ok, </br>
BUT... if you reboot in Normal Bootcamp mode, </br>
will Damage windows. </br>
VMware for OSX, and Parallels for OSX, </br>
are a different machine, and fool Windows Software Licencing Activation Maganer that is Activated. </br>
like a Legal Windowws "Pirate" Activator. </br>
But if you Reboot in Bootcamp "Native Mode",  </br>
if you install both Parallels and VMware Fusion Player, </br>
Windows will Go Crazy. </p>

Windows will Activate a Self-Defense Mechanism.. </p>

Refreshing the PC, does Not work. </br>
Reseting the PC, does Not work. </p>

Needs a Clean install. </p>

Problem #3. </p>

if you do: </br>
Diskpart </br>
list disk </br>
sel disk x </br>
clean </p>

it will clean the HDD, delete everything, like a spy movie. </p>

problem is, it will delete also the Windows Activation Keys, </br>
and important Files. </p>

when Windows Defense is Activated, </br>
does Not allow to Create a USB Recovery Drive, </br>
does Not allow to create a System Image Backup. </br>
You are Doomed. </p>

IF Windows is Retail version... </br>
Allow to Move/Transfer the license, </br>
if its OEM, you need to buy a New License. </p>

cmd </br>
slmgr -dli </p>

will reveal if the License is RETAIL or OWM. </br>
if you have OEM better install Linux. </p>

if you have RETAIL, the Nightmare Continues. </p>

RETAIL comes with a CARD, and the Activation Printed. </br>
IF you have multiple PCs with RETAIL version,  </br>
you have multiple CARDS. </p>

you need to find the correct CARD to Reactivate a Fresh / Clean Copy of Windows. </br>
if you want to avoid Nightmares in the Future... </br>
i strongly Recomend Clean installing Windows on a VirtualMachine VHD VHDX, </br>
VHDX can be attached to bcdboot drive, as a Real Drive. </br>
you can use a Virtual Drive as a Real Native... </p>

Installing 100% Native is inferior. "The method most people use". </p>

some people claim Windows Runs Faster in Virtual Machine. </br>
thats for another topic. </p>


IF you have Windows8.1 .iso </br>
Windows Update Manager that comes, does Not work... </br>
you need to download a KB with a Newer Version. </p>

here is for Win8 and Server 2012 R1 </br>
https://docs.microsoft.com/en-us/troubleshoot/windows-client/deployment/update-windows-update-agent </br>

here is for Win8.1 and Server 2012R2 </br>
https://support.microsoft.com/en-us/topic/windows-update-client-for-windows-8-1-and-windows-server-2012-r2-march-2016-758f2099-93d8-a2ae-a1fb-b8e75b9a4cb2 </br>

Joke: </br>
why are Not on the same page? </br>
Fragmentation. LOL. </p>

other places: </br>
https://www.catalog.update.microsoft.com/home.aspx </br>
and  </br>
KB website </p>

Latest Windows 8.1 Update is 1.5GB and comes with EDGE Browser. </br>
if you dont have EDGE you have an older Windows8.1 </p>

Generic / Emergency Activation Key does Not allow to Update to Latest Windows8.1 with EDGE. </br>

When you have a Complete Upgraded Windows, </br>
do a System Image Backup. </br>
it will save a lot of time, next time. </p>

if you have an HDD formatter with EXT4v2 Linux >16,  </br>
to see Ext4v2 in Windows there are 2 options: </br>
Free: </br>
http://www.acc.umu.se/~bosse/ </br>
and Payd: PAragon Linux Drivers for Windows. </p>

if you try to see Ext4v1 hdd with EXT2FSB v0.69 will Damage the Ext4v2, </br>
wont be Readable in Newer like Linux 20.10 etc... </br>
Repairing that is antoher Nightmare. </p>

here are some Screnshots of: </br>
cmd </br>
# slmgr -dli</br>
![slmgr-dli](https://user-images.githubusercontent.com/33388902/188486331-8705a86f-5f76-489b-b8bb-beb63ac6cd86.PNG)

# slmgr -? </br>
![slmgr help](https://user-images.githubusercontent.com/33388902/188486401-33bb498a-9fa9-42d4-801f-e08599b6d67d.PNG)

![slmgr help adv](https://user-images.githubusercontent.com/33388902/188486425-cec6f65a-909b-4c62-b3e9-a468e92e266d.PNG)

![slmgr help vol](https://user-images.githubusercontent.com/33388902/188486439-50665990-8dbd-44bc-b444-2232b2784188.PNG)

![slmgr help vol2](https://user-images.githubusercontent.com/33388902/188486451-8233330c-ab5d-4cdf-b1b6-ef469f796bb0.PNG)

![slmgr help vol3](https://user-images.githubusercontent.com/33388902/188486465-91e2f5d9-df87-4714-81ed-11f19b27e302.PNG)

![0-cmd](https://user-images.githubusercontent.com/33388902/188486542-29e74ce8-aaf9-4450-9658-7c46e34ce4af.PNG)

