# stereo-experiment


Stereo Camera setup in Unity
Renders left image to left eye (camera) and right image to right eye (camera) such that each eye sees image from different perspective.
Content inspired by: https://www.evolvingtech.com/for-teknowgeeks/rendering-stereoscopic-images-and-videos-for-your-vr-scenes-in-unity

1. Import SteamVR into Unity. E.g. https://circuitstream.com/blog/htc-vive-tutorial-setup/
2. Disable or delete Main Camera
3. Create 2 Quad GameObjects
4. Name them Quad_Left and Quad_Right
5. Download stereo pair of images from here: https://people.duke.edu/~ng46/topics/stereo.htm
6. Create Resource Folder in Assets
7. Drag and drop the stereo pair of images into Resource Folder
8. Drag left image into Quad_Left, and right image into Quad_Right
9. Create 2 layers, one for left eye and one for right eye by Edit > Project Settings > Tags and Layers. Populate User Layer 8 with "Left Eye Layer", and populate User Layer 9 with "Right_Eye_Layer"
10. Click on QuadLeft and set QuadLeft's layer to Left_Eye_Layer
11. Click on QuadRight and set QuadRight's layer to Right_Eye_Layer
12. Click on CameraRig, copy and paste Camera so now there are 2 cameras under CameraRig.
13. Rename the original Camera to Camera-Right
14. Rename copy of Camera to Camera-Left
15. Set Culling Mask of RIGHT camera to NOT show LEFT_Eye_Layer, and set Target Eye: RIGHT
16. Set Culling Mask of LEFT camera to NOT show RIGHT_Eye_Layer, and set Target Eye: LEFT
17. Run it, you'll see the stereo pair with depth! Close one eye at a time to see how image is different between right and left eyes...just like in real life!





Other potentially useful sources of information: 
1. https://forum.unity.com/threads/steamvr-how-to-display-content-in-left-right-eye.396236/
2. https://steamcommunity.com/app/250820/discussions/0/535152276589455019/?l=german
3. 
