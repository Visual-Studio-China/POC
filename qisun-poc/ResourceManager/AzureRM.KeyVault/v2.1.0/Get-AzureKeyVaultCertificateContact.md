---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=826269
schema: 2.0.0
ms.assetid: 996FA5F2-AFAE-4424-AFDB-2DEEAB5143D1
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.1.0/Get-AzureKeyVaultCertificateContact.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.1.0/Get-AzureKeyVaultCertificateContact.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureKeyVaultCertificateContact

## SYNOPSIS
Gets contacts that are registered for certificate notifications for a key vault.

## SYNTAX

```
Get-AzureKeyVaultCertificateContact [-VaultName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureKeyVaultCertificateContact** cmdlet gets contacts that are registered for certificate notifications for a key vault in Azure Key Vault.

## EXAMPLES

### Example 1: Get all certificate contacts
```
PS C:\>$Contacts = Get-AzureKeyVaultCertificateContact -VaultName "Contoso"
```

This command gets all of the contacts for the certificate objects in the Contoso key vault, and then stores them in the $Contacts variable.

## PARAMETERS

### -VaultName
Specifies the name of the key vault.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### List<Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateContact>

## NOTES

## RELATED LINKS

[Add-AzureKeyVaultCertificateContact](.\Add-AzureKeyVaultCertificateContact.md)

[Remove-AzureKeyVaultCertificateContact](.\Remove-AzureKeyVaultCertificateContact.md)

