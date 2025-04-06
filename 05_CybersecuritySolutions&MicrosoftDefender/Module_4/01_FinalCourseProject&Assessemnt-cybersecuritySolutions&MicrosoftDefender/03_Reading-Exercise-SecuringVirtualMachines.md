# Exercise: Securing virtual machines

[Exercise: Securing virtual machines 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/supplement/snNYp/exercise-securing-virtual-machines)

# Exercise: Securing virtual machines

## Introduction

Thus far, you have learned how to build and protect a virtual machine hosted within Microsoft Azure using different services like Azure Firewall, Bastion, and Microsoft 365 Defender. You also learned about Microsoft Sentinel, an infrastructure monitoring solution as well as other Microsoft Defender products for Cloud, Endpoint, Identity, and Office 365, and how they can be used to protect different aspects of a network using the Microsoft 365 Defender portal.

During the course you have joined Sam’s Scoops in exploring some of these services that can protect a virtual machine running web services for Sam’s Scoops. You completed a number of exercises that would help protect the Sam’s Scoops web VM; this included firewall protection, JIT and Bastion. You are now required to put this knowledge to the test by performing a number of tasks to protect another small business.

## Case study

A small business that provides IT services has a number of systems hosted in Microsoft Azure. The backend systems are hosted on Azure virtual machines, and they need to be securely configured and protected from threats.

You have been hired as a security engineer to put together a testing environment using the many different Microsoft security services. This testing environment will form the basis for how production VMs will be protected in the future for this IT services provider.

Your employer would like you to setup protection for a virtual machine in Azure using JIT, Azure Bastion, and Azure Standard Firewall. Once this has been setup, they would also like you to configure Microsoft Sentinel to monitor the testing environment before it is deployed on the production network.

## Instructions

### Step 1: Virtual machine setup

To start building a testing environment, a virtual machine is needed first. Deploy a virtual machine in a new resource group using the provided details in the table below. No public IP will be needed for this VM as Azure Bastion will be used for remote access. Revisit the video about [Spinning up a virtual machine](link_to_spinning_up_vm_video) for a reminder on how to create virtual machines.

| Resource Group name  | Services_Test                  |
| -------------------- | ------------------------------ |
| Region               | Choose A region near you       |
| VNet                 | Services_Test_Network          |
| Network              | 172.16.0.0/16                  |
| Subnet name          | VMs                            |
| Subnet range         | 172.16.1.0/24                  |
| Virtual Machine name | ServicesVM                     |
| Image                | Windows server 2022 Datacenter |
| Size                 | Standard_DS1_v2                |
| Username             | AzAdmin                        |
| Password             | P@$$@1234567                   |

All other settings can be left as default. Once deployed, power on the machine.

### Step 2: Hub network with VNet peering

Create a hub network with VNet peering to the Service_Test_Network, all inside a new resource group, ready for an Azure Standard Firewall deployment. Use the following table for the configuration details. The activity about [Resource group and VNet creation](link_to_vnet_creation_activity) will help you to remember how to create a hub and perform VNet peering.

| Resource Group name                      | Services_Security               |
| ---------------------------------------- | ------------------------------- |
| Region                                   | Same region you chose in step 1 |
| Hub VNet name                            | Services_Hub                    |
| Subnet                                   | 192.168.1.0/26                  |
| Subnet Template                          | AzureFirewall                   |
| VNet Peering Name                        | Hub_Test                        |
| Remote Virtual network peering link name | Test_Hub                        |

All other settings can be left as default. Once deployed, power on the machine.

### Step 3: Azure Standard Firewall deployment

Deploy an Azure Standard Firewall within the hub network using the following configuration details. Refer back to the video [Azure Firewall deployment](link_to_firewall_deployment_video) to remind you of all the necessary steps that need to be performed when deploying a firewall.

| Resource Group name  | Services_Security                                    |
| -------------------- | ---------------------------------------------------- |
| Region               | Same region you chose in step 1                      |
| Firewall Name        | ServicesFirewall                                     |
| Firewall SKU         | Standard                                             |
| Firewall Management  | Use firewall rules (classic) to manage this firewall |
| Virtual network name | Services_Secruity_Network                            |
| Public IP            | Add new                                              |
| Public IP name       | Services                                             |

All other settings can be left as default.

### Step 4: Just in Time Access (JIT) setup

Enable JIT access on the ServicesVM. RDP access is enabled by default. To remind you of the steps for enabling JIT access refer back to the video [Implementing just-in-time access](link_to_jit_video).

### Step 5: Azure Bastion configuration

Configure Azure Bastion for the ServicesVM. Refer back to the video [Bastion and virtual machines](link_to_bastion_video) for a reminder of the steps. Refer to the table below for configuration details.

| Instance Name | Services_Bastion                |
| ------------- | ------------------------------- |
| Region        | Same region you chose in step 1 |
| Tier          | Standard                        |
| VNet          | Services_Test_Network           |
| Subnet        | AzureBastionSubnet              |
| Subnet Range  | 172.16.2.0                      |

All other settings can be left as default.

### Step 6: Testing remote connectivity

Use Azure Bastion with JIT and connect to the Services VM using RDP to confirm that the deployment is working. Refer back to the video [Bastion and virtual machines](link_to_bastion_video) for a reminder of the steps.

### Step 7: Implement Microsoft Sentinel

Implement Microsoft Sentinel so you’re ready for testing and training. If you need a reminder of the steps to do so, refer back to the video [Microsoft Sentinel](link_to_sentinel_video). Use the following table for the configuration details.

| Workspace Instance name | ServiceSentinel |
| ----------------------- | --------------- |
| Resource group          | Services_Test   |

### Clean-up

If you are using your own Azure subscription, it is recommended that you follow the clean-up instructions to stop compute resources after completing each lesson. When you're working in your own subscription, it's also a good idea at the end of a project to identify whether you still need the resources you created. Resources left running can cost you money. You can delete resources individually or delete the resource group to delete the entire set of resources.

Please refer to the reading, [Clean up resources](link_to_cleanup_reading) for instructions on how to delete resources after you’ve completed the exercise.

Remember to also delete the Standard Firewall as it cannot be powered off and you will continue being charged if it stays active.

## Conclusion

Completing this final course project allows you to put into practice what you have learned about securing virtual machines. By setting up a testing environment for a small business you demonstrated your understanding of how to configure and deploy key Microsoft services. You first demonstrated how to deploy a virtual machine, before moving on to protecting the network by deploying an Azure firewall. Next, you demonstrated how to protect management ports on that VM by using JIT and Azure Bastion combined. And finally, you demonstrated how to deploy Microsoft Sentinel ready for different data connectors to be added in the future.
