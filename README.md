# Interactive Decision-Making Integrating Graph Neural Networks and Model Predictive Control for Autonomous Driving
## Abstract
Driving on the public roads is inherently an interactive task, i.e., autonomous vehicles' (AVs) actions will influence nearby traffic participants' reactions, and vice versa. Decision-making for AVs in highly interactive driving scenarios (e.g., dense traffic) requires accurately forecasting the impact of the AVs' intention on nearby traffic participants' motion. To this end, a hierarchical decision-making framework (HDM) is proposed to navigate through interactive scenarios safely and efficiently. Specifically, the upper layer of the HDM serves as a coarse-level policy generator, which utilizes the graph neural network (GNN) to provide interaction-aware guidance. The GNN predictor takes the historical states of nearby traffic participants, road structure information, and AVs' potential intentions as inputs. Subsequently, it predicts motions of other traffic participants in response to potential actions of the AVs, which is then systematically evaluated to generate interactive guidance. Furthermore, the learned policy is utilized to guide the lower layer, which utilizes a fine-level model predictive control (MPC)-based planner to ensure safety and kinematic feasibility. Finally, hardware-in-the-loop (HiL) experiment is carried out to show the effectiveness, including mandatory lane change in dense traffic flow and interaction with the human driver. Meanwhile, comparison results indicate that the proposed HDM can improve the driving safety and efficiency compared with baselines.

# Supplementary Videos of Qualitative Perfromance Evaluation Via Real-World Dataset
RDB 1 | RDB 2
:-------------------------:|:-------------------------:
https://github.com/user-attachments/assets/7fd36cc3-7939-476a-b5cb-4b0ee0940c6a | https://github.com/user-attachments/assets/9aa73c6e-4dc3-43db-946e-00ef0519e77a

RDB 3 | RDB 6
:-------------------------:|:-------------------------:

# Quantitative Performance Evaluation
### Crossroad Scenarios
Case 1 | Case 2
:-------------------------:|:-------------------------:
![crossroad_case1_mp4 00_00_00-00_00_30](https://github.com/user-attachments/assets/47db45ca-6160-4a81-9b6e-84bffe2e3613) | ![crossroad_case3_mp4 00_00_00-00_00_30](https://github.com/user-attachments/assets/d131c71b-7f30-49a2-b598-0d98d66f73ee)

### T-junction Scenarios
Case 1 | Case 2
:-------------------------:|:-------------------------:
![tjunction_case1_mp4 00_00_00-00_00_30](https://github.com/user-attachments/assets/1964ab21-5ee5-4ca2-aee3-19da4aa89570) | ![tjunction_case3_mp4 00_00_00-00_00_30](https://github.com/user-attachments/assets/d96811e4-472d-43c3-b572-82cd19283294)

### Roundabout Scenarios
Case 1 | Case 2
:-------------------------:|:-------------------------:
![Roundabout-2 00_00_00-00_00_30](https://github.com/user-attachments/assets/018cf04c-beb8-4476-b5f4-84b3efbf5986) | ![Roundabout-33 00_00_00-00_00_30](https://github.com/user-attachments/assets/22a591ca-b0c7-43de-8d4c-c386e06ed9dd)

# Supplementary Videos of ardware-in-the-Loop Experiments
## 1. Mandatory Lane Change in Dense Traffic Scenario
### Top View
![HiL-Mandatory lane change scenario-Case-2-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/386c15bf-57e5-4499-8545-73fcda925e2d)
### Vehicle View
![HiL-Mandatory lane change scenario-Case-2-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/c8e1beda-3c85-48fb-8f4d-356ca0facadc)

## 2. Interacting-with-Human-Driver
### Top View
![HiL-Interacting-with-Aggressive-HumanDriver-Top View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/075a8572-aee1-45eb-b068-80459171c11f) 
### Vehicle View
![HiL-Interacting-with-Aggressive-HumanDriver-Vehicle View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/33124517-a1ab-49c1-8adc-1af098a99d25)
### Human View
![HiL-Interacting-with-Aggressive-HumanDriver-Human View 00_00_00-00_00_30](https://github.com/Kayne0401/IMPC/assets/112403512/20edb960-dc0c-42aa-bd58-75d869d08d64)






