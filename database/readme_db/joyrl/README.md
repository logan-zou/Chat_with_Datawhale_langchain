# JoyRL

[![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)

`JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 

## Install

⚠️ Note that donot install JoyRL through any mirror image!!!

```bash
# you need to install Anaconda first
conda create -n joyrl python=3.8
conda activate joyrl
pip install -U joyrl
```

Torch install:

Pip install is recommended, but if you encounter network error, you can try conda install or pip install with mirrors.

```bash
# pip CPU only
pip install torch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0
# if network error, then GPU with mirror image
pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
# CPU only
conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cpuonly -c pytorch
# GPU 
conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cudatoolkit=11.3 -c pytorch -c conda-forge
```

## Usage

### Quick Start

the following presents a demo to use joyrl. As you can see, first create a yaml file to **config hyperparameters**, then run the command as below in your terminal. That's all you need to do to train a DQN agent on CartPole-v1 environment.

```bash
joyrl --yaml ./presets/ClassControl/CartPole-v1/CartPole-v1_DQN.yaml
```
or you can run the following code in your python file. 

```python
import joyrl
if __name__ == "__main__":
    print(joyrl.__version__)
    yaml_path = "./presets/ClassControl/CartPole-v1/CartPole-v1_DQN.yaml"
    joyrl.run(yaml_path = yaml_path)
```



## Documentation

More tutorials and API documentation are hosted on [JoyRL docs](https://datawhalechina.github.io/joyrl/) or [JoyRL 中文文档](https://datawhalechina.github.io/joyrl-book/#/joyrl_docs/main).

## Algorithms

|       Name       |                          Reference                           |                    Author                     | Notes |
| :--------------: | :----------------------------------------------------------: | :-------------------------------------------: | :---: |
| Q-learning | [RL introduction](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf) | [johnjim0816](https://github.com/johnjim0816) |       |
| Sarsa | [RL introduction](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf) | [johnjim0816](https://github.com/johnjim0816) | |
| DQN | [DQN Paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) | [johnjim0816](https://github.com/johnjim0816) | |
| Double DQN  |     [DoubleDQN Paper](https://arxiv.org/abs/1509.06461)      | [johnjim0816](https://github.com/johnjim0816) | |
| Dueling DQN | [DuelingDQN Paper](https://arxiv.org/abs/1511.06581) | [johnjim0816](https://github.com/johnjim0816) | |
| NoisyDQN | [NoisyDQN Paper](https://arxiv.org/pdf/1706.10295.pdf) | [johnjim0816](https://github.com/johnjim0816) | |
| DDPG | [DDPG Paper](https://arxiv.org/abs/1509.02971) | [johnjim0816](https://github.com/johnjim0816) | |
| TD3 | [TD3 Paper](https://arxiv.org/pdf/1802.09477) | [johnjim0816](https://github.com/johnjim0816) | |
| PPO | [PPO Paper](https://arxiv.org/abs/1707.06347) | [johnjim0816](https://github.com/johnjim0816) | |

## Why JoyRL?

| RL Platform                                                  | GitHub Stars                                                 | # of Alg. <sup>(1)</sup> | Custom Env                     | Async Training      | RNN Support        | Multi-Head Observation | Backend                                           |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------ | ------------------------------ | ------------------ | ------------------ | ---------------------- | ------------------------------------------------- |
| [Baselines](https://github.com/openai/baselines)             | [![GitHub stars](https://img.shields.io/github/stars/openai/baselines)](https://github.com/openai/baselines/stargazers) | 9                        | :heavy_check_mark: (gym)       | :x:                | :heavy_check_mark: | :x:                    | TF1                                               |
| [Stable-Baselines](https://github.com/hill-a/stable-baselines) | [![GitHub stars](https://img.shields.io/github/stars/hill-a/stable-baselines)](https://github.com/hill-a/stable-baselines/stargazers) | 11                       | :heavy_check_mark: (gym)       | :x:                | :heavy_check_mark: | :x:                    | TF1                                               |
| [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3) | [![GitHub stars](https://img.shields.io/github/stars/DLR-RM/stable-baselines3)](https://github.com/DLR-RM/stable-baselines3/stargazers) | 7        | :heavy_check_mark: (gym)       | :x:                | :x:                | :heavy_check_mark:     | PyTorch                                           |
| [Ray/RLlib](https://github.com/ray-project/ray/tree/master/rllib/) | [![GitHub stars](https://img.shields.io/github/stars/ray-project/ray)](https://github.com/ray-project/ray/stargazers) | 16                       | :heavy_check_mark:             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark:     | TF/PyTorch                                        |
| [SpinningUp](https://github.com/openai/spinningup)           | [![GitHub stars](https://img.shields.io/github/stars/openai/spinningup)](https://github.com/openai/spinningupstargazers) | 6                        | :heavy_check_mark: (gym)       | :x:                | :x:                | :x:                    | PyTorch                                           |
| [Dopamine](https://github.com/google/dopamine)               | [![GitHub stars](https://img.shields.io/github/stars/google/dopamine)](https://github.com/google/dopamine/stargazers) | 7                        | :x:                            | :x:                | :x:                | :x:                    | TF/JAX                                            |
| [ACME](https://github.com/deepmind/acme)                     | [![GitHub stars](https://img.shields.io/github/stars/deepmind/acme)](https://github.com/deepmind/acme/stargazers) | 14                       | :heavy_check_mark: (dm_env)    | :x:                | :heavy_check_mark: | :heavy_check_mark:     | TF/JAX                                            |
| [keras-rl](https://github.com/keras-rl/keras-rl)             | [![GitHub stars](https://img.shields.io/github/stars/keras-rl/keras-rl)](https://github.com/keras-rl/keras-rlstargazers) | 7                        | :heavy_check_mark: (gym)       | :x:                | :x:                | :x:                    | Keras                                             |
| [cleanrl](https://github.com/vwxyzjn/cleanrl)                | ![GitHub stars](https://img.shields.io/github/stars/vwxyzjn/cleanrl) | 9                        | :heavy_check_mark: (gym)       | :x:                | :x:                | :x:                    | [poetry](https://github.com/python-poetry/poetry) |
| [rlpyt](https://github.com/astooke/rlpyt)                    | [![GitHub stars](https://img.shields.io/github/stars/astooke/rlpyt)](https://github.com/astooke/rlpyt/stargazers) | 11                       | :x:                            | :x:                | :heavy_check_mark: | :heavy_check_mark:     | PyTorch                                           |
| [ChainerRL](https://github.com/chainer/chainerrl)            | [![GitHub stars](https://img.shields.io/github/stars/chainer/chainerrl)](https://github.com/chainer/chainerrl/stargazers) | 18                       | :heavy_check_mark: (gym)       | :x:                | :heavy_check_mark: | :x:                    | Chainer                                           |
| [Tianshou](https://github.com/thu-ml/tianshou)               | [![GitHub stars](https://img.shields.io/github/stars/thu-ml/tianshou)](https://github.com/thu-ml/tianshou/stargazers) | 20                       | :heavy_check_mark: (Gymnasium) | :x:                | :heavy_check_mark: | :heavy_check_mark:     | PyTorch                                           |
| [JoyRL](https://github.com/datawhalechina/joyrl)             | ![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl) | 9                        | :heavy_check_mark: (Gymnasium) | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark:     | PyTorch                                           |

Here are some other highlghts of JoyRL:

* Provide a series of Chinese courses [JoyRL Book](https://github.com/datawhalechina/joyrl-book) (with the English version in progress), suitable for beginners to start with a combination of theory

## Contributors

<table border="0">
  <tbody>
    <tr align="center" >
        <td>
         <a href="https://github.com/JohnJim0816"><img width="70" height="70" src="https://github.com/JohnJim0816.png?s=40" alt="pic"></a><br>
         <a href="https://github.com/JohnJim0816">John Jim</a>
         <p>Peking University</p>
        </td>
        <td>
            <a href="https://github.com/qiwang067"><img width="70" height="70" src="https://github.com/qiwang067.png?s=40" alt="pic"></a><br>
            <a href="https://github.com/qiwang067">Qi Wang</a> 
            <p>Shanghai Jiao Tong University</p>
        </td>
        <td>
            <a href="https://github.com/yyysjz1997"><img width="70" height="70" src="https://github.com/yyysjz1997.png?s=40" alt="pic"></a><br>
            <a href="https://github.com/yyysjz1997">Yiyuan Yang</a> 
            <p>University of Oxford</p>
        </td>
    </tr>
  </tbody>
</table>