---
title: "Run Windows PowerShell from SQL Server Management Studio | Microsoft Docs"
description: Learn how to start a Windows PowerShell session from Object Explorer in SQL Server Management Studio, with the path preset to the location of your choice of objects.
ms.prod: sql
ms.technology: sql-server-powershell
ms.topic: conceptual
ms.assetid: 1f841825-da1f-4062-9a81-3cdbab03845b
author: markingmyname
ms.author: maghan
ms.reviewer: matteot, drskwier
ms.custom: ""
ms.date: "03/14/2017"
---

# Run Windows PowerShell from SQL Server Management Studio

[!INCLUDE[SQL Server Azure SQL Database Synapse Analytics PDW ](../includes/applies-to-version/sql-asdb-asdbmi-asa-pdw.md)]

You can start Windows PowerShell sessions from **Object Explorer** in [!INCLUDE[ssManStudioFull](../includes/ssmanstudiofull-md.md)]. [!INCLUDE[ssManStudio](../includes/ssmanstudio-md.md)] launches Windows PowerShell, loads the **SqlServer** module, and sets the path context to the associated node in the **Object Explorer** tree.  

[!INCLUDE [sql-server-powershell-version](../includes/sql-server-powershell-version.md)]

When you specify running PowerShell for an object in **Object Explorer**, [!INCLUDE[ssManStudioFull](../includes/ssmanstudiofull-md.md)] starts a Windows PowerShell session in which the [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] PowerShell snap-ins have been loaded and registered. The path for the session is preset to the location of the object you right-clicked in Object Explorer. For example, if you right-click the [!INCLUDE[ssSampleDBobject](../includes/sssampledbobject-md.md)] database object in Object Explorer and select **Start PowerShell**, the Windows PowerShell path is set to the following:  

```powershell
SQLSERVER:\SQL\MyComputer\MyInstance\Databases\AdventureWorks2012>  
```

## Run PowerShell

### To run PowerShell from SQL Server Management Studio

1. Open **Object Explorer**.

2. Navigate to the node for the object to be worked on.

3. Right-click the object and select **Start PowerShell**.

## Permissions

When opened from [!INCLUDE[ssManStudio](../includes/ssmanstudio-md.md)], PowerShell does not run with Administrator privileges, which may prevent some activities such as calls to WMI.  
  
## See Also

- [SQL Server PowerShell](sql-server-powershell.md)