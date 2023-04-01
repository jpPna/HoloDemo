# HoloDemo
## Mixed Reality room configurator

   The main scene is under  Assets/Scene/**SampleScene** .

   This scene showcases my room configurator. It consists of a ´palm-up´ ´scrollable´ menu where each button spawns the selected item. The spawned objects have the ´Tap to Place´ component and can be manipulated to ´move/rotate/scale´. The menu displayed can be changed between one of the ´three rooms´ available (livingroom, kitchen and bedroom). Also, the menu counts with a button to toggle the ´Follow me´ behavior and another button that ´deletes all´ the objects spawned in the scene.	

   Try my other two scenes: 
   * **demo** displays the robot Kyle with a sci-fi gun that fires furniture while spinning around.
   * in **firstManipulator**, the objects can be repositioned by using the MRTK object manipulator, the component ´GridObjectCollection´ is applied to smaller verisions of the robot Kyle, and a sci-fi gun which visibility can be enabled/disabled with either the normal or the big button.	   

   Enjoy :robot:	


### Download repo and run

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

  3. Go to File -> Build Settings, choose Universal Windows Platform, set _Architecture_ to **ARM** and click _Switch Platform_.

  4. Fix conflicts Edit -> Project Settings -> XR Plug-in Management -> Project Validation, select _Fix All_ settings conflicts.

  5. Still in the XR Plug-in Management tab, change the _depth sumission mode_ to **depth 16 Bit** and add to the _interaction profiles_ the **Microsoft hand interaction profile**. 

  6. Close editor. Mixed Reality -> Project -> **Apply recommended project settings for HoloLens 2**.

  7. (Optional) Project Settings -> Player -> Other Settings, uncheck **Optimize Mesh Data** (to reduce build time). 
     


