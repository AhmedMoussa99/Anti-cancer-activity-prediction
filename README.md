# Anti-cancer-activity-prediction
It’s a bioassay problem, we want to build a model to predict which compounds of chemical components will be effective against non-small cell lung cancer and which are not, by using complex chemical structured data.
# problem formulation
It’s a bioassay problem, we want to build a model to predict which compounds of chemical components will be effective against non-small cell lung cancer and which are not, by using complex chemical structured data.

Our input here is 25024 sample for training set and 12326 sample for the testing set, 2 inputs features, the first input features represents the nodes and the second features represents the edges between these nodes Our output which if this chemical compound is effective (1.0)(1218 sample) or not (-1.0)(23806 sample).

# The challenges:
Our dataset set here is not an csv file but its sdf file (chemical file) each sample here represents nodes and the edges that connect these nodes and the output, so, we need a special function to extract the information from this file.

This a bioassay problem so we need a special type of neural networks that can handle and trained on this data to get the best results.

Our dataset is imbalanced 23806 of 0’s and 1218 of 1’s so we need to solve this issue.

# data mining function
Define the problem
collect the data
preprocessing the data
build and train the models
classification and prediction
evaluation
get insights from the results
The impact
Solving kind of this medical problem will achieve progress in the medical field, especially in lung cancer cure, it will make doctors and specialists find the possible and best medicine to cure this ill.

# The ideal solution
The ideal solution here was GCN network to classifiy nodes with these hyperparameters.

message_calculation_class = GANN hidden_dim = 32 , dense_intermediate_layer_activation = 'relu', num_layers = 12
