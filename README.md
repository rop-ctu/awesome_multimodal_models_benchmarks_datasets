# Awesome Robotics Datasets, Benchmarks & Models

Curated list of simulation and real-world datasets for robot learning, plus benchmarks, simulators, and notable models.

## Table of Contents
- [Other Awesome Lists](#other-awesome-lists)
- [Datasets](#datasets)
  - [Simulated](#simulated)
  - [Real-World](#real-world)
  - [Combined (Sim + Real)](#combined-sim--real)
  - [Dataset Collections](#dataset-collections)
- [Benchmarks](#benchmarks)
- [Physics-Based Simulation Frameworks](#physics-based-simulation-frameworks)
- [Models](#models)
- [Papers to include](#papers-to-include)

## Other Awesome Lists
- [Awesome-VLA-Robotics](https://github.com/ksDreamer/Awesome-VLA-Robotics)
- [Awesome-VLA-Papers](https://github.com/Psi-Robot/Awesome-VLA-Papers)
- [Awesome-VLA](https://github.com/Orlando-CS/Awesome-VLA)
- [awesome-ai-robotics](https://github.com/tc-huang/awesome-ai-robotics)
- [Awesome-Robot-Learning](https://github.com/RayYoh/Awesome-Robot-Learning)
- [Awesome-Implicit-NeRF-Robotics](https://github.com/zubair-irshad/Awesome-Implicit-NeRF-Robotics)
- [awesome-robotics-datasets](https://mint-lab.github.io/awesome-robotics-datasets/)
- [awesome-isaac-gym](https://github.com/robotlearning123/awesome-isaac-gym)
- [awesome-robotics](https://github.com/ahundt/awesome-robotics)
- [awesome-robotics papers](https://github.com/ahundt/awesome-robotics/blob/master/papers.md)
- [awesome-robotics-libraries](http://jslee02.github.io/awesome-robotics-libraries/)
- [awesome-human-robot-interaction](https://github.com/Po-Jen/awesome-human-robot-interaction)
- [awesome-deep-learning](https://github.com/ChristosChristofidis/awesome-deep-learning)
- [Awesome-object-pose-estimation](https://github.com/YoungXIAO13/ObjectPoseEstimationSummary)

---
# Datasets

## Simulated
| **NAME**                                                        | YEAR | SIZE                                                                                                                            | MODALITIES                                                                                                                                                                          | ROBOTS                                                                                                                                         | UNI / ORG                                                                    | Links                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **BEHAVIOR-1k <br>(2025 BEHAVIOR Challenge)**                   | 2025 | 🧩 50 tasks<br>full-length household<br><br>🕹️ 10,000<br>teleop. demos.                                                        | 🖼️  RGB, depth, and instance segmentation images<br><br>🤖 Robot state, action, task information                                                                                   | Galaxea R1 robot                                                                                                                               | Stanford                                                                     |  [🌐&nbsp;Website](https://behavior.stanford.edu/challenge/index.html)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2403.09227)<br>[💾&nbsp;Data](https://huggingface.co/datasets/behavior-1k/2025-challenge-demos)                                                                                                                                                           |
| **DexMimicGen**                                                 | 2025 | 🕹️ 21,000+ <br>demos.<br><br>🧩 9 tasks                                                                                        | 🖼️ Image <br><br>🤖 Robot state, action                                                                                                                                            | GR-1 <br>humanoid, bimanual <br>Panda<br>arms with dexterous hands                                                                             | NVIDIA Research,<br>UT Austin, <br>UC San Diego                              |  [🌐&nbsp;Website](https://dexmimicgen.github.io/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2410.24185)<br>[💾&nbsp;Data](https://huggingface.co/datasets/MimicGen/dexmimicgen_datasets/tree/main)                                                                                                                                                                        |
| **Lerobot (Meta-World+)**                                       | 2025 | 🧩 50 manip.<br>tasks                                                                                                           | 🖼️ RGB-D image<br><br>🤖 Robot action,  Environment state                                                                                                                          | Sawyer                                                                                                                                         | Farama foundation, LeRobot                                                    |   [🌐&nbsp;Website](https://meta-world.github.io/) <br>[💾&nbsp;Data](https://huggingface.co/datasets/lerobot/metaworld_mt50)                                                                                                                                                                                                                                          |
| **ManiSkill 3 (Datasets creation inprogress as of 1.9.2025)**   | 2024 | 🏠 16 envs.                                                                                                                     | 🤖 demos. (motion planning, teleop) <br> <br> 🖼️ RGB-D, point clouds                                                                                                               | Unitree <br>G1/H1,<br>Panda, <br>UR10e,<br>Allegro<br>Hand, <br>XArm, <br>[etc.](https://maniskill.readthedocs.io/en/latest/robots/index.html) | UC San Diego <br>(SU Lab)                                                    |   [🌐&nbsp;Website](https://www.maniskill.ai/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2410.00425)<br>[💾&nbsp;Data](https://huggingface.co/datasets/haosulab/ManiSkill_Demonstrations)                                                                                                                                                                                     |
| **LIBERO**                                                      | 2023 | 🧩 130 tasks                                                                                                                    | 🖼️ RGB images from workspace and wrist cameras <br><br>🤖 Proprioception <br><br>🗣️ Language task specifications <br><br>📝 PDDL scene descriptions                               | Panda                                                                                                                                          | UT Austin, Tsinghua U                                                        |  [🌐&nbsp;Website](https://libero-project.github.io/datasets)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2306.03310)<br>[💾&nbsp;Data](https://libero-project.github.io/datasets)<br>                                                                                                                                                                                      |
| **Habitat**                                                     | 2023 | Embodied Question Answering,<br>Visual <br>Language Navigation, Rearrange <br>Pick,<br>Object <br>and <br>point goal navigation | 🗣️ Scene description and language annotation (EQA, VLN)                                                                                                                            | Fetch, <br>Virtual <br>Human<br>Agents                                                                                                         | Facebook AI, Georgia Tech, <br>UC Berkeley, Simon Fraser, <br>Intel Research | (2.0)<br> [🌐&nbsp;Website](https://aihabitat.org/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2106.14405)<br>(3.0)<br>  [🌐&nbsp;Website](https://aihabitat.org/habitat3/) [📄&nbsp;Paper](https://arxiv.org/abs/2310.13724)<br>💾 [Data](https://huggingface.co/ai-habitat) |
| **MimicGen**                                                    | 2023 | 🕹️ 48,000 <br>task demos.<br><br>🧩12 tasks                                                                                    | 🖼️ Image<br><br>🤖 Robot state, action, task observation                                                                                                                           | Panda,<br>Sawyer,<br>IIWA,<br>UR5e                                                                                                             | The UTexas at Austin                                                         |   [🌐&nbsp;Website](https://mimicgen.github.io/) [📄&nbsp;Paper](https://arxiv.org/abs/2310.17596) [💾&nbsp;Data](https://huggingface.co/datasets/amandlek/mimicgen_datasets)                                                                                                                                                                                           |
| **ManiSkill 2**                                                 | 2023 | 🧩 20 tasks                                                                                                                     | 🤖 demos. (scene and robot states)<br><br>🖼️ Replay tools (point cloud, RGB-D)                                                                                                     | Panda                                                                                                                                          | UC San Diego, Tsinghua Uni.                                                  |   [🌐&nbsp;Website](https://maniskill2.github.io/)[📄&nbsp;Paper](https://arxiv.org/abs/2302.04659)💾 [Data](https://huggingface.co/datasets/haosulab/ManiSkill2)                                                                                                                                                                                                  |
| **CALVIN (Composing Actions from Language and Vision) Dataset** | 2022 | 🏠 4 envs.<br>(24 hours of teleoped. “play”)                                                                                    | 🖼️ RGB-D images from both static and gripper-mounted cameras<br><br>🗣️ Language Annotations<br><br>🤖 Action (tool center point), State Observation<br><br>🤏 Tactile image input | Panda                                                                                                                                          | UFreiburg                                                                    |   [🌐&nbsp;Website](http://calvin.cs.uni-freiburg.de/)  [📄&nbsp;Paper](https://arxiv.org/abs/2112.03227)  💾 [Data](https://github.com/mees/calvin/tree/main/dataset)                                                                                                                                                                                             |
| **RLBench (Perceiver-Actor Dataset)**                           | 2022 | Dataset <br>generator                                                                                                           | 🖼️ Multiple RBG, depth and mask camera views <br><br>🤖 Episode variation description                                                                                              | Panda                                                                                                                                          | UWashington, NVIDIA                                                          | ***Perceiver-Actor*** <br>  [🌐&nbsp;Website](https://peract.github.io/)[📄&nbsp;Paper](https://arxiv.org/abs/2209.05451)<br>***RLBench***<br>  [🌐&nbsp;Website](https://sites.google.com/view/rlbench)[📄&nbsp;Paper](https://arxiv.org/abs/1909.12271)                                                                                                                      |
| **Mobile Manipulation RoboTurk (MoMaRT)**                       | 2021 | 🕹️1200 demos. <br><br>🧩 5 tasks                                                                                               | 🖼️ Normalized LIDAR scan, RGB, depth<br><br>🤖 Objects states, robot actions, rewards and proprioception                                                                           | Fetch                                                                                                                                          | Stanford                                                                     |   [🌐&nbsp;Website](https://sites.google.com/view/il-for-mm/home) [📄&nbsp;Paper](https://arxiv.org/abs/2112.05251) [💾&nbsp;Data](https://sites.google.com/view/il-for-mm/datasets#h.ko0ilbky4y5u)                                                                                                                                                                     |
| **BEHAVIOR-100 Dataset**                                        | 2021 | 🕹️ 500 <br>VR demos.                                                                                                           | 🖼️ Semantic segmentation, instance segmentation, RGB, depth, highlight<br><br>🤖Proprioception, agent action                                                                       | VR agent                                                                                                                                       | Stanford                                                                     |   [🌐&nbsp;Website](https://behavior.stanford.edu/behavior_100/overview.html)  [📄&nbsp;Paper](https://arxiv.org/abs/2108.03332)  <br>💾 [Data](https://behavior.stanford.edu/behavior_100/dataset.html)                                                                                                                                                           |
| **D4RL**                                                        | 2020 | 🧩4 <br>Franka Kitchen with<br>4 subtasks                                                                                       | 🤖 robot and scene state observation                                                                                                                                                | Ant, <br>Hopper, Walker2D, <br>Panda                                                                                                           | Google,<br>UC Berkeley                                                       |   [🌐&nbsp;Website](https://sites.google.com/view/d4rl-anonymous/) [📄&nbsp;Paper](https://arxiv.org/abs/2004.07219) 💾 [Data](https://minari.farama.org/datasets/D4RL/kitchen/)                                                                                                                                                                                   |
| **ALFRED**                                                      | 2020 | 🕹️ 8,055 <br>expert demos. <br>(25,743<br>language directives)                                                                 | 🖼️ Resnet18 features, video sequence<br><br>🗣️ Language <br><br>🤖 Action                                                                                                         | AI2-THOR <br>agents                                                                                                                            | UWashington, Allen Institute for AI                                          |   [🌐&nbsp;Website](https://askforalfred.com/)  [📄&nbsp;Paper](https://arxiv.org/abs/1912.01734) [💾&nbsp;Data](https://github.com/askforalfred/alfred/tree/master/data)                                                                                                                                                                                                |
| **VirtualHome**                                                 | 2018 | 🧩2821<br>Activity <br>Programs,  <br><br>🧩 5193 Synthetic Programs                                                            | 🗣️ Semantic Segmentation, Natural Language Descriptions <br><br>🖼️ RGB-D data<br><br>🤖 Pose information                                                                          | Virtual <br>avatars                                                                                                                            | MIT, U Toronto                                                               |   [🌐&nbsp;Website](http://virtual-home.org/)[📄&nbsp;Paper](http://virtual-home.org/paper/virtualhome.pdf) [💾&nbsp;Data](https://github.com/xavierpuigf/virtualhome/blob/master/virtualhome/dataset/README.md)                                                                                                                                                         |
<details>
  <summary><i>Additional notes</i></summary>

<table>
  <thead>
    <tr>
      <th><strong>NAME</strong></th>
      <th>DATA FORMAT</th>
      <th>NOTES</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>BEHAVIOR-1k</strong> <br>(2025 BEHAVIOR Challenge)</td>
      <td>LeRobot format (parquet)</td>
      <td>Datasets of human-grounded dexterous bimanual manipulations in house-scale scenes part of the <a href="https://foundation-models-meet-embodied-agents.github.io/eai_challenge/">2025 EAI Challenge</a>.</td>
    </tr>
    <tr>
      <td><strong>DexMimicGen</strong></td>
      <td>HDF5</td>
      <td>Large-scale automated data<br>generation system from small number of human demos. for bi-manual manipulation.</td>
    </tr>
    <tr>
      <td><strong>Lerobot (Meta-World+)</strong></td>
      <td>LeRobot format (parquet)</td>
      <td>Single arm manipulation tasks. Generated using expert policies in the Meta-world simulation benchmarks.</td>
    </tr>
    <tr>
      <td><strong>ManiSkill 3 (Datasets creation inprogress as of 1.9.2025)</strong></td>
      <td>HDF5, JSON</td>
      <td>Single arm manipulation tasks (e.g peg insertion) and some simple humanoid (Unitree G1) and mobile manipulation tasks. In development; most environments are missing demos.</td>
    </tr>
    <tr>
      <td><strong>LIBERO</strong></td>
      <td>HDF5</td>
      <td>Single arm pick and place tasks, human-teleoperated demos. inside simulation.</td>
    </tr>
    <tr>
      <td><strong>Habitat</strong></td>
      <td>JSON</td>
      <td>Habitat 2.0 contains Scans and CAD Replicas (with simulation framework) of interiors. Embodied datasets mainly came with Habitat 3.0 datasets. Relevant Docs for Sim in Habitat 2.0</td>
    </tr>
    <tr>
      <td><strong>MimicGen</strong></td>
      <td>HDF5</td>
      <td>A system for automatically synthesizing large-scale datasets from a small number of human demos. by adapting them to new scene configurations, object instances, and robot arms.</td>
    </tr>
    <tr>
      <td><strong>ManiSkill 2</strong></td>
      <td>HDF5, JSON</td>
      <td>Replaced by ManiSkill 3 (which is still in beta).</td>
    </tr>
    <tr>
      <td><strong>CALVIN</strong> (<em>C</em>omposing <em>A</em>ctions from <em>L</em>anguage and <em>Vi</em>sio<span style="font-variant: small-caps;">n</span>) Dataset</td>
      <td>NumPy files</td>
      <td>Single arm manipulation with multiple drawers. Long horizon in terms of sequence length. Data colected with HTC Vive VR headset.</td>
    </tr>
    <tr>
      <td><strong>RLBench (Perceiver-Actor Dataset)</strong></td>
      <td>PNG, Pickle format</td>
      <td>Generated simulation single arm datasets using the RLBench datasets generation utility (using template policies). Data generator example: pregenerated 18 tasks in Perceiver-actor 💾 <a href="https://huggingface.co/datasets/hqfang/rlbench-18-tasks">Data</a></td>
    </tr>
    <tr>
      <td><strong>Mobile Manipulation RoboTurk (MoMaRT)</strong></td>
      <td>HDF5</td>
      <td>Simulated mobile manipulation in kitchen environments (e.g setting table from dishwasher, table cleanup to sink).</td>
    </tr>
    <tr>
      <td><strong>BEHAVIOR-100 Dataset</strong></td>
      <td>HDF5</td>
      <td>Datasets of human VR agents interacting with the simulation. First generation of BEHAVIOR replaced by BEHAVIOR 1K</td>
    </tr>
    <tr>
      <td><strong>D4RL</strong></td>
      <td>HDF5</td>
      <td>Franka Kitchen environment<br>containing several common household items: a microwave, a kettle,<br>an overhead light, cabinets, and an oven. The 4 subtasks are: <br>open the microwave, move the kettle, flip the light switch, and slide open the cabinet door,</td>
    </tr>
    <tr>
      <td><strong>ALFRED</strong></td>
      <td>JSON, Raw Images, MP4, PDDL</td>
      <td>Single room interactive visual dataset with high-level goal and low-level<br>natural language instructions for object and environment interaction.</td>
    </tr>
    <tr>
      <td><strong>VirtualHome</strong></td>
      <td>JSON</td>
      <td>Embodied household benchmark, activities in are represented by <em>programs</em> (sequence of actions) and <em>graphs</em> (definition of the environment where the activity takes place).</td>
    </tr>
  </tbody>
</table>
</details>

<details>
<summary><i>Full paper citations </i></summary>

- **BEHAVIOR-1k (2025 BEHAVIOR Challenge)**, BEHAVIOR-1K: A Benchmark for Embodied AI with 1,000 Everyday Activities and Realistic Simulation, 2022.12, Conference on Robot Learning. [📄&nbsp;Paper](https://arxiv.org/abs/2403.09227) [  🌐&nbsp;Website](https://behavior.stanford.edu/challenge/index.html) [💾 Dataset](https://huggingface.co/datasets/behavior-1k/2025-challenge-demos)
    
- **DexMimicGen**, DexMimicGen: Automated Data Generation for Bimanual Dexterous Manipulation via Imitation Learning, 2024.10, ICRA 2025. [📄&nbsp;Paper](https://arxiv.org/abs/2410.24185) [  🌐&nbsp;Website](https://dexmimicgen.github.io/) [💾 Dataset](https://huggingface.co/datasets/MimicGen/dexmimicgen_datasets/tree/main)
    
- **Lerobot (Meta-World+)**, Meta-World+: An Improved, Standardized, RL Benchmark, 2025.05. [📄&nbsp;Paper](https://arxiv.org/abs/2505.11289) [  🌐&nbsp;Website](https://meta-world.github.io/) [💾 Dataset](https://huggingface.co/datasets/lerobot/metaworld_mt50)
    
- **ManiSkill 3**, A Unified Simulator for Physics-Based Robot Learning, 2024.10. [📄&nbsp;Paper](https://arxiv.org/abs/2410.00425) [  🌐&nbsp;Website](https://www.maniskill.ai/) [💾 Dataset](https://huggingface.co/datasets/haosulab/ManiSkill_Demonstrations)
    
- **LIBERO**, LIBERO: Benchmarking Knowledge Transfer in Lifelong Robot Learning, 2023.06. [📄&nbsp;Paper](https://arxiv.org/abs/2306.03310) [  🌐&nbsp;Website](https://libero-project.github.io/datasets) [💾 Dataset](https://libero-project.github.io/datasets)
    
- **Habitat**, Habitat: A Platform for Embodied AI Research, 2019, ICCV. [📄&nbsp;Paper (v2.0)](https://arxiv.org/abs/2106.14405) [📄&nbsp;Paper (v3.0)](https://arxiv.org/abs/2310.13724) [  🌐&nbsp;Website](https://aihabitat.org/) [💾 Dataset](https://huggingface.co/ai-habitat)
    
- **MimicGen**, MimicGen: Language-guided Data Generation for Imitation Learning, 2023.10. [📄&nbsp;Paper](https://arxiv.org/abs/2310.17596) [  🌐&nbsp;Website](https://mimicgen.github.io/) [💾 Dataset](https://huggingface.co/datasets/amandlek/mimicgen_datasets)
    
- **ManiSkill 2**, ManiSkill2: A Unified Benchmark for High-Level Robot Manipulation Tasks, 2023.02. [📄&nbsp;Paper](https://arxiv.org/abs/2302.04659) [  🌐&nbsp;Website](https://maniskill2.github.io/) [💾 Dataset](https://huggingface.co/datasets/haosulab/ManiSkill2)
    
- **CALVIN Dataset**, CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks, 2021.12, IEEE Robotics and Automation Letters. [📄&nbsp;Paper](https://arxiv.org/abs/2112.03227) [  🌐&nbsp;Website](http://calvin.cs.uni-freiburg.de/) [💾 Dataset](https://github.com/mees/calvin/tree/main/dataset)
    
- **RLBench (Perceiver-Actor Dataset)**, Perceiver-Actor: A Multi-Task Transformer for Robotic Manipulation, 2022.09. [📄&nbsp;Paper](https://arxiv.org/abs/2209.05451) [  🌐&nbsp;Website](https://peract.github.io/) [💾 Dataset](https://huggingface.co/datasets/hqfang/rlbench-18-tasks)
    
- **Mobile Manipulation RoboTurk (MoMaRT)**, Learning Human-Guided Mobile Manipulation, 2021.12. [📄&nbsp;Paper](https://arxiv.org/abs/2112.05251) [  🌐&nbsp;Website](https://sites.google.com/view/il-for-mm/home) [💾 Dataset](https://sites.google.com/view/il-for-mm/datasets#h.ko0ilbky4y5u)
    
- **BEHAVIOR-100 Dataset**, BEHAVIOR: Benchmark for Everyday Household Activities in Virtual, Interactive, and Ecological Environments, 2021.08, CoRL 2021. [📄&nbsp;Paper](https://arxiv.org/abs/2108.03332) [  🌐&nbsp;Website](https://behavior.stanford.edu/behavior_100/overview.html) [💾 Dataset](https://behavior.stanford.edu/behavior_100/dataset.html)
    
- **D4RL**, D4RL: Datasets for Deep Data-Driven Reinforcement Learning, 2020.04, ICLR 2021. [📄&nbsp;Paper](https://arxiv.org/abs/2004.07219) [  🌐&nbsp;Website](https://sites.google.com/view/d4rl-anonymous/) [💾 Dataset](https://minari.farama.org/datasets/D4RL/kitchen/)
    
- **ALFRED**, ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks, 2019.12. [📄&nbsp;Paper](https://arxiv.org/abs/1912.01734) [  🌐&nbsp;Website](https://askforalfred.com/) [💾 Dataset](https://github.com/askforalfred/alfred/tree/master/data)
    
- **VirtualHome**, VirtualHome: Simulating Household Activities via a Generative and Interactive Model, 2018.06. [📄&nbsp;Paper](http://virtual-home.org/paper/virtualhome.pdf) [  🌐&nbsp;Website](http://virtual-home.org/) [💾 Dataset](https://github.com/xavierpuigf/virtualhome/blob/master/virtualhome/dataset/README.md)
  </details>
---
## Real-world

| **NAME**            | YEAR | SIZE                                                                                 | MODALITIES                                                                                                                                                                                                        | ROBOTS                                                     | UNI / ORG                                                                                                              | Links                                                                                                                                                                                                                                |
| ------------------- | ---- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **DROID**           | 2024 | 🏠 564 scenes<br><br>🧩 86 <br>tasks                                                 | 🖼️ full-HD stereo videos for all three cameras,<br><br>🤖 [RLDS](https://droid-dataset.github.io/droid/the-droid-dataset),<br><br>🗣️ [Language  annotation (added in 2025)](https://huggingface.co/KarlP/droid) | Panda                                                      | 13 Universities (Stanford, <br>Berkeley, <br>Princeton, Washington <br>and [others](https://droid-dataset.github.io/)) | [🌐&nbsp;Website](https://droid-dataset.github.io/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2403.12945)<br>[💾&nbsp;Data](https://colab.research.google.com/drive/1b4PPH4XGht4Jve2xPKMCh-AXXAQziNQa?usp=sharing)                    |
| **Mobile ALOHA**    | 2024 | 🧩 7 tasks                                                                           | 🖼️ Three camera positions, cam_high, cam_left_wrist, cam_right_wrist <br><br>🤖 action, effort ,  pose <br>                                                                                                      | Mobile base<br>(two ViperX arms, two WidowX<br>for teleop. | Stanford                                                                                                               | [🌐&nbsp;Website](https://mobile-aloha.github.io/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2401.02117)<br>[💾&nbsp;Data](https://drive.google.com/drive/folders/1FP5eakcxQrsHyiWBRDsMRvUfSxeykiDc)                                  |
| **BridgeData V2**   | 2023 | 🏠 24 envs.<br><br>🧩 13 skills                                                      | 🖼️ Multiple camera views and depth data<br><br>🤖 robot arm trajectory<br><br>🗣️ Natural language labels                                                                                                        | WidowX                                                     | UC Berkeley, Stanford, <br>Google <br>DeepMind, <br>CMU                                                                | [🌐&nbsp;Website](https://rail-berkeley.github.io/bridgedata/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2308.12952)<br>[💾&nbsp;Data](https://rail.eecs.berkeley.edu/datasets/bridge_release/data/)                                  |
| **RoboSet**         | 2023 | 🕹️ 30,050 trajectories<br><br>🧩 38 tasks                                           | 🖼️ RGB cam<br><br>🗣️ Language instructions <br><br>🤖 Proprio. (state, velocity)                                                                                                                                | Panda                                                      | Carnegie<br>Mellon <br>Uni.                                                                                            | [🌐&nbsp;Website](https://robopen.github.io/roboset/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2309.01918)<br>[💾&nbsp;Data](https://github.com/vikashplus/robohive/wiki/7.-Datasets)                                                |
| **Furniture Bench** | 2023 | 🧩 8<br>furniture <br>tasks<br><br>🕹️ 5100<br>teleop.<br>demos.                     | 🖼️  Wrist camera image, Front camera image <br><br>🤖 Robot state                                                                                                                                                | Panda                                                      | Korea <br>Advanced <br>Institute <br>of <br>Science <br>and <br>Technology                                             | [🌐&nbsp;Website](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2305.12821)<br>[💾&nbsp;Data](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html) |
| **RH20T**           | 2023 | 🕹️110,000 Robot <br>demos.<br><br>🕹️110,000 Human <br>demos.<br><br>🧩140<br>tasks | 🖼️ RGB image, Depth image, Binocular IR images, Audio<br><br>🤖 Robot proprioception<br> <br> 🤏 Fingertip tactile<br><br>🗣️ Task language description                                                          | Flexiv,<br>UR5,<br>Panda,<br>Kuka                          | Shanghai AI Labs, <br>Beihang Uni., Shanghai <br>Jiao Tong Uni.<br>Sydney, <br>UESTC                                   | [🌐&nbsp;Website](https://rh20t.github.io/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2307.00595)<br>[💾&nbsp;Data](https://rh20t.github.io/#download)                                                                                |
| **Dobb-E**          | 2023 | 🕹️ 13h of interactions<br><br>🏠 22 homes<br><br>🧩109 tasks                        | 🖼️ RGB video, depth video <br> <br> 🤖 Gripper 6D pose, gripper opening                                                                                                                                          | Stretch                                                    | New York Uni.                                                                                                          | [🌐&nbsp;Website](https://dobb-e.com/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2311.16098)<br> 💾 [Data](https://github.com/notmahi/dobb-e/)                                                                                        |
| **MT-Opt**          | 2021 | 🕹️ 800,000 episodes<br><br>🧩 12 real-world tasks                                   | 🖼️ RGB image <br><br>🤖 Robot <br>action, state                                                                                                                                                                  | Kuka                                                       | Robotics at Google                                                                                                     | [🌐&nbsp;Website](https://karolhausman.github.io/mt-opt/) <br> [📄&nbsp;Paper](https://arxiv.org/abs/2104.08212) <br> 💾 [Data](https://www.tensorflow.org/datasets/catalog/mt_opt)                                                  |
| **RoboNet**         | 2019 | 🕹️ 162,000 trajectories                                                             | 🖼️ RGB image <br><br>🤖 Action sequences, end-effector pose, gripper state                                                                                                                                       | Sawyer, Panda,<br>Kuka,<br>Baxter, WidowX, Fetch           | UC Berkeley, Stanford Uni., U Pennsylvania, CMU                                                                        | [🌐&nbsp;Website](https://www.robonet.wiki/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/1910.11215)<br>[💾&nbsp;Data](https://github.com/SudeepDasari/RoboNet/wiki/Getting-Started)                                                    |
| **BC-Z**            | 2021 | 🕹️ 25,877 demos.<br><br>🧩 100 tasks                                                | 🖼️ RGB image <br><br>🗣️ Language instructions <br><br>🤖 Actions                                                                                                                                                | Google Robots (7-DOF arms)                                 | Google, <br>UC Berkeley                                                                                                | [🌐&nbsp;Website](https://sites.google.com/view/bc-z/home)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2202.02005)<br>[💾&nbsp;Data](https://www.kaggle.com/datasets/google/bc-z-robot)                                                 |
| **ManiWAV**         | 2024 | 🧩 5 tasks                                                                           | 🖼️ RGB <br>fisheye lens <br>Wrist cam<br><br>🤖 Camera pos<br><br>🤏 Microphone in griper (ear-in-hand)                                                                                                          | UR5                                                        | Stanford, Columbia, Toyota Research Institute                                                                          | [🌐&nbsp;Website](https://maniwav.github.io/)<br>[📄&nbsp;Paper](https://arxiv.org/abs/2406.19464)<br>[💾&nbsp;Data](https://real.stanford.edu/maniwav/)                                                                             |
|                     |      |                                                                                      |                                                                                                                                                                                                                   |                                                            |                                                                                                                        |                                                                                                                                                                                                                                      |

<details>
  <summary><i>Additional notes</i></summary>

<table>
  <thead>
    <tr>
      <th>NAME</th>
      <th>DATA FORMAT</th>
      <th>NOTES</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>DROID</td>
      <td>RLDS</td>
      <td>One hardware setup across 13 institutions for data collection.</td>
    </tr>
    <tr>
      <td>Mobile ALOHA</td>
      <td>HDF5</td>
      <td>Bi-manual mobile manipulation. Co-training with existing static ALOHA datasets.</td>
    </tr>
    <tr> <td>ManiWAV</td> <td>MP4, wav, json</td> <td>Teleoperated dataset with microphones inside the compliant gripper for contact-rich manipulation. Moreover passively sensing the contact events and modes, or actively sensing the object  surface materials and states </td> </tr>
    <tr>-
      <td>BridgeData V2</td>
      <td>HDF5</td>
      <td>Teleoperation of the robot with a VR<br>controller.</td>
    </tr>
    <tr>
      <td>RoboSet</td>
      <td>HDF5</td>
      <td>A large-scale, real-world multi-task dataset for everyday household activities in kitchen scenes, collected via kinesthetic and teleoperated demonstrations.</td>
    </tr>
    <tr>
      <td>Furniture Bench</td>
      <td>Pickle format</td>
      <td>3D printed furniture tasks. Data collected with Oculus Quest 2 controller and a keyboard.</td>
    </tr>
    <tr>
      <td>RH20T</td>
      <td>Compressed tarball of MP4 and NumPy data</td>
      <td>Includes pairs of human and robot demonstrations for each task. Also contains single sentence task descriptions.</td>
    </tr>
    <tr>
      <td>Dobb-E</td>
      <td>Custom (includes RGB/depth videos and action annotations)</td>
      <td>An open-source framework using a low-cost tool ("The Stick") to collect the "Homes of New York (HoNY)" dataset for teaching robots household tasks via imitation learning.</td>
    </tr>
    <tr>
      <td>MT-Opt</td>
      <td>Offline RL dataset format</td>
      <td>Multi-robot collective learning system for data collection. Pick Place tasks with 7 Kukas.</td>
    </tr>
    <tr>
      <td>RoboNet</td>
      <td>TFRecord</td>
      <td>Open database for sharing robot experience from 7 different robot platforms and institutions.</td>
    </tr>
    <tr>
      <td>BC-Z</td>
      <td>RLDS (via TFDS)</td>
      <td>A large-scale imitation learning system for zero-shot and few-shot generalization to novel manipulation tasks not seen during training.</td>
    </tr>
  </tbody>
</table>
</details>

<details>
<summary><i>Full paper citations </i></summary>

- **DROID**, DROID: A Large-Scale Robot Learning Dataset with High-Quality Demonstrations, 2024.03. [📄&nbsp;Paper](https://arxiv.org/abs/2403.12945) [  🌐&nbsp;Website](https://droid-dataset.github.io/) [💾 Dataset](https://colab.research.google.com/drive/1b4PPH4XGht4Jve2xPKMCh-AXXAQziNQa?usp=sharing)
    
- **Mobile ALOHA**, Mobile ALOHA: A Low-Cost, Full-Body Mobile Robot for Daily Living, 2024.01. [📄&nbsp;Paper](https://arxiv.org/abs/2401.02117) [  🌐&nbsp;Website](https://mobile-aloha.github.io/) [💾 Dataset](https://drive.google.com/drive/folders/1FP5eakcxQrsHyiWBRDsMRvUfSxeykiDc)

- **ManiWAV**, ManiWAV: Learning Robot Manipulation from In-the-Wild Audio-Visual Data, 2024.06. [📄&nbsp;Paper](https://arxiv.org/abs/2406.19464) [ 🌐&nbsp;Website](https://maniwav.github.io/) [💾 Dataset](https://real.stanford.edu/maniwav/) 

- **BridgeData V2**, BridgeData V2: A Large-Scale Dataset for Learning General-Purpose Robot Manipulation Policies, 2023.08. [📄&nbsp;Paper](https://arxiv.org/abs/2308.12952)  [🌐&nbsp;Website](https://rail-berkeley.github.io/bridgedata/) [💾 Dataset](https://rail.eecs.berkeley.edu/datasets/bridge_release/data/)
    
- **RoboSet**, RoboSet: A Large-Scale Dataset for Robot Manipulation with Diverse Objects and Actions, 2023.09. [📄&nbsp;Paper](https://arxiv.org/abs/2309.01918) [  🌐&nbsp;Website](https://robopen.github.io/roboset/) [💾 Dataset](https://github.com/vikashplus/robohive/wiki/7.-Datasets)
    
- **Furniture Bench**, Furniture Bench: A Benchmark for Assembling Furniture with a Robot, 2023.05. [📄&nbsp;Paper](https://arxiv.org/abs/2305.12821) [  🌐&nbsp;Website](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html) [💾 Dataset](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html)
    
- **RH20T**, RH20T: A Benchmark for Robot Hand Dexterous Manipulation, 2023.07. [📄&nbsp;Paper](https://arxiv.org/abs/2307.00595) [  🌐&nbsp;Website](https://rh20t.github.io/) [💾 Dataset](https://rh20t.github.io/#download)
    
- **Dobb-E**, Dobb-E: A Dataset for Robot Manipulation with Unseen Objects, 2023.11. [📄&nbsp;Paper](https://arxiv.org/abs/2311.16098) [  🌐&nbsp;Website](https://dobb-e.com/) [💾 Dataset](https://github.com/notmahi/dobb-e/)
    
- **MT-Opt**, MT-Opt: A Multi-Task, Multi-Modal Robot Learning Framework, 2021.04. [📄&nbsp;Paper](https://arxiv.org/abs/2104.08212) [  🌐&nbsp;Website](https://karolhausman.github.io/mt-opt/) [💾 Dataset](https://www.tensorflow.org/datasets/catalog/mt_opt)
    
- **RoboNet**, RoboNet: A Dataset for Robot Grasping and Manipulation, 2019.10. [📄&nbsp;Paper](https://arxiv.org/abs/1910.11215) [  🌐&nbsp;Website](https://www.robonet.wiki/) [💾 Dataset](https://github.com/SudeepDasari/RoboNet/wiki/Getting-Started)
    
- **BC-Z**, BC-Z: A Large-Scale Robot Learning Benchmark for Dexterous Manipulation, 2022.02. [📄&nbsp;Paper](https://arxiv.org/abs/2202.02005) [  🌐&nbsp;Website](https://sites.google.com/view/bc-z/home) [💾 Dataset](https://www.kaggle.com/datasets/google/bc-z-robot)

</details>

---

## Combined (Sim + Real)

| **NAME**      | YEAR | SIZE                                                                                                                         | MODALITIES                                                                                                                                                                | ROBOTS | UNI / ORG             | Links                                                                                                                                                                                                                                    |
| ------------- | ---- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **RoboTurk**  | 2019 | ***Real*** <br>🕹️ 2144 demos.<br><br>***Sim*** <br>🕹️ 1070 Sawyer<br>PickPlace<br>🕹️1147 <br>Sawyer<br>NutAssembly demos. | ***Real***  <br>🖼️ Multiple camera views and depth data<br><br>🤖 control data from the user and joint data from the robot<br> <br> ***Sim***<br> 🤖 Robot state, action | Sawyer | Stanford              |   [🌐&nbsp;Website](https://roboturk.stanford.edu/index.html)<br>[📄&nbsp;Paper](https://arxiv.org/abs/1811.02790)<br>***Real*** <br>[💾&nbsp;Data](https://roboturk.stanford.edu/dataset_real.html)<br>***Sim*** <br>[💾&nbsp;Data](https://roboturk.stanford.edu/dataset_sim.html) |
| **RoboMimic** | 2021 | 🧩 5 tasks<br><br>🕹️ 500 human generated  trajectories<br><br>🕹️5400 machine generated trajectories<br>                    | 🤖 Robot state, action                                                                                                                                                    | Franka | Stanford,<br>UTAustin |  [🌐&nbsp;Website](https://robomimic.github.io/) [📄&nbsp;Paper](https://arxiv.org/abs/2108.03298)<br>[💾&nbsp;Data](https://robomimic.github.io/docs/datasets/robomimic_v0.1.html)                                                                         |

<details>
  <summary><i>Additional notes</i></summary>

<table>
  <thead>
    <tr>
      <th><strong>NAME</strong></th>
      <th>DATA FORMAT</th>
      <th>NOTES</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>RoboTurk</strong></td>
      <td>HDF5, MP4</td>
      <td>Real datasets contains laundry layout, tower creation, and object search tasks done (54 users).</td>
    </tr>
    <tr>
      <td><strong>RoboMimic</strong></td>
      <td>HDF5</td>
      <td>Dataset contains very simple tasks Lift, PickandPlace. Data collected using the RoboTurk platform.</td>
    </tr>
  </tbody>
</table>
</details>

<details>
<summary><i>Full paper citations </i></summary>

- **RoboTurk**, RoboTurk: A Crowd-Sourcing Platform for High-Quality Robot Data, 2018.11, CoRL 2018. [📄&nbsp;Paper](https://arxiv.org/abs/1811.02790) [  🌐&nbsp;Website](https://roboturk.stanford.edu/index.html) [💾 Dataset](https://roboturk.stanford.edu/dataset_real.html)
    
- **RoboMimic**, RoboMimic: A Dataset and Benchmark for Vision-Based Robot Manipulation, 2021.08. [📄&nbsp;Paper](https://arxiv.org/abs/2108.03298) [  🌐&nbsp;Website](https://robomimic.github.io/) [💾 Dataset](https://robomimic.github.io/docs/datasets/robomimic_v0.1.html)
</details>

---

## Dataset Collections


| **NAME**                     | YEAR | SIZE                                               | MODALITIES                                                                                                  | ROBOTS                                                                    | UNI / ORG                                                                                                            | Links                                                                                                                                                                                                                                                                                      |
| ---------------------------- | ---- | -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Open-X Embodiment**        | 2023 | 71 **datasets** (last checked 15.9.2025)           | 🖼️ RGB, depth cameras <br><br>🗣️ Language annotations<br><br>🤖 Robot state, action                       | Franka, Spot, Hello Stretch, UR5, Sawyer, ViperX,<br>...                  | Arizona State Uni.,<br>Carnegie Mellon Uni. ,Columbia Uni.,<br>ETH Zürich, Google DeepMind, and many [other]<br><br> |   [🌐&nbsp;Website](https://robotics-transformer-x.github.io/) [📄&nbsp;Paper](https://arxiv.org/abs/2310.08864) [💾&nbsp;Data](https://robotics-transformer-x.github.io/) 📊[Dataset overview](https://docs.google.com/spreadsheets/d/1rPBD77tk60AEIGZrGSODwyyzs5FgCU9Uz3h-3_t2A9g/edit?gid=0#gid=0)        |
| **ARIO (All Robots in One)** | 2024 | 🧩321,064 tasks <br>($\approx$ 3 million episodes) | 🖼️ RGBD,<br>Point cloud<br><br>🗣️ Language annotations,<br>Sound<br><br>🤖 Proprioception<br><br>🤏 Touch | Franka, Cobot<br>Magic, Cloud Ginger, UR5, Sawyer,<br>Konova Gen3,<br>... | Peng Cheng Laboratory, Southern U Science and Technology, Sun Yat-sen Uni., ARIO Alliance                            |   [🌐&nbsp;Website](https://imaei.github.io/project_pages/ario/) [📄&nbsp;Paper](https://arxiv.org/abs/2408.10899) [💾&nbsp;Dataset](https://imaei.github.io/project_pages/ario/) 📜[Full Task List](https://imaei.github.io/project_pages/ario/static/agilex%20cobot-magic%20data%20collection%20tasks.pdf) |


<details>

<summary><i>Additional notes</i></summary>

<table>

<thead>

<tr>

<th><strong>NAME</strong></th>

<th>DATA FORMAT</th>

<th>NOTES</th>

</tr>

</thead>

<tbody>

<tr>

<td><strong>Open-X Embodiment</strong></td>

<td>RLDS</td>

<td>Information about exact modalities and robots in <a href="https://docs.google.com/spreadsheets/d/1rPBD77tk60AEIGZrGSODwyyzs5FgCU9Uz3h-3_t2A9g/edit?gid=0#gid=0">google sheet overview</a>. To get SOTA results not all datasets are used (filtering is required). Open-X provides unified download and format of datasets.</td>

</tr>

<tr>

<td><strong>ARIO (All Robots in One)</strong></td>

<td>New standard, unified data format</td>

<td>Large part of dataset is recorded on Cobot Magic platform with long-horizon, bimanual manipulation tasks and also <strong>human-robot collaboration.</strong></td>

</tr>

</tbody>

</table>

</details>

<details>

<summary><i>Full paper citations </i></summary>

- **Open-X Embodiment**, Open-X Embodiment: A New Benchmark for Large-Scale Robot Learning, 2023.10. [📄&nbsp;Paper](https://arxiv.org/abs/2310.08864) [  🌐&nbsp;Website](https://robotics-transformer-x.github.io/) [💾 Dataset](https://robotics-transformer-x.github.io/)
- **ARIO (All Robots in One)**, All Robots in One: A New Standard and Unified Dataset for Versatile, General-Purpose Embodied Agents, 2024. [📄&nbsp;Paper](https://arxiv.org/abs/2408.10899) [  🌐&nbsp;Website](https://imaei.github.io/project_pages/ario/) [💾 Dataset](https://imaei.github.io/project_pages/ario/)

</details>

---
## Benchmarks

## Simulated

| NAME            | YEAR | TASKS                                                                                                          | SIMULATOR   | ROBOTS                      | UNI <br>/ ORG               | Links                                                                                                                                                                  |
| --------------- | ---- | -------------------------------------------------------------------------------------------------------------- | ----------- | --------------------------- | --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Habitat 3.0** | 2024 | [![Demo](/images/habitat.png)](https://github.com/facebookresearch/habitat-lab/blob/main/res/img/habitat3.gif) | Habitat     | Virtual<br>human<br>agents  | Meta AI                     | [📄&nbsp;Paper](https://arxiv.org/abs/2310.13724) [ 🌐&nbsp;Website](https://aihabitat.org/habitat3/) [🛠️ Code](https://github.com/facebookresearch/habitat-lab/)     |
| **LIBERO**      | 2023 | [![Demo](/images/libero.png)](/videos/libero.gif)                                                              | RoboSuite   | Panda                       | UT Austin, Tsinghua Univers | [📄&nbsp;Paper](https://arxiv.org/abs/2306.03310) [  🌐&nbsp;Website](https://libero-project.github.io/datasets) [🛠️ Code](https://github.com/Lifelong-Robot-Learning/LIBERO) |
| **BEHAVIOR-1K** | 2022 | [![Demo](/images/behavior.png)](/videos/behavior.gif)                                                          | iGibson 2.0 | Panda, Fetch, TurtleBot     | Stanford                    | [📄&nbsp;Paper](https://arxiv.org/abs/2403.09227) [  🌐&nbsp;Website](https://behavior.stanford.edu/) [🛠️ Code](https://github.com/StanfordVL/BEHAVIOR-1K)                       |
| **CALVIN**      | 2022 | [![Demo](/images/calvin.png)](/videos/calvin.gif)                                                              | PyBullet    | Panda                       | TU Dresden                  | [📄&nbsp;Paper](https://arxiv.org/abs/2112.03227) [ 🌐&nbsp;Website](http://calvin.cs.uni-freiburg.de/) [🛠️ Code](https://github.com/mees/calvin)                     |
| **ALFRED**      | 2020 | [![Demo](/images/alfred.png)](/videos/alfred.gif)                                                              | AI2-THOR    | Virtual agents (AI2-THOR)   | Allen Institute for AI      | [📄&nbsp;Paper](https://arxiv.org/abs/1912.01734) [ 🌐&nbsp;Website](https://askforalfred.com/) [🛠️ Code](https://github.com/askforalfred/alfred)                                  |
| **RLBench**     | 2020 | [![Demo](/images/rlbench.png)](/videos/rlbench.gif)                                                            | PyRep       | Panda                       | Imperial College London     | [📄&nbsp;Paper](https://arxiv.org/abs/1909.12271) [ 🌐&nbsp;Website](https://sites.google.com/view/rlbench) [🛠️ Code](https://github.com/stepjam/RLBench)             |
| **Meta-World**  | 2019 | [![Demo](/images/metaworld.png)](/videos/metaworld.gif)                                                        | MuJoCo      | Sawyer                      | UC Berkeley                 | [📄&nbsp;Paper](https://arxiv.org/abs/1910.10897) [ 🌐&nbsp;Website](https://meta-world.github.io/) [🛠️ Code](https://github.com/Farama-Foundation/Metaworld)         |
| **VirtualHome** | 2018 | [![Demo](/images/virtualhome.png)](/videos/virtualhome.gif)                                                    | Unity3D     | Virtual <br>human<br>agents | MIT, Stanford               | [📄&nbsp;Paper](https://arxiv.org/abs/1806.07011) [ 🌐&nbsp;Website](http://virtual-home.org/) [🛠️ Code](https://github.com/xavierpuigf/virtualhome)                                    |




<details>
<summary><i>Full paper citations </i></summary>

- **Habitat 3.0**, Habitat 3.0: A Co-Habitat for Humans, Avatars and Robots, 2023.10. [📄 Paper](https://arxiv.org/abs/2310.13724) [🌐 Website](https://aihabitat.org/habitat3/) [🛠️ Code](https://github.com/facebookresearch/habitat-lab)

- **LIBERO**, LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning, 2023.06. [📄&nbsp;Paper](https://arxiv.org/abs/2306.03310) [  🌐&nbsp;Website](https://libero-project.github.io/datasets) [🛠️ Code](https://libero-project.github.io/datasets)
    
- **BEHAVIOR-1K**, BEHAVIOR-1K: A Human-Centered, Embodied AI Benchmark with 1,000 Everyday Activities and Realistic Simulation, 2024.03. [📄&nbsp;Paper](https://arxiv.org/abs/2403.09227) [  🌐&nbsp;Website](https://behavior.stanford.edu/challenge/index.html) [🛠️ Code](https://huggingface.co/datasets/behavior-1k/2025-challenge-demos)
    
- **CALVIN**, CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks, 2021.12, IEEE Robotics and Automation Letters. [📄&nbsp;Paper](https://arxiv.org/abs/2112.03227) [  🌐&nbsp;Website](http://calvin.cs.uni-freiburg.de/) [🛠️ Code](https://github.com/mees/calvin)
    
- **Habitat 2.0**, Habitat 2.0: Training Home Assistants to Rearrange their Habitat, 2021.06, NeurIPS 2021. [📄&nbsp;Paper](https://arxiv.org/abs/2106.14405) [  🌐&nbsp;Website](https://aihabitat.org/) [🛠️ Code](https://github.com/facebookresearch/habitat-lab)
    
- **ALFRED**, ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks, 2019.12, CVPR 2020. [📄&nbsp;Paper](https://arxiv.org/abs/1912.01734) [  🌐&nbsp;Website](https://askforalfred.com/) [🛠️ Code](https://github.com/askforalfred/alfred)
    
- **RLBench**, The Robot Learning Benchmark & Learning Environment, 2019.09, CoRL 2019. [📄&nbsp;Paper](https://arxiv.org/abs/1909.12271) [  🌐&nbsp;Website](https://sites.google.com/view/rlbench) [🛠️ Code](https://github.com/stepjam/RLBench)
    
- **BEHAVIOR-100**, BEHAVIOR: Benchmark for Everyday Household Activities in Virtual, Interactive, and Ecological Environments, 2021.08, CoRL 2021. [📄&nbsp;Paper](https://arxiv.org/abs/2108.03332) [  🌐&nbsp;Website](https://behavior.stanford.edu/behavior_100/overview.html) [🛠️ Code](https://behavior.stanford.edu/behavior_100/dataset.html)
    
- **Meta-World**, Meta-World: A Benchmark for Evaluating Multi-Task and Meta-Learning in Robotics, 2019.10, ICRA 2020. [📄&nbsp;Paper](https://arxiv.org/abs/1910.10897) [  🌐&nbsp;Website](https://meta-world.github.io/) [🛠️ Code](https://github.com/rlworkgroup/metaworld)
    
- **VirtualHome**, VirtualHome: Simulating Household Activities via Programs, 2018.06, CVPR 2018. [📄&nbsp;Paper](http://virtual-home.org/paper/virtualhome.pdf) [  🌐&nbsp;Website](http://virtual-home.org/) [🛠️ Code](https://github.com/xavierpuigf/virtualhome)

</details>

---
## Real life


| NAME                                                              | YEAR | TASK TYPE                                                         | PLATFORM<br>/ SET UP                       | ROBOTS | UNI / ORG                                                                                                      | Links                                                                                                                                                                                            |
| ----------------------------------------------------------------- | ---- | ----------------------------------------------------------------- | ------------------------------------------ | ------ | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **RoboArena**                                                     | 2025 | [![Demo](/images/roboarena.png)](/videos/roboarena.gif)           | DROID                                      | Panda  | UC Berkeley, <br>Stanford, <br>UWashington, <br>UMontreal, <br>NVIDIA, <br>UPenn, <br>UT Austin, <br>Yonsei U. | [📄&nbsp;Paper](https://arxiv.org/abs/2506.18123)<br>[ 🌐&nbsp;Website](https://robo-arena.github.io/)<br>[🛠️Code](https://github.com/robo-arena/roboarena)                                     |
| **CT benchmark**                                                  | 2024 | [![Demo](/images/ct.png)](/videos/ct.gif)                         | 3D printed<br>city landscape model         | Kuka   | CEMMPRE, ARISE, University of<br>Coimbra                                                                       | [📄&nbsp;Paper](https://arxiv.org/abs/2402.00708)<br>[🛠️Code](https://github.com/Robotics-and-AI/collaborative-tasks-benchmark)                                                                 |
| **FMB**<br>(**F**unctional <br>**M**anipulation<br>**B**enchmark) | 2024 | [![Demo](/images/fmb.png)](/videos/fmb.gif)                       | 3D printed basic shape<br>objects          | Panda  | UC Berkeley                                                                                                    | [📄&nbsp;Paper](https://arxiv.org/abs/2401.08553)<br>[ 🌐&nbsp;Website](https://functional-manipulation-benchmark.github.io/)<br>[🛠️Code](https://github.com/rail-berkeley/fmb)                 |
| **FurnitureBench**                                                | 2023 | [![Demo](/images/furniturebench.png)](/videos/furniturebench.gif) | RealSense cameras and 3D printed furniture | Panda  | UC Berkeley,<br>KAIST                                                                                          | [🌐&nbsp;Website](https://clvrai.github.io/furniture-bench/)<br>[🛠️Code](https://clvrai.github.io/furniture-bench/)                                                                             |
| **Robothon Task Board**                                           | 2023 |                                                                   | Internet connected task box                | Any    | Modular Motions                                                                                                | [🌐&nbsp;Website](https://www.modularmotions.com/store/p4/iot-task-board-v2023.html)                                                                                                             |
| **NIST (Assembly<br>Task Boards)**                                | 2020 |                                                                   | Custom made task boards                    | Any    | NIST                                                                                                           | [📄&nbsp;Paper](https://pubmed.ncbi.nlm.nih.gov/33029555/)<br>[ 🌐&nbsp;Website](https://www.nist.gov/el/intelligent-systems-division-73500/robotic-grasping-and-manipulation-assembly/assembly) |



<details>
<summary><i>Full paper citations </i></summary>

- **CT Benchmark**, Benchmarking human-robot collaborative assembly tasks, 2024.[📄&nbsp;Paper](https://arxiv.org/abs/2402.00708) [🛠️ Code](https://github.com/Robotics-and-AI/collaborative-tasks-benchmark)
- **FurnitureBench**, Furniture Bench: A Benchmark for Assembling Furniture with a Robot, 2023.05. [📄&nbsp;Paper](https://arxiv.org/abs/2305.12821) [  🌐&nbsp;Website](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html) [🛠️ Code](https://clvrai.github.io/furniture-bench/docs/tutorials/dataset.html)
- **RoboArena**, Distributed Real-World Evaluation of Generalist Robot Policies, 2025.06. [📄&nbsp;Paper](https://arxiv.org/abs/2506.18123) [  🌐&nbsp;Website](https://robo-arena.github.io/)
- **FMB**, J. Luo, C. Xu, F. Liu, L. Tan, Z. Lin, J. Wu, P. Abbeel, and S. Levine. FMB: A functional manipulation benchmark for generalizable robotic learning. _arXiv preprint arXiv:2401.08553_, 2024. [📄&nbsp;Paper](https://arxiv.org/abs/2401.08553) [  🌐&nbsp;Website](https://functional-manipulation-benchmark.github.io/)
</details>

---
# Physics-Based Simulation Frameworks

| Framework                                                                                            | Associated Benchmarks & Environments                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **[NVIDIA Isaac Sim](https://developer.nvidia.com/isaac/sim)**                                       | [BEHAVIOUR-1K](https://behavior.stanford.edu/); [ARNOLD](https://arnold-benchmark.github.io/); [Isaac Lab ](https://isaac-sim.github.io/IsaacLab/main/index.html)[(ORBIT)](https://isaac-orbit.github.io/); [Isaac Lab Mimic](https://isaac-sim.github.io/IsaacLab/main/source/overview/teleop_imitation.html)                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**NVIDIA Isaac Gym**](https://developer.nvidia.com/isaac-gym)                                       | [Furniture Bench](https://clvrai.github.io/furniture-bench/); [AutoMate](https://bingjietang718.github.io/automate/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **[MuJoCo](https://github.com/google-deepmind/mujoco)**                                              | [Robosuite](https://robosuite.ai/) ([Robomimic](https://robomimic.github.io/), [LIBERO](https://libero-project.github.io/main.html), [MuBle](https://michaal94.github.io/MuBlE/), [CompoSuite](https://github.com/Lifelong-ML/CompoSuite), [RoboCasa](https://robocasa.ai/)); [Meta-World ](https://meta-world.github.io/)([Continual World](https://sites.google.com/view/continualworld)); [MuJoBan, MuJoXO, MuJoGo](https://github.com/google-deepmind/deepmind-research/tree/master/physics_planning_games);  [ALOHA sim](https://github.com/google-deepmind/mujoco_menagerie/tree/main/aloha/), [VLABench](https://vlabench.github.io/); [Gymnasium-Robotics](https://github.com/Farama-Foundation/Gymnasium-Robotics) |
| **[SAPIEN](https://sapien.ucsd.edu/)**                                                               | [ManiSkill 3](https://www.maniskill.ai/); [ManiSkill 2](https://maniskill2.github.io/) ( [SimplerEnv](https://simpler-env.github.io/), [ClevrSkills](https://github.com/Qualcomm-AI-research/ClevrSkills), [VLATest](https://github.com/ma-labo/VLATest))                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **[Unity](https://unity.com/)**                                                                      | [AI2-THOR](https://ai2thor.allenai.org/) ([ManipulaTHOR](https://prior.allenai.org/projects/manipulathor), [ProcTHOR](https://procthor.allenai.org/), [ALFRED](https://askforalfred.com/))                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **[iGibson 2.0](https://svl.stanford.edu/igibson/)**                                                 | [BEHAVIOUR-100](https://behavior.stanford.edu/behavior_100/overview.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **[PyBullet](https://pybullet.org/wordpress/)**                                                      | [CausalWorld](https://sites.google.com/view/causal-world/home), [Habitat-Sim](https://github.com/facebookresearch/habitat-sim), [Calvin](http://calvin.cs.uni-freiburg.de/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**CoppeliaSim** ](https://www.coppeliarobotics.com/)**([PyRep](https://github.com/stepjam/PyRep))** | [RLBench](https://sites.google.com/view/rlbench) ([AGNOSTOS](https://jiaming-zhou.github.io/AGNOSTOS/))                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [**Webots**](https://cyberbotics.com/)                                                               | [deepbots](https://github.com/aidudezzz/deepbots)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**Drake**](https://drake.mit.edu/)                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [**Genesis**](https://genesis-embodied-ai.github.io/)                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Text-Oriented**                                                                                    | [TextWorld](https://github.com/Microsoft/TextWorld); [ALFWorld](https://alfworld.github.io/); [Tales](https://microsoft.github.io/tale-suite/); [WebShop](https://webshop-pnlp.github.io/); [PCA-Bench](https://arxiv.org/pdf/2310.02071); [PlanBench](https://github.com/karthikv792/LLMs-Planning)                                                                                                                                                                                                                                                                                                                                                                                                                        |

---
# Models

- **RoboPen**, RoboAgent: Towards Sample Efficient Robot Manipulation with Semantic Augmentations and Action Chunking, 2023.09. [📄&nbsp;Paper](https://arxiv.org/abs/2309.01918) [  🌐&nbsp;Website](https://robopen.github.io/) [🛠️ Code](https://robopen.github.io/)
    
- **Octo**, Octo: An Open-Source Generalist Robot Policy, 2024.05. [📄&nbsp;Paper](https://www.semanticscholar.org/paper/1d2753d74025e7a71594506623be81f18b073adb) [🛠️ Code](https://github.com/octo-models/octo)
    
- **Hi Robot**, Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models, 2025.02. [📄&nbsp;Paper](https://arxiv.org/abs/2502.19417) [  🌐&nbsp;Website](https://www.themoonlight.io/en/review/hi-robot-open-ended-instruction-following-with-hierarchical-vision-language-action-models)
    
- **Do As I Can, Not As I Say (SayCan)**, Do As I Can, Not As I Say: Grounding Language in Robotic Affordances, 2022.04. [📄&nbsp;Paper](https://research.google/pubs/do-as-i-can-not-as-i-say-grounding-language-in-robotic-affordances/) [  🌐&nbsp;Website](https://say-can.github.io/)
    
- **Gemini Robotics**, Gemini Robotics: Bringing AI into the Physical World, 2025.03. [📄&nbsp;Paper](https://arxiv.org/abs/2503.20020) [  🌐&nbsp;Website](https://deepmind.google/models/gemini-robotics/)
    
- **RDT-1B**, RDT-1B: A Diffusion Foundation Model for Bimanual Manipulation, 2024.10. [📄&nbsp;Paper](https://www.alphaxiv.org/overview/2410.07864v1) [  🌐&nbsp;Website](https://rdt-robotics.github.io/rdt-robotics/) [🛠️ Code](https://github.com/thu-ml/RoboticsDiffusionTransformer)
    
- **RT-X**, Open X-Embodiment: Robotic Learning Datasets and RT-X Models, 2023.10. [📄&nbsp;Paper](https://arxiv.org/abs/2310.08864) [  🌐&nbsp;Website](https://robotics-transformer-x.github.io/) [🛠️ Code](https://github.com/kyegomez/RT-X)
    
- **pi0**, π0: A Foundation Model for Robotics with Sergey Levine, 2025.02. [📄&nbsp;Paper](https://arxiv.org/abs/2410.24164) [  🌐&nbsp;Website](https://physical-intelligence.com/) [🛠️ Code](https://github.com/Physical-Intelligence/openpi)
    
- **OpenVLA**, OpenVLA: An Open-Source Vision-Language-Action Model, 2025.05. [📄&nbsp;Paper](https://proceedings.mlr.press/v270/kim25c.html) [  🌐&nbsp;Website](https://openvla.github.io/) [🛠️ Code](https://openvla.github.io/) [🛠️ Code](https://github.com/openvla/openvla)
    
- **MolmoAct**, MolmoAct: Action Reasoning Models that can Reason in Space, 2025.08. [📄&nbsp;Paper](https://arxiv.org/abs/2508.07917) [  🌐&nbsp;Website](https://allenai.org/blog/molmoact) [🛠️ Code](https://github.com/allenai/molmoact)
	
- **ManiFlow**, A General Robot Manipulation Policy via Consistency Flow Training, 2025.09. [📄&nbsp;Paper](https://arxiv.org/abs/2509.01819) [  🌐&nbsp;Website](https://maniflow-policy.github.io/)
    
- **AutoMate**, Specialist and Generalist Assembly Policies over Diverse Geometries, 2024.07. [📄&nbsp;Paper](https://arxiv.org/abs/2407.08028) [  🌐&nbsp;Website](https://bingjietang718.github.io/automate/) [🛠️ Code](https://github.com/isaac-sim/IsaacGymEnvs/blob/automate/docs/automate.md)

---
# Papers to include
- datasets:
    - Papers without code:
		**[https://momagen-rss.github.io/](https://momagen-rss.github.io/)** (16.9.2025 no code yet)
	-  Datasets website unavailable till 26 October
		- [Songling_datasets](https://openi.pcl.ac.cn/ARIO/Songling_datasets), Songling Cobot Magic hardware platform, 2 tasks, 70 episodes, 3 RGBDs, 2 arms  
		- [SeaWave](https://openi.pcl.ac.cn/ARIO/SeaWave), Dataa Robot’s Cloud Ginger XR-1, 3 tasks and about 800 episodes.  
		- [PCL_CollectInReal](https://openi.pcl.ac.cn/ARIO/PCL_CollectInReal), Cobot Magic hardware platform, 48 tasks, 2414 episodes, 3 RGBDs, 2 arms
	

- benchmarks:
	- K. Kimble, K. Van Wyk, J. Falco, E. Messina, Y. Sun, M. Shibata, W. Uemura, and Y. Yokokohji. Benchmarking Protocols for Evaluating Small Parts Robotic Assembly Systems. _IEEE Robotics and Automation Letters_, 5(2), 2020. [📄&nbsp;Paper](https://pubmed.ncbi.nlm.nih.gov/33029555/) https://www.uml.edu/research/nerve/nist-assembly-task-board-form.aspx
	- https://arxiv.org/abs/2103.05140
	- https://www.nist.gov/el/intelligent-systems-division-73500/robotic-grasping-and-manipulation-assembly/assembly
	- https://www.modularmotions.com/store/p4/iot-task-board-v2023.html


