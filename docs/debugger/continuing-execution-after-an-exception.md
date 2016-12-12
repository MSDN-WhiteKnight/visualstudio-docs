---
title: "Continuing Execution After an Exception | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "FSharp"
  - "VB"
  - "CSharp"
  - "C++"
  - "JScript"
  - "VB"
  - "CSharp"
  - "C++"
helpviewer_keywords: 
  - "managed exceptions, continuing execution after"
  - "exceptions, continuing execution after"
  - "debugger, exceptions"
  - "managed code, exception handling"
  - "exception handling, continuing execution after"
  - "execution, continuing after an exception"
  - "program execution"
  - "threading [Visual Studio], continuing execution after exceptions"
  - "Exceptions dialog box"
  - "programs, executing"
ms.assetid: 6fe97aac-2131-4615-bd92-d3afee741558
caps.latest.revision: 25
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# Continuing Execution After an Exception
When the debugger breaks execution because of an exception, you will see the **Exception Helper**, by default. If you have disabled the **Exception Helper** in the **Options** dialog box, you will see the **Exception Assistant** (C# or Visual Basic) or the **Exception** dialog box (C++).  
  
 When the **Exception Helper** appears, you can try to fix the problem that caused the exception.
  
## Managed and Native Code  
 In managed and native code, you can continue execution in the same thread after an unhandled exception. The **Exception Helper** unwinds the call stack to the point where the exception was thrown.
  
## Mixed Code  
 If you hit an unhandled exception while debugging a mixed native and managed code, operating system constraints prevent unwinding the call stack. If you try rewinding the call stack using the shortcut menu, an error message explains that the debugger cannot unwind from an unhandled except during mixed-code debugging.  
  
## See Also  
 [Managing Exceptions with the Debugger](../debugger/managing-exceptions-with-the-debugger.md)