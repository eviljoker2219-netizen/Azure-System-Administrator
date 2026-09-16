Azure Services Used
1. Azure Monitor

Azure Monitor is used to monitor Azure resources and collect important monitoring information such as logs and metrics. In this project, it helps administrators observe the activity and performance of Azure resources and supports troubleshooting.

Cost: Basic monitoring capabilities are available without a separate charge, while some log collection, ingestion, and retention features are charged based on usage.

Alternative: Azure Resource Graph can be used to search and inspect Azure resources and their configurations, but it does not replace the complete monitoring capabilities of Azure Monitor.

2. Azure Diagnostic Settings

Azure Diagnostic Settings is the main service used in this project. It allows us to select the logs and metrics that need to be collected from Azure resources and specify where the data should be sent.

For example, diagnostic data can be sent to a Log Analytics Workspace, Storage Account, or Event Hubs.

Cost: Creating a Diagnostic Setting itself does not normally have a separate charge. However, the destination where the diagnostic data is stored or processed may have charges.

Alternative: Instead of manually configuring Diagnostic Settings for every resource, Azure Policy can be used to automatically deploy or enforce the required diagnostic configuration.

3. Log Analytics Workspace

Log Analytics Workspace is used to collect and analyze diagnostic logs from Azure resources in one centralized location. It allows administrators to search and investigate logs using Kusto Query Language (KQL).

In this project, Log Analytics helps verify that diagnostic data is being collected correctly and helps administrators troubleshoot resource and security-related events.

Cost: Log Analytics is mainly usage-based. Charges can depend on the amount of data ingested and the amount of data retained. Free allowances or Azure credits may be available depending on the subscription.

Alternative: Azure Storage Account can be used when the main requirement is to store diagnostic logs for long-term retention rather than frequently analyze them.

4. Azure Policy

Azure Policy is used to check whether Azure resources follow the standard diagnostic configuration defined for the project.

It can identify resources that have missing or incorrect diagnostic settings. Policies can also be configured to support automatic remediation for supported scenarios.

Cost: Azure Policy is generally available as an Azure governance service without a separate charge for creating and assigning policies.

Alternative: Azure Resource Graph can be used to identify and report resource configurations, but it is mainly useful for auditing and querying rather than enforcing configuration standards.

5. Azure Storage Account

Azure Storage Account can be used as an optional destination for diagnostic logs. It is useful when logs need to be stored for a longer period or archived.

Cost: Storage Accounts are generally charged based on storage capacity, transactions, redundancy, and other usage.

Alternative: Log Analytics Workspace can be used when the requirement is to actively search, query, and analyze logs instead of primarily storing them.

For this project, Storage Account is optional and does not need to be used if Log Analytics is sufficient.

6. Azure Event Hubs

Azure Event Hubs can be used to collect and stream diagnostic data in real time. It is useful when logs need to be forwarded to other applications or external processing systems.

Cost: Event Hubs is a paid Azure service, with the cost depending on the selected pricing tier and usage.

Alternative: Log Analytics can be used when the requirement is mainly log analysis, while Azure Storage can be used when the requirement is mainly log storage.

For this project, Event Hubs is optional because real-time event streaming is not required for the basic implementation.

7. Azure Resource Manager

Azure Resource Manager, also known as ARM, is the management layer used by Azure to create, manage, and organize resources.

In this project, it supports the deployment and management of Azure resources and their configurations.

Cost: Azure Resource Manager does not normally have a separate charge for managing resources. The resources created through it may have their own charges.

Alternative: Bicep can be used to define and deploy Azure resources in a simpler Infrastructure-as-Code format.

8. Azure CLI

Azure CLI is a command-line tool used to manage Azure resources and automate tasks. In this project, it can be used to check and configure diagnostic settings without performing every operation manually through the Azure Portal.

Cost: Azure CLI is free to use. However, the Azure services and resources managed through the CLI may have their normal usage charges.

Alternative: Azure PowerShell can be used to perform similar Azure administration and automation tasks.

9. Azure PowerShell

Azure PowerShell is another tool for managing and automating Azure resources. It can be used to check diagnostic settings, manage resources, and perform administrative tasks through PowerShell commands.

Cost: Azure PowerShell itself is free to use. The Azure resources managed through it may incur normal Azure charges.

Alternative: Azure CLI can be used instead of PowerShell for command-line automation.

10. Bicep

Bicep is Microsoft's Infrastructure-as-Code language for Azure. It allows Azure resources and configurations to be defined as code instead of creating everything manually.

In this project, Bicep can be used to deploy resources and standardized diagnostic configurations consistently.

Cost: Bicep itself is free to use. The Azure resources deployed using Bicep may have normal Azure charges.

Alternative: ARM Templates can be used as another Azure-native Infrastructure-as-Code approach.

Services Actually Needed for the Basic Project

For your current Azure Diagnostic Settings Standardisation project, the main services you need are:

Azure Monitor, Azure Diagnostic Settings, Log Analytics Workspace, and Azure Policy.

Azure Storage, Event Hubs, Azure CLI, PowerShell, and Bicep can be included as optional services or alternative approaches.
