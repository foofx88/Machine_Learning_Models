<h1><u>Exoplanet Exploration</u></h1>
<img src="/snips/exoplanets.jpg" alt="" width="360" height="150" align="right">
<p>Upon exploring the dataset - exoplanet_data.csv. There are various columns in the CSV file that might not make a lot of sense at first, after understanding what each data column means through <a href="https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html" target="_blank">NESI Archive</a></p>
<p>In this challenge, we will be utilizing 4 different models (Logistic Regression, K Nearest Neighbour, Random Forest and Deep Learning).
The data is initially cleaned before input to the models by dropping any N/A values. Then the required X and Y are identified. 
</p>

<hr>

<pThe X values use all columns except for 'koi_disposition' which is reserved for Y. 'koi_disposition' is used as the decider for the dataset as to confirm if an exoplanet can be categorized as 'Confirmed','Candidate','Falsed Positive'. 
</p>
