---
title: "APPLICATIONAREA Method"
ms.author: solsen
ms.custom: na
ms.date: 10/01/2018
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-financials
author: SusanneWindfeldPedersen
---

# ApplicationArea Method
Gets or sets the application areas for the current session.  
  
## Syntax  
  
```  
[ApplicationArea :=] APPLICATIONAREA([ApplicationArea])  
```  
  
#### Parameters  
 *ApplicationAreas*  
 Type: Text  
  
 A comma-separated list of application area tags to activate.  
  
 An application area tag has the format *name*, where *name* is the application area. The *name* can be any combination of letters (Aa-Zz) and numbers (0-9) without spaces. For example, to specify the **Basic** and **Fixed Assets** application areas, set the property to **Basic, FixedAssets**.  
  
## Property Value/Return Value  
 Type: Text  
  
 A comma-separated list of enabled application areas for the current session.  
  
## Remarks  
 This method lets you hide certain user interface elements (including page fields and actions, and report request page options) based on the application area to which they belong. Controls that define these items can be tagged with one or more application areas by setting the ApplicationArea property. When the ApplicationArea method is called in a client session, only those controls that are tagged with the application areas set by the method will be appear in the user interface.  
  
> [!NOTE]  
>  Currently, this functionality is intended for the application areas that are defined in **table 9178 Application Area Setup**. You can define your own application areas but be aware that the implementation might change in future release.  
  
## See Also  
 [ApplicationArea Property](../properties/devenv-ApplicationArea-Property.md)