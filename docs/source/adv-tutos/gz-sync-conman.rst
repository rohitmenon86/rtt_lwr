Gazebo Synchronization using Conman
===================================


Installation
------------

.. code-block:: bash

    mkdir -p ~/isir/conman_ws/src
    cd ~/isir/conman_ws/src
    wstool init
    wstool merge https://raw.githubusercontent.com/kuka-isir/rtt_lwr/rtt_lwr-2.0/lwr_utils/config/conman.rosinstall
    wstool update -j2
    cd ~/conman_ws/
    # Disable tests on 14.04
    catkin config --init --cmake-args -DCATKIN_ENABLE_TESTING=0 -DCMAKE_BUILD_TYPE=Release
    # Build
    catkin build
