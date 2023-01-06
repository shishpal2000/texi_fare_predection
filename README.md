# Taxi_Fare_Prediction
Predicting the fare of the taxi ride.

In the last few years, the number of for-hire vehicles operating in NYC has grown from 63,000 to more than 100,000.However, while the number of trips in app-based vehicles has increased from 6 million to 17 million a year, taxi trips have fallen from 11 million to 8.5 million.
Hence, the NYC Yellow Cab organization decided to become more data centric.
Then we have apps like Uber, OLA, Lyft, Gett, etc. how do these apps work? After all, that set price is not a random guess.

Objective:

The Objective behind this project to predicting fare and duration of a
     ride that can help passengers to decide when is the optimal time to start
     their commute.
It can also help drivers to decide which of two potential rides will be
     more profitable.
 
Approach used:
 ![image](https://user-images.githubusercontent.com/81008124/195773829-4c58b476-7edb-410e-a653-bebeff79f69d.png)
 
Data Preprocessing:
   In machine learning, data preprocessing is a major process of cleaning the data. Basically it is a process to convert raw data into clean data.Here cleaning 
   of data will be done by adding some columns in data such as pickup_date, pickup_day, pickup_hour, pickup_day_of_week, pickup_month, pickup_year.
  
  ![image](https://user-images.githubusercontent.com/81008124/195773965-1855bb40-1e8d-406f-918f-bdbd10ccf8b0.png)
     
  After adding some columns, I add some conditions to data such as value of pickup_longitude and dropoff_longitude should be
  greater than -78 and lesser than 70, pickup_latitude and dropoff_latitude should be greater than 37 and lesser than 45
  passenger_count should be greater than 0 and fare_amount should be greater than and equal to 2.5.
       
  ![image](https://user-images.githubusercontent.com/81008124/195777387-425fea95-a09b-47d6-b827-f216f720429f.png)

                  
Data Visualization:

  Data visualization helps to visualize the data easily using different graphs, charts, plots etc. So here 
  it is represented using scatter plot, bar graph and histogram, so that data can be analysed properly.
  Longtitude, latitude of pickup and dropoff location plotting: Maximum travels had been done in the range of -73 to 40, 
  but the rests are outliers which are present in the range of -700 and 400. This visualization is important for further processes.
     
  ![image](https://user-images.githubusercontent.com/81008124/195774887-9e555136-adf2-475d-81af-4b7dd48c9f8d.png)
     
  The above figure shows that most of the fare amount lies between 0 to 25.
     
  ![image](https://user-images.githubusercontent.com/81008124/195775043-f47eb155-64a5-4938-b983-b6d588022ed5.png)
     
     
  The above figure shows that the most of the time only one passenger used taxi to travel.

  ![image](https://user-images.githubusercontent.com/81008124/195775128-b504da3f-34c8-4fe8-8a07-d3ace62be010.png)
     
  The above figure shows that only in year 2015 the passenger counts lies between 6000 to 8000 otherwise in rest of the years 
  the passenger counts lies between 14000 to 16000.
     
  ![image](https://user-images.githubusercontent.com/81008124/195775489-083fe9bd-2edb-4493-a499-e670daff5f3b.png)
     
  The above figure shows that only at Sunday passenger count is low as compare to other days.
     
  ![image](https://user-images.githubusercontent.com/81008124/195775581-e9f249f7-5883-412a-8659-6b8c53b37dff.png)
  
   Total number of value of each passenger 
  
  ![image](https://user-images.githubusercontent.com/81008124/195775645-cd0193c1-906f-4601-a1d1-e8bb14600678.png)
  
  Total Pickup Locations
     
   ![image](https://user-images.githubusercontent.com/81008124/195775737-0f3d2d1b-d864-4039-8f82-0b5e42cd1dd9.png)
  
  Total Dropoff Locations

Model Selection:
   Model selection is the process of selecting a model among many models for a predictive problem. This project problem is to
   predict the fare_amount.This is a Regression problem. In regression problems, the dependent variable is continuous. In classification problems, 
   the dependent variable is categorical. So, we are going to deal with regression models on training data and predict it on test data. 
   In this research, I am using Random forest is a tree-based algorithm which can be used to solve regression, classification problems and
   Linear regression model, which is also helpful in regression models.I splitted the whole data into 2 parts: train data (75%) and 
   test data (25%). After that different models are approached. 
      
          
Experimental Results :

 Enter Pickup Coordinates
     ![image](https://user-images.githubusercontent.com/81008124/195773034-9ca2bc8c-a1d8-4a1b-bcbc-f9d755a499f6.png)

 Enter Dropoff Coordinates
     ![image](https://user-images.githubusercontent.com/81008124/195773083-1318274d-9b68-4ec8-8418-b3cb3b13ffd9.png)

 Enter Date
     ![image](https://user-images.githubusercontent.com/81008124/195773201-9e4d6790-092f-420f-97b9-4c9b61a1a4bc.png)

 Enter No. of passenger
     ![image](https://user-images.githubusercontent.com/81008124/195773269-13ccf584-405f-4f0d-837c-deed6685e88a.png)

 Enter Hour
     ![image](https://user-images.githubusercontent.com/81008124/195773302-d588b3e5-d026-47e9-a0a6-d5847f46a281.png)

 Enter Weekday
     ![image](https://user-images.githubusercontent.com/81008124/195773338-0b3c349a-f06b-4f53-b327-15c36cad93b4.png)

Output of Predicted Fare Amount
     ![image](https://user-images.githubusercontent.com/81008124/195773421-b1ecd455-6bd6-475c-86bd-ced4f36cac25.png)

Conclusion & Future Work:
    
  In this work, we have presented New York Taxi Fare Prediction system which predicts Value of Fare Amount from source to
  destination with the help of various attributes.My project used New York Taxi Fare Prediction Dataset from Kaggle 
  which contains 1,00,000 rows and 7 columns.To predict Value of Fare Amount I used Haversine Formula and Random Forest Regression.


     
