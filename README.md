### Exploratory Data Analysis on Diabetes Dataset
Exploratory data analysis is a crucial component of the data science process that allows you to investigate and summarize the main characteristics of a data set. It helps to detect anomalies; discover patterns and check assumptions we may have about our data. We will in this project do a deep dive into the Pima Indians diabetes data set to see what insights we can glean from the data.
<p align="left">
<img src="https://github.com/owtwo/Exploratory-Data-Analysis-on-Diabetes-Dataset/blob/main/images/correlation%20heatmap.png" style="float: left; width: 40%; margin-right: 1%; margin-bottom: 0.5em;"><img src="https://github.com/owtwo/Exploratory-Data-Analysis-on-Diabetes-Dataset/blob/main/images/pairplot.png" style="float: left; width: 45%; margin-right: 1%; margin-bottom: 0.5em;"><p style="clear: both;">

</p>

                
<details>
        <summary>Context</summary>
        <br>
        <p style='text-align:justify;'> 
                Diabetes is one of the most frequent diseases worldwide and the number of diabetic patients are growing over the years. The main cause of diabetes                   remains unknown, yet scientists believe that both genetic factors and environmental lifestyle play a major role in diabetes. A few years ago                         research was done on a tribe in America which is called the Pima tribe (also known as the Pima Indians). In this tribe, it was found that the ladies                 are prone to diabetes very early. Several constraints were placed on the selection of these instances from a larger database. In particular, all                     patients were females at least 21 years old of Pima Indian heritage. 
        </p>
</details>

<details>
        <summary>Objective</summary>
        <br>
        <p style='text-align:justify;'>
                Here, we are conducting exploratory data analysis (EDA) to understand the different aspects of diabetes in the Pima Indians tribe.
        </p>
</details>

<details>
        <summary>Data Dictionary</summary>
        <br>
        <p style='text-align:justify;'>
             The dataset has the following information:   
        <ul>
                <li><code>Pregnancies:</code> Number of times pregnant</li>
                <li><code>Glucose:</code> Plasma glucose concentration over 2 hours in an oral glucose tolerance test</li>
                <li><code>BloodPressure:</code> Diastolic blood pressure (mm Hg)</li>
                <li><code>SkinThickness:</code> Triceps skin fold thickness (mm)</li>
                <li><code>Insulin:</code> 2-Hour serum insulin (mu U/ml)</li>
                <li><code>BMI:</code> Body mass index (weight in kg/(height in m)^2)</li>
                <li><code>DiabetesPedigreeFunction:</code> A function which scores likelihood of diabetes based on family history.</li>
                <li><code>Age:</code> Age in years</li>
                <li><code>Outcome:</code> Class variable (0: person is not diabetic or 1: person is diabetic)</li>
        </ul>
        </p>
</details>

<details>
        <summary>Summary of key findings & insights</summary>
        <br>
        <p style='text-align:justify;'>
                After EDA we gleaned the following key insights:
        <ul>
                <li>Across the two classes of women (diabetic and non-diabetic), the <code>Age</code> distribution is such that the majority of ages range from 20
                    to 30 years. The number of diabetic Women in this category is smaller(around 90) compared to the number of non-diabetic women(around 349).</li>
                <li><code>Pregnancy</code> is positively correlated with all variables except for <code>Skinthickness</code>, <code>Insulin</code> and
                    <code>DiabetePedigreeFunction</code> which are negatively correlated. This seems to suggest that as the number of preganancies increase for a
                    woman, their <code>Glucose</code>, <code>BloodPressure</code>, <code>BMI</code> and <code>Age</code> also increase while
                    <code>Skinthickness</code>, <code>Insulin</code>, and <code>DiabetesPedigreeFunction</code> decrease. Some of these correlations may be spurious
                    in nature or be influenced more by an unknown third variable. Requires further investigation.</li>
                <li>There is a relatively strong positive correlation between <code>Age</code> and <code>Pregnancy</code> indicating that as patients grow older the
                    number of pregnancies increase. </li>
                <li><code>Age</code> shows a negative correlation with <code>skinthickness</code> which is understandable because as one gets older
                    <code>skinthickness</code> naturally decreases.</li>
                <li><code>Insulin</code> also has a relatively strong positive correlation with <code>skinthickness</code> but a weak one with <code>Glucose</code>,
                    <code>BloodPressure</code>, <code>BMI</code> and <code>DiabetesPedigreeFunction</code>. </li>
        </p>
</details>
