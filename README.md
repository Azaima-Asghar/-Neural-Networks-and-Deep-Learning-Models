# *Neural Networks and Deep Learning Models*

## *Project Overview*

Bek is a data scientist and programmer for the non-profit foundation, AlphhabetSoup. AlphhabetSoup help organizations that protect the environment and people's well-being and unify the world.The foundation has raised and donated over 10 billion dollars in the past 20 years, this money has been used to invest in life saving technologies and organize reforestation groups around the world.

Bek is incharge for data collection and analysis for the entire company. Her job is to analyze the impact of each donation and vet potential recipients. This helps ensure that the foundation's money is being used effectively. Unfortunately not every donation that company makes is impactful.The president of AlphhabetSoup Andy has asked Bek to predict which organizations are worth donating to and which are too high risk. He wants Bek to create a mathematical data driven solution that can do this accurately.

Bek has decided that this problem is too complicated for the statistical and machine learning models she has used earlier. Instead, she will design and train a deep learning neural network.

## *Resources*

* Data Source: charity_data.csv present in the      Resouces folder above.
* Open-source distribution software Anaconda and the Jupiter notebook.
* Python libraries: Sklearn, Pandas, Tensorflow.
* Visual Studio Code.

## *Data Preprocessing*

* Removed the *NAME and EIN* columns.
* Checked if there were any null values.
* Binned and encoded the *APPLICATION_TYPE and CLASSIFICATION*  columns.
* One Hot encoded the rest of the columns that were identified as features.
* Checked if we there were any unique values.

## *How many neurons and layers did you select for your neural network model? Why?*

There were 41 input features. I had chosen to reflect that number in the number of neurons used. I also decided to use 2 hidden layers as there were a lot more data to filter through. As well, by adding another layer, it would allow the model to better classify the data and with higher accuracy. The number of neurons in the first layer were 28 and the second layer had 13 neurons.

## *Were you able to achieve the target model performance? What steps did you take to try and increase model performance?*

The model performance was decent with an  accuracy of 73.2%. This is below the desired threshold of 75%. I attempted fitting models with more neurons and more hidden layers, different activation functions, and different optimizer algorithms but the accuracy of the model did not increase. 

##  *If you were to implement a different model to solve this classification problem, which would you choose? Why?* 

After looking at the performance of the model I tried other models such as random forest classifier and the logistic regression with different solvers.Random forest classifier gave an accuracy score of 71.8%. logistic regression gave an accuracy score of 70.6% with solver newton-cg where as the solver lbfgs performed worse.I would consider the random forest classifier as the model's accuracy was very close to the accuracy of the initial model and running the random forest classifier model is a lot faster than the neural network.

## *Results*

The results can be found in the file called AlphabetSoupChallenge.ipynb found above. 