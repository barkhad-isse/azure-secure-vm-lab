

## NSG Deployment Complete
<img width="1571" height="309" alt="Screenshot 2025-11-12 203107" src="https://github.com/user-attachments/assets/341306fd-c39e-4a4f-b44d-7117b0fb6dd6" />

- Shows a completed deployment of the Network Security Group nsg-securevm. The overview confirms the deployment succeeded, with status “OK,” and displays details such as subscription, resource group, and correlation ID.


## Inbound NSG Rules Configuration
<img width="2047" height="406" alt="image" src="https://github.com/user-attachments/assets/e158d170-76ab-46e5-b25b-6c6be095d73b" />

- Displays the configured inbound rules for nsg-securevm. A custom SSH rule allows port 22 only from the administrator’s public IP. Default Azure rules-AllowVnetInBound, AllowAzureLoadBalancerInBound, and DenyAllInBound-are listed beneath it, establishing the final traffic evaluation order.

## Network Interface and NSG Overview
<img width="2192" height="829" alt="513626700-aff8da68-ee14-4517-a9a3-05080d540f0c" src="https://github.com/user-attachments/assets/84c5d7c9-f689-4b32-80ff-618dc27b66e1" />


- The VM’s network interface with the attached Network Security Group. The active inbound rules are visible, including the SSH rule, the virtual network rule, the load balancer rule, and the deny-all rule. This confirms that the VM is using the intended NSG and that the security rules are being applied correctly to the network interface.

## Log Analytics Workspace Creation Review
  <img width="732" height="619" alt="Screenshot 2025-11-12 221540" src="https://github.com/user-attachments/assets/9c5b4e27-c624-4d8d-9bcf-b5402a3f43b1" />

- The final review step before creating the Log Analytics workspace. The configuration lists the chosen subscription, resource group, workspace name, region, and pricing tier. Validation has passed, confirming that the workspace settings are correct and ready for deployment.

## Log Analytics Workspace
<img width="1833" height="380" alt="Screenshot 2025-11-12 222102" src="https://github.com/user-attachments/assets/f6291b0d-b431-41ae-b768-0a54eb7a116d" />

- The main overview page after the Log Analytics workspace has been deployed. The workspace status is active, with details such as the resource group, region, subscription, and pricing tier clearly listed. Operational status is marked as healthy, confirming that the workspace is running without issues. Azure Monitor also displays a notice recommending an upgrade to AMA for improved data collection.

## Data Collection Rule - Collect and Deliver Configuration

 <img width="554" height="429" alt="Screenshot 2025-11-12 225334" src="https://github.com/user-attachments/assets/829bc5b2-b8aa-48c7-9736-1500b21dfb87" />

- The configuration step where data sources are selected and mapped to their destinations. Performance counters have been added as the chosen data source, and the data is set to be sent to Azure Monitor Logs. This step defines what the rule will collect from the virtual machine and where the collected data will be stored for analysis. 


## Data Collection Rule Overview
<img width="734" height="985" alt="Screenshot 2025-11-12 225941" src="https://github.com/user-attachments/assets/eaaa4615-55e7-46d0-8b6b-828f4eac7497" />

- Shows the overview of the dcr-securevm data collection rule after deployment. The rule is linked to the rg-securevm-swiss resource group and uses the Azure for Students subscription. One data source and one connected resource are active, and the platform is registered as Linux. All essential identifiers, such as the immutable ID and subscription details, are listed to confirm that the rule is properly created and recognized by Azure Monitor.


## Defender for Cloud Plan Configuration
<img width="1995" height="541" alt="513629711-62430db5-1d4a-4f37-90ee-cfd211ce0848" src="https://github.com/user-attachments/assets/e3c67fe8-110f-4b25-bb76-c0e7be49ad50" />


- Shows the configuration of Microsoft Defender for Cloud across the subscription. Foundational CSPM is active with full monitoring, while Defender CSPM is enabled for enhanced security posture management. Under Cloud Workload Protection, the Servers plan is turned on for one virtual machine, providing full monitoring coverage. Other workload protections such as App Service, Databases, Storage, and Containers remain available but disabled, allowing selective activation based on project needs.

## Defender for Cloud Security Recommendations
<img width="2048" height="854" alt="36e826c6-57e3-4b63-97f2-97e70ca76fed" src="https://github.com/user-attachments/assets/05443d33-5378-465c-b6c6-13c7828da455" />

- Shows a list of security recommendations generated for the environment by Defender for Cloud. Each recommendation highlights a potential security improvement, such as enabling backup, configuring endpoint protection, or enforcing encryption. The panel includes the risk level, affected resource, attack path presence, and current status. None of the recommendations are assigned yet, allowing them to be reviewed and prioritized based on security needs.

## Virtual Machine Resource Health - Security Recommendations
<img width="2446" height="615" alt="Screenshot 2025-11-12 234305" src="https://github.com/user-attachments/assets/177f36bf-6791-45ee-9a14-6656261a9f75" />

- Displays the security health status specifically for the virtual machine securevm01.
The view lists all active issues marked as unhealthy, such as missing disk encryption, missing guest configuration settings, lack of backup, and host-level attestation.
Each recommendation includes a severity rating, helping prioritize which hardening actions should be applied first to strengthen the VM’s security.
