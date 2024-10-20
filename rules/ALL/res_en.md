<sub>[Go back to README](../../README_en.md)</sub>

[日本語](./res_ja.md) | [English](./res_en.md) 

# Restaurant

Reference video: https://www.youtube.com/watch?v=CmZ_jPVntP8

> [!NOTE]  
> This is a sample video from the previous competition. The rules may differ from the rules in this year.


## Main Goal

The robot retrieves and serves orders to several customers in a restaurant previously unknown to the robot.


## Focus

This task focuses on *Task planning*, *Online mapping*, *Navigation in unknown environments*, *Gesture detection*, *Verbal interaction* and *Object manipulation*


## Setup

- **Locations**: This task takes place in a real restaurant fully equipped and in business. When this is not possible, the test can be conducted in any place with the appropriate locations other than the *Arena*. 
  - **Testing Location**: The Restaurant location will remain secret until the start of the test.
  - **Starting Location**: The robot starts next to the `Kitchen-bar`. It is a table located near the restaurant’s kitchen.
  - **Order Location**: The order should be conducted close to the table where the customer is waiting.
- **People**: Volunteers different from the active team will be required during this task.
  - **Customers**: There will be at least three (3) customers sit in different tables waiting to be taken their orders. However, during the task at least two (2) orders are required to be implemented.
  - **Barman**: Awaits at the other side of the `Kitchen-bar` for orders to be placed. The `Professional Barman` assists the robot on request.
- **Furniture**: The furniture is not standardized and will be kept the same as the restaurant or place selected for the task.
  - **Kitchen-bar**: A table where the requested objects from the robot will be placed on.
  - **Customer Area**: The customer will be sit on a not-predefiened chair close to a not-predefiened table.
- **Objects**: The objects will be selected from the announced object list. There will be no unknown objects.
  - **Food**: All the objects from the `Food` category will be allowed to be used.
  - **Drinks**: All the objects from the `Drink` category will be allowed to be used.
  - **Custom Container**: Team are allowed to use a self-made or preselected container to transport the objects to the customer.
- **Time Limit**: Fifteen (15) minutes

## Scenario

### Starting Phase

1. **Setup**: The `TC` instructs the team to move the robot to the `starting position`.
1. **Start**: The `TC` gives the `start signal` and starts the timer. At the same time, the team completes the final simple setup (pressing the starting button, etc.) and leaves the area. Complex setup procedures such as pressing more than two buttons are not allowed.

### Order Phase

1. **Detection**: The robot need to identifies the customers who want to be assited. Those customers who are waiving their hands.
2. **Approach Confirmation**: The robot cannot move from the Kitchin-Bar by its own. It needs to confirm with the Barman about its intention to take an order. If the Barman rejects it, the robot may restart the `Detection`. Otherwise, the robot may continue.
3. **Navigation**: Once the robot gots the Barman confirmation to approach to the customers side, the robot will move autonomously to the cliend who was waiving the hand.
4. **Order Taking**: When the robot reaches the customer position (close enough so that the customer does not need to get closer to the robot), the robot may take the order. **The number of items to be order are two (2)**.
5. **Order Confirmation**: The robot needs to confirm the order with the customer or show that the robot understood correctly the order.
6. **Order Request**: The robot will come back to the Kitchen-Bar, and ask the Barman the items requested from the order. Those items will be placed over the table.

### Delivery Phase

1. **Picking**: The robot will grasp the items placed over the table.
2. **Navigation**: The robot autonomously moves the previous customer.
3. **Handover**: The robot needs to place the order over the customer's table.
3. **Return**: After the order has been completed, the robot needs to return to the Kitchen-Bar. The `Order Phase` may be repeated, if there are customers waiting for the ir orders to be taken. (There is a minimum of two (2) orders for this task)


## Deus ex Machina

The following Deus ex Machina will be adopted in this task. 
Although no points are awarded for the corresponding action, it is possible to skip partial tasks with simpler methods and continue with the overall task.

| Action | Bypassing |
| --- | --- |
| Customer Detection | Perform waiving hand detection with a marker attached to or held by the customer |
| Navigation to Kitchen-Bar/customer position | The robot can follow a human to reach the Kitchen-Bar/customer position |
| Order Understanding | Perform oder taking with marker(s) shown by the customer |
| Pick/Place order items | The robot can request the Barman/customer to place/pick the order to/from the robot |

## Score Sheet

| Action | Score |
| --- | --- |
| **Main Task** |  |
| 1. Order Phase | |
| &emsp; - Detect calling or waving customer       | 2x40 |
| &emsp; - Reach a customer’s table                | 2x40 |
| &emsp; - Take the order correctly                | 2x40 |
| &emsp; - Return to Kitchen-Bar                   | 2x15 |
| 2. Delivery Phase | |
| &emsp; - Request the ordered items to the Barman | 2x10 |
| &emsp; - Pick up the given items from the Barman | 2x*n*x22.5 |
| &emsp; - Return to the previous customer         | 2x15 |
| &emsp; - Place the items on the table            | 2x*n*x22.5 |
|  |  |
| **Penalty** |  |
| Not looking at the customer during order taking  | -50 |
| Non-participation (without declaration)          | -500 |
|  |  |
| Total (including bonus tasks)                    | 500 |

> [!NOTE]
> *n*: number of items grasped/placed.

> [!CAUTION]
> If the order was not taken correctly, the following obtained points will be **reducted to half** until the next customer order.

**Score Sheet for the Scorer**: (TBD)RES-score_sheet
<!-- **Score Sheet for the Scorer**: [RES-score_sheet](./doc/iHR2024_RES-score_sheet.pdf) -->


## Instructions

### To Volunteer

Volunteers are from the same team cannot participate during the task, however the active team can select who to be the volunteer.

- Select three (3) volunteer to be clients.
- Select one (1) volunteer to be the Barman.
- Gather thirty (30) minutes before the test starts.
- Receive instructions about the task.
- The volunteers may follow the **request given by the robot only**,
and not act by their own.

### To Scorer

Scorers are selected according to the *General Rules* [Scoring System](./grr_en.md#scoring-system) and will perform the following tasks:

- Gather **thirty (30) minutes** before the test starts.
- Receive instructions about the score sheet.
- Score the competition.
- Confirm the score with the other scorers and TC.
- Submit the score sheet to the TC.

### To TC

- During `Setup Day`:
  - Check the `Testing Location`
  - Announce the `Food` and `Drink` category objects.
- Just before the test:
  - Prepare the `Food` and `Drink` category objects. 
- During the test:
  - Check whether the `Testing Location` was previously mapped or not.
