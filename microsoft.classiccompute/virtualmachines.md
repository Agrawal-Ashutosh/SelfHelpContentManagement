#I can't connect to my Linux VM

## **Recommended steps**
To resolve the most common issues, try one or more of the following steps.

1. Check VM's [Resource Health](data-blade:Microsoft_Azure_Support.ResourceHealthDetailBlade) for any platform issues.
2. Review your VM's [console log](data-blade:Microsoft_Azure_Classic_Compute.VirtualMachineSerialConsoleLogBlade) or screenshot to correct boot problems. Review errors in log such as FSTAB (file systems table), FSCK (file system consistency) or Networking errors.
3. [Reset Password](data-blade:Microsoft_Azure_Classic_Compute.PasswordResetBlade) to address authentication errors.
4. Restart the Virtual Machine to address startup issues.<br>
	Click 'Restart' at the top of the VM resource blade.
5. [Reset SSH configuration](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-linux-classic-reset-access/#sshconfigresetcli "Reset SSH using CLI") to fix any SSH issues.

## **Recommended documents**
[Detailed troubleshooting of SSH errors](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-linux-troubleshoot-ssh-connection/#detailed-troubleshooting-of-ssh-errors) <br>
[Automate Linux VM Customization Tasks Using CustomScript Extension](https://azure.microsoft.com/en-us/blog/automate-linux-vm-customization-tasks-using-customscript-extension/)


#I can't restart or resize an existing VM

## **Recommended steps**
To resolve the most common issues, try one or more of the following methods.

1. Review [Audit logs](data-blade:Microsoft_Azure_Insights.AzureDiagnosticsBladeWithParameter) to determine the failure reason.
2. Use following article for suggested actions by error code.<br>
	[Troubleshoot error codes for create or add a new VM](https://azure.microsoft.com/documentation/articles/virtual-machines-windows-allocation-failure/#error-string-lookup)
3. Try your request by using a smaller VM size or using a different cloud service. If using different cloud service, use following article.<br>
	[Configure regional Virtual Network to connect Cloud services](https://azure.microsoft.com/blog/vnet-to-vnet-connecting-virtual-networks-in-azure-across-different-regions/)
4. If creating a new VM by using a custom image, review the following article to verify that you followed the necessary steps to create the image.<br>
	[How to capture a classic Linux virtual machine as an image](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-linux-capture-image/)

## **Recommended documents**
[Troubleshooting allocation failure when you create, restart or resize a VM in Azure](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-windows-allocation-failure/)
 