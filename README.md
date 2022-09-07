# Windows-Endless-Nightmare </p>

Problem #0.</br>
i deleted my HDD, because i could Not make a System Image Backup or create a USB Recovery Drive, i thought Windows was damaged </br>
Refreshing windows did Not work, </br>
Reseting windows did Not work.</br>
sfc /scannow did Not work, </br>
DISM /online-cleanup did Not work,  </br>
Deleting Windows did Not work</br>
Because the problem are some KB "Updates" from 2022 that cannot be Uninstalled, </br>

The latest 4x 2022 Updates, 2x can be Unsinstalled, 2x cannot, 1 says it can, but Fails to Uninstall,</br>
the other does Not have Uninstall button. </p>

There are 100 KB Updates since 2014 for Windows8.1, </br>
None of the 2014 can be Uninstalled, because early Windows8.1 had many Errors & Conflics with Fast Boot, Power Settings & Time.</br>
2 or more KB "Updates" are very agressive, against the owner/user, against freedom, against private property, against privacy, total control of your machine, </br>
coercion against the civilian, called in the Nurember Code.</p>

IF you want to install W8.1x64</br>
use a generic/emergency key, it will allow to install, and will disapear as soon you go online,
Alternate use your Real Key but Deactivate before Going Online to Update. </br>
Win8.1 will allow to update without Key to a point before EDGE Browser Era. </br>
after complete Download, you need a real Key to Download the Updates After EDGE, </br>
Set Updates to Download & Do Not Install.</br>
install 1 by 1, slowly, test 1 per day, </br> 
to find the Dangerous "Updates" </br>
there is an "Update" that does not let you see the screen if you have a Newer machine z270.</br>
that same update is invisible, if you have a 2010 x58 machine. BEWARE!</p>

MS is using coercion against all W8.1 owners, to Buy W10/W11, before Extended Support Ends.</br>
at a gun point if they could.</br>
if you want to read all the time MS made me waste chasing problems they create, continue reading. </br>

This is when you regret being a legal owner of Windows.</br>
Windows is No more for me, i will Never buy Windows again,</br>
i have some legal licenses, i will install them on a .VHD without the dangerous KB, and forget about Windows.</br>
i cant take this bully anymore. </p>



------------

Problem #1. VMware </br>
There are 2 host versions, ESXi is for "Native/No HostOS" like Proxmox, or bcdboot.</br>
VMware Fusion Player 12.1.2 for OSX Catalina </br>
VMware Workstation Player 12 for Windows. </p>

VMware installs tools & drivers v11 that cannot be uninstalled.  </br>
similar to bootcamp drivers. </p>

Problem #2.  </br>
if you have a MacPro4,1/5,1 2009/2010=2012 </br>
The Bootcamp HDD can be used as a Virtual Machine directly, without Importing the HDD OS to a Real Virtual Machine. </br>
Works ok, </br>
BUT... if you reboot in Normal Bootcamp mode, </br>
will Damage windows. </br>
VMware for OSX, and Parallels for OSX, </br>
are a different machine, and fool Windows Activation Maganer that is Activated. </br>
like a Legal Windows "Pirate" Activator. </br>
but is Not permanent, is Temporal, Only works as long you pay / buy VMware or Parallels. </br>
if you Reboot in Bootcamp "Native Mode",  </br>
if you install both Parallels and VMware Fusion Player, </br>
Windows will Go Crazy. </p>

Windows will Activate a Self-Defense Mechanism.. </br>
Refreshing the PC, does Not work. </br>
Reseting the PC, does Not work. </br>
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

if you did that, or forgot something  </br>
you need Minitool Partition Recovery software </br>
will take a lot of time scanning the HDD,  </br>
but when scanned, recovery the Lost partitions is fast. </br>
problem is that if your HDD was used for something else in the past </br>
will also detect those, </br>
and if you recover the New HDD Partition,  </br> 
will be Flagged as LBA, Extended Partition. </br>
and Windows wont boot. </br>
you need to download Gparted Live USB </br>
copy the Recovered Partitions to another Drive, </br>
also the 350MB Fat32 bcd partition, </br>
veryfiry if your old HDD is MBR or GPT before deleting. </br>
delete the old HDD, including Tables </br>
create a New MBR or GPT, MBR if Windows8.1 was installed in a Bios Machine. </br>
copy back the partitions, as Primary. </br>
can also be done shrinking the partitions and copy the partition on it self, </br>
but it tales a lot more time. </br>
Windows Remembers the HDD it was installed, and Wont boot Activated if you change HDD. </br>
Activation Keys will be Deactivated.  </br>
thats why you need the old HDD it was installed. </br>
Gparted will copy UUID, and Windows will boot again. </br>
Windows verify Partition UUID, HDD Brand & Serial Number at Boot.  </br>
but is Not as Easy... </br>
you need to create a Windows Recovery USB drive in another machine, </br>
or download the install .iso, and create a USB installer with Rufus or Windows Creator Tool. </br>
to enter recovery cmd, and recreate the bcdboot partition, fixmbr, etc... </br>
diskpart  </br>
list disk  </br>
list volume </br>
sel vol x "the bcdboot partition" </br>
list volume "to verify is selected with *" </br>
delete "Never type Clean" </br>
partition will be deleted ans Free space will increase. </br>
create partition "again" </br>
list volume  </br>
list partition </br>
to verify  </br>
format & assing letter to volume / partition  </br>
type: </br>
help create  </br>
help format  </br>
help assing  </br>
when created, formatted and assigned a letter: </br>
list volume  </br>
exit  </br>
outside diskpart, type:  </br>
bcdboot f:\windows /s c: /f BIOS </br>
f = drive where is Windows  </br>
c: = drive where the boot partition will be created.
/f ALL has problems with DUET bootloader, with Mac UEFI.  </br>
/f UEFI or /f BIOS,  </br>
you can run /UEFI in old BIOS machines with DUET Bootloader, but is Not 100% effective. </br>
if you have an older machione or Mac /f BIOS </br>
if you move windows to a New Machione, Needs Boot mode Legacy to boot BIOS, </br>
or create bcdboot again with /f UEFI  </p>
you can create /f ALL and manually Rename the EFI dir to something else, and will boot BIOS. </br>
you can manually Rename the hidden bios files, leave EFI folder, and will Boot UEFI. </br>
but Not at the same time.  </p>

