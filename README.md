# React Hunter Returns
A project to bring back the OG React Hunter https://github.com/Lenshang/ReactHunter.

Nexus Mods page: https://www.nexusmods.com/monsterhunterworld/mods/6064

# Building React Hunter

## 1. Grab the latest Smart Hunter source code
Download the latest Smart Hunter from https://github.com/dragonyue0417/SmartHunter/releases (make sure you click (Source code (zip)) and put it into libs/SmartHunter directory, such that the SmartHunter.csproj file is found in ../libs/SmartHunter/SmartHunter/SmartHunter.csproj.

## 2. Download and install NPM
You need NPM. NPM for your system can be found at https://nodejs.org/en/download/. To check if it is correctly installed on Windows you can open Command Prompt and type: "node -v" and hit Enter, if a series of numbers come up you are ready for the next step.

## 3. Run "npm install" in reacthunter-web folder
Open CMD and CD to the directory containing the reacthunter-web folder, then execute "npm install".

## 4. Setup Visual Studio to automatically copy Smart Hunter build output into React Hunter build folder
Once NPM is installed, open the project in Visual Studio 2019. The project file is located at ../ReactHunter.sln, make sure you open the project using this file! Right-click "SmartHunter" on the right in the Solution Explorer -> Properties -> Build -> Output -> Output Path -> "../ReactHunter/bin/x64/Debug". Note that the output path listed here is the default one on my system and may be different for you depending on your VS configuration.

## 5. Install Nancy and other C# dependencies
In VS 2019, goto Project -> Manage NuGet Packages... -> Browse and browse for and install:
  - Nancy v2.0.0 by Andreas Håkansson
  - Nancy.Hosting.Self v2.0.0 by Andreas Håkansson
  - Netwonsoft.Json v13.0.1 by James Newton-King 

## 6. Change the dropdown from "Any CPU" to "x64" 
In the VS 2019 toolbar change the dropdown on the right from "Any CPU" to "x64" if "Any CPU" is selected.

## 7. Change Platform in Configuration Manager to "x64" 
In VS 2019, go back to the dropdown in the previous step and open the Configuration Manager, on the ReactHunter row change the Platform column to x64.

## 8. Run
Hit "Run" in the top toolbar (VS 2019 may prompt to restart as admin, accept and hit "Run" again after the restart) and wait for VS to finish building the project. If the React Hunter console window complains about anything (e.g. pattern scanning failing) you most likely didn't complete step 4 properly.
```
HealthNote:
{
	"messages": [
	{"msg": "<STYL MOJI_GREEN_DEFAULT>怪物剩余血量: 95%</STYL>", "ratio":0.95},
	{"msg": "<STYL MOJI_GREEN_DEFAULT>怪物剩余血量: 90%</STYL>", "ratio":0.90},
	{"msg": "<STYL MOJI_GREEN_DEFAULT>怪物剩余血量: 85%</STYL>", "ratio":0.85},
	{"msg": "<STYL MOJI_GREEN_DEFAULT>怪物剩余血量: 80%</STYL>", "ratio":0.80},
	{"msg": "<STYL MOJI_YELLOW_DEFAULT>怪物剩余血量: 75%</STYL>", "ratio":0.75},
	{"msg": "<STYL MOJI_YELLOW_DEFAULT>怪物剩余血量: 70%</STYL>", "ratio":0.70},
	{"msg": "<STYL MOJI_YELLOW_DEFAULT>怪物剩余血量: 65%</STYL>", "ratio":0.65},
	{"msg": "<STYL MOJI_YELLOW_DEFAULT>怪物剩余血量: 60%</STYL>", "ratio":0.60},
	{"msg": "<STYL MOJI_YELLOW_DEFAULT>怪物剩余血量: 55%</STYL>", "ratio":0.55},
	{"msg": "<STYL MOJI_ORANGE_DEFAULT>怪物剩余血量: 50%</STYL>", "ratio":0.50},
	{"msg": "<STYL MOJI_ORANGE_DEFAULT>怪物剩余血量: 45%</STYL>", "ratio":0.45},
	{"msg": "<STYL MOJI_ORANGE_DEFAULT>怪物剩余血量: 40%</STYL>", "ratio":0.40},
	{"msg": "<STYL MOJI_ORANGE_DEFAULT>怪物剩余血量: 35%</STYL>", "ratio":0.35},
	{"msg": "<STYL MOJI_ORANGE_DEFAULT>怪物剩余血量: 30%</STYL>", "ratio":0.30},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 25%</STYL>", "ratio":0.25},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 20%</STYL>", "ratio":0.20},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 17.5%</STYL>", "ratio":0.175},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 15%</STYL>", "ratio":0.15},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 12.5%</STYL>", "ratio":0.125},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 10%</STYL>", "ratio":0.1},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 9%</STYL>", "ratio":0.09},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 8%</STYL>", "ratio":0.08},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 7%</STYL>", "ratio":0.07},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 6%</STYL>", "ratio":0.06},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 5%</STYL>", "ratio":0.05},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 4%</STYL>", "ratio":0.04},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 3%</STYL>", "ratio":0.03},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 2%</STYL>", "ratio":0.02},
	{"msg": "<STYL MOJI_RED_DEFAULT>怪物剩余血量: 1%</STYL>", "ratio":0.01}
	]
	}
```

