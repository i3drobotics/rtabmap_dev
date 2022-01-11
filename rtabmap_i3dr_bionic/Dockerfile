# Image: i3drobotics/rtabmap:bionic

FROM i3drobotics/rtabmap:bionic_deps

# Build RTAB-Map project
RUN source /ros_entrypoint.sh && \
    git clone https://github.com/i3drobotics/rtabmap.git && \
    cd rtabmap/build && \
    ~/cmake -DWITH_ALICE_VISION=ON .. && \
    make -j$(nproc) && \
    make install && \
    cd ../.. && \
    rm -rf rtabmap && \
    ldconfig