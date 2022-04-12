---
layout: default
title: Installation for development
nav_order: 3
published: true
---

## Installation for development

**Step 1: Install Visual Studio**
Visual studio should install all the dependencies required but if not just ensure you have .NET 6.1

**Step 2: Install XNA SDK**
Flatredball already has everything you need [here](https://flatredball.com/visual-studio-2019-xna-setup/).
If the website is down, you can install it from the engine repo [here](https://github.com/Wargamer3/Project-Eternity/raw/master/XnaForVS2019.zip).

**Download the source code and some assets**
    1. The engine may be downloaded from [this location](https://github.com/Wargamer3/Project-Eternity)
    2. If you want the SRWE assets, they can be found [here](https://github.com/Wargamer3/SRWE-Assets). Clone it under the Project Eternity\Project EternityContent folder and follow the instructions.

**Make sure do the following steps after installing XNA:**

Copy 'C:/Program Files (x86)/MSBuild/Microsoft/XNA Game Studio' to 'C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/MSBuild/Microsoft/XNA Game Studio'

open CMD in administrator and go into "C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/MSBuild/Current/Bin"

type "C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/Common7/Tools/VsDevCmd.bat" & gacutil /i Microsoft.Build.Framework.dll

type "C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/Common7/Tools/VsDevCmd.bat" & gacutil /i Microsoft.Build.dll

type "C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/Common7/Tools/VsDevCmd.bat" & gacutil /i System.Collections.Immutable.dll

type "C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/Common7/Tools/VsDevCmd.bat" & gacutil /i Microsoft.Build.Utilities.Core.dll