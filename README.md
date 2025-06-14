# 🤖 LeRobot – Quick Installation Guide

This guide helps you install [LeRobot](https://huggingface.co/docs/lerobot) for development and experimentation.

## 🧱 Prerequisites

- [Miniconda or Anaconda](https://docs.conda.io/en/latest/)
- Python 3.10

## 🛠️ Installation Steps

```bash
# 1. Clone the repository
git clone https://github.com/huggingface/lerobot.git
cd lerobot

# 2. Create a new conda environment
conda create -n lerobot python=3.10 -y
conda activate lerobot

# 3. Install ffmpeg (for video rendering)
conda install ffmpeg -c conda-forge -y

# 4. Install the LeRobot package in editable mode
pip install -e .

# For simulation support (ALOHA, PushT environments)
pip install -e ".[aloha,pusht]"

# For motor control (Feetech and Dynamixel motors)
pip install -e ".[feetech,dynamixel]"

# For logging experiments with Weights & Biases
wandb login


# TODO
- [ ] set up robot
- [ ] get a camera mount for the
- [ ] calibrate
- [ ] setup data collection 
- [ ] collect data 
- [ ] Upload to huggingface
- [ ] setup training environment
- [ ] Train first model