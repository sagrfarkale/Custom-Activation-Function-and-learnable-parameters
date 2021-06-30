# Custom-Activation-Function-and-learnable-parameters
 
Introduction 

The activation function is an essential building block for every neural network. We can choose from a huge list of popular activation functions from popular Deep Learning frameworks, like ReLU, Sigmoid, Tanh, and many others. 

However, to create a state of the art model, customized particularly for your task, you may need to use a custom activation function, which is absent in Deep Learning framework you are using. Activation functions can be roughly classified into the following groups by complexity: 

Simple activation functions like SiLU, Inverse Square Root Unit (ISRU). You can quickly implement these functions using any Deep Learning framework. 

Activation functions with trainable parameters like Soft Exponential activation or S-shaped Rectified Linear Unit (SReLU). 

Activation functions, which are not differentiable at some points and require the custom implementation of the backward step, for example, Bipolar Rectified Linear Unit (BReLU 

 

 

 

“Choosing the right activation function for each layer is also crucial and may have a significant impact on metric scores and the training speed of the model.” 

 

 

Custom Activation and Learnable Parameters 

Custom Activation Functions allows you to define your own Activation function according to the need of model and which boosts its accuracy. There an many frameworks that support making custom activation function but Pytorch helps to add learnable parameters in it. In this project I made a seperate class which is inherited from nn.Module for making custom activation function, added two learnable parameters alpha and beta. The parameters thus get updated after every epoch which decreases the loss frequently.  

 

“In this project I used four Linear layers followed by three Batch Normalization with default hyperparameters and three Dropout Layers having p=0.4 and SoftMax function at last. Data was trained on 300 epochs, thus giving the training accuracy of 94 and above at the time of training and 95 at test time and above, which shows that the model is neither underfitted nor overly.” 

Training and test loss have been clearly shown in the code on github link. 

 

 

 

Outcomes of the model 

 

 

Precision 

Recall 

F-1 Score 

 

0 

0.95 

0.95 

0.95 

 

1 

0.94 

0.93 

0.94 

Accuracy 

 

 

 

0.95 

 

Alpha And Beta Plots 

 

 

 
