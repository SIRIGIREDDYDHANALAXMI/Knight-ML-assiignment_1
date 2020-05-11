# Knight-ML-assiignment_1

Dataset contains following types of columns :-
user_name              object
country                object
review_title           object
review_description     object
designation            object
points                  int64
price                 float64
province               object
region_1               object
region_2               object
winery                 object
variety                object
dtype: object
user_name              object
country                object
review_title           object
review_description     object
designation            object
points                  int64
price                 float64
province               object
region_1               object
region_2               object
winery                 object
dtype: object


I have dropped out username and review_2 columns in both train and test data
Secondly, I have converted all of the columns to category except for country (converted to string) , points and price
I have applied Labelbinarizer to country
and Count vectorizer to designation,province,winery,region_1 and region_2
and Tf-IDf vectorizer to review_title and title_description

I have created dummies for points and price to make up to csr matrix
and then I applied hstack on above mentioned categories and converted to csr matrix

then I have splited the traindata into x_train and x_test 
The model applied is LightbgmClassifier and RandomForestClassifier
I have averaged the models by stacking them

So, my final output has an accuracy of 0.12 :(

Would like to accept suggestion for better performance of the model !
