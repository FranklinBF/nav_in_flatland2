

python scenario_eval.py test_eval.yml png
## map1 -------------------------------------------------------
roslaunch arena_bringup start_arena_flatland.launch map_file:="map1"  disable_scenario:="false" scenario_file:="eval/obstacle_map1_obs25.json"

## ego
rosbag record -o ego_map1_obs25_vel10_classic /scenario_reset -e "(.*)police(.*)"

rosbag record -o ego_map1_obs25_vel05_classic /scenario_reset -e "(.*)police(.*)"

rosbag record -o ego_map1_obs25_vel03_classic /scenario_reset -e "(.*)police(.*)"

## teb
rosbag record -o teb_map1_obs25_vel10_classic /scenario_reset -e "(.*)police(.*)"

rosbag record -o teb_map1_obs25_vel05_classic /scenario_reset -e "(.*)police(.*)"

rosbag record -o teb_map1_obs25_vel03_classic /scenario_reset -e "(.*)police(.*)"


## cadrl --------------------------------------------------------------------------
## map1 -------------------------------------------------------
## obstacle 20 ------------------------------------------------
 
roslaunch arena_bringup start_arena_flatland.launch map_file:="map1"  disable_scenario:="false" scenario_file:="eval/obstacle_map1_obs20.json"

## vel 10 05 03 timespace
rosbag record -o cadrl_map1_obs20_vel10_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel05_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel03_timespace /scenario_reset -e "(.*)police(.*)"

## vel 10 05 03 spatialhorizon
rosbag record -o cadrl_map1_obs20_vel10_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel05_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel03_spatialhorizon /scenario_reset -e "(.*)police(.*)"

## vel 10 05 03 subsampling
rosbag record -o cadrl_map1_obs20_vel10_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel05_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel03_subsampling /scenario_reset -e "(.*)police(.*)"


## vel 10 05 03 goalsampling
rosbag record -o cadrl_map1_obs20_vel10_goalsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel05_goalsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs20_vel03_goalsampling /scenario_reset -e "(.*)police(.*)"



## obs
# obs 10, vel 0.5 
rosbag record -o cadrl_map1_obs10_vel05_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs10_vel05_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs10_vel05_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_map1_obs10_vel05_goalsampling /scenario_reset -e "(.*)police(.*)"


## map empty -------------------------------------------------------
## obstacle 30 ------------------------------------------------
roslaunch arena_bringup start_arena_flatland.launch map_file:="map_empty"  disable_scenario:="false" scenario_file:="eval/empty_map_obs30.json"


## vel 10 05 03 timespace
rosbag record -o cadrl_empty_obs30_vel10_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel05_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel03_timespace /scenario_reset -e "(.*)police(.*)"



## vel 10 05 03 spatialhorizon
rosbag record -o cadrl_empty_obs30_vel10_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel05_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel03_spatialhorizon /scenario_reset -e "(.*)police(.*)"

## vel 10 05 03 subsampling
rosbag record -o cadrl_empty_obs30_vel10_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel05_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel03_subsampling /scenario_reset -e "(.*)police(.*)"


## vel 10 05 03 goalsampling
rosbag record -o cadrl_empty_obs30_vel10_goalsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel05_goalsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs30_vel03_goalsampling /scenario_reset -e "(.*)police(.*)"

## obstacle 20 ------------------------------------------------
roslaunch arena_bringup start_arena_flatland.launch map_file:="map_empty"  disable_scenario:="false" scenario_file:="eval/empty_map_obs20.json"


rosbag record -o cadrl_empty_obs20_vel05_timespace /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs20_vel05_spatialhorizon /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs20_vel05_subsampling /scenario_reset -e "(.*)police(.*)"

rosbag record -o cadrl_empty_obs20_vel05_goalsampling /scenario_reset -e "(.*)police(.*)"



