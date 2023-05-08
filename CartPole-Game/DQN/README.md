# Training a Deep Learning Model with Keras-RL DQN Agent on CartPole Game

<b>Goal:</b> I will be training a (Keras-RL)agent using the cartpole game from OpenAI for the agent to balance the pole with a reward (score) of at least 200 which is the maximum steps that the agent can take. I will be building a deep learning model to train on the (Keras-RL) agent using a policy based learning.


<b>Goal of the game:</b>
The CartPole game is a very simple game. The environment consists of a cart that can move left to right and a pole that is placed vertically on top of the cart. The goal of the game is for the cart (the agent) to learn how to balance the bole by adjusting the cart left to right. 


<b>Structure:</b>
1. Creating Enviroments from OpenAI (using open ai gym)
2. Building a tf.keras DL model (using tensorflow and Keras)
3. Using keras-rl agents to train (Keras)
4. Saving the model

### Outcome
<b>Training the model for a number of 5000 episodes</b>
![CartPoleVideo50000 run](https://user-images.githubusercontent.com/78371221/236787743-5f57038c-1a51-47b5-8198-aba1fd8442ba.gif)

<b>Training the model for a number of 6000 episodes</b>
![CartPoleVideo60000 run](https://user-images.githubusercontent.com/78371221/236787903-db626112-ca25-466e-b375-adea0dec80c7.gif)

## Conclusion
It can be concluded that after training the model for longer, it becomes smarter using the neural network on the DQN agent.
