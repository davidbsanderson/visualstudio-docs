---
title: "&#39;&lt;eventname&gt;&#39; implicitly defines &#39;&lt;membername&gt;&#39;, which conflicts with a member implicitly declated in &lt;type&gt; &#39;&lt;typename&gt;&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 60ddb2f4-a204-41eb-b13b-b2bb13ddb69c
caps.latest.revision: 11
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
# &#39;&lt;eventname&gt;&#39; implicitly defines &#39;&lt;membername&gt;&#39;, which conflicts with a member implicitly declated in &lt;type&gt; &#39;&lt;typename&gt;&#39;
The name of a type member conflicts with the name of a member implicitly created for an event. Events implicitly create several variables. For example, the declaration `Event X` implicitly declares the names `XEventHandler`, `XEvent`, `add_X`, and `remove_X`.  
  
 **Error ID:** BC31059  
  
### To correct this error  
  
-   Rename the explicitly declared member to remove the naming conflict.  
  
## See Also  
 [NotInBuild:Declaration Statements in Visual Basic](assetId:///81f3c398-f45c-4d95-80bf-aa39d1a0fb30)   
 [Events](../Topic/Events%20\(Visual%20Basic\).md)