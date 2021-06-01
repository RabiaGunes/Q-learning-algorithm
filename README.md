# Maze-solver with Q-learning and Q-vizualisation.
This is a maze-solver using Q-learning. Main purpose of the project is to visualize agent Q-matrix. The Q- and R- matrices of the agent are built up during the exploration. The agent sends actions to the maze, and the maze replies with the reward. 
E.g. the agent starts at the position 1, with 2x2 Q- and R-matrices corresponding to the zeroth (not allowed move) position, and first (starting) position. When the agent steps into a not visited cell, its Q- and R- matrices expand by one row+column creating links to the new position. Zeros on the screen are then replaced by the calculated real Q values. Zero Q values on the screen are for visualization purposes only, in the ´brains´ of the agent they do not exist until explored.

Other notes:

1. I cheated a bit by making the agent to  link all moves that are not allowed (e.g. inner/outer walls) to the agent position 0. E.g. if a cell has three walls, the agent sees all of them as one link. 
2. The animation starts only after the calculation is finished.
3. Note that the maze is generated in a very simple way by randomizing walls positions, so agent and the goal could be locked away from each other.
