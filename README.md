# Monte carlo:- n*n grid world

## ***Developers*** 👦👧👦
                1. Murukuri S V S V Vasanth (College🏛️: IIIT NAYA RAIPUR,✉️- murukuri20102@iiitnr.edu.in)
                3. B.Avinash Reddy (College🏛️: IIIT NAYA RAIPUR,✉️- bavinashreddy18@gmail.com)
# Reinforcement-Learning-technique:- 10*10 Gridworld using Monte Carlo
solving a simple 4*4 Gridworld almost similar to openAI gym frozenlake using Monte-Carlo method Reinforcement Learning

WRITTEN BY MOHAMMAD ASADOLAHI  
Mohammad.E.Asadolahi@gmail.com  
https://github.com/mohammadAsadolahi  
this program is using Reinfrocement learning to solve a 4*4 gridworld like frozen lake enviroment in open ai gym  
the method used is policy iteration whitch is one of fundamental manners of Dynamic Programing  

     | S | O | O | O |  
     | O | O | O | * |  
     | O | * | O | O |  
     | O | * | O | T |  

  
  S= start cell  
  O= normal cells  
  *= penalized cells  
  T= terminate cell  
  
our agent goal is to find policy to go from S(start) cell to T(goal) cell with maximum reward(or minimum negative reward)  
valid actions are storend in GridWorld actions array.  
positive and negative rewards in each cell is stored in Gridworld  "Rewards" dictionary and can be modified by user .the current rewards for *(hole) cells ant T(goal) cell has been set to:  
self.rewards = {(3, 3): 5, (1, 3): -2, (2, 1): -2, (3, 1): -2}  
for example reward to go in (3,3) in enviroment witch is the goal will be +5 so agent gets +5 reward whenever go to cell (3,3)  
the size of Gridworld can be changed in GridWorld calss by adding space actions  
***************************
Algorithm Flow
***************************
  first we initialize a random policy that indicate prefered moves in every cell:  
 
