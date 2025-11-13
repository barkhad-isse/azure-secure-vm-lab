

## NSG Deployment Complete
<img width="1571" height="309" alt="Screenshot 2025-11-12 203107" src="https://github.com/user-attachments/assets/341306fd-c39e-4a4f-b44d-7117b0fb6dd6" />

- Shows a completed deployment of the Network Security Group nsg-securevm. The overview confirms the deployment succeeded, with status “OK,” and displays details such as subscription, resource group, and correlation ID.

  

## Inbound NSG Rules Configuration
<img width="2047" height="406" alt="image" src="https://github.com/user-attachments/assets/e158d170-76ab-46e5-b25b-6c6be095d73b" />
- Displays the configured inbound rules for nsg-securevm. A custom SSH rule allows port 22 only from the administrator’s public IP. Default Azure rules-AllowVnetInBound, AllowAzureLoadBalancerInBound, and DenyAllInBound—are listed beneath it, establishing the final traffic evaluation order.

## Network Interface and NSG Overview
<img width="2192" height="829" alt="Screenshot 2025-11-12 215613" src="https://github.com/user-attachments/assets/aff8da68-ee14-4517-a9a3-05080d540f0c" />
- Shows the VM’s network interface with the attached Network Security Group. The active inbound rules are visible, including the SSH rule, the virtual network rule, the load balancer rule, and the deny-all rule. This confirms that the VM is using the intended NSG and that the security rules are being applied correctly to the network interface.

##
  
- 

- **dcr_review_create.png**  
  Data Collection Rule page during the "review + create" step, summarizing the configuration before deployment.

- **defender_plans.png**  
  Microsoft Defender for Cloud “Defender plans” view showing Plan 1 enabled for servers and full monitoring coverage.

- **defender_recommendation_disk_encryption.png**  
  Recommendation detail from Defender for Cloud suggesting to enable Azure Disk Encryption or EncryptionAtHost for the VM.


