# Description
I used OpenAI's Acrobot enviroment to implement a Q-learning agent. I used Tensorflow/Keras to implement the neural network.

# Results
This is a gif of the learned policy. The network is pretty unstable. It improves a good deal for an episode or so and then seems to revert to a worse policy.

![Experiment 1](https://github.com/PeterJochem/Acrobot/blob/master/cumulativeReward-1.png "Trial 1")

![Learned Policy](https://github.com/PeterJochem/Acrobot/blob/master/learnedPolicy.gif "Learned Policy")



# Tensorflow and Virtual Enviroment Setup
It is easiest to run Tensorflow from a virtual enviroment on Linux. Here are instructions on how to setup Tensorflow and the virtual enviroment https://linuxize.com/post/how-to-install-tensorflow-on-ubuntu-18-04/

To activate the virtual enviroment: ```source venv/bin/activate```

# How to Run My Code
To have the network learn a policy from scratch, run ```python3 acrobot.py```. If the agent scores more than -250 points on an episode, then the network will be saved to a file called models/myModel.h5. To view the learned, solid policy run ```python3 displayTrainedModel.py```
