FROM osrf/ros:melodic-desktop-full

# 安装额外工具
RUN apt-get update && \
    apt-get install -y \
      ros-melodic-joint-state-publisher-gui \
      ros-melodic-teleop-twist-keyboard && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

# （可选）如果需要用 rosdep，保留下面两行
# RUN rosdep init && rosdep update
