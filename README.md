# 📈  Comparing Performance of Shallow and Deep MLP for Regression Analysis
<br/>
  
### 1. &nbsp; Research Objective <br/><br/>

- _The purpose of this study is to train and evaluate a multi-layer perceptron regression model for the function y=sqrt(x), where x is an integer between 1 and 100. In such cases where the data is limited and the problem is simple, we hypothesize that a simpler model structure may perform better. To test this hypothesis, we will use the MLPRegressor module from sklearn to train and evaluate a shallow model with one hidden layer and two nodes per layer, and a deep model with four hidden layers and eight nodes per layer. The goal is to compare the performance of these models and determine which one performs better._ <br/><br/><br/> 

### 2. &nbsp; Key Components of the Neural Network Model and Experimental Settings  <br/><br/>

- _Input Nodes : 1_ <br/>
_Output Nodes : 1_ <br/>

  - _The model includes one input node and one output node due to the single input and output value_ <br/><br/>

- Number of Hidden Layers in Shallow Model : 1 <br/>
Number of Hidden Nodes in Shallow Model : 2 <br/>
Number of Hidden Layers in Deep Model : 4 <br/>
Number of Hidden Nodes in Deep Model : 8 <br/>

  - _The number of hidden layers in a neural network is a key factor that affects its ability to learn complex patterns._
  - _Generally,  increasing the number of hidden layers can provide advantages in learning complex features, but it may also come with the trade-offs of larger model size and longer training time._ 
  - _On the other hand, having fewer hidden layers can make the model simpler and faster to train, but it may not be able to capture complex relationships in the data._ <br/><br/>

- _Activation Function : Logistic Function (Sigmoid Function)_ <br/>

  - _In this experiment, instead of the commonly used relu function in regression analysis, the logistic function (sigmoid function) is utilized, which outputs values between 0 and 1._

  - _When training with a small dataset, overfitting can be a problem due to the lack of diversity in the data._ 
  - _However, the logistic function has the unique property of saturation as the slope approaches 0. By leveraging this property, the number of nodes in the hidden layer can be limited to adjust the model size, leading to model simplification, prevention of overfitting, and improvement of generalization ability._ <br/><br/>

- _Optimization Algorithm : L-BFGS (Limited-memory BFGS)_ <br/>

  - _L-BFGS estimates gradients by using a subset of the data instead of processing the entire dataset at once._ 
  - _Due to the potential for memory shortages, L-BFGS may not be suitable for processing very large datasets, and other optimization algorithms should be considered._
  - _However, when working with small datasets, L-BFGS can be advantageous in reducing training time and memory usage._ <br/><br/>

- _Cost Function : MSE (Mean Squared Error_) <br/>

  - _In regression analysis, the MSE (Mean Squared Error) is a commonly used evaluation metric that calculates the average of the squared differences between the predicted values and the actual values._ 
  - _This makes the MSE a reliable indicator of the error between the predicted and actual values in the model._ <br/><br/>

- _Maximum Number of Learning Iterations : 100_ <br/>

  - _In this experiment, the model is trained by iterating up to a maximum of 100 times._ 
  - _The number of iterations during training affects the speed and accuracy of the model, and I, as the researcher conducting the experiment, have set the number of iterations based on my experience of tuning deep learning models._ 
  - _Setting the number of iterations too low can result in underfitting, where the model is not trained enough, while setting it too high can result in overfitting._ 
  - _Therefore, I have chosen what I believe to be the most appropriate number of iterations._ <br/> <br/> <br/> 

### 4. &nbsp; Key Components of the Neural Network Model and Experimental Settings  <br/><br/>

- _The purpose of this study was to train and evaluate a multi-layer perceptron regression model for the function y=sqrt(x) using integers from 1 to 100 based on the hypothesis that a simpler structure may perform better on a small and simple problem. At this time, the performance of the models was evaluated using a metric called MAPE (Mean Absolute Percentage Error), which measures the average percentage error between the predicted and actual values. Just to let you know, the closer the model's predicted values are to the actual values, the lower the MAPE value and the closer the MAPE value is to 0, the better the model's performance is considered to be._ <br/><br/>

- _In this study, the MAPE value for the Deep Model was 0.35, while the MAPE value for the Shallow Model was 0.01, indicating that the performance of the Shallow Model was superior. Furthermore, when we examine the scatter plot, most of the data predicted by the Shallow Model matches the actual data, while the Deep Model only predicts values between 6.3509680903363845 and 6.351427249440577._ <br/><br/>

- _The reason for these results is believed to be overfitting in the Deep Model due to the simple problem and small amount of data. When predicting simple problems or with small amounts of data, a Shallow Model that does not experience overfitting may perform better, and this implies that increasing the number of parameters or deepening the network structure does not always lead to good results._ <br/><br/>

- _Therefore, it is important to design the model appropriately based on the complexity of the problem, as well as the diversity and quantity of data, as Deep Model may not always guarantee better results in all situations._ <br/><br/>



--------------------------
### 💻 S/W Development Environment
<p>
  <img src="https://img.shields.io/badge/Windows 10-0078D6?style=flat-square&logo=Windows&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google Colab-black?style=flat-square&logo=Google Colab&logoColor=yellow"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/>
</p>
<p>
  <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit learn-blue?style=flat-square&logo=scikitlearn&logoColor=F7931E"/>
  <img src="https://img.shields.io/badge/Numpy-013243?style=flat-square&logo=Numpy&logoColor=blue"/>
</p>

### 🚀 Machine Learning Model
<p>
  <img src="https://img.shields.io/badge/MLP-5C5543?style=flat-square?"/>
</p> 
