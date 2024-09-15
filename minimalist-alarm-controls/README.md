# Minimalist Alarm Controls
![image](https://github.com/user-attachments/assets/dc7db2d8-4fa0-4faf-87c6-d7d38c5e59c3)
## Features
- Exit delay timer
- Alarm Controls
- Override buttons
  - Arm Silent (Custom Bypass)    
  - Arm Away  
  - Disarm    
  - Trigger

## Usage
Copy the code from `card.yaml`   
Paste it into a manual card, keep it in YAML view   
Update the lines with `# TODO` with the entities/strings needed.   
Required entities:   
  - Timer   
  - Alarm Control Panel 

You need to paste the timer entity ID into 1 line   
You need to paste the alarm_control_panel ID into 9 lines   
You need to input the alarm code into 4 lines   

  
You need to have the [Timer Bar Card](https://github.com/rianadon/timer-bar-card) frontend H.A.C.S Repo installed.
  
[![H.A.C.S Add Custom Repo](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=rianadon&repository=timer-bar-card)  

Next,   
Copy the code from `automation.yaml`  
Create a new automation  
Switch it to YAML mode  
Paste the code into the field
Update the lines with `# TODO` with the entities/scripts needed.
Required entities:
  - Timer   
  - Alarm Control Panel
  - Alarm Arming Script
  - Alarm Armed Away Script
  - Alarm Armed Home Script
  - Alarm Armed Custom Bypass Script
  - Alarm Triggered Script
  - Alarm Disarmed Script


You need to paste the timer entity ID into 4 lines   
You need to paste the alarm_control_panel ID into 11 lines   
You need to paste under each option, after the timer.finish and before the While Not Triggered loop the script that holds the armed actions for that specific mode
You need to paste under each option, after the While Not Triggered loop the script that holds the triggered actions for that specific mode
You need to paste the script that holds the actions for disarming at the end of the If Alarm Disarmed option

Soon I'll make a blueprint for this
