---
title: CTRL+F (Break to KD)
description: The CTRL+F key cancels commands or breaks into the debugger.
ms.assetid: 45bb7eaf-cb79-4fb4-a01d-373bfb1957c3
keywords: ["CTRL+F (Break to KD) Windows Debugging"]
ms.author: windowsdriverdev
ms.date: 05/23/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
topic_type:
- apiref
api_name:
- CTRL+F (Break to KD)
api_type:
- NA
---

# CTRL+F (Break to KD)


The CTRL+F key cancels commands or breaks into the debugger. (This control key is particularly useful when you are using CDB to debug KD itself.)

``` syntax
CTRL+F  ENTER 
```

## <span id="ddk_meta_ctrl_f_dbg"></span><span id="DDK_META_CTRL_F_DBG"></span>


### <span id="Environment"></span><span id="environment"></span><span id="ENVIRONMENT"></span>Environment

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Debuggers</strong></p></td>
<td align="left"><p>CDB, KD</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Modes</strong></p></td>
<td align="left"><p>user mode, kernel mode</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Targets</strong></p></td>
<td align="left"><p>live, crash dump</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Platforms</strong></p></td>
<td align="left"><p>all</p></td>
</tr>
</tbody>
</table>

 

Remarks
-------

Under typical conditions, CTRL+F is identical to the standard break commands ([**CTRL+C**](ctrl-c--break-.md) in KD and CDB, and [Debug | Break](debug---break.md) or CTRL+BREAK in WinDbg.)

However, if you are debugging KD with CDB, these two keys will work differently. CTRL+C will be intercepted by the host debugger (CDB), while CTRL+F will be intercepted by the target debugger (KD).

## <span id="see_also"></span>See also


[**.breakin (Break to the Kernel Debugger)**](-breakin--break-to-the-kernel-debugger-.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[debugger\debugger]:%20CTRL+F%20%28Break%20to%20KD%29%20%20RELEASE:%20%285/15/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




