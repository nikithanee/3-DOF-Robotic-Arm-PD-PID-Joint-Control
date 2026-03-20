# 3 DOF Robotic Arm - PD/PID - Joint-Control
Analytical design and simulation of joint-space controllers  for a 3-DOF robotic arm, modelled as an inverted pendulum,  implemented in ROS + Gazebo as part of IN3140 at UiO.



## What's covered
- Symbolic dynamics derivation of a 3-DOF arm (Python)
- Laplace transform & transfer function derivation
- Analytical PD controller design using critically damped
  second-order system (ζ=1, ω=6 → Kp=36, Kd=12)
- P, PD, PI, and PID controller implementation in ROS
- Step response analysis: settling time, overshoot, 
  steady-state error
- Ziegler-Nichols tuning for PI controller

## Tech stack
`ROS` `Gazebo` `Python` `Control Theory` `PID` `Laplace Transform`

## Key results
| Controller | Settling time | Overshoot | Steady-state error |
|------------|--------------|-----------|-------------------|
| P only     | ~10s         | High      | Present           |
| PD (tuned) | <1s          | Minimal   | Present           |
| PI         | ~3s          | None      | Eliminated        |
