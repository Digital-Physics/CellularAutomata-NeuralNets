# CellularAutomata-NeuralNets
This Python code predict the next state of a two-dimensional cellular automaton by using neural nets.

Basically it is a neural net that has been trained to take as input a 10x10 grid of pixels, where each of these squares are either on (1) or off (0), and predict what the next state of the 10x10 pixel pattern should look like. Now hidden from the neural net are the dynamics by which the 10x10 grid is updated from one state to the next. The neural net learns to make predictions by only being fed lots of examples of inputs and outputs, which is called "supervised learning". Essentially it's a toy model for "predicting (a variant of) life" (Check out "Conway's game of life" if you aren't familar with it.) 

I'd like to make a "reinforcement learning" model next, where the neural net interacts with the system (i.e. flips certain pixels from on to off) over many steps, while the dynamics of the system continue to play out. The goal for the neural net would be to learn to get the cellular automaton (CA) to closely reproduce an image at the end of say 10 time steps, if it can only flip a few pixels, say 3, at each time step. 

After that, I'd like to figure out how to encode the neural net system in the "game of life" itself. This is actually possible (although probably difficult and cumbersome) since the game of life is known to be "Turing complete".

After that, you'd have a toy model of the universe, with an "agent" (i.e. a Ceullular Automaton implementation of Neural Net) in it that is both following the physical laws of the universe (i.e. the cellular automaton update rules), and also interacting with the environment (i.e. other parts of the CA) in an intelligent kind of way, towards a goal. (The only action taking place outside the CA universe would be the "agent's" ability to "flip" certain bits.) (Of course this system would be hard coded into the initial state of the Cellular Automaton, as opposed to evolved from a simpler or even random initial state, like in our big bang model of the universe.)

I don't think I'll actually do some of these steps after the reinforcement learning, but it's fun to think about :) 
