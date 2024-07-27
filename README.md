# Interactive Decision-Making Integrating Graph Neural Networks and Model Predictive Control for Autonomous Driving
Driving on the public roads is inherently an interactive task, i.e., autonomous vehicles' (AVs) actions will influence nearby traffic participants' reactions, and vice versa. Decision-making for AVs in highly interactive driving scenarios (e.g., dense traffic) requires accurately forecasting the impact of the AVs' intention on nearby traffic participants' motion. To this end, a hierarchical decision-making framework (HDM) is proposed to navigate through interactive scenarios safely and efficiently. Specifically, the upper layer of the HDM serves as a coarse-level policy generator, which utilizes the graph neural network (GNN) to provide interaction-aware guidance. The GNN predictor takes the historical states of nearby traffic participants, road structure information, and AVs' potential intentions as inputs. Subsequently, it predicts motions of other traffic participants in response to potential actions of the AVs, which is then systematically evaluated to generate interactive guidance. Furthermore, the learned policy is utilized to guide the lower layer, which utilizes a fine-level model predictive control (MPC)-based planner to ensure safety and kinematic feasibility. Finally, hardware-in-the-loop (HiL) experiment is carried out to show the effectiveness, including mandatory lane change in dense traffic flow and interaction with the human driver. Meanwhile, comparison results indicate that the proposed HDM can improve the driving safety and efficiency compared with baselines.

# Supplementary Videos of the HiL Testing Results
## Mandatory Lane Change in Dense Traffic Scenario
### Top View
![HiL-Mandatory lane change scenario-Case-2-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/386c15bf-57e5-4499-8545-73fcda925e2d)

### Vehicle View
![HiL-Mandatory lane change scenario-Case-2-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/c8e1beda-3c85-48fb-8f4d-356ca0facadc)

## Interacting-with-Human-Driver
### Top View
![HiL-Interacting-with-Aggressive-HumanDriver-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/075a8572-aee1-45eb-b068-80459171c11f)

### Vehicle View
![HiL-Interacting-with-Aggressive-HumanDriver-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/33124517-a1ab-49c1-8adc-1af098a99d25)

### Human View
![HiL-Interacting-with-Aggressive-HumanDriver-Human View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/20edb960-dc0c-42aa-bd58-75d869d08d64)

# Supplementary Videos of Decision-Making Performance Evaluation and Comparison

### Roundabout Scenarios
Case 1 | Case 2
:-------------------------:|:-------------------------:
https://github.com/user-attachments/assets/89c1c309-ff8a-4d33-94be-d1550e3d686b | https://github.com/user-attachments/assets/e4764fe6-c32f-4352-aed9-0708b32fbccc





