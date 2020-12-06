#  URP, Light, Glow, Shadow, HDR, Cinemachine to your 2D Project
![Cover Photo](doc/cover.PNG)
1. Create new 2D Project, by default URP and Post Processing facilities not integrated to your 2D project, that's why we need to add this to our project from Windows -> PackageManager
2. Right click on your project Create->Render->Universal Renderer Pipeline-> Universal Renderer Pipeline (Forward) Asset.  Create 2D Renderer Pipeline-> 2D Universal Renderer, add this to previously createed URP Asset (by default its use 3D Renderer), also check HDR over the URP Asset. Goto your Edit->Project Setting->Graphics-> Scriptable Render Pipeline Settings, assign newly created one to it.
3. Goto your main camera, Check Post Proccessing, add Universal Additional Camera Data (Script)
4a. Create New Game Object, Named it Volume, add Volume to it, select mode to Global.
b. Add new profile to Volume, Add Override->Bloom, Check Threshold, Intensity, Scatter, Tint, Dirt Texture and Dirt Intensity, change Intensity to 12, Tint Color Orange, other as you like.
4. Add anything to your Scene (2D or 3D Object), Create new Marital-> change Base Map and Emission Map HDR Color.

## Add Light
When you add URP to your project, its turns your games elements into black or magenta because its use Default Materials, To Fix this add 2D light from Asset->Light->2D Light->Global Light. Go to Edit->Renderer Pipeline->URP-> Upgrade Project Material to URP Material, it will change your Material to Lit Material.


## Cast Shadow
To cast shadow to you GO, add Shadow Caster 2D to that GO, adjust your light shadow casting option.

## Add Cinemamachine Camera
1. Add Cinemachinec Package from Package Manager
2. Unity Main Menu Create a Virtual Camera, it will automatically crate your camera as Virtual camera by adding CinemachjineBrain to you camera and a CM Virtual object to the project.
3. add you main game player object to CinemachineVirtulaCamera-> Follow.
---------------------------------------------------------------
For camera shake add Cinemachine Impulse Listener and Source to your Virtual machine


## Add Pixel Perfect Camera
For Pixel Art Game add pixel perfect camera both Main Camera and CM Virtual Camera(Self PPC)
