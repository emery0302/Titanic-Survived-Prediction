# Titanic-Survived-Prediction
This a competition on Kaggle.
The data are provided by https://www.kaggle.com/c/titanic

The data contain the informaiton of passagers on Titanic.
survival:	Survival	(0 = No, 1 = Yes)
PassagerID: Passenger id number
Name: Passenger name
Sex: Passenger gender	 (0 = female, 1 = male)
Age: Passenger age
Pclass:	Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd
Sibsp: number of siblings / spouses aboard the Titanic
Parch: number of parents / children aboard the Titanic	
Ticket:	Ticket number	
Fare:	Passenger fare	
Cabin:	Cabin number	
Embarked:	Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton


Based on the informaiton of the passagers and whether they survived the disaster, we aim to build a model to predict whether the passagers survived in test dataset.

I cleaned the data by replace average age to unknown age, and "S" present unknown Port of Embarkation (Embarked).
In addition, the numbers of sibling and parents/children are combined to form a variable: FamilySize, which represents the number of family members.

To observe the relationship between variables and outcome, I separated the variable into continuous and categorical variables, and observe whether there is different survival rate.

The random forest is the appraoch used to train data and predict the results for the data "test".
