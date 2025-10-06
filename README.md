# Ladybug Ros Driver

## 2. Prerequisited

### 2.1 Ubuntu and ROS

Ubuntu 18.04~20.04.  [ROS Installation](http://wiki.ros.org/ROS/Installation).

## 1. Compile

```
catkin_make -DCMAKE_POLICY_VERSION_MINIMUM=3.5 -DPYTHON_EXECUTABLE=/usr/bin/python3
```

## 2. Configuration

### 2.1 Trigger Synchronization
To enable Trigger Synchronization: **trigger_enabled** option set to be **true**

#### Note:
Modification 1:
We initialize a struct: 
```
struct time_stamp{
    int64_t high;
    int64_t low;
};
```
Create a pointer to the timestamp entity:
```
time_stamp *pointt;
```



