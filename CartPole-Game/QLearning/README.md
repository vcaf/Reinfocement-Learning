# Q-Learning on CartPole Game
![image](https://user-images.githubusercontent.com/78371221/236788371-220021ff-1de9-4d75-8426-91d5faf2c87b.png)

<b>Goal of the notebook:</b> in this notebook I will be training the CartPole game to play itself using QLearning.

<b>Goal of the game:</b> is to keep the pole in the vertical position by applying horizontal acions (forces) to the cart which are:
- Moving Left : denoted by 0
- Moving Right : denoted by 1

<b>The game is terminated when the following conditions appear:</b>
- Pole angle passes a certain agnle: greater than 12 degrees or 0.2095 radians.
- Cart passes out of the screen: if the cart is greater than 2.4.
- if the number of steps in an episode is greater than 200 (for the version i am using which is v0)

<b>The reward system:</b> The agent is given a 1 point reward for every step it takes within an episode.

## Results

### Results of the Game before using QLearning
[random_interaction.webm](https://user-images.githubusercontent.com/78371221/236788968-c1347e8a-9d1a-4e68-96aa-33b549c45b49.webm)

### Results of the Game with using QLearning
![applying_trained_model_last_5_epi](https://user-images.githubusercontent.com/78371221/236788623-e3f6750e-1948-42b9-a455-25eb2f01314d.gif)

## Conclusion
To conclude, the goal of the notebook was to try QLearning on the CartPole game so I can gain additional knowledge in applying the learning style and compare it to other learning styles.
