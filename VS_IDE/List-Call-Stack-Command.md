---
title: "List Call Stack Command"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-general
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: a8b20bf2-81d2-4069-aea8-23e6b15b4347
caps.latest.revision: 12
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# List Call Stack Command
Displays the current call stack.  
  
## Syntax  
  
```  
Debug.ListCallStack [/Count:number] [/ShowTypes:yes|no]  
[/ShowNames:yes|no] [/ShowValues:yes|no] [/ShowModule:yes|no]  
[/ShowLineOffset:yes|no] [/ShowByteOffset:yes|no]  
[/ShowLanguage:yes|no] [/IncludeCallsAcrossThreads:yes|no]  
[/ShowExternalCode:yes|no] [Thread:n] [index]  
```  
  
## Arguments  
 `index`  
 Optional. Sets the current stack frame and displays no output.  
  
## Switches  
 Each switch can be invoked using either its complete form or a short form.  
  
 /Count:`number` [or] /C:`number`  
 Optional. Maximum number of call stacks to display. The default value is unlimited.  
  
 /ShowTypes:`yes`&#124;`no` [or] /T:`yes`&#124;`no`  
 Optional. Specifies whether to display parameter types. Default value is `yes`.  
  
 /ShowNames:`yes`&#124;`no` [or] /N:`yes`&#124;`no`  
 Optional. Specifies whether to display parameter names. Default value is `yes`.  
  
 /ShowValues:`yes`&#124;`no` [or] /V:`yes`&#124;`no`  
 Optional. Specifies whether to display parameter values. Default value is `yes`.  
  
 /ShowModule:`yes`&#124;`no` [or] /M:`yes`&#124;`no`  
 Optional. Specifies whether to display the module name. Default value is `yes`.  
  
 /ShowLineOffset:`yes`&#124;`no` [or] /#:`yes`&#124;`no`  
 Optional. Specifies whether to display the line offset. Default value is `no`.  
  
 /ShowByteOffset:`yes`&#124;`no` [or] /B:`yes`&#124;`no`  
 Optional. Specifies whether to display the byte offset. Default value is `no`.  
  
 /ShowLanguage:`yes`&#124;`no` [or] /L:`yes`&#124;`no`  
 Optional. Specifies whether to display the language. Default value is `no`.  
  
 /IncludeCallsAcrossThreads:`yes`&#124;`no` [or] /I:`yes`&#124;`no`  
 Optional. Specifies whether to include calls to or from other threads. Default value is `no`.  
  
 /ShowExternalCode:`yes`&#124;`no`  
 Optional. Specifies whether to display Just My Code for the callstack. When Just My Code is off, all non-user code is displayed. When Just My Code is on, non-user code is displayed as `[external]` in the callstack output.  
  
 Thread:`n`  
 Optional. Displays the callstack for thread `n`. If no thread is specified, diplays the callstack for the current thread.  
  
## Remarks  
 Changes made to the arguments or switches apply to future invocations of this command. If you issue Debug.ListCallStackby itself, the entire call stack displays. If you specify an index, for example,  
  
```  
Debug.ListCallStack 2  
```  
  
 then the current stack frame is set to that frame (in this case, the second frame).  
  
 You can also write this command using its pre-defined alias, kb. For example, you can enter  
  
```  
kb 2  
```  
  
 to set the current stack frame to the second frame.  
  
## Example  
  
```  
>Debug.CallStack /Count:4 /ShowTypes:yes  
```  
  
## See Also  
 [List Disassembly Command](../VS_IDE/List-Disassembly-Command.md)   
 [List Threads Command](../VS_IDE/List-Threads-Command.md)   
 [Visual Studio Commands](../VS_IDE/Visual-Studio-Commands.md)   
 [Command Window](../VS_IDE/Command-Window.md)   
 [Find/Command Box](../VS_IDE/Find-Command-Box.md)   
 [Visual Studio Command Aliases](../VS_IDE/Visual-Studio-Command-Aliases.md)