# nav_in_flatland2


## map1 -------------------------------------------------------
roslaunch arena_bringup start_arena_flatland.launch map_file:="map1"  disable_scenario:="false" scenario_file:="eval/obstacle_map1_obs25.json"



## map empty -------------------------------------------------------
roslaunch arena_bringup start_arena_flatland.launch map_file:="map_empty"  disable_scenario:="false" scenario_file:="eval/empty_map_obs30.json"