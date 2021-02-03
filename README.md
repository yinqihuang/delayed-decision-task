# Delayed Decision Task
Each episode starts by a view of the empty grid. Then a random image of a shape (square, triangle, circle) is shown in one of the squares (cue). The color, size and exact location of the shape within the grid-location is randomized. After a random number of delay frames, images of two shapes are shown in two random gridlocations (tests). The shape in one of the “test” images matches that in the “cue” image. 

# Neural Network Model
Train a neural network to learn selecting the recurring shape with cross-entropy loss. Apply 3 convolutional layers with increasing order of filter size = (8, 16, 32) and fixed kernel size = (2, 2). Apply 3 max pooling layers after the convolutional layer followed by a LSTM layer. 
