---
title: "Compiler Error CS0838"
ms.custom: na
ms.date: 10/01/2016
ms.devlang: 
  - CSharp
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 22495e47-3331-42ef-921c-f76ff03ef1f7
caps.latest.revision: 7
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
# Compiler Error CS0838
An expression tree may not contain a multidimensional array initializer.  
  
 Multidimensional arrays in expression trees cannot be initialized by using an array initializer.  
  
### To correct this error  
  
1.  Create and initialize the array before creating the expression tree.  
  
## Example  
 The following example generates CS0838:  
  
```  
// cs0838.cs  
using System;  
using System.Linq;  
using System.Linq.Expressions;  
  
namespace TestNamespace  
{  
    class Test  
    {  
        static int Main()  
        {  
  
            Expression<Func<int[,]>> expr =  
                () => new int[2, 2] { { 1, 2 }, { 3, 4 } }; // CS0838  
  
            // try the following 2 lines instead  
            int[,] nums = new int[2, 2] { { 1, 2 }, { 3, 4 } };  
            Expression<Func<int[,]>> expr2 = () => nums;   
  
            return 1;  
        }  
    }  
}  
  
```  
  
## See Also  
 [Expression Trees](../Topic/Expression%20Trees%20\(C%23%20and%20Visual%20Basic\).md)