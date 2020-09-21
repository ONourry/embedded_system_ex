# 九州大学チームA

## How to run

1. Use hisazumi/aprisrc-sitl docker image

* https://hub.docker.com/repository/docker/hisazumi/aprisrc-sitl
* https://github.com/hisazumi/aprisrc-sitl

2. Download this project in catkin_ws/src in the conatiner
```
cd ~/catkin_ws/src
git clone https://github.com/hisazumi/gnc.git
```

3. Import to your bridgepoint workspace

* launch bridgepoint (just type 'bridgepoint' on termianl in the container)
* File menu -> Import -> General/Existing Project into Workspace -> Select root directory
* and select imported directory (it should be ~/catkin_ws/src/gnc)
* Build on BridgePoint (Ctrl+B or Project menu -> Build all)

4. Run in terminal

* Before executing gnc, run simulator.sh, sitl.sh, and apm accroding to README.md of the container.
```
rosrun gnc ctrl
```

# scenario
## Rescure Mission
1. Explotion happend.
2. Use drone to locate survive.
3. Start to fly from firefigher.
4. Look aruound the buildings(fire station, police station, industrial building)
5. Go back to firefighter.
