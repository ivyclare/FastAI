## Questionnaire - Chapter 1

1. **Do you need these for deep learning?**
   - Lots of math T / F  =>  <span style="color:red"> False </span>
   - Lots of data T / F  =>  <span style="color:red"> False </span>
   - Lots of expensive computers T / F  =>  <span style="color:red"> False </span>
   - A PhD T / F  =>  <span style="color:red"> False </span>

2. **Name five areas where deep learning is now the best in the world.**

    - <span style="color:red"> Computer Vision e.g Object Detection </span>
    - <span style="color:red"> Natural Language processng e.g Machine Translation </span>
    - <span style="color:red"> Recommender Systems like on Netflix and YouTube </span>
    - <span style="color:red"> Medicine e.g diagnosing diabetic retinopathy </span>
    - <span style="color:red"> Time series prediction e.g Stock market prediction </span>

3. **What was the name of the first device that was based on the principle of the artificial neuron?**

      <span style="color:red"> The **Mark I Perceptron** developed by Rosenblat </span>

4. **Based on the book of the same name, what are the requirements for "Parallel Distributed Processing"?**
    - <span style="color:red">A set of processing units  </span>
    - <span style="color:red"> A state of activation  </span>
    - <span style="color:red"> An output function for each unit  </span>
    - <span style="color:red"> A pattern of connectivity among units  </span>
    - <span style="color:red"> A propagation rule for propagating patterns of activities through the network of connectivities  </span>
    - <span style="color:red"> An activation rule for combining the inputs impinging on a unit with the current state of that unit to produce a new level of activation for the unit  </span>
    - <span style="color:red"> A learning rule whereby patterns of connectivity are modified by experience  </span>
    - <span style="color:red"> An environment within which the system must operate  </span>

5. **What were the two theoretical misunderstandings that held back the field of neural networks?**

      <span style="color:red"> That neural networks were too big and slow to be useful pratically  </span>

6. **What is a GPU?**

      <span style="color:red"> Stands for **Graphical Processing Unit**. It is a kind of processor that can run multiple calculations at a time </span>

7. **Open a notebook and execute a cell containing: `1+1`. What happens?**

      <span style="color:red"> 2 is printed below the cell </span>

8. **Follow through each cell of the stripped version of the notebook for this chapter. Before executing each cell, guess what will happen.**

      <span style="color:red"> Done </span>

9. **Complete the Jupyter Notebook online appendix.**

      <span style="color:blue"> NOT DONE  </span>

10.**Why is it hard to use a traditional computer program to recognize images in a photo?**

   <p style="color:red">
   This is because traditional computer programs require explicit step by step code that has to be written by the programmer and implementing this for a task like recognizing images can be quite challenging to the programmer as we don't really understand the steps taken by the brain process and recognize images. 
   </p>   
    

11. **What did Samuel mean by "Weight Assignment"?**

      <span style="color:red"> Weight Assignment is the allocation of random variables which define how the program will operate.These variables(Weights) are updated during training and are also called parameters.</span> 
   
12. **What term do we normally use in deep learning for what Samuel called "Weights"?**

      <span style="color:red"> Parameters   </span> 
   
13. **Draw a picture that summarizes Arthur Samuel's view of a machine learning model**
   
      <p style="color:red">
      Input => Model => Output
      Weights =>
       </p> 

14. **Why is it hard to understand why a deep learning model makes a particular prediction?**
      
      <p style="color:blue"> Because the weight selection process is stochastic </p> 

15. **What is the name of the theorem that a neural network can solve any mathematical problem to any level of accuracy?**
      
      <p style="color:red"> The Universal Approximation Theorem  </p> 

16. **What do you need in order to train a model?**

      <p style="color:blue"> Data(Input) and Parameters   </p> 
     

17. **How could a feedback loop impact the rollout of a predictive policing model?**
      
      <p style="color:red"> A predictive policing model is trained on data that shows the location of arrests. In this case, the model will be predicting arrests and not crime and therefore only shows/reflects the bias in existing policing systems  </p> 
      
