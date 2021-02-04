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
      This function will also have two parameters, both of them lists. It will return the Euclidean distance between the two lists. For details about this distance.
      
#### get_standard_deviation
      This function will have two parameters, a matrix and a column number. It will return the
      standard deviation of the elements in the column number passed as a parameter. For details about
      how to calculate this standard deviation.
      
#### get_standardised_matrix
      This function will take one parameter, a matrix (list of lists). It will return a matrix containing the
      standardised version of the matrix passed as a parameter. This function will somehow use the
      get_standard_deviation function above. 


