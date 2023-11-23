# Deep Learning


- Input Layers
Real values from the data
- Hidden Layers
Layers in between input and output ( 3 or more layers is considered as a "deep network" )
- Output layer 
Final estimate of the output

## Recurrent Neural Networks 
a recurrent neuron sends output back to itselft!
RNN are specifically designed to work with sequence data ( Time Series, Sentences, Audio, Car Trajectories, Music )
a sequence is like a vector of informations where the index point its point in time and the values are the training values
 

### LSTM

- Why ?
An issue RNN face is that after awhile the network will begin to "forget" the first inputs, as information is lost at each step going through the RNN.
Long Short-Term Memory provide a sort of "long-term memory" for networks, it was created to address these RNN issues.
- How ?
1. What to forget : the words goes through un sigmoid layer and  based on the output ( 0, 1 ) the words are kept are not
2. What to store : the first part is a sigmoid layer ( input gate layer ) exactly like above based on the output ( 0, 1 ), the second part is hyperbolic tangent layer which create a vector of (new candidate values) that could be added to the cell.
3. combine the first two steps to create an update to the cell state



