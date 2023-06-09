# HoloDemo
## Mixed Reality room configurator

   The main scene is under  Assets/Scene/**SampleScene** .

   This scene showcases my room configurator. It consists of a `palm-up` `scrollable` menu, which when a button is pressed, the selected `item spawns`. The spawned objects have the `Tap to Place` component and can be manipulated to `move/rotate/scale`. The menu displayed can be changed between one of the `three rooms` available (living room, kitchen and bedroom). Also, the menu counts with a button to toggle the `Follow me` behavior and another button that `deletes all` the objects spawned in the scene.

   Try my other two scenes: 
   * **demo** displays the robot Kyle with a sci-fi gun that fires furniture while spinning around.
   * In **firstManipulator**, the objects can be repositioned by using the MRTK object manipulator, the component `Grid Object Collection` is applied to smaller verisions of the robot Kyle, and a sci-fi gun visibility can be enabled/disabled with either the normal or the big button.	   

   Enjoy! :rage1:	


##
### Demos

Demo1: 
   * the menu is shown when the `palm is visible` (it disappears when the hand is put away).
   * an object is `spawned` when pressing its corresponding button and placed with the `Tap to Place` component.
   * the object is manipulated `move/rotate/scale`.
   
![](videos/demo01.gif)

Demo2: 
   * `change the room` with the previous/next buttons.
   * the menus are `scrollable`.
   
![](videos/demo02.gif)

Demo3: 
   * one can create and customize the configuration of the house interior objects.
   * pressing the `Follow me` button toggles the menu to stay visible and at reach distance.
   * the `Delete all` button destroy all the furtniture Game Objects.
   
![](videos/demo03.gif)

<sub>   pssst... the images are actually GIF, if they are not playing, click on them :eyes: </sub> <br>
or go to the YouTube playlist: <br>
https://www.youtube.com/playlist?list=PLAM5gVPZMtq_4Ogx6wm71eEORe5u08gh1


##
### Setup

   1. Once downloaded the repo, for Unity to resolve the packages properly, run the [Mixed Reality Feature Tool](https://learn.microsoft.com/en-us/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool) and import the features to the Unity project:
      - Mixed Reality toolkit:
         - Mixed Reality toolkit examples
         - Mixed Reality toolkit extensions
         - Mixed Reality toolkit foundation
         - Mixed Reality toolkit satandard assets
         - Mixed Reality toolkit test utilities
         - Mixed Reality toolkit tools
      - Platform support
         - Mixed Reality OpenXR plugin
     
  2. Restart Unity and, in the _MRTK configurator_ window, double click _Unity OpenXR plugin_.

  3. Go to File :arrow_right: Build Settings, choose Universal Windows Platform, set _Architecture_ to **ARM** and click _Switch Platform_.

  4. Fix conflicts Edit :arrow_right: Project Settings :arrow_right: XR Plug-in Management :arrow_right: Project Validation, select _Fix All_ settings conflicts.

  5. Still in the XR Plug-in Management tab, change the _depth sumission mode_ to **depth 16 Bit** and add to the _interaction profiles_ the **Microsoft hand interaction profile**. 

  6. Close editor. Mixed Reality :arrow_right: Project :arrow_right: **Apply recommended project settings for HoloLens 2**.

  7. (Optional) Project Settings :arrow_right: Player :arrow_right: Other Settings, uncheck **Optimize Mesh Data** (to reduce build time). 
     


