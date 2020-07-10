# Azure Storage monitoring policy samples

The samples contained here can be used with Azure Policy to enable the collection of Azure Storage logs for use in Azure Monitor logs. Each template supports parameterization and can be used in [remediation tasks](https://docs.microsoft.com/azure/governance/policy/how-to/remediate-resources) to enable diagnostic settings for existing storage accounts that are not compliant if you use the value **DeployIfNotExists** for the **effect** parameter.

## Samples

* [azurepolicy_all_LA.json](azurepolicy_all_LA.json) - Enable diagnostics for the root storage account as well as blobs, files, tables, and queues for all metrics and logs
* [azurepolicy_blobServices_LA.json](azurepolicy_blobServices_LA.json) - Enable diagnostics for blobs only (can be used in combination with other individual polices) for all metrics and logs
* [azurepolicy_fileServices_LA.json](azurepolicy_fileServices_LA.json) - Enable diagnostics for files only (can be used in combination with other individual polices) for all metrics and logs
* [azurepolicy_LA.json](azurepolicy_LA.json) - Enable diagnostics for the root storage account only (can be used in combination with other individual polices) for all metrics
* [azurepolicy_queueServices_LA.json](azurepolicy_queueServices_LA.json) - Enable diagnostics for queues only (can be used in combination with other individual polices) for all metrics and logs
* [azurepolicy_tableServices_LA.json](azurepolicy_tableServices_LA.json) - Enable diagnostics for tables only (can be used in combination with other individual polices) for all metrics and logs

> **Note:** Individual policies can be used in a standalone manner or packaged in an [Azure Policy initiative](https://docs.microsoft.com/azure/governance/policy/concepts/initiative-definition-structure).
