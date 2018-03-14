---
UID: NF:dbgeng.IDebugBreakpoint.GetCurrentPassCount
title: IDebugBreakpoint::GetCurrentPassCount method
author: windows-driver-content
description: The GetCurrentPassCount method returns the remaining number of times that the target must reach the breakpoint location before the breakpoint is triggered.
old-location: debugger\getcurrentpasscount.htm
old-project: debugger
ms.assetid: ff9b9988-6790-48d1-8423-60c63b0a90cf
ms.author: windowsdriverdev
ms.date: 2/27/2018
ms.keywords: ComOther_b9308489-679e-4ced-bd73-84cbeaadc669.xml, GetCurrentPassCount method [Windows Debugging], GetCurrentPassCount method [Windows Debugging], IDebugBreakpoint interface, GetCurrentPassCount method [Windows Debugging], IDebugBreakpoint2 interface, GetCurrentPassCount,IDebugBreakpoint.GetCurrentPassCount, IDebugBreakpoint, IDebugBreakpoint interface [Windows Debugging], GetCurrentPassCount method, IDebugBreakpoint2 interface [Windows Debugging], GetCurrentPassCount method, IDebugBreakpoint2::GetCurrentPassCount, IDebugBreakpoint::GetCurrentPassCount, dbgeng/IDebugBreakpoint2::GetCurrentPassCount, dbgeng/IDebugBreakpoint::GetCurrentPassCount, debugger.getcurrentpasscount
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	dbgeng.h
api_name:
-	IDebugBreakpoint.GetCurrentPassCount
-	IDebugBreakpoint2.GetCurrentPassCount
product: Windows
targetos: Windows
req.typenames: DOT4_ACTIVITY, *PDOT4_ACTIVITY
---

# IDebugBreakpoint::GetCurrentPassCount method


## -description


The <b>GetCurrentPassCount</b> method returns the remaining number of times that the target must reach the breakpoint location before the breakpoint is triggered.


## -syntax


````
HRESULT GetCurrentPassCount(
  [out] PULONG Count
);
````


## -parameters




### -param Count [out]

The remaining number of times that the target must hit the breakpoint before it is triggered.  The number of times that the target must pass the breakpoint <u>without</u> triggering it is the value that is returned to <i>Count</i>, minus one.


## -returns



<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>
 

This method can also return error values.  For more information, see <a href="https://msdn.microsoft.com/713f3ee2-2f5b-415e-9908-90f5ae428b43">Return Values</a>.




## -remarks



The <a href="https://msdn.microsoft.com/library/windows/hardware/ff548104">GetPassCount</a> method returns the number of hits that were originally required to trigger the breakpoint. <b>GetCurrentPassCount</b> returns the number of hits that still must occur to trigger the breakpoint. For example, if a breakpoint was created with a pass count of 20, and there have been 5 passes so far, <b>GetPassCount</b> returns 20 and <b>GetCurrentPassCount</b> returns 15.

After the target has hit the breakpoint enough times to trigger it, the breakpoint is triggered every time that it is hit, unless <a href="https://msdn.microsoft.com/library/windows/hardware/ff556759">SetPassCount</a> is called again.  You can also call <b>SetPassCount</b> to change the pass count before the breakpoint has been triggered. This call resets the original pass count and the remaining pass count.

If the debugger executes the code at the breakpoint location while stepping through the code, this execution does not contribute to the number of times that remain before the breakpoint is triggered.

The <a href="https://msdn.microsoft.com/library/windows/hardware/ff548095">GetParameters</a> method also returns the information that is returned in <i>Count</i>.

For more information about breakpoint properties, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff539284">Controlling Breakpoint Flags and Parameters</a>.


