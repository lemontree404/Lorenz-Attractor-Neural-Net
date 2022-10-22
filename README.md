# Lorenz-Attractor-Neural-Net
An attempt to build a whitebox and blackbox neural network model that is able to replicate the Lorenz Attractor (for set parameters)

# Data:
  The data was genereated by generating 100K points by using the Lorenz Equations iteratively (Euler's Method). 
  ## Lorenz Equations:
  &nbsp; ![download](https://user-images.githubusercontent.com/90332850/197321876-33839ba3-ab50-4dd3-99fb-2c00c20f31e2.png)
  
  There are 3 input variables x(n), y(n) and z(n) and 3 output variables x(n+1), y(n+1) and z(n+1)
  
# Neural Net Design:
  ![image](https://user-images.githubusercontent.com/90332850/197322148-d72e27c9-62a3-47da-9eb6-09e8929d922c.png)
  
  Input Dimensions : [3,1]  
  Hidden Layers: 2 (10 neurons each)  
  Output Dimensions : [3,1]  
  
  ### Activation Functions Used:
  * Hidden Layer 1: ReLU
  * Hidden Layer 2: ReLU
  * Output Layer: Linear
  
 # Results:
 
 The performance of the 2 models were compared on their ability to reproduce the Lorenz Attractor. While the black box approach was able to was able to roughly 
 reproduce the attractor, the white box model was not able to do so even though it seemed to be learning and updating its weights through back propagation.
