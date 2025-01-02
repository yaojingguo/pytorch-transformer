conda create -n transformer python=3.9

tensorboard --bind_all --logdir runs/tmodel

jupyter lab --ip 0.0.0.0 --port 8000

`python train.py`
- cpu: very slow
- mps: trigger the following error:
```
Processing Epoch 00:   0%|                                                                                                                                                 | 0/3638 [00:00<?, ?it/s][1]    6698 bus error  python train.py
```