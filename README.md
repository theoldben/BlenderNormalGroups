# BlenderNormalGroups

Eevee has severe frame-rate drops with animated objects that have normal maps on them. The problem has been reported and can be viewed with a nice sample file here:  

https://developer.blender.org/T64458


![Comparison of Node Group versus Normal Map](/img/realtime_replacement_comparison.png "Comparison of Node Group versus Normal Map")

This Addon replaces Normal Map Nodes in Blender to improve EEVEE Viewport Performance.
The performance gains are significant. 

![Node Group](/img/node_group_for_realtime_eevee_speedup.png "Node Group")

Install the addon, go to the Shader Editor and extend its Tool Bar.  
You will see two buttons, aptly named after the setups they will toggle.  
**Normal** will give you the **regular Normal Map Setup**  
**Custom** will replace the existing Normal Map Nodes with the **Custom Setup** to speed up the Viewport. Switch this back to regular for rendering.

![Shader Editor Tool Bar Buttons](/img/normal_map_custom_group_shader_editor_buttons.png "This is where you find the buttons to toggle the script: Tool Bar in the Shader Editor")

You will see this **Node Group** replacing the **Normal Map Node**  


![Shader Editor Custom Setup Active](/img/custom_maps_toggled.png "Custom Setup Active")

This is based on this idea by pcanback: https://blenderartists.org/t/way-faster-normal-map-node-for-realtime-animation-playback-with-tangent-space-normals/1175379

I am only maintaining this add-on, the heavy lifting was done by anonymous persons and BeheadedKamikaze https://github.com/BeheadedKamikaze

Now contains the necessary fixes to make it 2.83 compatible, graciously provided by Xavier Cho https://github.com/mysticfall .
Many thanks for these!

**Tested in 3.0.** Works just fine.

**Compatibility with 4.0 added**, this will break compatibility with 2.8 through 3.0. 
If you need the addon for these Blender versions, you can get it **from the according branch**. 

Please note also, that if you have a file that still has normal groups from an older version in it, those will break the newer script. **Please convert those back to regular normal nodes in your older blender version and save the file for transfer to a newer one.**
