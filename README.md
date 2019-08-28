# F1/10 racecar simulator docker image
Based on:  <https://hub.docker.com/r/dorowu/ubuntu-desktop-lxde-vnc/> and <https://github.com/madhurbehl/f1tenth_docker>

## Quick start
```
docker run -it -p 6080:80 f110penn/f110sim
```
To use with a joystick (change your udev input name accordingly)
```
docker run -it -p 6080:80 --device=/dev/input/js0 f110penn/f110sim
```
Then open your browser and go to http://127.0.0.1:6080/.
After you've connected to the Ubuntu in Docker, click the button at the bottom left of the screen, go to System Tools --> LXTerminal.
In the terminal, run
```
roslaunch racecar_simulator simulator.launch
```
