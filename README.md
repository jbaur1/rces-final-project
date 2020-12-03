# rces-final-project
Final project repository for RCES

My Binder:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jbaur1/rces-final-project/HEAD)

### Project Description:

This project aims to derive and analyze the velocity of a lava flow site at Fissure 8 from the 2018 Lower East Rift Zone of Kilauea in Hawaii,  from drone imagery collected by the USGS. This research is part of a larger project to understand and model multi-phase (lava, bubbles, and crystals) lava flows, and ultimatley better predict lava flow emplacement. Velocity vector fields are produced using particle image velocimetry (PIV), and analyzed through xarray. 

### Workflow:

More broadly, the scripts provided outline a workflow to derive and analyze surface velocity from drone video footage

1. Video_to_Frames: Input: Video Data -> Output: 1 second frames in form of jpeg or tiff
2. Frames_to_PIV: Input: Frame Images -> Output: Velocity fields in form of csv files for each image generated through OpenPIV - Particle Image Velocimetry
3. PIV_to_Xarray: Input: PIV csv files -> Output: Organizes data across time, space and drone flight dimensions. Converts velocity fields to m/s, and corrects for drone motion
4. Xarray_to_GIF: Input: Xarray -> Creates GIFs showing velocity for each frame and how it changes overtime 
5. final_project: Analyzes the velocity fields and creates figures to conceptualize data

(Note: only scripts for PIV_to_Xarray and final_project are compatible with Binder - others are meant to be downloaded and run on local drive)

### Scientific Questions:

- How can I accuratley extract lava flow surface velocity from drone footage?
- How does lava flow velocity at Site 6 change throughout a day?
- What is the average speed of the flows?
- Understaning the influence of channel width on the apparent velocity?
   
   
Datasetlinks: https://drive.google.com/drive/folders/1oVIuvti11dBUmHZYhcskmi8HZL38j-q3?usp=sharing

