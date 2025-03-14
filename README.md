This project is a Deep Q Learning project where a simple snake game learns about the env and tries to earn the maximum score.

Q stands for the quality of the action.
using *Bellman Equation for loss function*

Its Q-net - so not complicated. Just a simple feed-forward net with a few layers.

**Reward**

|   |   |
|---|---|
| - eat food  | +10  |
| - game over | -10  |
| - else:  | 0 |

**Action**

This defines our next move

|   |   |
|---|---|
|  [1,0,0] -> | straight  |
|  [0,1,0] -> | right turn  |
|  [0,0,1] -> | left turn  |

**State (11 values)**

Things the model needs to know about the environment
```
[danger straight, danger right, danger left, 

direction left, direction right,
direction up, direction down,

food left, food right,
food up, food down
]
```

### TO Run

Clone the repo
```bash
git clone https://github.com/Omega-Centauri-21/DeepQ_snake.git
```
Install the requirements
```bash
pip install requirements.txt
```

And enjoy
```bash
python3 agent.py
```