# Highway-Env: Reinforcement Learning Project

RL course final project — training agents to drive on a highway using DQN (from scratch) and PPO (Stable-Baselines3).

**Students:** DOUDOU Hissein, ADMANTA Kamelia

![](https://raw.githubusercontent.com/eleurent/highway-env/gh-media/docs/media/highway.gif?raw=true)

## Results

| Model | Mean Reward | Notes |
|-------|-------------|-------|
| DQN (ours) | **33.40 ± 8.15** | Best score, built from scratch |
| PPO (SB3) | ~27.8 | Plateaued early |

Evaluated on the hard config: 40 aggressive vehicles, tight spacing.

## Setup

```bash
git clone https://github.com/hissein02/Highway-env-project.git
cd Highway-env-project
```

Install with [uv](https://docs.astral.sh/uv/) (recommended):
```bash
uv sync
```

Or with pip:
```bash
pip install -r requirements.txt
```

## Usage

Open `Final_Project.ipynb` and run all cells. Training flags (`TRAIN_DQN`, `TRAIN_PPO`) are set to `False` by default — the notebook loads pre-trained weights and runs evaluation directly.

To retrain, set the flags to `True` and run the training cells.

## Files

| File | Description |
|------|-------------|
| `Final_Project.ipynb` | Main notebook with all code |
| `highway_dqn_v6.pth` | DQN weights (PyTorch) |
| `highway_ppo_v4.zip` | PPO weights (SB3) |
| `REPORT.pdf` | Project report |

## Resources

- [Highway-Env docs](http://highway-env.farama.org/quickstart/)
- [Stable-Baselines3 docs](https://stable-baselines.readthedocs.io/en/master/)