18. **Do we always have to use 224x224 pixel images with the cat recognition model?**
      
      <p style="color:red"> No we don't. If using a pretrained model, it is recommended to use an image size of 224x224 pixels, but this can be changed as needded.  </p> 
      
19. **What is the difference between classification and regression?**
      
      <p style="color:red"> In classification, the model predicts a category or class while regression predicts one or more numerical quantities like temperature </p> 
      
20. **What is a validation set? What is a test set? Why do we need them?**
      
      <p style="color:red"> A validation set is a certain percentage of the entire data that is used to evaluate the performance of the model during trianing while a test set is data that the model has never seen before that is kept aside to measure the quality of the model after training is completed.  Using the validation set during training can show us if our model is not performing well (overfitting or underfitting) and we can then modify our model and restart training. While the test set is important because it shows us how our model will perform on data it has never seen before. </p> 
      
21. **What will fastai do if you don't provide a validation set?**

      <p style="color:red"> Fast AI automatically creates a validation set for you (20% of the data) which it will use to evaluate your model </p> 

22. **Can we always use a random sample for a validation set? Why or why not?**
     
     <p style="color:red"> Not always. In cases like image classification it is necessary to use a random sample so that the model learns the characteristics of all data it may see in the future but in cases like time series prediction, the data is continous and dependent on time and if samples are taken random it will not be representative of the future data. In this case, if we have monthly data for one year, the first 9 months can used as training data while the last 3 months can be used for validation </p> 
     
23.**What is overfitting? Provide an example.**


   <p style="color:red"> Overfitting is the point where our model memorizes the dataset instead of learning from the dataset. An example of overfitting can be seen when the validation loss is very different from the training loss (Usually training loss is high and validation is low). This will lead to our model producing bad predictions on the test data or data it has never seen before. e.g a model saying a cat is a dog </p> 

24. **What is a metric? How does it differ to "loss"?**
      
      <p style="color:red"> A metric is a measure that is used to evaluate the performance of our model after training like error_rate, accuracy etc while the loss is used during training to evaluate how well the model is performing by comparing the model result to the target (ground truth or label), getting the error and using this error to update the weights.  </p> 

25. **How can pretrained models help?**
      
      <p style="color:red">Pretraiend models are very useful because they contain weights that have typically been trained on large datasets with very deep models and for a long time. These weights can then be used as a starting weights for our model and after training our model for a few epochs we start getting great results. Hence, they save time and resources needed to get very good results. </p> 

26. **What is the "head" of a model?**

      <p style="color:red"> The head of a pretrained model is the last part of that model i.e the section after the convolutional layers of the a pretrained model(known as the backbone) where you customize the layers as required by your model </p> 


27. **What kinds of features do the early layers of a CNN find? How about the later layers?**
      <p style="color:red"> The early layers of a CNN find features like edges, corners, circles etc while later layers start bring these features together to find higher level semantics and concepts like text, dog faces, car wheels, flowers etc </p> 

28. **Are image models only useful for photos?**

      <p style="color:red"> No, Image models can be used in other less likely areas like sound, where the sounds can be converted to images which are then used in the image models. </p> 

29. **What is an "architecture"?**

      <p style="color:red"> An architecture is the actual mathematical function that we are passing the input data and parameters to  </p> 

30. **What is segmentation?**

      <p style="color:red"> Segmentation is creating a model that can recognize each and every pixel in an image </p> 

31. **What is `y_range` used for? When do we need it?**

      <p style="color:red"> y_range is used to tell the model the range of the target variable. It can be used when we have continous number (not a category) like when the target is ratings </p> 

32. **What are "hyperparameters"?**

      <p style="color:red"> Hyperparameters are parameters that cannot be gotten from the dataset but is explicitly specified by the programmer</p> 

33. **What's the best way to avoid failures when using AI in an organization?**

      <p style="color:red">  To make sure test data is kept aside which will be used to evaluate the model performance after it has been trained </p> 

