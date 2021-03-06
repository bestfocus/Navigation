# Navigation
This is for completing an Udacity Reinforcement Learning project.
The goal of this project is to train an agent to pick up only yellow bananas (there are also blue bananas) in a large and square world through a Unity evironment.

The features of this project include:
* How to open a new environment to run a different version of Python from the one in the base environment
* How to use reinforcement learning (see code)
* How to use deep learning to train the agent for reinforcement learning (see code)

The instructions for running the code are provided below. The code is written in Python 3 and PyTorch.

1. The state and action spaces, and when the environment is considered solved:
  - 1. The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction.
  - 2. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to: moving forward, backward, left and right.
  - 3. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas. The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.
  
2. Instructions for installing dependencies or downloading needed files for Windows are provided on https://github.com/udacity/deep-reinforcement-learning#dependencies. The process is summarized as follows:
  - 1. Download AnaConda3
  - 2. Open the AnaConda Powershell Prompt to enter the following commands to create and activate a new env "drlnd" using an old Python version 3.6 required by this project:
    ```
    conda create --name drlnd python=3.6
    conda activate drlnd
    ```
  - 3. In the new env "drlnd", run the following to install the old PyTorch version for installing Unity provided by Udacity:
    ```
    conda install pytorch=0.4.0 -c pytorch
    git clone https://github.com/udacity/deep-reinforcement-learning.git
    cd deep-reinforcement-learning/python
    pip install .
    ```
  - 4. Create an IPython kernel for the drlnd environment:
    ```
    python -m ipykernel install --user --name drlnd --display-name "drlnd"
    ```
3. How to run the code in the repository, to train the agent:
  - 1. Replace the notebook Navigation.ipynb in deep-reinforcement-learning/p1_navigation with the code given here and also copy model.py and dqn_agent.py to the same folder.
  - 2. For Windows, download the file https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip, unzip the file and place the files and folders in the same folder.
  - 3. Open Jupyter Notebook.
  - 4. On Notebook, open Navigation.ipynb and select drlnd in the Kernel.
  - 5. Run the code in each cell. The results for the weights are stored in the checkpoint.pth file. The rewards per episode are shown in a plot in the Notebook. The environment with bananas viewed from the angle of the agent is shown in another window.
  - 6. After the goal is reached, the environment is close and the project is completed.

# References
1. Udacity Deep Reinforcement Learning Nanodegree Program https://www.udacity.com/
2. Human-level control through deep reinforcement learning http://files.davidqiu.com//research/nature14236.pdf
3. Deep Reinforcement Learning with Double Q-learning https://arxiv.org/pdf/1509.06461.pdf
4. Prioritized Experience Replay https://arxiv.org/abs/1511.05952
5. Dueling Network Architectures for Deep Reinforcement Learning https://arxiv.org/abs/1511.06581
