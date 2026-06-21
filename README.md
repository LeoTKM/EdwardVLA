<h1>Edward</h1>



https://github.com/user-attachments/assets/791dabf5-62d8-4858-8ad2-1717c6c8230b


## Training Process
Fine-tuned a $\pi_{0}$ base policy using 70 episodes of manually collected data spanning two tasks: (1) placing a brown box on top of a moisturizing cream container, and (2) placing all objects on the table into a brown box.

Ran inference on a M5 Apple silicon computer, intervened during task operation when needed and collected correction trajectories (HIL) to further fine tune the model to improve its accuracy.

## Code
The Python scripts and CLI commands can be found in the `/src` directory. The data collection, training and inference processes were conducted using a __*SO101 leader-follower setup*__. Lerobot provides native libraries for integrating the arms and training the $\pi_{0}$ model. 
  - Install [Lerobot](https://huggingface.co/docs/lerobot/installation)
  - Run `conda activate lerobot` for every new CLI window

## Dataset
[Link to the dataset](https://huggingface.co/datasets/LeoTKM/record-test_20260621_132657)
