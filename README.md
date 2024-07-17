# Interactive Decision-Making Integrating Graph Neural Networks and Model Predictive Control for Autonomous Driving
Driving on the public roads is inherently an interactive task, i.e., autonomous vehicles' (AVs) actions will influence nearby traffic participants' reactions, and vice versa. Decision-making for AVs in highly interactive driving scenarios (e.g., dense traffic) requires accurately forecasting the impact of the AVs' intention on nearby traffic participants' motion. To this end, a hierarchical decision-making framework (HDM) is proposed to navigate through interactive scenarios safely and efficiently. Specifically, the upper layer of the HDM serves as a coarse-level policy generator, which utilizes the graph neural network (GNN) to provide interaction-aware guidance. The GNN predictor takes the historical states of nearby traffic participants, road structure information, and AVs' potential intentions as inputs. Subsequently, it predicts motions of other traffic participants in response to potential actions of the AVs, which is then systematically evaluated to generate interactive guidance. Furthermore, the learned policy is utilized to guide the lower layer, which utilizes a fine-level model predictive control (MPC)-based planner to ensure safety and kinematic feasibility. Finally, hardware-in-the-loop (HiL) experiment is carried out to show the effectiveness, including mandatory lane change in dense traffic flow and interaction with the human driver. Meanwhile, comparison results indicate that the proposed HDM can improve the driving safety and efficiency compared with baselines.
## CrossRoad Scenario

### Case1
![2月29日-CrossRoad-Episode-8 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/c5ecf36c-82a9-4c07-a10c-c57b22f6b174)


### Case2
![2月29日-CrossRoad-Episode-25 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/577f177a-fadc-45f5-8389-b9a353134bc3)


### Case3
![2月29日-CrossRoad-Episode-30(paper) 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/681ffe83-f5f5-4cc1-b1a4-a67652f33953)

## T-Junction Scenario
### Case1
![2月29日-T_junction-Episode-4 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/18b9cc16-17c2-41a3-957d-12166ef83815)

### Case2
![2月29日-T-Junction-Episode-26 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/9633d8e6-de9b-45cb-9ed5-3ea2778b892a)

### Case3
![2月29日-T-Junction-Episode-74 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/fbb4938b-d8d4-4352-a38e-44935a957c5a)

## Roundabout Scenario
### Case1
![2月29日-Roundabout-Episode-0 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/eee0f0a0-7b17-48df-82ca-00ea7ab0932d)

### Case2
![2月29日-Roundabout-Episode-1 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/b4a31e6c-feb9-42ad-b644-f9dce77260e8)

### Case3
![2月29日-Roundaoubt-Episode-2 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/606ef7a7-d59c-43d9-89cc-54084978f190)

## Ramp Scenario
### Case1
![2月29日-Ramp-Episode-0 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/a0553329-4661-4403-883f-ac04add61094)

### Case2
![2月29日-Ramp-Episode-1 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/999bb0b2-7147-40bf-bd20-ccfffce17533)

### Case3
![2月29日-Ramp-Episode-2 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/5b57a8f6-d5ca-4cbb-9b9d-43e14f5bf5d9)

# HiL Testing Results
## Mandatory Lane Change Scenario
### Case 1 Top View
![HiL-Mandatory lane change scenario-Case-1-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/e6eb77af-77f0-499c-902e-a90aae0cc7bb)

### Case 1 Vehicle View
![HiL-Mandatory lane change scenario-Case-1-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/4db10c42-e9c7-4821-ab2c-8dacca7e168d)

### Case 2 Top View
![HiL-Mandatory lane change scenario-Case-2-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/386c15bf-57e5-4499-8545-73fcda925e2d)

### Case 2 Vehicle View
![HiL-Mandatory lane change scenario-Case-2-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/c8e1beda-3c85-48fb-8f4d-356ca0facadc)

## Interacting-with-Courteous-HumanDriver
### Top View
![HiL-Interacting-with-Courteous-HumanDriver-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/9843a689-d955-41aa-8677-483755f184a7)

### Vehicle View
![HiL-Interacting-with-Courteous-HumanDriver-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/6cd52dd2-9823-40e8-a109-3343c6ac6583)

### Human View
![HiL-Interacting-with-Courteous-HumanDriver-Human View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/e0fc6a05-dd1d-4b4d-a225-8904ca1e1a5f)

## Interacting-with-Aggressive-HumanDriver
### Top View
![HiL-Interacting-with-Aggressive-HumanDriver-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/075a8572-aee1-45eb-b068-80459171c11f)

### Vehicle View
![HiL-Interacting-with-Aggressive-HumanDriver-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/33124517-a1ab-49c1-8adc-1af098a99d25)

### Human View
![HiL-Interacting-with-Aggressive-HumanDriver-Human View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/20edb960-dc0c-42aa-bd58-75d869d08d64)

