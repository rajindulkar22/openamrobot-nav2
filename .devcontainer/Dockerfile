FROM osrf/ros:jazzy-desktop-full

SHELL ["/bin/bash", "-c"]

RUN apt-get update && apt-get install -y \
    python3-colcon-common-extensions \
    python3-rosdep \
    python3-vcstool \
    python3-pip \
    git \
    tree \
    nano \
    sudo \
    && rm -rf /var/lib/apt/lists/*

RUN rosdep init || true

RUN echo "source /opt/ros/jazzy/setup.bash" >> /etc/bash.bashrc
