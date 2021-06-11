
<h1 style="color:blue">Detecting Pima Indians Diabetes 👨‍⚕️🩺🏥</h1><br>
<h2>Project overview</h2>
<p>A machine learning project used to to identify whether the patient has diabetes or not based on diagnostic measurements through different machine learning models instead
of going to the medical centers and wait for the results</p><br>
<h2>Problem description : 📖📚 </h2>
<p>Given the diabetes dataset which has 
<ul>
  <li>Pregnancies: No. of times pregnant</li>
  <li>Glucose: Plasma Glucose Concentration (mg/dl)</li>
  <li>Blood Pressure: Diastolic Blood Pressure(mmHg)</li>
  <li>Skin Thickness: A value used to estimate body fat.</li>
  <li>Insulin: 2-Hour Serum Insulin (mu U/ml)</li>
  <li>BMI: Body Mass Index (weight in kg/ height in m2)</li>
  <li>Diabetes Pedigree Function: It provides information about diabetes history in relatives and genetic relationship of those relatives with patients. Higher Pedigree Function means patient is more likely to have diabetes.</li>
  <li>Age:Age (years)</li>
  <li>Outcome: Class Variable (0 or 1) where ‘0’ denotes patient is not having diabetes and ‘1’ denotes patient having diabetes.</li> 
</ul><br>
<h4> 🎈🎉And by performing data pre-processing before applying ML models we can reach an acceptable accuracy🎈🎉</h4>

</p><br>
<h2>Procedure💡</h>
<h3>Data Insight 🔭🔍🔍🕵🏻‍♂️</h3>
<p> we have to have insight into what our dataset looks like at first so we use <code>data.info</code> & <code>data.describe</code> to achieve our goal </p>
<i> Some data attribute like Blood Pressure , Skin Thickness , Age cannot be = 0 so we can know right away that it is an error</i>
<h3>Data cleaning 🧹🧽</h3>

<p> We use the IQR technique to remove outliers from our dataset </p>
<ol>
  <li> Calculate Q1 ( first quartile ) that exists in the first 25% of the data </li>
  <li> Calculate Q3 ( first quartile ) that exists in the last 75% of the data </li>
  <li> Calculate IQR by following the rule IQR = Q3-Q1 </li>
  <li> Consider the data that falls in the range between Q1-1.5 IQR and Q3+1.5 IQR </li>
</ol>
<h3>Further Exploration through plots 🕵🏻‍♂️</h3>
<p> Histogram</p>
<img src="https://cdn.discordapp.com/attachments/820090984553119765/853052231238025256/unknown.png" width="370"/><br>
<h3> Machine Learning Models 💻🤔 <h3>
<p> we implemented machine learning models to check their difference in accuracy in predicting whether or not the patient is diabetic by using the library 
  <code>scikit-learn</code> </p>
  <ul>
    <li>Logistic Regression/li>
    <li>K-Nearest Neighbors</li> 
    <li>Support Vector Machine</li> 
    <li>Decision Tree</li> 
    <li>Random Forest </li>
  </ul>

