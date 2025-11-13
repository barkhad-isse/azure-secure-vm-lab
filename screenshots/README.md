

## NSG Deployment Complete
<img width="1571" height="309" alt="Screenshot 2025-11-12 203107" src="https://github.com/user-attachments/assets/341306fd-c39e-4a4f-b44d-7117b0fb6dd6" />

- Shows a completed deployment of the Network Security Group nsg-securevm. The overview confirms the deployment succeeded, with status “OK,” and displays details such as subscription, resource group, and correlation ID.

  

- **nsg_inbound_custom_rules.png**  
  Custom inbound security rules for the NSG, including the SSH rule that allows TCP port 22 only from your public IP address.

- **network_settings_after_nsg.png**  
  The network interface overview where the NSG is associated with the VM's network interface, confirming enforcement of security rules.

- **dcr_collect_deliver.png**  
  Data Collection Rule configuration page in the "collect and deliver" step, selecting performance counters and routing them to Log Analytics.

- **dcr_review_create.png**  
  Data Collection Rule page during the "review + create" step, summarizing the configuration before deployment.

- **defender_plans.png**  
  Microsoft Defender for Cloud “Defender plans” view showing Plan 1 enabled for servers and full monitoring coverage.

- **defender_recommendation_disk_encryption.png**  
  Recommendation detail from Defender for Cloud suggesting to enable Azure Disk Encryption or EncryptionAtHost for the VM.


