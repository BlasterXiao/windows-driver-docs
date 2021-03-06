---
title: Adding GDL Extensions to an Existing GPD File
author: windows-driver-content
description: Adding GDL Extensions to an Existing GPD File
ms.assetid: 5ba2a447-e133-47bb-aa1e-93abe75c6eef
keywords:
- in-box autoconfiguration support WDK printer , GDL extensions
- GDL files WDK printer
- extensions WDK GDL files
- GPD files WDK GDL extensions
- GPD files WDK GDL extensions , adding
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Adding GDL Extensions to an Existing GPD File


If you intend to add support for autoconfiguration to an existing in-box GPD file, you should:

1.  Create the GDL file. The GDL file should have the **\*BidiQuery** and **\*BidiResponse** elements that correspond to the **\*Feature**/**\*Option** constructs, as specified in the PPD file. Note that you must add these elements only for features that require bidi information.

2.  Include the GDL file as part of the driver-dependent file list.

This section includes:

[New Keyword for GPD Schema](new-keyword-for-gpd-schema.md)

[Autoconfiguration Flow for GPD in Windows Vista](autoconfiguration-flow-for-gpd-in-windows-vista.md)

[Adding Constructs to Your GDL File for GPD](adding-constructs-to-your-gdl-file-for-gpd.md)

 

 


--------------------
[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bprint\print%5D:%20Adding%20GDL%20Extensions%20to%20an%20Existing%20GPD%20File%20%20RELEASE:%20%289/1/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")


