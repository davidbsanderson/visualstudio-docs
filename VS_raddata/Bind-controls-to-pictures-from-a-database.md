---
title: "Bind controls to pictures from a database"
ms.custom: na
ms.date: 10/07/2016
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
ms.assetid: 9748815e-3556-49e8-86b1-c6aa593c6163
caps.latest.revision: 15
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
# Bind controls to pictures from a database
You can use the **Data Sources** window to bind an image in a database to a control in your application. For example, you can bind an image to an <xref:System.Windows.Controls.Image?qualifyHint=False> control in a WPF application, or to a <xref:System.Windows.Forms.PictureBox?qualifyHint=False> control in a Windows Forms application.  
  
 Pictures in a database are typically stored as byte arrays. Items in the **Data Sources** window that are stored as byte arrays have their control type set to **None** by default, because byte arrays can contain anything from a simple array of bytes to the executable file of a large application. To create a data-bound control for a byte array item in the **Data Sources** window that represents an image, you must select the control to create.  
  
 The following procedure assumes that the **Data Sources** window is already populated with an item that is bound to your image. For more information, see [How to: Connect to Data in a Database](../VS_raddata/How-to--Connect-to-Data-in-a-Database.md).  
  
### To bind a picture in a database to a control  
  
1.  Make sure that the design surface you want to add the control to is open in the WPF Designer or the Windows Forms Designer.  
  
2.  In the **Data Sources** window, expand the desired table or object to display its columns or properties.  
  
3.  Select the column or property that contains your image data, and select one of the following controls from its drop-down control list:  
  
    -   If the WPF designer is open, select **Image**.  
  
    -   If the Windows Forms designer is open, select **PictureBox**.  
  
    -   Alternatively, you can select a different control that supports data binding and that can display images. If the control that you want to use is not in the list of available controls, you can add it to the list and then select it. For more information, see [Add custom controls to the Data Sources window](../VS_raddata/Add-custom-controls-to-the-Data-Sources-window.md).  
  
## See Also  
 [Bind WPF controls to data in Visual Studio](../VS_raddata/Bind-WPF-controls-to-data-in-Visual-Studio1.md)