also may need other bcdboot commands, like:  </br>
bcdboot fixmbr </p>

After all that, Windows will Boot again,
but if you try to create a USB Recovery Drive or make System Image Backup and FAIL.  </br>
you need copy important files manually out,  </br>
and Deactivate Windows Activation Key Licence. </br>
to clean install again Windows from USB .iso and Download again all Updates. </p>

when Windows Defense is Activated, </br>
does Not allow to Create a USB Recovery Drive, </br>
does Not allow to create a System Image Backup. </br>
You are Doomed. </p>
DSIM /Online /RestoreHealth does Not work, even if Finish Ok with No errors. </br>
sfc /scannow also does Not work, will finish Ok No error. </p>
Windows Jail </p>

IF Windows is Retail version... </br>
Allows to Move the hdd to other machine and Reactivate </br>
but Not WTG WindowsToGo using USB3.0 that needs Enterprise Not Pro licence. </br>
Pro also allows to Deactivate & Transfer / Reactivate the license to a clean isntall. </br>
if its OEM license, is machine locked, </br>
you need to buy a New License if you move windows to another machine. </p>
but can be reinstalled in the same machine, if hardware does Not change. </p>
most OEM keys are in the UEFI of Newer machines since 2013 </br>
older machines with BIOS only, keys are in a paper outside. </br>
some purchased OEM come in a White Envelope. </p>

cmd </br>
slmgr -dli "will reveal your future." </p>

reveals if the Activated License is RETAIL or OEM. </br>
if you have OEM. </p>

if you have RETAIL, the Nightmare Continues. </p>
if you have OEM, you need the perfect installer .iso  </br>
Retail Key will Not Activate OEM iso, needs Clean install Again. </br>
OEM Key will Not Activate Retail iso, needs Clean install Again. </br>
same with other versions. </p>
Key and installer need to be compatible, are locked. </p>

usually old machines like HP Stream 7 requires a OEM iso with Bing </br>
that iso does Not have the Upgrade problem of the Retail ISO </p>

RETAIL comes with a CARD, and the Activation Printed. </br>
IF you have multiple PCs with RETAIL version,  </br>
you have multiple CARDS. </p>

you need to find the correct CARD to Reactivate a Fresh / Clean Copy of Windows. </br>
if you want to avoid Nightmares in the Future... </br>
i strongly Recomend Clean installing Windows on a VirtualMachine VHD VHDX, </br>
VHDX can be attached to bcdboot drive, as a Real Drive. </br>
you can use a Virtual Drive as a Real Native... </p>

https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/boot-to-vhd--native-boot--add-a-virtual-hard-disk-to-the-boot-menu?view=windows-11
</p>
Installing 100% Native is inferior. "The method most people use". </p>

some people claim Windows Runs Faster in Virtual Machine. </br>
thats for another topic. </p>

IF you have Windows8.1 .iso </br>
Windows Update Manager does Not work... </br>
you need to download a KB with a Newer manager Version. </p>

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
Payd: Paragon Linux Drivers for Windows. </p>

if you try to see Ext4v2 hdd with EXT2FSB v0.69 will Damage the Ext4v2, </br>
wont be Readable in Newer like Linux 20.10 etc... </br>
Repairing that is antoher Nightmare. </br>
Ext2Fsb v0.69 works with Ext4v1 Linux 10.10 era. </p>

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

# slmgr /upk </br>
![image](https://user-images.githubusercontent.com/33388902/188495677-9d7277d7-5d66-4527-a76c-b60606aa40f8.png)


![0-cmd](https://user-images.githubusercontent.com/33388902/188486542-29e74ce8-aaf9-4450-9658-7c46e34ce4af.PNG)

