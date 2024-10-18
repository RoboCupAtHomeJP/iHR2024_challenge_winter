<sub>[Go back to README](../../README_en.md)</sub>

[日本語](./cml_ja.md) | [English](./cml_en.md) 

# Carry My Luggage（CML）

Reference video: https://youtu.be/dzyJ1dHTulc

> [!NOTE]  
> This is a sample video from the previous competition. The rules may differ from the rules in this year.


## Main Goal

The robot helps the operator to carry some luggage to a car which is parked outside (imaginary).
After the robot grabs the luggage, it will follow the operator from a `known environment` to an `unknown environment`.
Then, it will autonomously return to the `starting point`.


## Focus

*Finger-pointing recognition*, *manipulation*, *person following*, *navigation in unmapped environments*, *social navigation*.


## Setup

- **Locations**: The competition will take place both inside and outside the arena.
  - **Known Environment**: The `inside` of the Arena can be mapped in advance 
  - **Unknown Environment**: Mapping the `outside` of the arena is not allowed.
  - **Starting Location**: The robot starts at a predefined location in the `living room`, and will be announced on the setup day.
  - **Goal Location**: The robot final location to hand the bag is decided by the TC during the beginning of the task.
- **Objects**: At least two (2) paper bags will be used.
  - **Placement**: Those are placed near the operator (within 2\[m\] distance and visible to the robot).
  - **Size**: The bags size will be within 350 x 100 x 350\[mm\] and will be used and announced on the setup day.
- **People**: The operator will point to the paper bag to be used during the competition while standing in front of the robot. The operator will be selected from volunteers.
- **Time Limit**: 7 minutes


## Procedure

### Starting Phase

1. **Setup**: The `TC` instructs the team to move the robot to the `Starting location`.
2. **Start**: The `TC` gives the `start signal` and starts the timer. At the same time, the team completes the final simple setup (pressing the starting button, etc.) and leaves the area. Complex setup procedures such as pressing more than two buttons are not allowed.
3. **Pointing**: The operator points to the bag that is specified at the start signal.
4. **Picking**: The robot picks up the bag pointed at by the operator.

### Follow-Me Phase

1. **Delivery**: When the robot grasps the bag and becomes ready to follow a person, the robot needs to inform the operator that the robot is ready.
2. **Walking**: The operator starts walking from a `known environment` towards the `unknown environment`.
3. **Following**: The robot follows the operator. When the operator reaches the goal, the operator will inform the robot that the operator has reached the `goal location`.
4. **Bonus**: During the `Following`, the robot may face up to three obstacles which are selected by the team in advance.
    - Small objects on the ground (such as building blocks)
    - Hard-to-see 3D objects (such as chairs or glasses)
    - Opening and closing barriers (such as guide poles)

> [!CAUTION]
> **Natural walking**: The operator is not allowed to look back to the robot or stop moving during the `Walking` phase.

### Navigation Phase

1. **Handover**： The operator receives the bag when the operator announces to have reached the goal.
2. **Navigation**: The robot autonomously moves from the `unknown environment` to the `Starting Location` in the `known environment`.
3. **Goal**: When the robot returns to the `Starting Location`, the task is complete.
4. **Bonus**: The robot joins at the end of the queue (with 2-4 people) near the goal position.


## Deus ex Machina

The following `Deus ex Machina` will be adopted in this task.
Although no points are awarded for the corresponding action, it is possible to skip partial tasks with simpler methods and continue with the overall task.

| Action | Bypassing |
| --- | --- |
| Bag Quantity | Limit the number of placed bags to one (1). |
| Bag Picking  | The robot makes the operator to pick the pointed bag. The robot needs to inform the position of the paper bag. |
| Use markers  | Perform *Following* with a marker attached to or held by the operator. |


## Score Sheet

| Action | Score |
| --- | :---: |
| **Main Task** |  |
| 1. Starting phase | |
| &emsp; - Detect the selected bag | 50 |
| &emsp; - Grasp the selected bag  | 100 |
| 2. Follow-me phase | |
| &emsp; - Go out of the arena following the operator        | 50 |
| &emsp; - Arriving at the `goal location` outside the arena | 50 |
| 3. Navigation phase | |
| &emsp; - Autonomously enter the arena                   | 25 |
| &emsp; - Autonomously return to the `Starting Location` | 25 |
|  |  |
| **Bonus Tasks** |  |
| 2. Follow-me phase | |
| &emsp; - Avoid small objects on the ground (such as blocks)              | 50 |
| &emsp; - Avoid visually confusing 3D objects (such as chairs or glasses) | 50 |
| &emsp; - Avoid opening and closing barriers (such as guide posts)        | 50 |
| 3. Navigation phase | |
| &emsp; - Join at the end of the queue near the goal | 50 |
| **Penalty** |  |
| Not attending | -500 |
|  |  |
| Total (including bonus tasks) | 500 |

> [!NOTE]
> Bonus will be scored if one of the main task of the corresponding phase is completed.

**Score Sheet for the Scorer**: [CML-score_sheet](./doc/RCJ2024_OPL_CML-score_sheet.pdf)


## Instructions

### To Volunteer

Volunteers are freely selected by the competing team, and will perform the following tasks:

- Select one (1) volunteer for the `Follow-me phase`.
- Select from two (2) to four (4) people who make a queue near the goal.
- Gather **thirty (30) minutes before** the test starts.
- Receive instructions about the task.
- The guests may follow the orders given by the robot only, and not act by their own.

> [!NOTE]
> If the competing team is not able to gather enough volunteers,
support from other teams will be requested.

### To Scorer

Scorers are selected according to the `General Rules` [Scoring System](./gr_en.md#scoring-system) and will perform the following tasks:

- Gather **thirty (30) minutes before** the test starts.
- Receive instructions about the score sheet, guests' information and command.
- Score the competition.
- Confirm the score with the other scorers and TC.
- Submit the score sheet to the TC.

> [!WARNING]
> Any information about the guests must not be shared with the competing team.
Such action may result to the penalty in the scoring or disqualification of the team.

### To TC

- During `Setup Day`:
  - Select the robot's `Starting Location` and announce it.
  - Announce the paper bag to be used in the task.
  - Announce the bonus obstacles to be used.
  - Announce the paper bag placement area.
- Just before the test:
  - Place the bonus obstacles for the `Follow-Me Phase`, if the team requests it.
  - Instruct where the bag needs to be placed.
- During the test:
  - Instruct the bag that the operator should point at.
  - Announce the `goal location` in `Follow-Me Phase`.
