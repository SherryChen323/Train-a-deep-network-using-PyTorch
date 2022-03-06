# Train-a-deep-network-using-PyTorch
- For all the following sections, train the model for 50 epochs and plot the curve for loss, training accuracy, and test accuracy evaluated every epoch.
1. Run the tutorial code out of the box and make sure you get reasonable results. You will report these results in Section 4, so no report needed here.
2. Change the code to have only a single fully connected layer. The model will have a single layer that connects the input to the output. What is the number of parameters? In PyTorch, ”nn.Linear” can be used for fully connected layer.
3. Change the code to have multiple fully connected layers. Try having a layer from input to 120 neurons and then a layer to 84 neurons, and finally a layer to 10 neurons, one for each category. What happens if you do not use ReLU? Describe why.
4. Change the code by adding two convolutional layers along with maxpooling layers before the fully connected layers. This will be similar to the example in the tutorial. Use this model for the following sections.
5. Try multiple batch sizes to see the effect and describe the findings. Please use batch size of 1, 4, and 1000. If 1000 does not fit into the memory of your machine, please feel free to reduce it to a largest possible number.
6. Try multiple learning rates to see the effect and describe the findings. Please use learning rates of 10, 0.1, 0.01, and 0.0001.
7. Please add some data augmentation to avoid overfitting. Note that you need to do this only for the trainnig and not the testing. You may use line 208 from Imagenet sample code:
https://github.com/pytorch/examples/blob/master/imagenet/main.py
”RandomResizedCrop” samples a random patch from the image to train the model on. ”RandomHor- izontalFlip” flips randomly chosen images horizontally.
8. Change the loss function from Cross Entropy to Mean Squared Error and report the effect.
