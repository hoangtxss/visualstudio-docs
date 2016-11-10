---
title: "How to: Apply a Shader to a 3-D Model"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-general
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: a3877bd6-abd8-4a9d-842c-6848b6c2f335
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
# How to: Apply a Shader to a 3-D Model
This document demonstrates how to use the Model Editor to apply a Directed Graph Shader Language (DGSL) shader to a 3-D model.  
  
 This document demonstrates this activity:  
  
-   Applying a shader to a 3-D model  
  
## Applying a shader to a 3-D model  
 You can apply a shader effect to a 3-D model to give it an interesting appearance.  
  
 Before you begin, make sure that the **Properties** window is displayed.  
  
#### To apply a shader to a 3-D model  
  
1.  Begin with a 3-D scene that contains one or more models. If you don't have a suitable 3-D scene, create one as described in [How to: Create a Basic 3-D Model](../VS_IDE/How-to--Create-a-Basic-3-D-Model.md). You also have to have a DGSL shader that you can apply to the model. If you don't have a suitable shader, create one as described in [How to: Create a Basic Color Shader](../VS_IDE/How-to--Create-a-Basic-Color-Shader.md) and make sure that you have saved it to a file before you continue.  
  
2.  In **Select** mode, select the model that you want to apply the shader to, and then in the **Properties** window, in the **Filename** property of the **Effect** property group, specify the DGSL shader that you want to apply to the model.  
  
 Here's a model that has the basic color effect applied to it:  
  
 ![3&#45;D scene that shows the basic color effect](../VS_IDE/media/Digit-3D-Model-Effect.png "Digit-3D-Model-Effect")  
  
 After you apply a shader to a model, you can open it in the Shader Designer by selecting the model, and then in the **Properties** window, in the **(Advanced)** property of the **Effect** property group, choosing the ellipsis (**...**) button.  
  
## See Also  
 [How to: Create a Basic 3-D Model](../VS_IDE/How-to--Create-a-Basic-3-D-Model.md)   
 [How to: Create a Basic Color Shader](../VS_IDE/How-to--Create-a-Basic-Color-Shader.md)   
 [Model Editor](../VS_IDE/Model-Editor.md)   
 [Shader Designer](../VS_IDE/Shader-Designer.md)