<sub>[Go back to README](../../README_en.md)</sub>

[日本語](./sg_ja.md) | [English](./sg_en.md) 

# Storing Groceries (SG)

Reference video: https://www.youtube.com/watch?v=cA3MnJoOB1g

> [!NOTE]
> This is a sample video from the previous competition. The rules may differ from the rules in this year.


## Main Goal

The robot needs to categorize the objects from the table to the cabinet, placing them based on the category or similarity of the grasped object.


## Focus
*Object detection and recognition*, *Object feature recognition*, *Object manipulation*

## Setup

- **Locations**: The competition will take place inside the arena.
  * **Starting Location:** Before the test, the robot waits outside the Arena (in front of the `Entrance`) and navigates to the `testing location` when the door is open.
  * **Testing location:** This area has a shelf and a table nearby.
- **People**: No people are involved in the test, unless the robot requires human assistance.
- **Furniture**
  * **Table**: The table has 5-10 objects placed on it and the robot can choose which ones to grasp and in what order.
  <!-- On small tables, objects will be added as the robot frees up space. -->
  * **Cabinet**: The cabinet contains objects on different shelves.
  <!-- * **Cabinet door:** The cabinet door is open by default, but the team leader can request the door to be closed and score additional points for opening it. If the robot fails to open the door, it must clearly state this and request the referee to open it. -->
- **Time Limit**: Ten (10) minutes
- **Objects**: The objects will be selected from the announced object list. There will be no unknown objects.
  * **Table objects**: The objects on the table are arranged arbitrarily.
  * **Cabinet objects**: The objects on the cabinet are arranged in groups based on category or likeliness.

## Procedure

### Starting Phase

1. **Setup**: The `TC` instructs the team to move the robot to the `Starting Location`.
2. **Start**: The `TC` gives the `start signal` and starts the timer. At the same time, the team completes the final simple setup (pressing the starting button, etc.) and leaves the area. Complex setup procedures such as pressing more than two buttons are not allowed.
3. **Door opening**: One person from the team opens the door at the `start signal`. The robot recognizes that the door has opened and autonomously enters the arena.

### Storing Phase

1. **Navigation:** The robot moves to the `testing location` when the arena door is open, and goes towards the table where the objects are placed.
2. **Detection**: The robot detects and announce the object to be grasped.
3. **Picking**: The robot picks up the object which was previously announced during the `detection` section.
4. **Sorting**: The robot moves towards the cabinet, and finds the location to be placed. In this case, the robot needs to reason why that location was selected.
5. **Placing**: The robot places the object in the announce location durin the `shorting` section.
6. **Bonus**: During the `Picking` and `Placing` section, the robot may face up `tiny` and/or `heavy` obstacles which are defined in the object list.

> [!IMPORTANT]
**New category:** Objects that do not semantically belong to any of the categories represented on the shelves should be grouped together on a new shelf.


## Deus ex Machina

The following `Deus ex Machina` will be adopted in this task.
Although no points are awarded for the corresponding action, it is possible to skip partial tasks with simpler methods and continue with the overall task.

| Action | Bypassing |
| --- | --- |
| Object Grasping | `TC` holds the object instructed by the robot and gives it to the robot (or places it in a specific location). At this time, the robot needs to accurately convey the object's position, name, instructions, etc to the `TC` |
| Object Placement | `TC` places the object that the robot is holding (or is in a specific location) in the location specified by the robot. At this time, the robot needs to accurately convey the object's placement position, name, instructions, etc to the `TC` |


## Score Sheet

| Action | Score |
| --- | :---: |
| **Main Task** |  |
| &emsp; - Navigating to the table                                  | 10 |
| &emsp; - Perceiving object and categorizing it correctly          | 5x10 |
| &emsp; - Picking up an object for transportation to the cabinet   | 5x18 |
| &emsp; - Reasoning the location to place the handled object       | 5x10 |
| &emsp; - Placing an object in the cabinet                         | 5x18 |
| &emsp; - Placing an object next to similar objects on the cabinet | 5x18 |
|  |  |
| **Bonus Tasks** |  |
| &emsp; - Picking up a tiny object  | 30 |
| &emsp; - Placing a tiny object     | 30 |
| &emsp; - Picking up a heavy object | 30 |
| &emsp; - Placing a heavy object    | 30 |
|  |  |
| **Penalty** |  |
| Not attending | -500 |
|  |  |
| Total (including bonus tasks) | 500 |

> [!NOTE]
> Bonus will be scored if one of the main task of the corresponding phase is completed.

**Score Sheet for the Scorer**: (TBD)SG-score_sheet
<!-- **Score Sheet for the Scorer**: [SG-score_sheet](./doc/iHR2024_SG-score_sheet.pdf) -->

## Instructions

### To Volunteer

No volunteers will be needed for this task.

### To Scorer

Scorers are selected according to the *General Rules* [Scoring System](./grr_en.md#scoring-system) and will perform the following tasks:

- Gather **thirty (30) minutes** before the test starts.
- Receive instructions about the score sheet.
- Score the competition.
- Confirm the score with the other scorers and TC.
- Submit the score sheet to the TC.

### To TC

- During *Setup Days*:
  - Prepare the `Objects` to be used during the task.
- Before the test:
  - Place 5-10 objects on the table.
  - Place objects in the cabinet, grouping them by category or likeliness.
  - Select the `small` and `heavy` objects and announce it.
