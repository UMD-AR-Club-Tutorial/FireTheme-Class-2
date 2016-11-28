FireTheme: Class 2
==================

##Fire Class Part 2
###This class will continue from part one and will go over putting out fire with water. We will simulate this in our Unity project with fire particles that are spawned in the scene from the part one project. The fire will become more intense and become widespread. The user of the simulation will have to pour water over the multiple fires. A human model will be taken from an online 3D model repository. Part three will develop the human model and finish a prototype simulation that one could build off of and improve.

##Licensing Information: NO LICENSE

##Project source download:  
https://github.com/UMD-AR-Club-Tutorial/FireTheme-Class-1.git

##Authors & Contributors

#####- Brian Servia  
#####- Mikhail Sorokin

#####Any questions can be sent to: umd.ar.club@gmail.com | umdvrclub@gmail.com

```
.:  
./Assets  
./ProjectSettings  
.gitignore  
README.md  
```
```
Assets:  
./Materials (Color)  
./Material  
./Scene  
./Scripts  
Assets(Blender).meta  
InkyDeals_Metal_016.jpg  
InkyDeals(Color).meta  
Materials(Color).meta  
New Material.mat  
New Material.mat.meta  
Scene.meta  
Scripts.meta  
Smoke.mat  
Smoke.mat.meta  
ojaq.obj  
ojaq.obj.meta  
shutterstock.mat  
shutterstock.mat.meta  
shutterstock_8562066.jpg  
shutterstock_7862066.jpg.meta  
smoke_texture2741.jpg  
smoke_texture2741.jpg.meta  
```
```
ProjectSettings:  
AudioManager.asset  
ClusterInputManager.asset  
DynamicsManager.asset  
EditorBuildSettings.asset  
EditorSettings.asset  
GraphicsSettings.asset  
InputManager.asset  
NavMeshAreas.asset  
NetworkManager.asset  
Physics2DSettings.asset  
ProjectVersion.txt  
QualitySettings.asset  
TagManager.asset  
TimeManager.asset  
UnityAdsSettings.asset  
UnityConnectSettings.asset  
```

##Download And Opening Scene  

###A] ZIP Folder
      
####1) Go to: https://github.com/UMD-AR-Club-Tutorial/FireTheme-Class-1.git

####2) Click "Clone or download," then proceed to click "Download ZIP."

####3) Unzip folder.

####4) Open and create new project in Unity.

####5) Go to Unzipped folder (FireTheme-Class-1) and double click "Assets" --> "Scene," and drag  
####   the scene ("FirstStove") to the Project window in Unity.

####6) Open Scene in Unity by double cliking "FirstStove."

####7) Finally go back to the FireTheme-Class-1 folder and drag:  
	./Materials  
	./Materials(Color)  
	./Scripts  
	InkyDeals_Metal_016  
	New Material  
	ojaq  
	shutterstock  
	shutterstock_78562066  
	Smoke  
	smoke_texture2741  
  
####  to the Assets section in Unity.


###B] Cloning (using Git Bash, similar with other command prompts)

####1) Go to: https://github.com/UMD-AR-Club-Tutorial/FireTheme-Class-1.git and copy this link on clipboard.

####2) Open Git Bash and choose location (path) to have the FireTheme-Class-1 folder.

####3) Type on Git Bash "git clone https://github.com/UMD-AR-Club-Tutorial/FireTheme-Class-1.git"

####4) After folder is created in the desired location, open the folder and create new project in Unity.

####5) Go into the FireTheme-Class-1 folder and double click "Assets" --> "Scene," and drag
####   the scene ("FirstStove") to the Project window in Unity.

####6) Open Scene in Unity by double clicking "FirstStove."

####7) Finally go back to the FireTheme-Class-1 folder and drag:
	./Materials  
	./Materials(Color)  
	./Scripts  
	InkyDeals_Metal_016  
	New Material  
	ojaq  
	shutterstock  
	shutterstock_78562066  
	Smoke  
	smoke_texture2741  
  
####   to the Project window in Unity.


##Steps Of Tutorial In Unity:

###1) Right click on the Hierarchy window, hover over 3D Object, click Plane to create an object. After created, right click the Plane object and click Rename, in order to change name from Plane to floor. 
###2) Go to the transform settings of the floor, and make sure the position (x,y,z) are all zero. Scale the floor: x = 10, y = 1, z = 10.
###3) Right click on the Hierarchy window, hover over 3D Object, click Capsule to create an object. After created, right click the Capsule object and click Rename, in order to change name from Capsule to user.
###4) Go to the transform settings of the user, and change the position to x = 0, y = 3, z = 0. 
###5) Drag and drop the Camera object into the user object (Assuming Unity created a Camera object automatically), making the Camera object a child of user. (If the Camera object wasn't created for you in the beginning of the scene, create the camera object, and drag and drop it in the user object).
###6) Make sure both transform location settings, of user and camera, are all zero for x, y and z.
###7) Click on the user object on the Hierarchy, then click on Add Component and type "Ridigbody." 
###This will make the user have physics based properties (gravitational influence). 
###8) Go to the Project window and double click the Scripts folder. In the folder drag and drop the PlayerMov script into user.
###9) Do the same for the camera with the CameraMov script.
##*If you have any question about the scripts, you can come to AR Club's office hours, or VR club's lab hours. In addition here is reference to Unity's scripts API: https://docs.unity3d.com/ScriptReference/index.html *
###10) Drag and drop the Stove object from the Project window, to the Hierarchy window. (expect the object to be bigger than the size of your Scene window).
###11) Click on the Stove object in the Hierarchy, and change the scale setting in the transform section to x = .02, y = .02, z = .02, then change the position to x = -10.08, y = .08, z = -1.29.
###12) Click the "Create" button on the Hierarchy and make a "Particle System" object. Name this object "Smoke" to build up to to the fire that we will make.
###13) We will update the particle system on the smoke now. Click on the "Smoke" object in the hierarchy and change the following parameters:
	- "Start Delay" >= 10
	- "Start Color" a shade of Black/Grey
	- "Shape" - Cone with "Angle" 10, "Radius" 0.25 and "Emit From" Base
	-  "Color Over Lifetime" make full opaque in begining and transparent in the end.
	- "Start Delay" - Set to 5 seconds or later.
###14) Play around with the particle system settings and see the different results you can get!