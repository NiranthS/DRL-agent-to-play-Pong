# DRL-agent-to-play-Pong

In 2013, DeepMind published a paper which caught the attention of the both the press and the machine learning community. In the paper they developed a system that uses Deep Reinforcement Learning (Deep RL) to play various Atari games, including Breakout and Pong. The system was trained purely from the pixels of an image / frame from the video-game display as its input, without having to explicitly program any rules or knowledge of the game. More strikingly, the system detailed in the paper beat human performance across multiple Atari games using an (almost) identical architecture across the games, and is based on relatively simple concepts which have been known and studied in the Reinforcement Learning (RL) and Machine Learning (ML) fields respectively for decades

<p align="center">
   <img src="https://miro.medium.com/max/300/1*P4l2XZUffcJfJQjQ125wSw.gif">
</p>

* This is one such implementation of a Deep Reinforcement Learning agent to play Pong game from pixels.

* The agent mainly consists of a Convolutional Neural Network(CNN) which predicts the action to be taken.

* The CNN takes input which is difference of two consecutive frames(frameskip=5) which were preprocessed using the mitdeeplearning library.
 
* In Pong, rather than feeding our network one image at a time, it can actually improve performance to input the difference between two consecutive frames, which really gives us information about the movement between frames and how the game is changing ie in which direction is the ball moving.

* After training for days, I was able to achieve a score of 20-6 using the above implementation.

* Including more frames in the input and with more computational power the result could be improoved.

