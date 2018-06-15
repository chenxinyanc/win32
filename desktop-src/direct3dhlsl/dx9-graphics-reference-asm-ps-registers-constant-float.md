---
title: Constant Float Register
description: Pixel shader input register for a 4D floating-point constant.
ms.assetid: e4f46a48-c81e-4105-901b-332b92fa6195
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Constant Float Register

Pixel shader input register for a 4D floating-point constant.

They can be set using [def - ps](def---ps.md) or [**SetPixelShaderConstantF**](https://msdn.microsoft.com/library/windows/desktop/bb174452).

The behavior of shader constants has changed between Direct3D 8 and Direct3D 9.

-   For Direct3D 9, constants set with defx assign values to the shader constant space. The lifetime of a constant declared with defx is confined to the execution of that shader only. Conversely, constants set using the APIs SetXXXShaderConstantX initialize constants in global space. Constants in global space are not copied to local space (visible to the shader) until SetxxxShaderConstants is called.
-   For Direct3D 8, constants set with defx or the APIs both assign values to the shader constant space. Each time the shader is executed, the constants are used by the current shader regardless of the technique used to set them.

## Examples

Here is an example declaring two floating-point constants within a shader.


```
def c40, 0.0f,0.0f,0.0f,0.0f;
```



These constants are loaded every time [**SetPixelShader**](https://msdn.microsoft.com/library/windows/desktop/bb174450) is called.

If you are setting constant values with the API, there is no shader declaration required.

## Related topics

<dl> <dt>

[Registers](dx9-graphics-reference-asm-ps-registers.md)
</dt> </dl>

 

 



