# BlenderNormalGroups

Eevee has severe frame-rate drops with animated objects that have normal maps on them. The problem has been reported and can be viewed with a nice sample file here:  

https://developer.blender.org/T64458


![Comparison of Node Group versus Normal Map](/img/realtime_replacement_comparison.png "Comparison of Node Group versus Normal Map")

This Addon replaces Normal Map Nodes in Blender to improve EEVEE Viewport Performance.
The performance gains are significant. 

![Node Group](/img/node_group_for_realtime_eevee_speedup.png "Node Group")

This is based on this idea by pcanback: https://blenderartists.org/t/way-faster-normal-map-node-for-realtime-animation-playback-with-tangent-space-normals/1175379

I am only maintaining this add-on, the heavy lifting was done by anonymous persons and BeheadedKamikaze https://github.com/BeheadedKamikaze
