# Azure-System-Administrator

## Azure Diagnostic Settings Standardisation Across the Estate

### Project Overview

This project aims to standardize Azure Diagnostic Settings across Azure environments. Azure resources like databases, storage accounts, and virtual machines generate logs and metrics that help with monitoring and troubleshooting.

When diagnostic settings are configured independently by different teams, resources can have different log categories, retention periods, or missing configurations.

The goal of this project is to create a unified and standard way to manage and verify diagnostic settings across Azure resources and subscriptions.

Azure Monitor and Log Analytics can be used to collect and analyze logs and metrics. Azure Storage and Event Hubs can also be used for storage and integration needs.

The configuration can be automated and validated using Azure Policy, Azure CLI, PowerShell, and Infrastructure as Code.

---

## 1. Problem Statement

In Azure, different resources and subscriptions may have diagnostic settings configured manually. This can result in:

* Missing diagnostic settings
* Incorrect log categories
* Inconsistent retention periods
* Different configurations between resources
* Difficulty in monitoring and troubleshooting
* Security and compliance gaps

There is a need for a standard and automated way to configure and verify diagnostic settings across Azure resources.

---

## 2. Use Cases

The system is used by an Azure administrator or cloud operations team to maintain consistent diagnostic settings across Azure resources.

### Key Use Cases

* Build a standard diagnostic setup.
* Ensure Azure resources follow the defined standard.
* Find resources with missing or incorrect diagnostic settings.
* Send logs and metrics to Log Analytics.
* Automatically enforce or remediate required settings.
* Monitor the compliance status of Azure resources.
* Help administrators troubleshoot and investigate events.

---

## 3. Aims

* To create a standard configuration for Azure Diagnostic Settings.
* To collect important logs and metrics from Azure resources.
* To reduce differences between diagnostic configurations.
* To identify resources that do not follow the defined standard.
* To automate configuration and compliance checking.
* To improve monitoring and troubleshooting.
* To reduce manual work for Azure administrators.
* To provide better visibility and support security and compliance requirements.

---

## 4. Requirements

### Hardware Requirements

* Computer or Laptop
* Minimum 4 GB RAM
* Stable Internet Connection

### Software Requirements

* Microsoft Azure Account
* Azure Portal
* Azure CLI
* PowerShell
* Azure Resource Manager
* ARM/Bicep or Terraform *(if required)*

---

## 5. Azure Services Used

* **Azure Monitor** – Monitoring and collecting logs and metrics.
* **Azure Diagnostic Settings** – Configuring logs and metrics for Azure resources.
* **Log Analytics Workspace** – Collecting and analyzing diagnostic logs.
* **Azure Policy** – Checking and enforcing compliance.
* **Azure Storage Account** – Storing diagnostic logs when required.
* **Azure Event Hubs** – Sending diagnostic data for integration when required.
* **Azure Resource Manager** – Managing Azure resources and configurations.


            
