# uTinyRipper_plus
[![Download uTinyRipper](https://a.fsdn.com/con/app/sf-download-button)](https://github.com/wiiboi69/UtinyRipper_plus/releases)

UtinyRipper_plus is a continuous of UTinyRipper which is a tool for extracting assets from serialized files (*CAB-*\*, *\*.assets*, *\*.sharedAssets*, etc.) and assets bundles (*\*.unity3d*, *\*.assetbundle*, etc.) and converting them into native Engine format.

Supported versions: 1.x to 2019.x, 2020.x or greater won't be supported yet

## Export features
* Scenes
* Prefabs (GameObjects with transform components)
* AnimationClips (legacy, generic, humanoid)
* Meshes
* Shaders (native listing)
* Textures
* Audio
* Fonts
* Movie textures
* Materials
* AnimatorControllers
* Avatars
* Terrains
* TextAssets
* Components:
  * MeshRenderer
  * SkinnedMeshRenderer
  * Animation
  * Animator
  * Canvas
  * Light
  * ParticleSystem
  * Colliders
  * Rigidbody
  * AudioSource
  * Camera
  * MonoBehaviour (Mono only)
  * MonoScript (Mono only)

## Structure

* *uTinyRipperCore*

   Core library. It's designed as an single module without any third party dependencies.
   
* *uTinyRipperGUI*

   Basic graphic interface application. It has some extra converters, so additionally it exports:
   * AudioClip .wav export
   * Texture2D .png export (with Sprites)
   * Shader DirectX blob export
   * References to build-in Engine assets
   
* *uTinyRipperConsole* and *uTinyRipperConsoleNETCore*

   Sample console application which is designed to test Core library functionality.   
   It's a command line application. Drag and drop resource file(s) or/and folder(s) onto the .exe to retrieve the assets. It will then automaticly try to find resource dependencies, create a 'Ripped' folder and extract all supported assets into the created directory.
   As this is a sample application, I'm not going to improve it in any way.



### Requirements:

If you want to build a solution, you'll need:

 \- .NET Framework 4.7.2 + .NET Core 2.0 SDK

 \- Compiler with C# 7.3 syntax support (Visual Studio 2017)


If you want to run binary files, you need to install:

 \- [.NET Framework 4.7.2](https://support.microsoft.com/en-us/help/4054530/microsoft-net-framework-4-7-2-offline-installer-for-windows)
 
 \- [Microsoft Visual C++ 2015](https://www.microsoft.com/en-us/download/details.aspx?id=53840) Redistributables

 \- [Unity 2017.3.0f3 or greater](https://unity3d.com/get-unity/download/archive) (NOTE: your editor version must be no less than the game's version)
 
