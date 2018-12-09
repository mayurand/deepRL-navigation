# Udacity Deep Reinforcement Nanodegree Project 1: Navigation
This repository contains implementation of Navigation project at Udacity's Deep Reinforcement Learning Nanodegree program.

In this project an agent is trained to navigate (and collect bananas!) in a large, square world.
![Banana](images/banana.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

## Getting Started

### Dependencies

To set up your python environment to run the code in this repository, follow the instructions below.

1. Install Anaconda for Python3 from [here](https://www.anaconda.com/download).

2. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name p1_drlnd python=3.6
	source activate p1_drlnd
	```
	- __Windows__: 
	```bash
	conda create --name p1_drlnd python=3.6 
	activate p1_drlnd
	```
	
3. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.
	- Next, install the **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control).
	- Then, install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).
	
4. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/mayurand/deepRL-p1-navigation.git
cd deepRL-p1-navigation/python
pip install .
```

5. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `p1_drlnd` environment.
```bash
python -m ipykernel install --user --name p1_drlnd --display-name "p1_drlnd"
```


### Environment setup

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the deepRL-p1-navigation repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 

3. Test if the environment is correctly installed:
```bash
cd deepRL-p1-navigation/p1_navigation #navigate to the p1_navigation directory
source activate p1_drlnd  #Activate the python environment
jupyter notebook
```

4. Open the `Test_the_environment.ipynb` and run the cells with SHIFT+ENTER. If the environment is correctly installed, you should get to see the Unity environment in another window and values for state and action spaces under `2. Examine the State and Action Spaces`. 

### Train the agent or run a trained agent
1. To train an agent for the above environment:
```bash
cd deepRL-p1-navigation/p1_navigation #navigate to the p1_navigation directory
source activate p1_drlnd  #Activate the python environment
jupyter notebook
```
2. Open the `Navigation.ipynb` and run the cells with SHIFT+ENTER. 

3. To directly run the trained model, navigate to the `4. Watch a Smart Agent!` in the notebook and run the code.

__Note:__ Before running code in a notebook, change the kernel to match the `p1_drlnd` environment by using the drop-down `Kernel` menu. 


