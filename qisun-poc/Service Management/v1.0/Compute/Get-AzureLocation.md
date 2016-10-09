---
external help file: SMAzure_Compute.xml
online version: 007cc1d1-12ff-4ef0-a480-39b958aff004
schema: 2.0.0
updated_at: 10/7/2016 9:35 AM
ms.date: 10/7/2016
ms.topic: reference
source_repo: https://github.com/SummerSun/azure-docs-powershell-int
source_branch: master
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/3c5913303624ba7a7970d6758aac68ea04359cee/azureps-cmdlets-docs/Service%20Management/v1.0/Compute/Get-AzureLocation.md
---

# Get-AzureLocation
## SYNOPSIS
Gets the available data center locations for the current Azure subscription.

## SYNTAX

```
Get-AzureLocation
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The Get-AzureLocation cmdlet returns a list object with the available Azure data centers and their properties for the current Azure subscription.
Before you run this cmdlet, you need to set your current subscription with Select-AzureSubscription and Set-AzureSubscription.

## EXAMPLES

### Example 1
```
C:\PS> Get-AzureLocation
```

This command gets a list of available data centers, and their properties, for the current subscription.

## PARAMETERS

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
