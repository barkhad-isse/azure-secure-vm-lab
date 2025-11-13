

## NSG Deployment Complete
<img width="1571" height="309" alt="Screenshot 2025-11-12 203107" src="https://github.com/user-attachments/assets/341306fd-c39e-4a4f-b44d-7117b0fb6dd6" />

- Shows a completed deployment of the Network Security Group nsg-securevm. The overview confirms the deployment succeeded, with status “OK,” and displays details such as subscription, resource group, and correlation ID.

  

## Inbound NSG Rules Configuration
<img width="2047" height="406" alt="image" src="https://github.com/user-attachments/assets/e158d170-76ab-46e5-b25b-6c6be095d73b" />
- Displays the configured inbound rules for nsg-securevm. A custom SSH rule allows port 22 only from the administrator’s public IP. Default Azure rules-AllowVnetInBound, AllowAzureLoadBalancerInBound, and DenyAllInBound—are listed beneath it, establishing the final traffic evaluation order.

## Network Interface and NSG Overview
<img width="2192" height="829" alt="Screenshot 2025-11-12 215613" src="https://github.com/user-attachments/assets/aff8da68-ee14-4517-a9a3-05080d540f0c" />
- Shows the VM’s network interface with the attached Network Security Group. The active inbound rules are visible, including the SSH rule, the virtual network rule, the load balancer rule, and the deny-all rule. This confirms that the VM is using the intended NSG and that the security rules are being applied correctly to the network interface.

## Log Analytics Workspace Creation Review
  <img width="732" height="619" alt="Screenshot 2025-11-12 221540" src="https://github.com/user-attachments/assets/9c5b4e27-c624-4d8d-9bcf-b5402a3f43b1" />

- Shows the final review step before creating the Log Analytics workspace. The configuration lists the chosen subscription, resource group, workspace name, region, and pricing tier. Validation has passed, confirming that the workspace settings are correct and ready for deployment.

## Log Analytics Workspace
<img width="1833" height="380" alt="Screenshot 2025-11-12 222102" src="https://github.com/user-attachments/assets/f6291b0d-b431-41ae-b768-0a54eb7a116d" />

- the main overview page after the Log Analytics workspace has been deployed. The workspace status is active, with details such as the resource group, region, subscription, and pricing tier clearly listed. Operational status is marked as healthy, confirming that the workspace is running without issues. Azure Monitor also displays a notice recommending an upgrade to AMA for improved data collection.


