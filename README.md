# Awesome Embodied AI Resources 

A curated list of papers and open-source resources focused on Embodied AI, intended to keep pace with the anticipated surge of research in the coming months. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents

<br>

- [Robotic Manipulation](#robotic-manipulation)
  - [Imitation Learning](#imitation-learning)
  - [Reinforcement Learning](#reinforcement-learning)
- [Navigation](#navigation)
- [Locomotion](#locomotion)

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

  [📄 Paper](https://arxiv.org/pdf/2402.05421) | [🌐 Project Page](None) | [💻 Code](None) 
<br>

### Reinforcement Learning:

## Navigation：

## Locomotion：

