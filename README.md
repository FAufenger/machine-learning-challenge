# machine-learning-challenge

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.
To help process this data, the following models utilize machine learning capable of classifying candidate exoplanets from the raw dataset.

<br>

### Preprocess the Data: 

 * Preprocess the dataset prior to fitting the model.
 * Perform feature selection and remove unnecessary features.
 * Use various Scalers to scale the numerical data.
 * Separate the data into training and testing data.


### Tune Model Parameters

 * Use GridSearch to tune model parameters.
 * Tune and compare different classifiers.
 
 <hr>

<br>
The best result so far is the standard_scalar_logisticRegression_gridSearch although the other are also quite close to the score. one even 0.0002 away!

<hr>

### MinMax_scalar_SCV_gridSearch

 * Training Data Score: 0.8472248712569139
 * Testing Data Score: 0.852974828375286

 * Grid Params: {'C': 50, 'gamma': 0.0001}
 * Best grid Score: 0.8840364141785344

<hr>

### standard_scalar_SCV_gridSearch 

 * Training Data Score: 0.891474346748045	
 * Testing Data Score: 0.8993135011441648

 * Grid Params: {'C': 10, 'gamma': 0.0001}
 * Best grid Score: 0.8884211790218238

<hr>

### standard_scalar_logisticRegression_gridSearch

 * Training Data Score: 0.8868968148006866
 * Testing Data Score: 0.8947368421052632
 
 * Grid Params: {'C': 50, 'max_iter': 200}
 * Best grid Score: 0.8836536432371069

<hr>

### Random Tree

 * Training Data Score: 1.0
 * Testing Data Score: 0.8975972540045767
    
 * Grid Params: {'max_depth': 10, 'min_samples_split': 2}
 * Best grid Score: 0.8834624396917456

<br>
While these models are close to 90 percent accuracy, I believe that they should be a higher before sending over for NASA to use. 
<br><br>
I plan to contunue tuning and trying other models, nural networks as well
