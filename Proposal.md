<h1 align="center"> CS301 Project Proposal<h1> 
  
## What is the problem that you will be investigating? Why is it interesting?
There are a lot of algorithms that can predict how busy a certain store could be at a certain time during a certain day. However, there is no such algorithm for GDS (the cafeteria at NJIT) which we are planing to create. We find it interesting because it is closely related to us and we believe that after the progect is done, we could submit it to NJIT so they could add this feature to the "NJIT Go" app. 



## What reading will you examine to provide context and background?
"5 Machine Learning Techniques for Sales Forecasting"  https://towardsdatascience.com/5-machine-learning-techniques-for-sales-forecasting-598e4984b109
This reading is a good refference of how to forcast for cycles such as each week or each month. Further, we believe that Sales forecasting should be realy close to visits of GDS if we view each swipe as a purchase. 


## What data will you use? If you are collecting new data, how will you do it?
Initialy, we are planing to collect the data manualy for one week. We will be taking shifts, recording how many people are entering the cafeteria. Although this is an expencive method of collecting the information, we believe that if NJIT recognizes the potential of this algorithm, they could let us use the data of the swipes that are being done to enter the cafeteria, or else they could let us use their GDS camera and we would implement already existing algorithms that detect the ammount of people on the video. 

## What method or algorithm are you proposing? If there are existing implementations, will you use them and how? How do you plan to improve or modify such implementations? You don’t have to have an exact answer at this point, but you should have a general sense of how you will approach the problem you are working on.

For the methods we are planing to use either ARIMA (autoregressive integrated moving average) or LTSM (Long Short-Term Memory) models because they are used for sequential data trying to predict the future in a series and we believe that GDS visits are similiar for every day of the week. We are planing to improve the implementations that other stores use for predicting their sales by using the maximum number of meal plans. Since every year we will be having a different number of students attending, we could be using the proportion out of the maximum number of meal plans purchased. We will basicaly have the information about the maximum number of visitors each year, which other stores don't have. Further more, we are planing to be constantly updating our model with new data coming in every day. 

## How will you evaluate your results? Qualitatively, what kind of results do you expect (e.g. plots or figures)? Quantitatively, what kind of analysis will you use to evaluate and/or compare your results (e.g. what performance metrics or statistical tests)?
For a visual prediction we will be plotting 7 plots for each day of the week, using x-axis for time and y-axis for the capacity.  To anylize the acuracy of the preditions, we will be collecting a validation data, separate from test data to evaluate our errors and see were the model could be improved. 
