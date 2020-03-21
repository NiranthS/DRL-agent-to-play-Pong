# DRL-agent-to-play-Pong
A Deep Reinforcement Learning agent to play the Atari Pong game.  
The agent consists of a CNN with the difference of current frame and the previous frame of the environment(with frameskip=5) as input.  
The frames are preprocessed using the preprocess function of mitdeeplearning library which converts the frame into the shape (80,80,1).  
In Pong, rather than feeding our network one image at a time, it can actually improve performance to input the difference between two consecutive observations, which really gives us information about the movement between frames and how the game is changing.
