#I can't connect to my Linux VM

##Recommended steps
To resolve the most common issues, try one or more of the following steps.

1. Check VM's [Resource Health](data-blade1) for any platform issues.
2. Review your VM's console log or screenshot to correct boot problems. Review errors in log such as FSTAB (file systems table), FSCK (file system consistency) or Networking errors.
3. Reset Password to address authentication errors.
4. Restart the Virtual Machine to address startup issues. Click 'Restart' at the top of the VM resource blade.
5. [Reset SSH configuration](Link1) to fix any SSH issues.
6. Need more help?

##Recommended documents
[Detailed troubleshooting of SSH errors](Link2) <br>
[Automate Linux VM Customization Tasks Using CustomScript Extension](Link3)

##metadata
linux;324567
 

data-blade1: data-blade:Microsoft_Azure_Support.ResourceHealthDetailBlade
Link1: https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-linux-classic-reset-access/#sshconfigresetcli "Reset SSH using CLI "
Link2: https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-linux-troubleshoot-ssh-connection/#detailed-troubleshooting-of-ssh-errors
Link3: https://azure.microsoft.com/en-us/blog/automate-linux-vm-customization-tasks-using-customscript-extension/