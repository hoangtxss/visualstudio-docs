---
title: "Indirect constraint &#39;&lt;constraint1&gt;&#39; obtained from the type parameter constraint &#39;&lt;typeparameter1&gt;&#39; conflicts with the indirect constraint &#39;&lt;constraint2&gt;&#39; obtained from the type parameter constraint &#39;&lt;typeparameter2&gt;&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 37abd3b4-25dc-4959-8617-ce93a02bbf47
caps.latest.revision: 9
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
# Indirect constraint &#39;&lt;constraint1&gt;&#39; obtained from the type parameter constraint &#39;&lt;typeparameter1&gt;&#39; conflicts with the indirect constraint &#39;&lt;constraint2&gt;&#39; obtained from the type parameter constraint &#39;&lt;typeparameter2&gt;&#39;
A generic type is declared with conflicting constraints due to a combination of indirect constraints.  
  
 The following statement can generate this error.  
  
```  
Public Class testClass(Of t1 As {t2, t3}, t2 As Structure, t3 As Class)  
```  
  
 The indirect constraints `Structure` and `Class` cause a conflict for type parameter `t1`, because the `Structure` constraint requires that the corresponding type argument be a value type, while `Class` requires that it be a reference type.  
  
 **Error ID:** BC32109  
  
### To correct this error  
  
-   Change the type parameter constraints to avoid conflicting constraints.  
  
## See Also  
 [Generic Types in Visual Basic](../Topic/Generic%20Types%20in%20Visual%20Basic%20\(Visual%20Basic\).md)   
 [Type List](../Topic/Type%20List%20\(Visual%20Basic\).md)   
 [Structure (Visual Basic)](assetId:///263ce115-ac36-4c05-8cb7-0e0eead5c6d0)   
 [Class (Visual Basic)](assetId:///0777c6e6-46bc-451b-ad70-57b49d4ef4f7)   
 [Value Types and Reference Types](../Topic/Value%20Types%20and%20Reference%20Types.md)