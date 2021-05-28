## Installation

1. Clone the project 
2. pip install .

## Usage

#### ErForce

**Client creation:**
```python
from erforce.client import ErForceClient
client = ErForceClient()
```

**Command creation:**
```python
from erforce.model import RobotCommand, MoveLocalVelocity

move_command = MoveLocalVelocity(forward=0, left=0, angular=0)
robot_command = RobotCommand(robot_id=0, move_command=move_command, kick_speed=0, kick_angle = 0, dribbler_speed=0)

client.send_action_command(robot_command)
```


#### GrSim 

TBD
