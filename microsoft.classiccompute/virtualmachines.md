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
 
#My VM is slow

## **Recommended steps**
Try following steps to diagnose and mitigate VM performance issues.

* Review your application error logs, traces and metrics to determine if any application level bottlenecks causing performance issues.<br>
Restart Application and machine as a quick way to recover from one-time issues.

* Review OS (Operating System) level metrics such as CPU, memory usage, IO and network to see if any resource has consistent high utilization.<br>
On Windows you can use Perfmon tool. On Linux, use commands such as Top, VmStat, Lsof & Tcpdump.

* Use VM Diagnostics and Storage Diagnostics in Azure Portal to identify if any resource being overutilized or throttled.
	* [Enable diagnostics, monitor, identify and remediate issues with Azure VMs and Storage](https://support.microsoft.com/en-us/kb/3150851)
 

* Address any VM OS issues by restarting the VM <br>
	* Click 'Restart' at the top of the VM resource blade.

* Scale up the Virtual Machine to a different VM type or series for increased performance.<br>
Click ‘Size’ in the Settings blade of the VM resource.

* Consider using Premium Storage account if its an I/O intensive use-case. <br>
[Premium Storage: High-Performance Storage for Azure Virtual Machine Workloads](https://azure.microsoft.com/en-us/documentation/articles/storage-premium-storage/) 

## **Recommended documents**
[Detailed troubleshooting of Azure Storage ](https://azure.microsoft.com/en-us/documentation/articles/storage-monitoring-diagnosing-troubleshooting/)

#Test problem type

## **Recommended steps**
Try following steps to diagnose and mitigate VM performance issues.

* Review your application error logs, traces and metrics to determine if any application level bottlenecks causing performance issues.<br>
Restart Application and machine as a quick way to recover from one-time issues.

* Review OS (Operating System) level metrics such as CPU, memory usage, IO and network to see if any resource has consistent high utilization.<br>
On Windows you can use Perfmon tool. On Linux, use commands such as Top, VmStat, Lsof & Tcpdump.

* Use VM Diagnostics and Storage Diagnostics in Azure Portal to identify if any resource being overutilized or throttled.
	* [Enable diagnostics, monitor, identify and remediate issues with Azure VMs and Storage](https://support.microsoft.com/en-us/kb/3150851)
 

* Address any VM OS issues by restarting the VM <br>
	* Click 'Restart' at the top of the VM resource blade.

* Scale up the Virtual Machine to a different VM type or series for increased performance.<br>
Click ‘Size’ in the Settings blade of the VM resource.

* Consider using Premium Storage account if its an I/O intensive use-case. <br>
[Premium Storage: High-Performance Storage for Azure Virtual Machine Workloads](https://azure.microsoft.com/en-us/documentation/articles/storage-premium-storage/) 

## **Recommended documents**
[Detailed troubleshooting of Azure Storage ](https://azure.microsoft.com/en-us/documentation/articles/storage-monitoring-diagnosing-troubleshooting/)