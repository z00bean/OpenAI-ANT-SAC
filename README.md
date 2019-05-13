# OpenAI-ANT-SAC
UML COMP.7030- Directed research

SAC code forked from: https://github.com/pranz24/pytorch-soft-actor-critic
To run: 

```$python3 main.py --env-name Ant-v2 --cuda```
  
The result would be dumped in a tensorboard log file inside a folder named "runs".

RLKit: This is preety much the original code from: https://github.com/vitchyr/rlkit (To install,please follow the instructions given here.)
Examples of how to run the algorithms is in the "examples" folder.

The training data is dumped in files inside a directory named "Data".

If you plan to visualize on a non GPU machine, make sure that you train with CPU on the server VM. Or you need to make changes to the ndarray after loading the data. Also, you might have to use torch.load() instead of joblib.load().
Also make sure that torch and numpy versions match.
multiworld package must be installed for rlkit to work.
