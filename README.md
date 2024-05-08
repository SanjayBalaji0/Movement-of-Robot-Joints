# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
Developed by: S Sanjay Balaji
RegisterNumber: 23005804
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```







## Output
### 1. Generic Articulated Robot
![image](https://github.com/SanjayBalaji0/Movement-of-Robot-Joints/assets/145533553/a481cebd-66d8-4e5b-862b-6b0e5f76e5c4)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/SanjayBalaji0/Movement-of-Robot-Joints/assets/145533553/2b020a50-cf05-41eb-976e-c65a5c4cf6d8)

### 3. Movement of Joint1
![image](https://github.com/SanjayBalaji0/Movement-of-Robot-Joints/assets/145533553/c28f3f87-fb75-4a11-9715-84f42027e5d7)

### 4. Movement of Joint2
![image](https://github.com/SanjayBalaji0/Movement-of-Robot-Joints/assets/145533553/0d4f22fe-3140-4eca-9b28-40a272033099)

### 5. Movement of Joint3
![image](https://github.com/SanjayBalaji0/Movement-of-Robot-Joints/assets/145533553/e9974ea5-e1a9-4ebb-a978-5312019465e1)


## Result 
Thus the different robots joints are moved with the help of python list.


