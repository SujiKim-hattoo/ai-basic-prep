## What are Hyperparameters? 하이퍼파라미터란?

* **Parameter**
    * Internal variables that a model learns **from the data** during the training process.
    * They are not set by the user.
    * *e.g., weights and biases in a neural network.*

* **Hyperparameter**
    * External configuration variables that are set **by the user before training** to control the model's learning process.
    * They are adjusted through experimentation to optimize model performance.
    * *e.g., learning rate, number of layers in a neural network.*

* **Hyperparameter Tuning**
    * The process of finding the optimal set of hyperparameters that minimizes the model's loss function and maximizes its performance.
    * It's an experimental process, as there is no single best set of hyperparameters for all problems.


## Key Hyperparameters in Deep Learning 딥러닝의 주요 하이퍼파라미터

#### 1. Optimizer & Training Hyperparameters

* **Learning Rate ($α$)**: The step size used to update the model weights during each iteration. It is one of the most critical hyperparameters for model convergence.
    * *Too high*: The model may converge too quickly to a suboptimal solution or diverge.
    * *Too low*: The training process can be very slow or get stuck.
* **Batch Size**: The number of training samples processed before the model's parameters are updated. This affects memory usage and the stability of the training process.
* **Epochs**: The number of times the entire training dataset is passed forward and backward through the model.
    * *Too few*: May lead to underfitting.
    * *Too many*: Can lead to overfitting and increased training time.
* **Optimizer**: The algorithm used to change the attributes of the neural network, such as weights, to minimize the losses.

#### 2. Model Architecture Hyperparameters

* **Number of Hidden Layers**: Sets the **depth** of the model. More layers can capture more complex patterns but increase the risk of overfitting and computational cost.
* **Number of Nodes/Units per Layer**: Sets the **width** of each layer, determining the model's representational capacity.
* **Activation Function**: A function that introduces non-linearity into the model, allowing it to learn complex data patterns. (e.g., `ReLU`, `Sigmoid`, `Tanh`).


## Hyperparameter Tuning Techniques 하이퍼파라미터 튜닝 기법

* **Grid Search**
    * Exhaustively searches through a manually specified grid of hyperparameter values to find the best combination.
    * Can be very computationally expensive and slow for a large number of hyperparameters.
* **Random Search**
    * Samples random combinations from a given range of hyperparameter values for a fixed number of iterations.
    * Often more efficient than Grid Search, as it can find good combinations faster when only a few hyperparameters are critical.
* **Bayesian Optimization**
    * An informed search method that uses the results from previous iterations to decide which set of hyperparameters to try next.
    * It builds a probability model to predict which parameters are most likely to perform well, making it more efficient than search methods.


## Summary 요약
To improve deep learning performance, key hyperparameters like learning rate and batch size and the number of layers and nodes must be carefully selected and tuned.

***

## References 참고
* [AWS: What is hyperparameter tuning?](https://aws.amazon.com/what-is/hyperparameter-tuning/)
* [IBM: What is Hyperparameter Tuning?](https://www.ibm.com/think/topics/hyperparameter-tuning)
