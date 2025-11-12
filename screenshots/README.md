# Screenshot Descriptions

This document provides descriptions for each screenshot used in the Azure Secure VM Lab project. When adding images to the `screenshots` folder, ensure the file names match those referenced below.

- **nsg_overview.png**  
  Network Security Group overview showing the default inbound and outbound rules after the NSG is created.

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

If you capture additional screenshots, follow this pattern: use a descriptive file name and provide a concise explanation of what the screenshot shows and its relevance to the project.
