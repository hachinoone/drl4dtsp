# drl4dtsp

This code solves dynamic trvaeling saleman problem with deep reinforcement learning. For more details, please see our paper [Solving Dynamic Traveling Salesman Problems With Deep Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/9537638) which has been accepted at IEEE-TNNLS. If this code is useful for your work, please cite our paper:

```
@article{zhang2021solving,
  title={Solving Dynamic Traveling Salesman Problems With Deep Reinforcement Learning},
  author={Zhang, Zizhen and Liu, Hong and Zhou, MengChu and Wang, Jiahai},
  journal={IEEE Transactions on Neural Networks and Learning Systems},
  year={2021},
  publisher={IEEE}
}
```

## Dependencies

* python >= 3.6.3
* NumPy
* Scipy
* PyTorch>=1.7
* tensorboard_logger

## Quick Start

For training TSP instances with 19 customers and using rollout as REINFORCE baseline with model M1:

```
python m1/train.py --baseline rollout --graph_size 19
```

For training TSP instances with 19 customers and using rollout as REINFORCE baseline with model M2:

```
python m2/train.py --baseline rollout --graph_size 19
```

## Acknowledgements

Our code is adpated from [https://github.com/wouterkool/attention-learn-to-route](https://github.com/wouterkool/attention-learn-to-route).
