# snAI-ke
### A smart bot that learns to play Snake Game with Reinforcement Learning

- Algorithm used is Evolutionary Algorithm to create random set then apply a fit function to determine the best performing bot, which will go through a mutation and recreation for the next set.
  - fitness function: gets positive points for fruits eaten, and negative points for wall collision and also time spent without eating to elminate inifinite useless loops
  - mutation rate: 0.05 || mutation type: static

- The learning part itself is done using a Feed Forward Neural Network:
  - Input layer with 24 nodes
Vision in 16 directions
4 for head current direction
4 for tail current direction
  - Output layer with 4 nodes: action direction (segmoid)
  - Hidden layers: 2 layers 20x12 nodes (relu)

