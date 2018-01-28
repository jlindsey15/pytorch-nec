# PyTorch implementation of NEC
This repo contains a PyTorch implementation of a [Neural Episodic Control](https://arxiv.org/abs/1703.01988) agent.

# Environment Setup
1. Install [conda](https://conda.io/docs/user-guide/install/index.html) for Python 2.7.

2.
```
conda create --name nec --file conda_requirements.txt
source activate nec
pip install -r pip_requirements.txt
```

3. Install [PyTorch](http://github.com/pytorch/pytorch).

# Usage
```
python run_nec.py --env=GYM_ENV_ID
```
where GYM_ENV_ID is the environment ID of the [gym](http://github.com/openai/gym) environment you which to train on.

# Results

![nec_pong_gif](./nec_pong.gif)

A game of Pong as played using the value function learned from a NEC agent

![nec_pong_png](./nec_pong.png)

Plot of total reward per episode of Pong vs. episode number
