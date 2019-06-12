# DFFN-for-regression
Model a deep feed forward network for regression


Part 1: Model a deep feed forward network for regression
Assume that you are given a polynomial with multiple inputs and multiple outputs of the form: (𝑦1,𝑦2,…,𝑦𝑐)=𝑃(𝑥1,𝑥2,…,𝑥𝑑)



![Capturqe](https://user-images.githubusercontent.com/32982938/59371390-8bdc9c80-8d4d-11e9-8166-7e2cf65cd9a4.PNG)


For this given set of polynomials, generate 𝑁𝑡 instances to train a network. Create an additional 𝑁𝑣 instances for validation of the trained model.
1. Choose 𝑁𝑡 to be 900.
2. In your training data add some noise to 𝑦𝑖’s from a normal distribution with 𝜇=0 and 𝜎=0.001.
3. Build a feed forward network with exactly 3 hidden layers:
o Each layer should include exactly 4 nodes in the beginning.
o Use a combination of activation functions in these layers (use the same activation for each node at a given layer).
4. Define your loss function:
o Use MSE for loss function.
5. Train your algorithm with SGD.
o Use appropriate learning rates and the number of epochs.
o Report the training and validation errors.
6. Repeat Steps 2-4 with another set of activation functions (3 different combinations), learning rates (3 different schemes) and number of epochs (after finding a reasonable number of epochs in the first trial, increase by 50% for 2 times).
7. Choose your best parameters after Step 5.
8. Add new nodes at a time to each hidden layer:
o Start from the first hidden layer, add one node, train and record results.
o Move to the second hidden layer, add one node, train and record results.
o Move to the third hidden layer, add one node, train and record results.
o Repeat Step 8 until bias and variance curve is drawn (see Figure 1).
9. Increase 𝑁𝑡 by 4% and repeat Step 8.
10. Report your all results.
Figure


![Capture](https://user-images.githubusercontent.com/32982938/59371323-62237580-8d4d-11e9-8c60-4e66516c6c6f.PNG)


