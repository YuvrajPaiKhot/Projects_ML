# This is an obesity level prediction model created using multiclass classification

## The dataset contains the following columns :
**Gender** – Male or Female.  
**Age** – The person’s age in years.  
**Height** – Height in meters.  
**Weight** – Weight in kilograms.  
**family_history_with_overweight** – Whether the person has a family history of being overweight (yes/no).  
**FAVC** – If the person frequently consumes high-calorie foods (yes/no).  
**FCVC** – Frequency of vegetable consumption (scale from 1 to 3).  
**NCP** – Number of main meals per day.  
**CAEC** – Frequency of consuming food between meals (Never, Sometimes, Frequently, Always).  
**SMOKE** – Whether the person smokes (yes/no).  
**CH2O** – Daily water intake (scale from 1 to 3).  
**SCC** – If the person monitors their calorie intake (yes/no).  
**FAF** – Physical activity frequency (scale from 0 to 3).  
**TUE** – Time spent using technology (scale from 0 to 3).  
**CALC** – Frequency of alcohol consumption (Never, Sometimes, Frequently, Always).  
**MTRANS** – Main mode of transportation (Automobile, Bike, Motorbike, Public Transportation, Walking).  
**NObeyesdad** – Obesity level (Insufficient Weight, Normal Weight, Overweight Level I, Overweight Level II, Obesity Type I, Obesity Type II, Obesity Type III).  

As you can see, some of the columns have binary values like Male, Female, yes, no.
I have used binary encoding to convert these values to 0 and 1

The real task was converting the categorical columns which have more than 2 types of values (CAEC, CALC, MTRANS) into numerical values with some ordinal relationship.
I have used one hot encoding to convert these values and establish a relationship between them.

We have used LogisticRegression() function from sklearn to train the model and make predictions. Initial accuracy was 86%

## Then I had the idea of introducing a new feature, BMI into the dataset. (Feature Engineering)
### BMI(Body Mass Index) = Weight(kg) / Height(m) ^ 2

After feature engineering, the accuracy score increased to 90%

This project taught me a lot about working with categorical data, feature engineering, Label and One Hot Encoding, and solidified my understanding of multiclass 
logistic regression.
