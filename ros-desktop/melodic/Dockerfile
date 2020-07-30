FROM dorowu/ubuntu-desktop-lxde-vnc:bionic

#ROS
RUN apt-get update \
    && apt-get install -y dirmngr \
    && sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list' \
    && apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654 \
    && apt-get update \
    && apt-get install -y \
        git \
        iputils-ping \
        python-rosdep \
        ros-melodic-desktop-full \
    && rosdep init \
    && rosdep update \
    && rm -rf /var/lib/apt/lists/*

RUN echo "source /opt/ros/melodic/setup.bash">>/root/.bashrc
