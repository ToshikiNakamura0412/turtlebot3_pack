# turtlebot3

## install and build
```bash
# clone repository
cd /path/to/your/catkin_ws/src
git clone https://github.com/ToshikiNakamura0412/turtlebot3.git
cd turtlebot3
vcs import pkgs < .rosinstall

# build
cd /path/to/your/catkin_ws
rosdep install -riy --from-paths src --rosdistro noetic # Install dependencies
catkin build -DCMAKE_BUILD_TYPE=Release                 # Release build is recommended
```
