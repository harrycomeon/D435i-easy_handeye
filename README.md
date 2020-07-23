# D435i-easy_handeye

这是一个D435i在UR5 机械臂上进行手眼标定的包

注意这几个坐标的选择，经过实验，发现眼在手外的手眼标定是获得tracking_base_frame和robot_base_frame的坐标变换，而眼在手上获得的是tracking_base_frame和robot_effector_frame

        <arg name="tracking_base_frame" value="camera_color_frame" />
        <arg name="tracking_marker_frame" value="camera_marker" />
        <arg name="robot_base_frame" value="base_link" />
        <arg name="robot_effector_frame" value="tool0" />

链接：

https://blog.csdn.net/harrycomeon/article/details/107521715
