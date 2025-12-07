# AMD_Robotics_Hackathon_2025_Bowling_Pin_Fixer

**Team:** Charaka

**Members:**
- Satwik Arawalli
- Sourish Chatterjee
- Ayesha Habib

**Summary:**

This project presents an autonomous robotic system designed to detect, grasp, and reposition fallen bowling pins to an upright orientation. The system employs a multi-camera vision setup integrated with SO-101 robotic arms, utilizing an Action Chunking Transformer (ACT) model trained through imitation learning. The robot processes visual input from three camera perspectives (top-view, front-view, and wrist-mounted) to generate precise manipulation trajectories. Through end-to-end learning on demonstration data, the system achieves accurate pick-and-place operations for color-coded bowling pins (blue and green), demonstrating robust spatial reasoning and dexterous manipulation capabilities. 

**How To Use**:

- Set up 3 cameras (a top view, a front view and a wrist-attached camera) along with the SO-101 arms as shown in the figure.
- Place two bowling pins - one blue and one green in front of the robot, on either side.
- Run inference using our model

![Setup](IMG_4282.png)

**Mission 1:**

- Dataset URL - https://huggingface.co/datasets/ayeshahab/blue_marker8
- Model URL - https://huggingface.co/sourishwicon/AMD_Open_Robotics_2025_Team_Charaka_Phase1_blue_makrker

**Mission 2:**

- Dataset URL - https://huggingface.co/datasets/sourishwicon/2_color_merger_fin_3
- Model URL - https://huggingface.co/sourishwicon/2_color_merger_fin_3

**Technical Summary:**

*Model:* Action Chunking Transformer (ACT) with ResNet18 vision backbone, 52M parameters

*Architecture:* 4 encoder layers, 1 decoder layer, 512-dim embeddings, 8 attention heads, VAE-augmented (latent dim: 32)

*Hardware:* AMD Instinct MI300X VF GPU

**Demo Video:**

https://drive.google.com/file/d/1RE1xJceVO0dqtqg6kzZnoT6KFTwnNZbw/view?usp=sharing
