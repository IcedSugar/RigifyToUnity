# Rigify to Unity

A script/guide on how to transfer rigify from blender to Unity3D

## Environment

* Blender 2.79
* Unity 2017.2

## Guide

This is how I get it to work

### Exporting from Blender

Model and rig

```
-Create/rig/skin your model
-Make a single frame resting action (optional, but advised)
-Select the resting action in the editor (or the one you want)
-Select all mesh objects you want to export along with the rig
-Open and run the script
-Export Selected only to .FBX
```

Animation

```
-Select the animation you want in the action editor
-Open and run the script
-Export Selected only to .FBX
```
Note: no need to select mesh objects for the animation

### Importing to Unity

Model and rig

```
-Put your .FBX in the Unity project
-Set rig type to Humanoid
-Assign the bone structure (Hips/Spine/Chest/UpperChest = DEF-spine/DEF-spine.001/DEF-spine.002/DEF-spine.003)
```

Animation

```
-Put your .FBX in the Unity project
-Set rig type to Humanoid
-Set the Avatar to that of your skinned .FBX 
```

## Acknowledgements

ChichigeBobo's original script [RigifyToUnreal](https://github.com/chichige-bobo/BlenderPython/blob/master/RigifyToUnreal/RigifyToUnreal.py):
