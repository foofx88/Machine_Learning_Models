<h3>Machine Learning Demo - Exoplanet Exploration</h3>
<hr>
<img src="/snips/exoplanets.jpg" alt="" width="360" height="150" align="right">
<p>Upon exploring the dataset - exoplanet_data.csv. There are various columns in the CSV file that might not make a lot of sense at first, after understanding what each data column means through <a href="https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html" target="_blank">NESI Archive</a></p>
<p>In this challenge, we will be utilizing 4 different models (Logistic Regression, K Nearest Neighbour, Random Forest and Deep Learning).
The data is initially cleaned before input to the models by dropping any N/A values. Then the required X and Y are identified. 
</p>

<hr>
<h3>Data preprocessing</h3>
<img src="/snips/initialised_data.JPG" alt="" width="700" height="350">

<p>
Train Test Split is created first, then data preprosessing starts from scaling the data using MinMaxScaler. <br>
<img src="/snips/setXandY.JPG" alt="" width="700" height="130"> <br>
The X values use all columns except for 'koi_disposition' which is reserved for Y. 'koi_disposition' is used as the decider for the dataset as to confirm if an exoplanet can be categorized as 'Confirmed','Candidate','Falsed Positive'. <br>

Because the data in column 'koi_disposition' are of a string value and is classified as categorical data, it needs to be converted into meaningful numbers in order to be used by Machine learning algorithms. 
</p>

<hr>

<h3>Models Comparison</h3>
<img src="/snips/comparison.png" alt="" width="704" height="214">
<p>Looking at the results from the 4 models. Random Forest had the best score with the testing data score at 91%.Deep learning followed with a close 90% whereas the other 2 models LR and KNN did alright but still not as good. It made sense that Random Forest performed the best here as there are 40 columns worth of data and each column could be the decider to predict a new Exoplanet
Other than that, as the end result is to classify a newly discovered exoplanet, Random Forest works best with classification. By using all the features (X) in the dataset, it randomly creates decision trees to predict results from each decision trees and only the prediction with the maximum votes are presented as the final prediction. </p>
<p>Hence, that is why with this dataset and its required results, Random Forest would be the best model to do the predictions</p>
  
