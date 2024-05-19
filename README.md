# putm_ws

Clone the repository with all the submodules
```bash
git clone --recurse-submodules git@github.com:PUT-Motorsport/putm_ws.git
```

Launch putm_controller and putm_vcl
```bash
ros2 launch launch/putm_ws.launch.py
```

Publish a message to the rtd topic
```bash
ros2 topic pub putm_vcl/rtd putm_vcl_interfaces/msg/Rtd "{rtd_state: 1}"
```

Publish a message to the frontbox topic
```bash
ros2 topic pub putm_vcl/frontbox putm_vcl_interfaces/Frontbox "{pedal_position: 0.5}"
```
