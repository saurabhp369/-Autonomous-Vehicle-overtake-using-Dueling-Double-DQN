This project aims to develop an intelligent autonomous vehicle decision-making method for oncoming traffic overtaking scenarios using Dueling Double DQN reinforcement learning.

Environment Used: highway-env

Training Platform: Google Colab

## Dueling Double Deep Q-Network
* Dueling Double Deep Q-Network (Dueling Double DQN or D3QN) is a modification of the Deep Q-Network (DQN) algorithm.

* It splits the network into two streams: a state value stream and an advantage stream.

* State value stream estimates the value of being in a particular state.

* Advantage stream estimates the advantages of each possible action in that state.

* Two streams are then combined to get the Q-value estimates.

![D3DQN](https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/34493c58-e942-4dd4-90f1-0333fbf0efd5)

## Instructions to run the code:
    1) Unzip given package. Upload it to Google Drive.
    
    2) Open the D3DQN.ipynb in Google Colab with GPU runtime and run the cells.
    
    3) Make sure to change the variable named "path" according to your drive folder location.
    
    4) The data stored in "model_files" are the 3 final checkpoints of the trained model and the data stored in "log_files" contain the training loss and reward history as loss.csv and reward.csv
    
    5) If you are training the network, be sure to empty the contents of "model_files" and "log_files" without deleting the folders themselves.
 
## Output:
The following results were obtained after training the model for around 35000 iterations and 410 episodes: 

<img width="484" alt="loss" src="https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/1238d7c8-1913-43d3-a698-a87706e7a92c">
<img width="470" alt="rewards" src="https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/b3e17b6a-f646-4c6e-b8cb-89827787fe32">

Video capturing the simulation output for episode 20, 200, and 400 were recorded to provide visual representations of the agent’s performance.

* Episode 20

![episode_20](https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/fac40888-7d42-4fe0-b5e5-36de0fff2016)

* Episode 200

![episode_200](https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/41d1c32f-fa14-48e2-974c-5b8d6c7a97d9)

* Episode 400

![episode_400](https://github.com/saurabhp369/-Autonomous-Vehicle-overtake-using-Dueling-Double-DQN/assets/67332856/679ff15f-9445-429c-a8b0-e88f248e8c5e)
