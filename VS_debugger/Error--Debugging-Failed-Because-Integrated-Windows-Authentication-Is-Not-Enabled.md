---
title: "Error: Debugging Failed Because Integrated Windows Authentication Is Not Enabled"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - FSharp
  - VB
  - CSharp
  - C++
  - aspx
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-debug
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 6027cd94-74cf-470f-b7ce-6f6b68bc56ba
caps.latest.revision: 19
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
# Error: Debugging Failed Because Integrated Windows Authentication Is Not Enabled
Authentication of the user who requested debugging was prevented by an authentication error. This can occur when you try to step into a Web application or an XML Web service. One cause of this error is that integrated Windows authentication is not enabled. To enable it, follow the steps in "To enable integrated Windows authentication."  
  
 If you have enabled integrated Windows authentication and this error still appears, it is possible that this error is caused because **Digest Authentication for Windows Domain Servers** is enabled. In this situation you should contact with your network administrator.  
  
### To enable integrated Windows authentication  
  
1.  Log on to the Web server by using an administrator account.  
  
2.  Click **Start** and then click **Control Panel**.  
  
3.  In **Control Panel**, double-click **Administrative Tools**.  
  
4.  Double-click **Internet Information Services**.  
  
5.  Click the Web server node.  
  
     A **Web Sites** folder opens underneath the server name.  
  
6.  You can configure authentication for all Web sites or for individual Web sites. To configure authentication for all Web sites, right-click the **Web Sites** folder and then click **Properties**. To configure authentication for an individual Web site, open the **Web Sites** folder, right-click the individual Web site, and then click **Properties**.  
  
     The **Properties** dialog box is displayed.  
  
7.  Click the **Directory Security** tab.  
  
8.  In the **Anonymous access and authentication control** section, click **Edit**.  
  
     The **Authentication Methods** dialog box is displayed.  
  
9. Under **Authenticated access**, select **Integrated Windows authentication**.  
  
10. Click **OK** to close the **Authentication Methods** dialog box.  
  
11. Click **OK** to close the **Properties** dialog box.  
  
12. Close the **Internet Information Services** window.  
  
### To enable integrated Windows authentication in Windows Vista/IIS 7  
  
1.  Log on to the Web server by using an administrator account.  
  
2.  Turn on Windows Authentication and II6 Management Compatibility, if you have not previously done this, by following these steps:  
  
    1.  Click **Start**, click **Control Panel** and then click **Programs**.  
  
    2.  Under **Programs and Features**, click **Turn Windows features on or off**.  
  
         The User Access Control dialog box appears and prompts you for permission to continue.  
  
    3.  Click **Continue**.  
  
         The Windows Features dialog box appears.  
  
    4.  In the feature list, expand the **Internet Information Services** node.  
  
    5.  Under **Internet Information Services**, expand the **World Wide Web Services** node.  
  
    6.  Under **World Wide Web Services**, click **Security**.  
  
    7.  Click **Windows Authentication**.  
  
    8.  Under **Internet Information Services**, expand the **Web Management Tools** node.  
  
    9. Under **Web Management Tools**, expand the **IIS 6 Management Compatibility** node, and select the **IIS 6 Metabase and IIS 6 Configuration Compatibility** check box.  
  
    10. Under **Web Management Tools**, select **IIS Management Console** and Click **OK.**  
  
    11. Restart the computer for these changes to take effect.  
  
3.  Click **Start** and then, click **Control Panel**.  
  
4.  Click **Classic View**, and then double-click **Administrative Tools**.  
  
5.  In the **Name** column and double-click **Internet Information Services (IIS) Manager**.  
  
6.  In the **Connections** column, expand the node for your server.  
  
     A **Web Sites** folder opens underneath the server name.  
  
7.  Expand the **Web Sites** node and click the Web site for which you want to enable integrated Windows authentication.  
  
8.  The title of the center pane changes to the name of the Web site that you selected. In this pane, under the **IIS** heading, double-click **Authentication**.  
  
     The title of the pane changes to **Authentication**.  
  
9. In the **Authentication** pane, in the **Name** column, right-click **Windows Authentication** and then click **Enable**.  
  
10. Close the **Internet Information Services (IIS) Manager** window.  
  
## See Also  
 [Debugging Web Applications: Errors and Troubleshooting](../VS_debugger/Debugging-Web-Applications--Errors-and-Troubleshooting.md)   
 [Microsoft Digest Authentication](http://go.microsoft.com/fwlink/?LinkId=77938)   
 [Running Web Applications on Windows Vista with IIS 7.0 and Visual Studio](../Topic/Running%20Web%20Applications%20on%20Windows%20Vista%20with%20IIS%207.0%20and%20Visual%20Studio.md)