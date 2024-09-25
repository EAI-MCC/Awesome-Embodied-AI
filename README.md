# Awesome Embodied AI Resources 

A curated list of papers and open-source resources focused on Embodied AI, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

<br>

- [Robotic Manipulation](#robotic-manipulation)
  - [Imitation Learning](#imitation-learning)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Large Model](#large-model)
- [Navigation](#navigation)
- [Locomotion](#locomotion)
- [Other](#other)
  
<br>

<br>

## Robotic Manipulation:

### Imitation Learning:
### 2024:
#### 1. [RSS 2024]RVT-2: Learning Precise Manipulation from Few Demonstrations 
**Authors**: Ankit Goyal, Valts Blukis, Jie Xu, Yijie Guo, Yu-Wei Chao, Dieter Fox 
<details span>
<summary><b>Abstract</b></summary>
In this work, we study how to build a robotic system that can solve multiple 3D manipulation tasks given language instructions. To be useful in industrial and household domains, such a system should be capable of learning new tasks with few demonstrations and solving them precisely. Prior works, like PerAct [40] and RVT [17], have studied this problem, however, they often struggle with tasks requiring high precision. We study how to make them more effective, precise, and fast. Using a combination of architectural and system-level improvements, we propose RVT-2, a multitask 3D manipulation model that is 6X faster in training and 2X faster in inference than its predecessor RVT. RVT-2 achieves a new state-of-the-art on RLBench [24], improving the success rate from 65% to 82%. RVT-2 is also effective in the real world, where it can learn tasks requiring high precision, like picking up and inserting plugs, with just 10 demonstrations. Visual results, code, and trained model are provided at: https://robotic-view-transformer-2.github.io/.
</details>

  [📄 Paper](https://arxiv.org/pdf/2406.08545v1) | [🌐 Project Page](https://robotic-view-transformer-2.github.io/) | [💻 Code](https://github.com/nvlabs/rvt) 

#### 2. Flow as the Cross-Domain Manipulation Interface
**Authors** Mengda Xu, Zhenjia Xu, Yinghao Xu, Cheng Chi, Gordon Wetzstein, Manuela Veloso, Shuran Song
<details span>
<summary><b>Abstract</b></summary>
We present Im2Flow2Act, a scalable learning framework that enables robots to acquire manipulation skills from diverse data sources. The key idea behind Im2Flow2Act is to use object flow as the manipulation interface, bridging domain gaps between different embodiments (i.e., human and robot) and training environments (i.e., real-world and simulated). Im2Flow2Act comprises two components: a flow generation network and a flow-conditioned policy. The flow generation network, trained on human demonstration videos, generates object flow from the initial scene image, conditioned on the task description. The flow-conditioned policy, trained on simulated robot play data, maps the generated object flow to robot actions to realize the desired object movements. By using flow as input, this policy can be directly deployed in the real world with a minimal sim-to-real gap. By leveraging real-world human videos and simulated robot play data, we bypass the challenges of teleoperating physical robots in the real world, resulting in a scalable system for diverse tasks. We demonstrate Im2Flow2Act's capabilities in a variety of real-world tasks, including the manipulation of rigid, articulated, and deformable objects.
</details>

  [📄 Paper](https://www.arxiv.org/abs/2407.15208) | [🌐 Project Page](https://im-flow-act.github.io/) | [💻 Code](Coming soon) 

#### 3. DiffTOP: Differentiable Trajectory Optimization for Deep Reinforcement and Imitation Learning
**Authors** Weikang Wan, Yufei Wang, Zackory Erickson, David Held
<details span>
<summary><b>Abstract</b></summary>
This paper introduces DiffTOP, which utilizes Differentiable Trajectory OPtimization as the policy representation to generate actions for deep reinforcement and imitation learning. Trajectory optimization is a powerful and widely used algorithm in control, parameterized by a cost and a dynamics function. The key to our approach is to leverage the recent progress in differentiable trajectory optimization, which enables computing the gradients of the loss with respect to the parameters of trajectory optimization. As a result, the cost and dynamics functions of trajectory optimization can be learned end-to-end. DiffTOP addresses the ``objective mismatch'' issue of prior model-based RL algorithms, as the dynamics model in DiffTOP is learned to directly maximize task performance by differentiating the policy gradient loss through the trajectory optimization process. We further benchmark DiffTOP for imitation learning on standard robotic manipulation task suites with high-dimensional sensory observations and compare our method to feed-forward policy classes as well as Energy-Based Models (EBM) and Diffusion. Across 15 model-based RL tasks and 35imitation learning tasks with high-dimensional image and point cloud inputs, DiffTOP outperforms prior state-of-the-art methods in both domains.
</details>

  [📄 Paper](https://arxiv.org/pdf/2402.05421) | [🌐 Project Page](None) | [💻 Code](Not available) 
<br>

### Reinforcement Learning:
### Large Model
#### 1. ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation
**Authors**  Wenlong Huang, Chen Wang, Yunzhu Li, Ruohan Zhang, Li Fei-Fei
<details span>
<summary><b>Abstract</b></summary>
Representing robotic manipulation tasks as constraints that associate the robot and the environment is a promising way to encode desired robot behaviors. However, it remains unclear how to formulate the constraints such that they are 1) versatile to diverse tasks, 2) free of manual labeling, and 3) optimizable by off-the-shelf solvers to produce robot actions in real-time. In this work, we introduce Relational Keypoint Constraints (ReKep), a visually-grounded representation for constraints in robotic manipulation. Specifically, ReKep is expressed as Python functions mapping a set of 3D keypoints in the environment to a numerical cost. We demonstrate that by representing a manipulation task as a sequence of Relational Keypoint Constraints, we can employ a hierarchical optimization procedure to solve for robot actions (represented by a sequence of end-effector poses in SE(3)) with a perception-action loop at a real-time frequency. Furthermore, in order to circumvent the need for manual specification of ReKep for each new task, we devise an automated procedure that leverages large vision models and vision-language models to produce ReKep from free-form language instructions and RGB-D observations. We present system implementations on a wheeled single-arm platform and a stationary dual-arm platform that can perform a large variety of manipulation tasks, featuring multi-stage, in-the-wild, bimanual, and reactive behaviors, all without task-specific data or environment models. Website at this https URL.
</details>

  [📄 Paper](https://arxiv.org/pdf/2409.01652) | [🌐 Project Page](https://rekep-robot.github.io/) | [💻 Code](https://github.com/huangwl18/ReKep) 
<br>

## Navigation：

## Locomotion：

## Other:

### 1. Open-TeleVision: Teleoperation with Immersive Active Visual Feedback
**Authors** Xuxin Cheng, Jialong Li, Shiqi Yang, Ge Yang, Xiaolong Wang
<details span>
<summary><b>Abstract</b></summary>
Teleoperation serves as a powerful method for collecting on-robot data essential for robot learning from demonstrations. The intuitiveness and ease of use of the teleoperation system are crucial for ensuring high-quality, diverse, and scalable data. To achieve this, we propose an immersive teleoperation system Open-TeleVision that allows operators to actively perceive the robot's surroundings in a stereoscopic manner. Additionally, the system mirrors the operator's arm and hand movements on the robot, creating an immersive experience as if the operator's mind is transmitted to a robot embodiment. We validate the effectiveness of our system by collecting data and training imitation learning policies on four long-horizon, precise tasks (Can Sorting, Can Insertion, Folding, and Unloading) for 2 different humanoid robots and deploy them in the real world. The system is open-sourced at: this [https URL](https://robot-tv.github.io/)
</details>

 [📄 Paper](https://arxiv.org/abs/2407.01512) | [🌐 Project Page](https://robot-tv.github.io/) | [💻 Code](https://github.com/OpenTeleVision/TeleVision) 
