# Q-learning on Gym (Cartpole)

* Agent: performs actions on its surroundings and receives a reward for associated action. For our case, the agent is the cart, and it can move left or right.

* Environment: space an agent interacts with. For our case, the environment is a 1D line

* Reward: function that determines the action's reward. For our case, is the time interval which the pole stays balanced without falling


I will be using OpenAI's [gym](https://www.gymlibrary.dev/) environment for populate the cart and the pole.

<img src='https://miro.medium.com/v2/resize:fit:4800/format:webp/1*HNcp0AcTME4WRKqfoDc_dw.png'/>


# Q-learning

Q-learning uses a function called Q function which takes an action and state (representation of the environment) as the input. The output is the discounted cumulative future reward. For our case, this function can be represented recursively in time steps. Q-learning has an unique property where it does not require a model of the environment for learning. In practice, the Q-function is implemented with a lookup table with states in rows and actions in coluns. This table is filled dynamically while learning.

<img src='https://miro.medium.com/max/828/1*ajQ89I72kdiv0sSVo_FwCg.png'/>

