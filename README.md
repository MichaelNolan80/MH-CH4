# Building a Hacking Virtual Lab
## Downloading and Install the Software - 

- 1 - I started by download the lastest VMware Software <a href="https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware%20Workstation%20Pro">From here. You need to be signed in.</a> Make sure you pick the right operating system you are putting the VMware on. 
- 2 - I downloaded Kali Linux <a href="https://www.kali.org/get-kali/#kali-installer-images">From here.</a>
- 3 - I installed the VMware onto an extra partition on my hard drive.
- 4 - I now look at what system resorces my laptop have so I knew how much I have to give.
- 5 - I have 32gbs of RAM and my processer is - 12th Gen Intel(R) Core(TM) i7-1265U   1.80 GHz. This means I have 10 cores and 12 threads
- 6 - Installed Kali making sure I give it enough disk space,(40 GB) im going to keep it on a single file as this part of the hard drive is just for the VM ware. Ill add 2 cores with 2 proccerers each. Ill add 4GBs of RAM and see how I get on.
- 7 - Iv added a few extra steps for good practice - Once Kali has loaded its time to update the operating system. with Sudo Apt Update.
- 8 Now its time to upgrade - Sudo apt upgrade -y
![image](https://github.com/user-attachments/assets/9abc75b4-3ffb-4a78-a1a9-da40249d10b8)]
- 9 - now we remove any unwanted packets left behind on the update/upgrade - sudo apt autoremove
- 10 - now that we are done we are going to take a snap shot of the operating system in case we brake something later.
- ![image](https://github.com/user-attachments/assets/c63d77f8-f2ec-45b2-9a63-171c95a262fa)

- 11 - Now we are going to download two systems that are purposley vulnerable one is Metasploitable 2 and the other is windows 7 pre patched. 
- 12 - Time to down load <a href="https://sourceforge.net/projects/Metasploitable/">Metasploitable 2.</a>, This was not as easy as i has hoped so headed to youtube for some help. as the folder did not have a clear file to use. Turns out the have to create the VM without an OS but then add it after. I got the info from <a href="https://www.youtube.com/watch?v=5F7j2E94p9Y">INfoSec Pat Here.</a>

- 13 - As this VM does not need amy resorces I have give it 20GB hard drive and 2GB of RAM. I did have an issue with my mouse getting stuck, im using multipal monitors and i found disconnecting my laptop form the docking station sorted it so i could releave it, there maybe a mouse issue with VMware that i will look into.
- 14 - now its time to download and install windows 7, you habe to make sure you find a pre-patched version of this as as we need the exploits still available. I had a copy so I used that.
- 15 - Im going to give it 40GBs of hard drive and 4 GBs for RAM, lets see how we get on.
- 16 - now thats done we have to install MySQL on the Windows 7 system <a href="http://www.oldversion.com/windows/mysql-community-server-5-5-15">From here.</a>
![image](https://github.com/user-attachments/assets/7156e84a-1b22-4ef5-917e-6be71e8d21bd)
- 17 - Im having a little issue with the files so im going to add a shared folder so that i can put files into the folder from my local drive and can access them from the VM's.This is done by closing the VM to start then right clicking the VM, options and Shared Folders. 
- ![image](https://github.com/user-attachments/assets/a551baef-0854-4fc1-b9ef-7937ba59f975)

- 18 - Iv created a Shared folder in the VM Folder to keep everything net. I have added all the VMs to the access list for the Shared Folder. 
![image](https://github.com/user-attachments/assets/6e56b9f2-5cdc-49c8-ad74-6cb6fdbd1040)

- 19 - So theres extra steps for this to work with legacy OS's, pop up is sending me to get <a href=" https://packages-prod.broadcom.com/tools/frozen/linux/linux.iso">This File.</a>  and then go to <a href="https://knowledge.broadcom.com/external/article?legacyId=1014294">website to get the instructions.</a>




