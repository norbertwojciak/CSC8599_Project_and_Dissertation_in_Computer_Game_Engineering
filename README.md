Troubleshooting 

1) Freeze on load issue (stops at 39%):
If the project stops loading at about 39% It may be that the project doesn't open up properly the first time. To bypass this, open the DefaultEngine.ini (in Config folder), search for the following line and remove it: r.CustomDepth=3
If this doesn’t help, open the DefaultEngine.ini (in Config folder) again and remove the following line: r.EarlyZPass=2
Or 
r.DefaultFeature.MotionBlur=False
Save, close and open the project. Then go to the project settings, search for "Custom Depth Stencil Pass" and set it to "Enabled with Stencil". Also make sure you have enough free space on your drive.

2) Freeze on load issue (stops at 95%):
If the game stops at 95% loading, please wait as it is compiling shaders.

3) Loading the game first time on a computer:
It might take a while to compile all shaders when the game is first loaded. If you see light problems or you can see “Preview” on items/buildings while playing, then click “Build” in the editor and wait for Unreal Engine to rebuild the project (this may take awhile).