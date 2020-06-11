## System Identification of Roll-to-Roll Printing Process	

**Project description:** R2R printing process is an upcoming technology for mass production of flexible electronics. It involves a flexible substrate which travels over multiple rollers, similar to a printing press. In a roll-to-roll process, precise control of the web (substrate) speed and tension is critical to ensure print quality, since improper web speed and tension would lead to severe damage to the substrates. Multiple ways of controlling these parameters for printing have been tried and tested. Implementation of these controllers require user to have some knowledge about the physical model of the process and then linearizing it to obtain a set of equations which can solved to minimize errors in the calculated value and the actual value in the process.

<img src="images/sys_id/roll2roll.png?raw=true"/>


### Schematic Representation

The state variable x(t) which represents the state of the system and can be calculated regressively by estimating the state space form. A discrete form of this equation just requires replacing the time t with kth sample value.

<img src="images/sys_id/schematic.png?raw=true"/>

<img src="images/sys_id/equations.jpg?raw=true"/>

### Training
<img src="images/sys_id/training_data.JPG?raw=true"/>


### Testing
<img src="images/sys_id/test_data.JPG?raw=true"/>


### Validation
<img src="images/sys_id/validation.JPG?raw=true"/>


### For more info
[Detailed Project Report](/pdf/sys_id_project_report.pdf)