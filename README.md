# PIPE-MONITORING-SYSTEM-AND-HAZARD-DETECTION

**ABSTRACT**
<p align = "justify">
The major objective of our project as the name reflects is to monitor the pipe health and detect hazards which would begin by finding cracks if any in a pipe. The cracks 
and blockages of the pipe will be identified by analyzing the efficiency of the pipe. The efficiency of the pipe can be calculated by analyzing the height of the measuring 
container for liquid flowing through the pipe. This can be achieved by running a machine learning algorithm on the dataset of heights of the measuring cylinder at different time stamps.
</p>

![image](https://user-images.githubusercontent.com/87383888/125573005-be1fb399-e547-4193-b6eb-5461d78fc757.png)

**INTRODUCTION**
<p align = "justify">
Bursting of pipes has been a serious problem nowadays. Overuse of the pipes, formation of scales inside the pipe, cracks due to extreme weather conditions cause 
the damage to pipes. These damages lead to leaking and breaking of pipes, hence decreasing the efficiency. To avoid this loss, keeping the water/liquid rate constant, 
a level detecting sensor can be placed at the end of the pipe which monitors the level of water filled in the container. This data is uploaded to the cloud. 
The data is preprocessed in Jupyter software. Now, different regression algorithms are applied to predict the rate when the capacity of the pipe will reduce to a threshold value. In the model we have used to algorithms, multiple linear regression and SVM model, out of which the best fitting algorithm is the multiple regression algorithm. With such a sensor model and a machine algorithm we can predict when the pipe depreciates to a level such that it has to either repaired or replaced. This is surely advantageous to the owner of the pipe, as it help in keeping up the efficiency of the system and also avoid the fatal accidents which could lead to huge loss.
</p>
![image](https://user-images.githubusercontent.com/87383888/125573140-ee4aa1e9-dde8-49eb-834d-d6f95cbc0bef.png)
<p align = "justify">
This is a diagrammatic representation of the level detecting sensor. Here an ultrasonic sensor is used to determine the depth to which the water is filled in the 
container. Once the height is obtained the height of the water level will be Water level = Total height – Ultrasonic reading 
</p>
**FLOWCHART**

![image](https://user-images.githubusercontent.com/87383888/125573235-f0527e55-85e2-4e35-af35-426079ba90bf.png)

**COMPONENTS USED**
<p align = "justify">
1. Level detecting sensor - to find the level in the measuring cylinder.
2. TINKERCAD – Software to simulate the level detecting sensor: In TINKERCAD we will use the ultrasonic sensor as the level detecting sensor
3. Jupyter – to run the python machine learning code
</p>
![image](https://user-images.githubusercontent.com/87383888/125573304-d12490db-e698-4ac3-a01e-91bd995f9d2d.png)

**ALGORITHMS USED**
<p align = "justify">
1. Multiple Regression algorithm
2. Support Vector Machine
</p>
**LITERATURE REVIEW**
<p align = "justify">
1. Pipeline rupture: Alberta resident unaware of 2009 blast: Cracks in the pipe led to gas leakage.
2. Flyover work damages pipeline; water supply in Dadar, Kalachowkie and Parel: The flyover works above the pipe led to the damages in the pipe and ultimately led to a 
break. The break led to a wastage of water. 
</p>
**WORKING**

**Support Vector Machine**
<p align = "justify">
A Support Vector Machine models the situation by creating a feature space, which is a finite-dimensional vector space, each dimension of which represents a "feature" 
of a particular object. In the context of spam or document classification, each "feature" is the prevalence or importance of a particular word.The goal of the SVM is to train a model that assigns new unseen objects into a particular category. It achieves this by creating a linear partition of the feature space into two categories. Based on the features in the new unseen objects (e.g. documents/emails), it places an object "above" or "below" the separation plane, leading to a categorization (e.g. spam or non-spam). This makes it an example of a non-probabilistic linear classifier. It is non-probabilistic, because the features in the new objects fully determine its location in feature space and there is no stochastic element involved. Support vector machines (SVM) are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis.
</p>
CONS:
<p align = "justify">
1. It doesn't perform well, when we have large data set because the required training time is higher 
2. It also doesn't perform very well, when the data set has more noise i.e. target classes are overlapping
3. SVM doesn't directly provide probability estimates, these are calculated using an expensive five-fold cross-validation. It is related SVC method of Python scikitlearn library.
</p>

Pros:
<p align = "justify">
1. It works really well with dear margin of separation 
2. It is effective in high dimensional spaces. 
3. It is effective in cases where number of dimensions is greater than the number of samples. 
4. It uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.
</p>
Applications:
<p align = "justify">
1. Face detection 
2. Text and hypertext categorization 
3. Classification of images 
4. Bioinformatics 
5. Handwriting recognition 
6. Protein fold and remote homology detection 
7. Generalized predictive control (GPC) 
</p>
Multiple regression
<p align = "justify">
1. Multiple regression analysis is a powerful technique used for predicting the unknown value of a variable from the known value of two or more variables. 
2. It also called as predictors. 
3. Method used for studying the relationship between a dependent variable and two or more independent variables. 
4. The variable whose value is too predicted is known as the dependent variable. 
5. The ones whose known values are used for prediction known Independent (exploratory) variables. 
</p>
Advantage
<p align = "justify">
Once a multiple regression equation has been constructed, one can check how good it is by examining the coefficient of determination(R2). R2 always lies between 0 
and 1. All software provides it whenever regression procedure is run. The closer R2 is to 1, the better is the model and its prediction. 
</p>
Assumptions
<p align = "justify">
Multiple regression technique does not test whether data is linear. On the contrary, it proceeds by assuming that the relationship between the Y and each of Xi's is linear. 
Hence as a rule, it is prudent to always look at the scatter plots of (Y, Xi), i= 1, 2,…,k. If any plot suggests non linearity, one may use a suitable transformation to 
attain linearity.
</p>
**TINKERCAD CIRCUIT DIAGRAM**

![image](https://user-images.githubusercontent.com/87383888/125573971-e3046ca7-731f-4224-ad6b-d2288d03fd52.png)

![image](https://user-images.githubusercontent.com/87383888/125573977-5e65ae89-0aa6-448b-b5d6-dc5a0b51c41c.png)

**DATASET**

![image](https://user-images.githubusercontent.com/87383888/125573945-729cdcb0-0558-4929-bd2d-a4baa209bacb.png)

![image](https://user-images.githubusercontent.com/87383888/125573951-39b165c4-6649-4429-8a5a-f3b3abf911f2.png)

The dataset contains 16154 rows and 8 columns. 

Columns:
<p align = "justify">
1. Date
2. Data Temperature Avg Temp
3. Data Temperature Max Temp (Day)
4. Data Temperature Min Temp (Night)
5. Data Wind Speed
6. Rainfall (mm)
7. Data Precipitation
8. H (here h is the height of the cylinder up to which water/liquid filled)
</p>
**CODE SNAPSHOTS**

![image](https://user-images.githubusercontent.com/87383888/125574001-628ede03-1d09-42fd-958a-7796f35bfd61.png)

![image](https://user-images.githubusercontent.com/87383888/125574011-755a8c08-7a89-44e8-bd5a-8de1a698cdf6.png)

![image](https://user-images.githubusercontent.com/87383888/125574020-b6b642fb-245a-49e2-8575-55d204aabb30.png)

![image](https://user-images.githubusercontent.com/87383888/125574032-bfadb2c1-c437-4925-ad9b-f961af4b39f0.png)

![image](https://user-images.githubusercontent.com/87383888/125574045-bc445d26-82ff-4c4d-9277-634991c676c4.png)

**RESULTS**

![image](https://user-images.githubusercontent.com/87383888/125574074-de8bb457-1781-44e8-a61c-b5f13048d4e9.png)

![image](https://user-images.githubusercontent.com/87383888/125574078-a8b237e9-f2b5-458f-8562-40fe748d34f6.png)

**CONCLUSION**
<p align = "justify">
We can see that both SVM algorithm and multiple regression models give us results of dates when the efficiency of the pipe will reduce to 92%. I set the threshold of the efficiency of the pipe as 92%. This threshold value can vary from owner to owner. Threshold value is set as to when the person needs to take decision to either replace or repair the pipe. The result from the multiple regression model is close to 11th April, 2020, and the result from the SVM model is 2nd April, 2020. On manually analyzing the dataset I can conclude that for this dataset, I get accurate results when I apply the multiple regression algorithm. The threshold value of 92% can be changed and set as per the owner’s choice and the machine learning algorithm can be run accordingly. In conclusion, according to the dataset the pipe facing these environmental conditions, at this location will depreciate to 92% of its efficiency on 11th April, 2020 that is 4 months after it is installed. 
</p>
