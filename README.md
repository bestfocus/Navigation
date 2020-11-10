# Navigation
This is for completing an Udacity Reinforcement Learning project.
The goal of this project is to train an agent to pick up only yellow bananas (there are also blue bananas) in an Unity evironment.

The instruction for running the code is provided below. The code is written in Python 3 and PyTorch.

1. The state and action spaces, and when the environment is considered solved:
  a. The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction.
  b. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to: moving forward, backward, left and right.
  c. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas. The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.
  
2. Instructions for installing dependencies or downloading needed files for Windows are provided on https://github.com/udacity/deep-reinforcement-learning#dependencies. The process is summarized as follows:
  a. Download AnaConda3
  b. Open the AnaConda Powershell Prompt to enter the following commands to create and activate a new env "drlnd":
    conda create --name drlnd python=3.6
    conda activate drlnd
  c. In the new env "drlnd", run the following to install the old pytorch version for running Unity:
    conda install pytorch=0.4.0 -c pytorch
    git clone https://github.com/udacity/deep-reinforcement-learning.git
    cd deep-reinforcement-learning/python
    pip install .
  d. Create an IPython kernel for the drlnd environment:
    python -m ipykernel install --user --name drlnd --display-name "drlnd"

3. How to run the code in the repository, to train the agent:
  a. Replace the notebook Navigation.ipynb in deep-reinforcement-learning/p1_navigation with the code given here and also copy model.py and dqn_agent.py to the same folder.
  b. For Windows, download the file https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip, unzip the file and place the files and folders in the same folder.
  c. Open Jupyter Notebook.
  d. On Notebook, open Navigation.ipynb and select drlnd in the Kernel.
