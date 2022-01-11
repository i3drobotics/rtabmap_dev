# Image: i3drobotics/rtabmap:bionic_dev

FROM i3drobotics/rtabmap:bionic_deps

# Build RTAB-Map project
RUN source /ros_entrypoint.sh && \
    git clone https://github.com/i3drobotics/rtabmap.git

WORKDIR /root/rtabmap