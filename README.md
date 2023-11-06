# Notes

**Note01:** There is a bug with the github DownloadZIP(".map" asset files are Git LFS files, Github DownloadZIP results in the ".map" file only 1KB).  **You should clone this repository by HTTPs or SSH of this git, Not by Github DownloadZIP.**



**Note02**: The "**UEGS Model**" is not visible in your project? [This is because the material compiling did not succeed, need to recompile the following material.](https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public#this-is-because-the-material-compiling-did-not-succeed-need-to-recompile-the-following-material-1)

> /Script/Engine.Material'/UEGaussianSplatting/ASTs/MATs/M_UEGS_GaussianSplatting_Main_Translucent.M_UEGS_GaussianSplatting_Main_Translucent'

**See more**: https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public#1-the-uegs-model-is-not-visible



# Community Communication

**Discord**: https://discord.gg/kCc8qM3C



# Updated versions

## v1.1.0

> Supports the ".ply" file exported by the 3DGaussianSplatting Editor "**SuperSplat**"
>
> **"SuperSplat" Editor**: https://playcanvas.com/super-splat



# Introduce

## PRODUCT TITLE：

**UEGaussianSplatting: 3D Gaussian Splatting Rendering Feature For UE**

**UE Marketplace:** https://www.unrealengine.com/marketplace/en-US/product/uegaussiansplatting-3d-gaussian-splatting-rendering-feature-for-ue
![image-20231103194613673](README/00_Res/01_Images/image-20231103194613673.png)

## SHORT DESCRIPTION：

A high-performance and high-quality 3D Gaussian Splatting real-time rendering plugin for Unreal Engine, Optimized for spatial point data.

## LONG DESCRIPTION：

**Documentation and Example Project:** https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public

UEGaussianSplatting is a powerful plugin for Unreal Engine that brings real-time rendering of 3D Gaussian Splatting model resources with high performance and high quality. 

It utilizes octree optimization for spatial point data, dynamic LOD rendering, and supports automatic collision generation. 

This plugin also offers very fast ".ply" resource importing and GaussianSplatting Asset editing preview window. 

UEGaussianSplatting uses a completely custom rendering component instead of the traditional particle system (Niagara), allowing it to bypass particle count limitations. 

Future updates will include real-time clipping and editing of GaussianSplatting asset data, as well as export functionality.

## TECHNICAL INFORMATION：

### Features: 

- Features:
  - High-performance and high-quality 3D Gaussian Splatting real-time rendering.
  - Octree optimization for spatial point data.
  - Dynamic LOD rendering.
  - Automatic collision generation.
  - Support for ".ply" resource quick import.
  - GaussianSplatting Asset editing preview window.
  - Custom rendering component, not limited by particle count.

### Code Modules: 

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



# User Guide

## What is "3D Gaussian Splatting"?

### Paper: "3D Gaussian Splatting for Real-Time Radiance Field Rendering" 

https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/

![image-20231103220722999](README/00_Res/01_Images/image-20231103220722999.png)

### Youtube: "3D Gaussian Splatting: How's This The Future of 3D AI?"

https://www.youtube.com/watch?v=C708Mh7EHZM

![image-20231103220831300](README/00_Res/01_Images/image-20231103220831300.png)

### "3D Gaussian Splatting" Resource Platform: "**poly.cam**"

https://poly.cam/explore?feed=splat

![image-20231103221034458](README/00_Res/01_Images/image-20231103221034458.png)

## How to use this Example Project: "[ExampleProjects/UEGSDemo](https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public/tree/main)"?

### 1. Get this "**UEGaussianSplatting**" plugin from UnrealEngine Marketplace:

https://www.unrealengine.com/marketplace/en-US/product/uegaussiansplatting-3d-gaussian-splatting-rendering-feature-for-ue

![image-20231103214105396](README/00_Res/01_Images/image-20231103214105396.png)

### 2. Clone this Example Project from: https://github.com/YHK-UEPlugins-Public/018_UEGaussianSplatting_Public

**Note**: Need to use the Git clone method, not the zip download method (which can be problematic due to LFS files).

![image-20231103214351242](README/00_Res/01_Images/image-20231103214351242.png)



### 3. Copy the "**UEGS**" plugin  from UnrealEngine Install Path to the "Plugins" folder of this Example Project.

Copy the "**UEGS**" plugin of UnrealEngine Install Path:

![image-20231103214537911](README/00_Res/01_Images/image-20231103214537911.png)

Copy it to the "**Plugins**" folder of this Example Project:

![image-20231103214818683](README/00_Res/01_Images/image-20231103214818683.png)



### 4. Make sure the "`UEGSDemo.uproject`" is associated with the correct engine version. And click the "**`UEGSDemo.uproject`**" to open this Example Project.

"`.\ExampleProjects\UEGSDemo\UEGSDemo.uproject`":

![image-20231103215203598](README/00_Res/01_Images/image-20231103215203598.png)

### 5. Find and open the Example Maps:

/Script/Engine.World'/Game/UEGSDemo/MAPs/MAP_UEGSDemo_Overview_01.MAP_UEGSDemo_Overview_01'

![image-20231103215528964](README/00_Res/01_Images/image-20231103215528964.png)

**Note**: Since the "**3D Gaussian Splatting**"(Or named "**UEGS Model**" in this "UEGaussianSplatting" Plugin) file is relatively large, and the storage space of Git repository on GitHub is limited. So only these 4 "3D Gaussian Splatting" sample files and levels are uploaded at present.

### 6. If the The "UEGS Model" is not visible, should recompile the following material:

### This is because the material compiling did not succeed, need to recompile the following material.

`/Script/Engine.Material'/UEGaussianSplatting/ASTs/MATs/M_UEGS_GaussianSplatting_Main_Translucent.M_UEGS_GaussianSplatting_Main_Translucent'`

![image-20231103212133746](README/00_Res/01_Images/image-20231103212133746.png)

1. Open the "**`M_UEGS_GaussianSplatting_Main_Translucent`**" Material and move a node to make the "**Apply**" button clickable. 
2. And Click the "**Apply**" button(**Note**: do not click the "**Save**" button until the Shader Compiling finished), this will recompile this Material. 
3. After the Shader compilation of this material has been all completed, click the "**Save**" button to save this material.

![image-20231103212231090](README/00_Res/01_Images/image-20231103212231090.png)

### 7. For other issues, please refer to the "**Issues Fixing**" chapter below.



## Get new "3D Gaussian Splatting" resources from "[poly.cam](https://poly.cam/explore?feed=splat)" and import into our UE Example Project

### 1. Open one "3D Gaussian Splatting" resource in the "[poly.cam](https://poly.cam/explore?feed=splat)", and click the "Save Capture" Button. Save it to our own Album(Note: advance registration and login required).

https://poly.cam/capture/9badeef6-8005-4324-9979-1260adc8dba5

![image-20231103221428310](README/00_Res/01_Images/image-20231103221428310.png)

![image-20231103221618657](README/00_Res/01_Images/image-20231103221618657.png)

![image-20231103221713100](README/00_Res/01_Images/image-20231103221713100.png)

![image-20231103221749723](README/00_Res/01_Images/image-20231103221749723.png)

### 2. Open the "3D Gaussian Splatting " resource from the corresponding Album. Click the "Download" button to download it as a ".ply" file.

https://poly.cam/albums

![image-20231103222000155](README/00_Res/01_Images/image-20231103222000155.png)

![image-20231103222156559](README/00_Res/01_Images/image-20231103222156559.png)

![image-20231103222316566](README/00_Res/01_Images/image-20231103222316566.png)

### 3. Drag the "**.ply**" file into the "Content Browser" of the UE Example Project(With "**UEGaussianSplatting**" plugin Enabled.)

![image-20231103222704283](README/00_Res/01_Images/image-20231103222704283.png)



## Editing the ".ply" File of "3DGaussianSplatting" 

### Method 01: Use the Online Editing Tool "SuperSplat" to edit the ".ply" file of "3DGaussianSplatting" 

**Test File**: https://poly.cam/capture/ba00df8c-5295-4314-b17a-f6227259179b

Get more from: https://poly.cam/explore?feed=splat

![image-20231106102515541](README/00_Res/01_Images/image-20231106102515541.png)

**“SuperSplat” Online Editing Tool**: https://playcanvas.com/super-splat

![image-20231106102429815](README/00_Res/01_Images/image-20231106102429815.png)

After exporting the ".ply" file, **drag** the exported "**.ply**" file into the **ContentBrowser** of UnrealEngine Project(Ensure that the "**UEGaussianSplatting**" plugin is enabled) :

![image-20231106102852714](README/00_Res/01_Images/image-20231106102852714.png)

## "UEGS" Plugin Instructions

### 1. Clipping Volume: Clip the excess parts of the UEGS model

#### Method01: Use the "AUEGaussianSplattingClippingVolume" Volume to Clip the UEGS Model Points(Clipping in this way is achieved by hiding transparent particles, so there is no change in performance)

##### Sample01

Before Clipping:

![image-20231104151704614](README/00_Res/01_Images/image-20231104151704614.png)

After Clipping:

![image-20231104151035409](README/00_Res/01_Images/image-20231104151035409.png)

##### Sample02

Before Clipping:

![image-20231104151820123](README/00_Res/01_Images/image-20231104151820123.png)

After Clipping:

![image-20231104151908837](README/00_Res/01_Images/image-20231104151908837.png)

### 2. "Build Collision" for "UEGS Asset"

Build Collision:

![image-20231103232311388](README/00_Res/01_Images/image-20231103232311388.png)

Make sure the collision properties(Such as "Collision Presets" Property) are set correctly:

![image-20231103232537340](README/00_Res/01_Images/image-20231103232537340.png)

Show Collision info in the viewport:

![image-20231103232737164](README/00_Res/01_Images/image-20231103232737164.png)

### 3. Double-click a "UEGS" Asset to open its Asset Preview Editor:

![image-20231103232843371](README/00_Res/01_Images/image-20231103232843371.png)

## Tips Summary

### 1. Drag the "**.ply**" file into the "Content Browser" of the UE Example Project(With "**UEGaussianSplatting**" plugin Enabled), will auto import the "**.ply**" file as a "UEGS Model" Asset.

The "**3D Gaussian Splatting**" file("**.ply**" file) will be imported very quickly into the Content Browser. 

![image-20231103222704283](README/00_Res/01_Images/image-20231103222704283.png)

Drag this new imported "**3D Gaussian Splatting**" Asset(Or Named "UEGS Asset" or "UEGS Model") into one Level(Or named "Map"). Capture Thumbnail for the "UEGS Asset" if you need.

![image-20231103223217332](README/00_Res/01_Images/image-20231103223217332.png)

### 2. If the brightness seems too bright in the editor, can adjust the Exposure appropriately

![image-20231103223859027](README/00_Res/01_Images/image-20231103223859027.png)

### 3. If the overall clarity of the image is not enough, can appropriately increase the value of "ScreenPercentage"; If the frame rate is too low, you can lower the value of "ScreenPercentage" appropriately.

![image-20231103225141818](README/00_Res/01_Images/image-20231103225141818.png)

### 4. If the frame rate is too low, can appropriately change the "PointSize" in the "UEGS" Actor from the default 9 to a lower value (such as 5, Note: that lowering this value will result in a loss of clarity).

![image-20231103225602917](README/00_Res/01_Images/image-20231103225602917.png)

### 5. When the number of  ".ply" asset points is too large, if the display error is caused by the insufficient points budget, can change the "SortUEGaussianSplattingPoints" property from the default 1 to 5 or 10 in "`Project Settings -> UEGaussianSplatting`", which can avoid the display problem caused by the insufficient points budget. 

**Note**: Setting a larger points budget value will cost more rendering performance when displaying complex ".ply" asset.

![image-20231103230208181](README/00_Res/01_Images/image-20231103230208181.png)

### 6. Running the Game in "Standalone Game" mode will result in a higher frame rate than running it directly in the editor. Properly set the screen resolution, can get a more appropriate frame rate.

Such as setting the resolution to "1920x1080, window mode" by console command: "`r.setres 1920x1080 w`"

![image-20231103231509519](README/00_Res/01_Images/image-20231103231509519.png)

![image-20231103231558604](README/00_Res/01_Images/image-20231103231558604.png)

# Issues Fixing

## 1. The "UEGS Model" is not visible?

### This is because the material compiling did not succeed, need to recompile the following material.

`/Script/Engine.Material'/UEGaussianSplatting/ASTs/MATs/M_UEGS_GaussianSplatting_Main_Translucent.M_UEGS_GaussianSplatting_Main_Translucent'`

![image-20231103212133746](README/00_Res/01_Images/image-20231103212133746.png)

1. Open the "**`M_UEGS_GaussianSplatting_Main_Translucent`**" Material and move a node to make the "**Apply**" button clickable. 
2. And Click the "**Apply**" button(**Note**: do not click the "**Save**" button until the Shader Compiling finished), this will recompile this Material. 
3. After the Shader compilation of this material has been all completed, click the "**Save**" button to save this material.

![image-20231103212231090](README/00_Res/01_Images/image-20231103212231090.png)

## 2. UEGaussianSplatting rendering effect is too bright

### (Recommended) Method 01: Set the "Game Settings" of "Explosure" in Viewport to false to restore the Unlit type translucent particles to their original brightness(For Editor Only)

Before modification, scene object is too bright:

![image-20231028214011921](README/00_Res/01_Images/image-20231028214011921.png)

After modification, the brightness effect behaves normally:

![image-20231028214056956](README/00_Res/01_Images/image-20231028214056956.png)



## 3. Occasionally a little bit of frame rate drop when changing the Angle of view or moving a certain distance? This is a known issue, and further performance optimizations are underway.

This is due to the fact that translucent particles need to be sorted, and this operation is very performance consuming when the points number is too large. So currently, translucent particles are sorted only after the Angle of view is rotated by a certain Angle or moved by a certain distance. Performance will be further optimized later to avoid the occasional drop in frame rate.

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
