FROM osrf/ros:humble-desktop
ENV DEBIAN_FRONTEND=dialog


RUN apt-get update \
 && apt-get install -y software-properties-common \
 && add-apt-repository -y ppa:kisak/kisak-mesa \
 && apt update \ 
 && apt -y upgrade 

RUN apt-get install -y \
  libnlopt-dev \
  libnlopt-cxx-dev \
  ros-humble-xacro \
  ros-humble-joint-state-publisher \
  ros-humble-srdfdom \
  && rm -rf /var/lib/apt/lists/* 

RUN mkdir /src && mkdir /src/sandbox_ws
