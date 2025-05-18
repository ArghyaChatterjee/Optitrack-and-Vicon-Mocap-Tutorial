# Optitrack and Vicon Mocap Tutorial

This is a tutorial repository for the OptiTrack and Vicon motion capture system.

[![](media/mocap.png)](https://youtu.be/VcUyDthACsI) 

## Start with calibration
- You have to start with the calibration process first since each time you open the system, the cameras may have moved from their previous position. Do the calibration with the wand and set the ground plane accordingly.
- Set the reference orientation of the 3 markers centroid to be (0, 0, 0). Right click on the centroid of the markers --> Reset Pivot.

## Rigid Object Pose Estimation
### Live View the Rigid Body pose
- You can see the marker pose of each rigid body in the info panel in the left tab. On the left panel, you can see the calibration, data, builder, and info.

### Set an offset to the Rigid Body Pose from marker
- You can also set a offset from your marker. See this: https://docs.optitrack.com/motive/rigid-body-tracking

### Marker Placement Rule
- Here is a guideline on how to place a marker: https://docs.optitrack.com/motive/rigid-body-tracking
- Avoid placing the markers in symmetrical shapes such as squares, isosceles, or equilateral triangles. Symmetrical arrangements make asset identification difficult and may cause the Rigid Body assets to flip during capture.

### Clock Synchronization (from opti-track host to local PC)
- Chrony ROS [[Tutorial]](https://wiki.ros.org/ROS/NetworkSetup)
- Chrony [[repo]](https://chrony-project.org/documentation.html)

<div align="center">
    <img src="media/camera_to_object.png" width="78%">
</div>

### Marker Pose Estimation
- Aligning rigid body pivot point with a replicated 3D Model [[website]](https://docs.optitrack.com/motive/rigid-body-tracking/aligning-rigid-body-pivot-point-with-a-replicated-3d-model)
- Rigid Body Animation [[code]](https://aaronolsen.github.io/tutorials/motion/unification.html)

### Resources
- Mocap4ROS2 Setup [[website]](https://docs.optitrack.com/robotics/mocap4ros2-setup)
- Mocap4ROS2 Optitrack Demos [[readme]](https://github.com/OptiTrack/mocap4ros2_optitrack_demos/blob/main/robot_arm_follower_demo/instructions.md)
- Data Streaming [[website]](https://v22.wiki.optitrack.com/index.php?title=Data_Streaming)
- How to Make a Perfect Rigid Body for optical Motion Capture [[video]](https://www.youtube.com/watch?v=WHCQjihvpuk)

## Articulated Object Pose Estimation

<div align="center">
    <img src="media/skel-body25.gif" width="26%">
    <img src="media/skel-total.gif" width="26%">
    <img src="media/skel-multi.gif" width="26%">
</div>

<div align="center">
    <img src="media/mesh-smpl.gif" width="26%">
    <img src="media/mesh-smplx.gif" width="26%">
    <img src="media/mesh-manol.gif" width="26%">
</div>

### Resources
- Blender Plugin [[code]](https://github.com/JonathanCamargo/BlendOsim) [[paper]]()
- Pose2SimBlender [[code]](https://github.com/davidpagnon/Pose2Sim_Blender)
- Pose2Sim [[code]](https://github.com/perfanalytics/pose2sim) [[paper]]() 
- SOMA [[code]](https://github.com/nghorbani/soma) [[paper]]()
- Fair Motion [[code]](https://github.com/facebookresearch/fairmotion) [[paper]]()
- Deep Motion [[code]](https://github.com/DeepMotionEditing/deep-motion-editing) [[paper]]() 
- Hand Embodiment [[code]](https://github.com/dfki-ric/hand_embodiment) [[paper]]() 


## Robot Pose Estimation
### Using Opti-Track Motion Capture

<div align="center">
    <img src="media/mocap_to_camera.png" width="78%">
</div>

### Using Vicon Motion Capture
<div align="center">
    <img src="media/frames.png" width="26%">
    <img src="media/traj.png" width="26%">
    <img src="media/interp.png" width="26%">
</div>
<div align="center">
    <img src="media/gt_vicon.png" width="78%">
</div>

### Resources 
- Vicon2GT [[code]](https://github.com/rpng/vicon2gt) [[pdf]](https://github.com/ArghyaChatterjee/All-About-Optitrack-Motion-Capture-Mocap/blob/main/tr_vicon2gt.pdf)
- Full body reCalibration with the Noitom Perception Neuron Pro [[video]](https://www.youtube.com/watch?v=V1supw4XfOs)

## Manipulator Pose Estimation

<div align="center">
    <img src="media/robot_1.png" width="39%">
    <img src="media/robot_2.png" width="39%">
</div>

### Resources
- Eye in Hand Toolbox [[code]](https://github.com/liaochikon/Eye-in-hand-toolbox)
- Hand Eye Calibration [[website]](https://campar.in.tum.de/Chair/HandEyeCalibration)

## ROS Resources
- Mocap4ROS2 Project [[code]](https://github.com/MOCAP4ROS2-Project) [[paper]]() [[video]]() 
- Mocap4ROS2 Optitrack [[code]](https://github.com/MOCAP4ROS2-Project/mocap4ros2_optitrack) [[paper]]() [[video]]()
- Mocap4ROS2 Vicon [[code]](https://github.com/MOCAP4ROS2-Project/mocap4ros2_vicon) [[paper]]() [[video]]() 
- Mocap4ROS Vicon [[code]](https://github.com/IntelligentRoboticsLabs/mocap4ros_vicon) [[paper]]() [[video]]()
- Opti-Track Mocap ROS2 [[code]](https://github.com/tud-phi/ros2-mocap_optitrack) [[paper]]() [[video]]()
- NATNet ROS CPP [[code]](https://github.com/ArghyaChatterjee/natnet_ros_cpp) [[paper]]() [[video]]() 

