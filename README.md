# Pixyalator
 A Unity 2D/URP Package that allows different resolutions for different layers (Good for Modern Pixel Art Games)

Inside is a unitypackage file. Simply open it with your unity project open and hit "Install".

## Usage
Replace your Main Camera with the "Player Camera" Prefab and add additional scripts (such as player tracking) from there. 
(Don't worry that there is no actual camera on the object. The PixCam script will handle that at runtime)
PLEASE DON'T EDIT ANYTHING IN THE PixCam SCRIPT BELOW THE PART THAT SAYS "DON'T CHANGE" UNLESS YOU KNOW WHAT YOU'RE DOING!

Set the "Render Cam Pos" to something super far from your scene, with z<-12 preferably. Otherwise you may see ugly render texture quads.
Set your preferred orthographic size in the "Size" field.

If you'd wish to have a separate transform for camera movement, you can replace the "User Camera" field with that transform. (The Pix Cam script should work from anywhere/any object in the scene)

### Layers
Add as many PixCam Layers as you want in the "Layers" Field!
The layers will be auto-sorted at runtime based off their "order" field.
(Each layer has its own camera, so too many layers may cause performance issues)
Name each layer what you want! It has no bearing on functionality.
Add the Unity layers you want to be rendered to the layermask.
Set the Resolution you want! *(Currently no testing has been done on non-16:9 resolutions)*
This resolution will be upscaled to get that pixel-y look!
