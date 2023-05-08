
# Reinforcement Learning and Q learning —An example of the "taxi problem" in Python
I have chosen to follow the tutorial when proceeding to reinforcement learning problems for the reason that it is still a bit confusing for myself. Concepts such as Markov Decision Process, Reward Functions, Bellman Equation seems to be in a different universe. Going through this learning process myself, I found that going through an example and practical implementation of reinforcement learning model has helped a lot in clearing up the concepts.

## The taxi Problem
![image](https://user-images.githubusercontent.com/78371221/236786923-ccd09f01-4886-49e0-95d1-459ec50e7a59.png)


### Problem:
- Starting at a random state, the job is to get the taxi to the passenger’s location, pick up the passenger and drive to the destination, drop the customer, and then the episode ends.
- There are 4 designated locations in the grid indicated by <b>Red — 0 , Green — 1, Yellow — 2, and Blue — 3, </b>the blue letter correspond to pick up location and purple letter indicate the drop off location. The solid lines indicate walls that the taxi cannot pass, whereas the filled rectangle is the taxi, when it is yellow it is empty and when it is green it is carrying a passenger.

![image](https://user-images.githubusercontent.com/78371221/236786972-e95bb3c3-abea-42fb-886e-f7a464f7641b.png)

- Each state is defined by a 4 entries tuple: （taxi_row, taxi_col, passenger_location, destination). For example, the image shows state (2,3,2,0), which means we are at position row index 2 (note that python index start at 0 so this means row 3), and column index 3, the passenger is at Yellow, encoded by 2 and our destination is red, encoded by 0.
- State Space: The state soace indicates all possible states which are consist of 500 possible states, with 25 possible taxi positions, 5 possible locations of the passenger (including the case when the passenger is in the taxi), and 4 destination locations
- Action space: There are 6 discrete deterministic actions: 0 — move south, 1 — move north, 2 — move east, 3 — move west, 4 — pickup passenger , 5 — drop off passenger
- Rewards: Except for delivering the passenger with gets a reward of +20, each extra step has a penalty of R=-1, executing “pickup” and “drop-off” actions illegally results in R=-10


