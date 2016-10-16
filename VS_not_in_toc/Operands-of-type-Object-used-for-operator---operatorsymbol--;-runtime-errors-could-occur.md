---
title: "Operands of type Object used for operator &#39;&lt;operatorsymbol&gt;&#39;; runtime errors could occur"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: f61944ba-863b-4a82-aae4-249bda52ec8d
caps.latest.revision: 10
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
# Operands of type Object used for operator &#39;&lt;operatorsymbol&gt;&#39;; runtime errors could occur
An expression uses an operator for which one or both operands are of the [Object Data Type](../Topic/Object%20Data%20Type.md).  
  
 When a variable or expression evaluates to `Object`, the compiler must perform *late binding*, which causes extra operations at run time. It also exposes your application to potential run-time errors. For example, suppose you assign a <xref:System.Windows.Forms.Form?qualifyHint=False> to an `Object` variable and then try to use it with the [/ Operator (Visual Basic)](../Topic/-%20Operator%20\(Visual%20Basic\)3.md). If you do this, the runtime throws an <xref:System.InvalidCastException?qualifyHint=False> because Visual Basic cannot convert a <xref:System.Windows.Forms.Form?qualifyHint=False> object to a numeric value.  
  
 By default, this message is a warning. For information on hiding warnings or treating warnings as errors, see [Configuring Warnings in Visual Basic](../VS_IDE/Configuring-Warnings-in-Visual-Basic.md).  
  
 **Error ID:** BC42019  
  
### To correct this error  
  
-   If possible, arrange the operands to evaluate to data types for which the operator is defined.  
  
## See Also  
 [Arithmetic Operators in Visual Basic](../Topic/Arithmetic%20Operators%20in%20Visual%20Basic.md)