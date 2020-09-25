# Test crowd simulation under rmf demo

Welcome to crowd simulation demo under rmf project. You can perform the crowd simulation under office and airport scenario under rmf project.

## repo lists
```
repositories:
  rmf/rmf_core:
    type: git
    url: https://github.com/osrf/rmf_core.git
    version: master
  rmf/rmf_schedule_visualizer:
    type: git
    url: https://github.com/osrf/rmf_schedule_visualizer.git
    version: master
  rmf/traffic_editor:
    type: git
    url: https://github.com/FloodShao/traffic_editor.git
    version: master
  rmf/rmf_demos:
    type: git
    url: https://github.com/osrf/rmf_demos.git
    version: master
  meng_core:
    type: git
    url: https://github.com/osrf/menge_core.git
    version: master
  building_crowdsim_pr_test:
    type: git
    url: https://github.com/FloodShao/building_crowdsim_pr_test.git
    version: master
```

## Steps:
1. Make sure you have the actor model `model://MaleVisitorPhone` in `~/.gazebo/models`. This is the default actor we are using in this repo. You can find this model in <https://app.ignitionrobotics.org/OpenRobotics/fuel/models/Male%20visitor>

2. `colcon build` the whole workspace

3. Go to the source folder `src/building_crowdsim_pr_test/maps/office`

4. Launch the simulation using `ros2 launch office.launch.xml` or `ros2 launch office_ign.launch.xml` for office scenario.

## Models:
You can use the `basic_actor` model provided in [actor_mode](./models/actor) to use the basic dae file installed in `/usr/share/gazebo-11/media/models`. Animation switch is also supportted for this basic actor. The idle animation is "stand.dae". You can copy the actor folder to `~/.gazebo/models/` to use.

The related files are at `src/building_crowdsim_pr_test/maps/office_basic`.

(You might also check <https://app.ignitionrobotics.org/OpenRobotics/fuel/models/actor%20-%20relative%20paths> for basic actor)

