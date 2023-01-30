Introduction:
The problem being solved in this code is to classify whether a client will subscribe to a term deposit
or not. This classification is performed using the data from the Bank Marketing Dataset, which
contains information about the clients of a banking institution. The code uses a neural network
approach to solve this problem.

Data processing:
The code reads in the data from the Bank Marketing Dataset in the form of a .csv file and performs
data processing on it. Firstly, the columns are renamed to remove any unwanted quotes. Then, the
'unknown' values in the data are replaced with NaN. For the columns 'job', 'education', and 'default',
the NaN values are filled with the mode of the column. This is done to avoid loss of information.
Finally, the data is transformed using one-hot encoding for the columns 'job', 'marital', 'education',
'default', 'housing', 'loan', 'contact', 'month', 'day_of_week', 'poutcome'. One-hot encoding is used to
convert categorical variables into numerical variables.

Modelling:
The code uses two different models to solve the classification problem. Firstly, a Multi-layer
Perceptron (MLP) classifier from the scikit-learn library is used. The MLP classifier is trained on80% of the data and tested on the remaining 20% of the data. The performance of the model is
evaluated using the accuracy score, which gives the proportion of correct predictions. The code also
plots the confusion matrix to visualize the performance of the model.

Conclusion:
The code performs a successful classification of clients who will subscribe to a term deposit or not.
The choice to fill the NaN values with the mode of the column and to use one-hot encoding for the
categorical variables improved the performance of the model. The deep neural network model
created using the Keras library performed better than the MLP classifier. One of the scientific
bottlenecks was to choose the best data processing techniques and the best neural network
architecture. I was unable to visualize the network architecture using the MLP classifier, so I had to
use the Keras library to do so. I successfully overcame this bottleneck by using the appropriate data
processing techniques and choosing a suitable deep neural network architecture.
