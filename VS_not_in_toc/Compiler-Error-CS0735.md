---
title: "Compiler Error CS0735"
ms.custom: na
ms.date: 10/01/2016
ms.devlang: 
  - CSharp
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: c49925fb-067c-4f29-9bef-a22115ae1507
caps.latest.revision: 4
manager: douge
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
# Compiler Error CS0735
Invalid type specified as an argument for TypeForwardedTo attribute  
  
 The following sample generates CS0735.  
  
```  
// CS735.cs  
// compile with: /target:library  
using System.Runtime.CompilerServices;  
[assembly:TypeForwardedTo(typeof(int[]))]   // CS0735  
[assembly:TypeForwardedTo(typeof(string))]   // OK  
```