# StreamBurningwND

## Introduction
This repository is for a hydro-correction tool that utilizes national datasets published by U.S. federal agencies. The aim of hydro-correction is to modify digital elevation models (DEMs) to improve the accuracy of hydrological modeling. Common hydro-conditioning techniques include sink filling, stream burning, and ridge walling. The stream burning process entails integrating vector streamlines into a DEM layer to either lower the elevation at streamline locations or raise the surrounding terrain.

Allen and Howard (2015) devised a stream-burning technique employing high-resolution airborne Light Detection and Ranging (LiDAR) DEMs for a low-lying region in northeastern North Carolina, complemented by ditch features from the National Hydrography Dataset (NHD). This ArcGIS tool is built upon their research. The toolbox encompasses four codes. Refer to the flowchart (Figure 1) for a detailed overview of the processes. 


 ![image](https://github.com/Y-HChen/StreamBurningwND/assets/127795437/568142e9-0e8f-47f5-8ed0-08f03febc8ac)

Figure 1. Detailed flow chat for four codes included in StreamBurningwND.

**This tool require ESRI ArcGIS Pro 3.0, it is designed as a Toolbox that you can add to ArcGIS Pro.**

**Before running this tool, make sure your ArcGIS Pro is licensed with 3D Analyst and Spatial Analyst Extensions.**


For your practices, we also include a sample dataset for a watershed in Norfolk, Virginia. These files including: 
1.	Five Las files: Light detection and ranging (LiDAR) point clouds data from [The National Map v2](https://apps.nationalmap.gov/downloader/).
2.	NHDFlowline_Sample.shp: National Hydrography Dataset (NHD) Flowline from [The National Map v2](https://apps.nationalmap.gov/downloader/). 
3.	NOAA_SLR_3mDEM_Sample.tif: A 3-m digital elevation model (DEM) from [NOAA Sea Level Rise Data Download](https://coast.noaa.gov/slrdata/).
4.	StreamBuringwND.atbx: A Toolbox for stream burning with ArcGIS Pro 3.0.

![image](https://github.com/Y-HChen/StreamBurningwND/assets/127795437/65d11cf3-1cfa-4479-bd45-b6aeb5af4301)

Figure 2. Sample files and a toolbox provided in this use case.

Link to [toolbox](https://github.com/Y-HChen/StreamBurningwND/blob/main/StreamBurningwND.atbx)

Link to [toolbox and sample files (Google Drive)](https://drive.google.com/file/d/1JChLh-uEP3MnKqBxNBexXNmmceQjsBRR/view)


## How to use?
Unzip the file and add the *“StreamBuringwND.atbx”* toolbox into ArcGIS Pro by right clicking the Toolboxes and selecting “Add ToolBox” in Catalog pane. You should see four script-based tools showing in the added toolbox.

![image](https://github.com/Y-HChen/StreamBurningwND/assets/127795437/f4653e59-e61f-4429-a415-792dde61e91e)

For step by step using the sample files, please refer to [Manual](https://github.com/Y-HChen/StreamBurningwND/blob/main/StreamBurningwND_Manual_ArcGISPro3.pdf)

![image](https://github.com/Y-HChen/StreamBurningwND/assets/127795437/9802a298-1231-45d1-be2c-2dfec2d38372)

*The hillshade on the right-hand side depicts the flowline buffer zones "burned" onto the original DEM, facilitating the connection of the stream across the road (see red arrow).*

## Reference
Allen, T. R., & Howard, R. (2015). [Improving Low-Relief Coastal LiDAR DEMs with Hydro-Conditioning of Fine-Scale and Artificial Drainages](https://doi.org/10.3389/feart.2015.00072). Frontiers in Earth Science 3. 10.3389/feart.2015.00072
