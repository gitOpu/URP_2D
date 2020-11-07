Use URP Lighting to your 2D Project

![Cover Photo](doc/cover.PNG)

1. Create new 2D Project, by default URP and Post Processing facilities not integrated to your 2D project, that's why we need to add this to our project from Windows -> PackageManager
2. Right click on your project Create->Render->Universal Render Pipeline-> Universal Render Pipeline (Forward). Goto your Edit->Project Setting->Graphics-> Scriptable Render Pipeline Settings, assign newly created one to it.
3. Goto your main camera
a. add Universal Additional Camera Data (Script) and
b. Volume to it, add new profile to Volume, Add Override->Bloom, Check Intensity and Tint, change Intensity to 2, Tint Color Orange
c. Check Post Processing on camera
4. Add anything to your Scene (2D or 3D Object), Create new Marital-> change Base Map and Emission Map HDR Color.