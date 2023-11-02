# Post-Migration Tasks for Azure

This repository provides a comprehensive guide on essential post-migration tasks after migrating to Azure. It offers vital insights into ensuring the security, resilience, and optimal performance of your migrated resources.

## Workbook

### Overview

After a successful migration to Azure, users must undertake various critical tasks to maintain the security and performance of their resources. This workbook guides users through these tasks, ensuring that resources remain protected against unforeseen events, potential vulnerabilities, and that they operate efficiently.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/b9ef880e-5b85-476e-8881-a3757dcd5c11)


### How to import this Workbook on your Subscription

#### 1. Open Monitor and navigate to the Workbooks menu

To begin the installation process, you'll first need to access Azure Monitor from your Azure portal. Once you're in Azure Monitor, locate and click on the "Workbooks" menu on the left pane.  
On the Workbooks dashboard, you'll see a button to "+ New" a new Workbook. Click on this option to initiate the creation of a new Workbook.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/d690c397-dc0a-4cec-b3ab-932fa329597d)

#### 2. Import Workbook
Now, instead of starting a Workbook from scratch, you'll want to import the one provided in this GitHub repository. Look for an "Import" option, usually represented by an upward arrow or a similar icon. Click on it. Browse to the location where you've saved the `Post-Migration Tasks for Azure.workbook` file and select it to upload. Once uploaded, you should now see the contents of the Workbook reflected in your Azure portal.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/35ef1afb-5098-486a-8f93-35f7cdc67961)

Then paste the entire contents of the `Post-Migration Tasks for Azure.workbook` into the editor section.
This file can be found under the `workbook` distribution in the repository. Then click `Apply`.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/296702b3-2c11-4323-9246-6620c6a5b23a)

Finally, press the Save button to save the Workbook as resource to the desired Resource Group.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/2092add5-97dc-4fb5-acd9-19a69731be73)

### Backup And BCDR

- **Virtual Machine Backups:** It is paramount to set up backups for your virtual machines to guard against unforeseen circumstances.
- **Setting up BCDR (Business Continuity and Disaster Recovery):** Ensure that your applications remain available during planned and unplanned outages. Having a BCDR plan ensures that you can recover to a predefined state if necessary.

The workbook provides:
- Lists of virtual machines with and without Azure Site Recovery configured.
- Lists of virtual machines with and without Azure Backup configured.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/cb0b8373-389f-4b1f-a909-3c1e3784e071)

### Extension for security and monitoring

Extensions in your Virtual Machine are crucial for ensuring compliance, security, and effective monitoring. This section of the workbook verifies the presence of vital extensions in your VMs:
- **MDE Extension:** Microsoft Defender for Endpoint is essential for real-time protection against threats and integrates advanced threat detection capabilities into VMs.
- **GuestConfiguration Extension:** Ensures VM compliance with corporate Azure policies.
- **Azure Monitoring Agent:** Provides critical performance metrics and event logs for VMs, essential for observing and understanding the VM's operational health.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/dd261c20-0dcc-42b9-bfbc-5362b04a13c4)

### Alert settings

To ensure timely responses and proactiveness in managing potential issues, the workbook provides an overview of alert configurations for each Azure subscription. It covers:
- Active alerts for specific subscriptions.
- Incident-related alerts notifying users of potential disruptions or anomalies.
- Scheduled maintenance alerts to prepare users for potential operational interruptions.
- Health advisories offering guidance on best practices and optimizations for Azure resources.
- Security advisories informing users about potential vulnerabilities and enhancing Azure resources' security posture.

By regularly reviewing and acting upon these tasks, users can ensure the seamless and secure functioning of their Azure resources.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/014321a5-819d-49eb-afb9-e31ceaa303e5)

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
