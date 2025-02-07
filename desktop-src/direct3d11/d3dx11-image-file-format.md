---
title: D3DX11_IMAGE_FILE_FORMAT enumeration
description: Note The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps. Image file formats supported by D3DX11Createxxx and D3DX11Savexxx functions.
ms.assetid: 89fa9ab8-3be0-4dc5-a533-94edb01df36a
keywords:
- D3DX11_IMAGE_FILE_FORMAT enumeration Direct3D 11
- LPD3DX11_IMAGE_FILE_FORMAT enumeration pointer Direct3D 11
topic_type:
- apiref
api_name:
- D3DX11_IMAGE_FILE_FORMAT
api_location:
- D3DX11tex.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
---

# D3DX11\_IMAGE\_FILE\_FORMAT enumeration

> [!Note]  
> The D3DX (D3DX 9, D3DX 10, and D3DX 11) utility library is deprecated for Windows 8 and is not supported for Windows Store apps.

 

Image file formats supported by D3DX11Createxxx and D3DX11Savexxx functions.

## Syntax


```C++
typedef enum D3DX11_IMAGE_FILE_FORMAT { 
  D3DX11_IFF_BMP          = 0,
  D3DX11_IFF_JPG          = 1,
  D3DX11_IFF_PNG          = 3,
  D3DX11_IFF_DDS          = 4,
  D3DX11_IFF_TIFF         = 10,
  D3DX11_IFF_GIF          = 11,
  D3DX11_IFF_WMP          = 12,
  D3DX11_IFF_FORCE_DWORD  = 0x7fffffff
} D3DX11_IMAGE_FILE_FORMAT, *LPD3DX11_IMAGE_FILE_FORMAT;
```



## Constants

<dl> <dt>

<span id="D3DX11_IFF_BMP"></span><span id="d3dx11_iff_bmp"></span>**D3DX11\_IFF\_BMP**
</dt> <dd>

Windows bitmap (BMP) file format. Contains a header that describes the resolution of the device on which the rectangle of pixels was created, the dimensions of the rectangle, the size of the array of bits, a logical palette, and an array of bits that defines the relationship between pixels in the bitmapped image and entries in the logical palette. The file extension for this format is .bmp.

</dd> <dt>

<span id="D3DX11_IFF_JPG"></span><span id="d3dx11_iff_jpg"></span>**D3DX11\_IFF\_JPG**
</dt> <dd>

Joint Photographic Experts Group (JPEG) compressed file format. Specifies variable compression of 24-bit RGB color and 8-bit gray-scale Tagged Image File Format (TIFF) image document files. The file extension for this format is .jpg.

</dd> <dt>

<span id="D3DX11_IFF_PNG"></span><span id="d3dx11_iff_png"></span>**D3DX11\_IFF\_PNG**
</dt> <dd>

Portable Network Graphics (PNG) file format. A non-proprietary bitmap format using lossless compression. The file extension for this format is .png.

</dd> <dt>

<span id="D3DX11_IFF_DDS"></span><span id="d3dx11_iff_dds"></span>**D3DX11\_IFF\_DDS**
</dt> <dd>

DirectDraw surface (DDS) file format. Stores textures, volume textures, and cubic environment maps, with or without mipmap levels, and with or without pixel compression. The file extension for this format is .dds.

</dd> <dt>

<span id="D3DX11_IFF_TIFF"></span><span id="d3dx11_iff_tiff"></span>**D3DX11\_IFF\_TIFF**
</dt> <dd>

Tagged Image File Format (TIFF). The file extensions for this format are .tif and .tiff.

</dd> <dt>

<span id="D3DX11_IFF_GIF"></span><span id="d3dx11_iff_gif"></span>**D3DX11\_IFF\_GIF**
</dt> <dd>

Graphics Interchange Format (GIF). The file extension for this format is .gif.

</dd> <dt>

<span id="D3DX11_IFF_WMP"></span><span id="d3dx11_iff_wmp"></span>**D3DX11\_IFF\_WMP**
</dt> <dd>

Windows Media Photo format (WMP). This format is also known as HD Photo and JPEG XR. The file extensions for this format are .hdp, .jxr, and .wdp.

To work properly, **D3DX11\_IFF\_WMP** requires that you initialize COM. Therefore, call [**CoInitialize**](https://docs.microsoft.com/windows/desktop/api/objbase/nf-objbase-coinitialize) or [**CoInitializeEx**](https://docs.microsoft.com/windows/desktop/api/combaseapi/nf-combaseapi-coinitializeex) in your application before you call D3DX.

</dd> <dt>

<span id="D3DX11_IFF_FORCE_DWORD"></span><span id="d3dx11_iff_force_dword"></span>**D3DX11\_IFF\_FORCE\_DWORD**
</dt> <dd>

Forces this enumeration to compile to 32 bits in size. Without this value, some compilers would allow this enumeration to compile to a size other than 32 bits. This value is not used.

</dd> </dl>

## Remarks

See [Types of Bitmaps (GDI+)](https://msdn2.microsoft.com/library/ms536393.aspx) for more information on some of these formats.

## Requirements



|                   |                                                                                        |
|-------------------|----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3DX11tex.h</dt> </dl> |



## See also

<dl> <dt>

[D3DX Enumerations](d3d11-graphics-reference-d3dx11-enums.md)
</dt> </dl>

 

 





