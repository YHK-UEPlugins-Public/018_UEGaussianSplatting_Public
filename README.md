**Note:** There is a bug with the github DownloadZIP(".map" asset file are Git LFS file, Github DownloadZIP results in the ".map" file only 1KB).  **You should clone this repository by HTTPs or SSH of this git, Not by Github DownloadZIP.**



# PRODUCT TITLE：

**UEGaussianSplatting: 3D Gaussian Splatting Rendering Feature For UE**

**UE Marketplace:** 

# SHORT DESCRIPTION：

A high-performance and high-quality 3D Gaussian Splatting real-time rendering plugin for Unreal Engine, Optimized for spatial point data.

# LONG DESCRIPTION：

**Documentation and Example Project:** https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public

UEGaussianSplatting is a powerful plugin for Unreal Engine that brings real-time rendering of 3D Gaussian Splatting model resources with high performance and high quality. 

It utilizes octree optimization for spatial point data, dynamic LOD rendering, and supports automatic collision generation. 

This plugin also offers very fast ".ply" resource importing and GaussianSplatting Asset editing preview window. 

UEGaussianSplatting uses a completely custom rendering component instead of the traditional particle system (Niagara), allowing it to bypass particle count limitations. 

Future updates will include real-time clipping and editing of GaussianSplatting asset data, as well as export functionality.

# TECHNICAL INFORMATION：

## Features: 

- Features:
  - High-performance and high-quality 3D Gaussian Splatting real-time rendering.
  - Octree optimization for spatial point data.
  - Dynamic LOD rendering.
  - Automatic collision generation.
  - Support for ".ply" resource quick import.
  - GaussianSplatting Asset editing preview window.
  - Custom rendering component, not limited by particle count.

## Code Modules: 

- **UEGaussianSplatting**(Runtime)
- **UEGaussianSplattingEditor**(Editor)

**Number of C++ Classes:** 30.
**Supported Development Platforms:** Windows, Mac and Linux.

**Supported All Target Build Platforms, such as:** Win64, Mac, Linux.

**Documentation and Example Project:** 
https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public

**Advantages:**

- High-quality real-time rendering of complex 3D Gaussian Splatting models.
- Efficient use of resources with octree optimization and dynamic LOD rendering.
- Easy integration with existing Unreal Engine projects.
- No particle count limitations, allowing for more complex scenes.

**Improvement Plan:**

1. Implement real-time clipping and editing of GaussianSplatting Asset data.
2. Add export functionality for edited GaussianSplatting Assets.
3. Continuously improve performance and optimize resource usage.
4. Regularly update the plugin to ensure compatibility with the latest Unreal Engine releases.



# Issues Fixing

## UEGaussianSplatting rendering effect is too bright

### (Recommended) Method 01: Set the "Game Settings" of "Explosure" in Viewport to false to restore the Unlit type translucent particles to their original brightness(For Editor Only)

Before modification, scene object is too bright:

![image-20231028214011921](README/00_Res/01_Images/image-20231028214011921.png)

After modification, the brightness effect behaves normally:

![image-20231028214056956](README/00_Res/01_Images/image-20231028214056956.png)

# GALLERY

![000_GALLERY_01](README/00_Res/01_Images/000_GALLERY_01.jpg)

![000_GALLERY_01_01](README/00_Res/01_Images/000_GALLERY_01_01.jpg)

![000_GALLERY_01_02](README/00_Res/01_Images/000_GALLERY_01_02.jpg)

![000_GALLERY_01_03](README/00_Res/01_Images/000_GALLERY_01_03.jpg)

![000_GALLERY_01_04](README/00_Res/01_Images/000_GALLERY_01_04.jpg)

![000_GALLERY_02](README/00_Res/01_Images/000_GALLERY_02.jpg)

![000_GALLERY_03](README/00_Res/01_Images/000_GALLERY_03.jpg)

![000_GALLERY_04](README/00_Res/01_Images/000_GALLERY_04.jpg)

![000_GALLERY_05](README/00_Res/01_Images/000_GALLERY_05.jpg)

![000_GALLERY_06](README/00_Res/01_Images/000_GALLERY_06.jpg)

![000_GALLERY_07](README/00_Res/01_Images/000_GALLERY_07.jpg)

![000_GALLERY_08](README/00_Res/01_Images/000_GALLERY_08.jpg)

![000_GALLERY_09](README/00_Res/01_Images/000_GALLERY_09.jpg)
