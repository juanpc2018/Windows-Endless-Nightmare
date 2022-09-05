# Windows-Endless-Nightmare

Problem #1. VMware
There are 2 host versions, ESXi is for "Native/No HostOS" like Proxmox:
Fusion Player 12.1.2 for OSX Catalina
Workstation Player 12 for Windows.

VMware installs some tools v11 that cannot be uninstalled.

Problem #2. 
if you have a MacPro4,1/5,1 2009/2010=2012
The Bootcamp HDD can be used as a Virtual Machine directly, without Importing the HDD OS to a Real Virtual Machine.
Works ok,
BUT... if you reboot in Normal Bootcamp mode,
will Damage windows.
VMware for OSX, and Parallels for OSX,
are a different machine, and fool Windows Software Licencing Activation Maganer that is Activated.
like a Legal Windowws "Pirate" Activator.
But if you Reboot in Bootcamp "Native Mode", 
if you install both Parallels and VMware Fusion Player,
Windows will Go Crazy.

Windows will Activate a Self-Defense Mechanism..

Refreshing the PC, does Not work.
Reseting the PC, does Not work.

Needs a Clean install.

Problem #3.

if you do:
Diskpart
list disk
sel disk x
clean

it will clean the HDD, delete everything, like a spy movie.

problem is, it will delete also the Windows Activation Keys,
and important Files.

when Windows Defense is Activated,
does Not allow to Create a USB Recovery Drive,
does Not allow to create a System Image Backup.
You are Doomed.

IF Windows is Retail version...
Allow to Move/Transfer the license,
if its OEM, you need to buy a New License.

cmd
slmgr -dli

will reveal if the License is RETAIL or OWM.
if you have OEM better install Linux.

if you have RETAIL, the Nightmare Continues.

RETAIL comes with a CARD, and the Activation Printed.
IF you have multiple PCs with RETAIL version, 
you have multiple CARDS.

you need to find the correct CARD to Reactivate a Fresh / Clean Copy of Windows.
if you want to avoid Nightmares in the Future...
i strongly Recomend Clean installing Windows on a VirtualMachine VHD VHDX,
VHDX can be attached to bcdboot drive, as a Real Drive.
you can use a Virtual Drive as a Real Native...

Installing 100% Native is inferior. "The method most people use".

some people claim Windows Runs Faster in Virtual Machine.
thats for another topic.


IF you have Windows8.1 .iso
Windows Update Manager that comes, does Not work...
you need to download a KB with a Newer Version.

here is for Win8 and Server 2012 R1
https://docs.microsoft.com/en-us/troubleshoot/windows-client/deployment/update-windows-update-agent

here is for Win8.1 and Server 2012R2
https://support.microsoft.com/en-us/topic/windows-update-client-for-windows-8-1-and-windows-server-2012-r2-march-2016-758f2099-93d8-a2ae-a1fb-b8e75b9a4cb2

other places:
https://www.catalog.update.microsoft.com/home.aspx
and 
KB website

Latest Windows 8.1 Update is 1.5GB and comes with EDGE Browser.
if you dont have EDGE you have an older Windows8.1

Generic / Emergency Activation Key does Not allow to Update to Latest Windows8.1 with EDGE.

When you have a Complete Upgraded Windows,
do a System Image Backup.
it will save a lot of time, next time.

if you have an HDD formatter with EXT4v2 Linux >16, 
to see Ext4v2 in Windows there are 2 options:
Free:
http://www.acc.umu.se/~bosse/
and Payd: PAragon Linux Drivers for Windows.

if you try to see Ext4v1 hdd with EXT2FSB v0.69 will Damage the Ext4v2,
wont be Readable in Newer like Linux 20.10 etc...
Repairing that is antoher Nightmare.

here are some Screnshots of:
cmd
slmgr -dli
![slmgr-dli](https://user-images.githubusercontent.com/33388902/188486331-8705a86f-5f76-489b-b8bb-beb63ac6cd86.PNG)

slmgr -?
![slmgr help](https://user-images.githubusercontent.com/33388902/188486401-33bb498a-9fa9-42d4-801f-e08599b6d67d.PNG)

![slmgr help adv](https://user-images.githubusercontent.com/33388902/188486425-cec6f65a-909b-4c62-b3e9-a468e92e266d.PNG)

![slmgr help vol](https://user-images.githubusercontent.com/33388902/188486439-50665990-8dbd-44bc-b444-2232b2784188.PNG)

![slmgr help vol2](https://user-images.githubusercontent.com/33388902/188486451-8233330c-ab5d-4cdf-b1b6-ef469f796bb0.PNG)

![slmgr help vol3](https://user-images.githubusercontent.com/33388902/188486465-91e2f5d9-df87-4714-81ed-11f19b27e302.PNG)


![0-cmd](https://user-images.githubusercontent.com/33388902/188486542-29e74ce8-aaf9-4450-9658-7c46e34ce4af.PNG)

