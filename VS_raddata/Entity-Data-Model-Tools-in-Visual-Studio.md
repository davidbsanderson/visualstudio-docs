---
title: "Entity Data Model Tools in Visual Studio"
ms.custom: na
ms.date: 10/10/2016
ms.devlang: 
  - VB
  - CSharp
  - C++
  - aspx
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 1b06b573-84aa-4458-b3f5-e238df47bf45
caps.latest.revision: 21
manager: ghogen
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# Entity Data Model Tools in Visual Studio
Entity Framework is an object-relational mapping technology that enables .NET developers to work with relational data by using domain-specific objects. It eliminates the need for most of the data-access code that developers usually need to write. Entity Framework is the recommended object-relational mapping (ORM) modeling technology for new .NET applications.  
  
 As of March 2016, the most current released version is [Entity Framework 6](https://msdn.microsoft.com/en-us/data/ef) . [Entity Framework 7](https://docs.efproject.net/en/latest/) is in pre-release.  
  
 Entity Data Model Tools are designed to help you build Entity Framework applications. The complete documentation for Entity Data Model Tools is here: [Entity Framework](https://msdn.microsoft.com/en-us/data/jj590134).  
  
 With Entity Data Model Tools, you can create a *conceptual model* from an existing database and then graphically visualize and edit your conceptual model. Or, you can graphically create a conceptual model first, and then generate a database that supports your model. In either case, you can automatically update your model when the underlying database changes and automatically generate object-layer code for your application. Database generation and object-layer code generation are customizable.  
  
 These are the specific tools that make up Entity Data Model Tools in Visual Studio 2015:  
  
-   You can use the ADO.NET **Entity Data Model Designer** (**Entity Designer**) to visually create and modify entities, associations, mappings, and inheritance relationships. The **Entity Designer** also generates C# or Visual Basic object-layer code.  
  
-   You can use the **Entity Data Model Wizard** to generate a conceptual model from an existing database and add database connection information to your application.  
  
-   You can use the **Create Database Wizard** to create a conceptual model first and then create a database that supports the model.  
  
-   You can use the **Update Model Wizard** to update your conceptual model, storage model, and mappings when changes have been made to the underlying database.  
  
    > [!NOTE]
    >  Starting with Visual Studio 2010, Entity Data Model Tools do not support SQL Server 2000.  
  
 The tools generate or modify an .edmx file. This file contains information that describes the conceptual model, the storage model, and the mappings between them. For more information, see  [EDMX](https://msdn.microsoft.com/en-us/data/jj650889.aspx).  
  
 Entity Framework Power Tools help you build applications that use the Entity Data Model. The tools can generate a conceptual model, validate an existing model, produce source-code files that contain object classes based on the conceptual model, and produce source-code files that contain views that the model generates. For detailed information, see [Pre-Generated Mapping Views](https://msdn.microsoft.com/en-us/data/dn469601.aspx).  
  
## Related topics  
  
|Title|Description|  
|-----------|-----------------|  
|[ADO.NET Entity Framework](../Topic/ADO.NET%20Entity%20Framework.md)|Describes how to use Entity Data Model Tools, which Entity Framework provides, to create applications.|  
|[Entity Data Model](../Topic/Entity%20Data%20Model.md)|Provides links and information for working with data that is used by applications built on Entity Framework.|  
|[Getting Started on Full .NET (Console, WinForms, WPF, etc.)](https://docs.efproject.net/en/latest/platforms/full-dotnet/getting-started.html)|Provides tutorials on how to create .NET desktop applications that use Entity Framework 7.|  
|[ASP.NET 5 Application to New Database](https://docs.efproject.net/en/latest/platforms/aspnetcore/new-db.html)|Describes how to create a new ASP.NET 5 application by using Entity Framework 7.|  
  
## See Also  
 [Visual Studio data tools for .NET](../VS_raddata/Visual-Studio-data-tools-for-.NET.md)