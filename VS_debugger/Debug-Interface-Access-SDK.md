---
title: "Debug Interface Access SDK"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-debug
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 4c0abe53-11d3-4b7a-bdc7-b054f85aaf40
caps.latest.revision: 12
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
# Debug Interface Access SDK
The Microsoft Debug Interface Access Software Development Kit (DIA SDK) provides access to debug information stored in program database (.pdb) files generated by Microsoft postcompiler tools. Because the format of the .pdb file generated by the postcompiler tools undergoes constant revision, exposing the format is impractical. Using the DIA API, you can develop applications that search for and browse debug information stored in a .pdb file. Such applications could, for example, report stack trace-back information and analyze performance data.  
  
## In This Section  
 [Getting Started](../VS_debugger/Getting-Started--Debug-Interface-Access-SDK-.md)  
 Gives an overview of the DIA SDK features and specifies where the DIA SDK is installed as well as the required header and library files.  
  
 [Querying the .Pdb File](../VS_debugger/Querying-the-.Pdb-File.md)  
 Provides instructions on how to use the DIA API to query the .pdb file.  
  
 [Symbols and Symbol Tags](../VS_debugger/Symbols-and-Symbol-Tags.md)  
 Discusses how symbols and symbol tags are used in the DIA API.  
  
 [Reference](../VS_debugger/Debug-Interface-Access-SDK-Reference.md)  
 Contains the interfaces, methods, enumerations, and structures of the DIA API.  
  
 [Dia2dump Sample](../VS_debugger/Dia2dump-Sample.md)  
 Illustrates how to use the DIA API to search for and browse debug information.  
  
 [Dia2dump.cpp Source File](../VS_debugger/Dia2dump.cpp-Source-File.md)  
 Source code used by [Dia2dump Sample](../VS_debugger/Dia2dump-Sample.md) to demonstrate the DIA API.