# Automatic-Cancer-Diagnostic

### It is quite expensive to determine whether a particular patient has cancer or not. In this project, we will be predicting whether the patient has a cancer or not using the past data.

### We will be using a certain set of dunction to predict the outcome.

#### load_from_csv
      This function will have one parameter, a file name (including, if necessary, its path). The function
      will read the CSV file and return a matrix (list of lists) in which a row in the file is a row in the
      matrix. If the file has n rows, the matrix should have n elements (each element is a list). Notice that in
      CSV files a comma separates columns (CSV = comma separated values). You can assume the file
      will contain solely numeric values (and commas, of course) with no quotes.
      
      
#### get_distance
      This function will also have two parameters, both of them lists. 
      It will return the Euclidean distance between the two lists. For details about this distance.
      
#### get_standard_deviation
      This function will have two parameters, a matrix and a column number. It will return the
      standard deviation of the elements in the column number passed as a parameter. For details about
      how to calculate this standard deviation.
      
#### get_standardised_matrix
      This function will take one parameter, a matrix (list of lists). It will return a matrix containing the
      standardised version of the matrix passed as a parameter. This function will somehow use the
      get_standard_deviation function above. 

#### get_k_nearest_labels
      This function will have four parameters: a list (a row of the matrix containing the data of the file
      data), a matrix (list of lists) containing the data from the file learning_data, and a matrix containing the
      data of the file learning_data_labels, and the last parameter is a positive integer k.
      This function should find the k rows of the matrix learning_data that are the closest to the list passed
      as a parameter. It will somehow use the get_distance function to do so. After finding these k rows,
      it should find and return the related rows in the matrix learning_data_labels.
      
#### get_mode
      This function will have one parameter, a matrix (list of lists). This matrix will have only one column
      (which will be returned by get_k_nearest_labels). This function should return the mode of the
      numbers in this matrix. The mode of a sequence of numbers is the number with the highest frequency
      (the one which repeats the most).

#### classify
      This will have 4 parameters:
      - The matrixes for data, learning_data, and learning_data_labels. For the algorithm to work correctly
      the matrixes data and learning_data will be standardised beforehand.
      - k, a positive integer
      It will return a matrix; in this document we call this matrix data_labels.
     
#### get_accuracy
      This function will have two parameters. A matrix containing the data from the file
      correct_data_labels, and a matrix containing the matrix data_labels (the output of the function
      classify)
      This function will calculate and return the percentage of accuracy. If both matrixes have exactly
      the same values (in exactly the same row numbers) then the accuracy is of 100%. If only half of the
      values of both tables match exactly in terms of value and row number, then the accuracy is of 50%,
      etc.
      
#### run_test
      The aim of this function is just to run a series of tests. By consequence, here we can use hard-coded
      values for the strings containing the filenames of data, correct_data_labels, learning_data and
      learning_data_labels.
      This function will create one matrix for each of these: correct_data_labels, learning_data and
      learning_data_labels (using load_from_csv). It will standardise the matrix data and the matrix
      learning_data (using get_standardised_matrix). Then, it will run the algorithm (using classify) and
      calculate the accuracy (using get_acuracy) for a series of experiments.
