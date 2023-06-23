FROM osrf/ros:rolling-desktop
ENV DEBIAN_FRONTEND=dialog


RUN apt-get update \
 && apt-get install -y software-properties-common \
 && add-apt-repository -y ppa:kisak/kisak-mesa \
 && apt update \ 
 && apt -y upgrade 

RUN apt-get install -y \
  libnlopt-dev \
  libnlopt-cxx-dev \
  ros-rolling-xacro \
  ros-rolling-joint-state-publisher \
  ros-rolling-srdfdom \
  # Packages for moveit
  ros-rolling-object-recognition-msgs \
  ros-rolling-octomap-msgs \
  ros-rolling-ros-testing \
  ros-rolling-eigen-stl-containers \
  ros-rolling-generate-parameter-library \
  libfcl-dev \
  ros-rolling-geometric-shapes \
  ros-rolling-ruckig \
  ros-rolling-control-msgs \
  ros-rolling-controller-manager-msgs \
  ros-rolling-stomp \
  freeglut3-dev \
  ros-rolling-graph-msgs \
  ros-rolling-warehouse-ros \
  libompl-dev \
  ros-rolling-control-toolbox \
  ros-rolling-launch-param-builder \
  ros-rolling-controller-manager \
  ros-rolling-joint-state-broadcaster \
  ros-rolling-joint-trajectory-controller \
  && rm -rf /var/lib/apt/lists/* 

RUN mkdir /src && mkdir /src/sandbox_ws
