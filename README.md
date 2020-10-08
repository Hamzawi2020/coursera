# coursera
Problem:
Some hospitals will get long time to rescue the injury people from severe accidents because of the 
location of the accident. In our project, we aim to predict the severity types of accidents and try 
to provide this information to hospitals to be ready with the ambulances. As a result, that will decrease 
number of the maturity in the country. 
-	We can also use the output of our model to warn the people in the risky regions to be more cautious.  

Stockers:
-	Hospitals. 
-	Citizens who have vehicles.

Data Description:
Output (SEVERITYCODE): Our model predicts the severity of the accident whether there is injury or property damage. 
Input: latitude and longitude (x,y), the date of the accident(INCDATE), whether the human under 
       alcohol or drugs(UNDERINFL), weather (Weather), Round conditions (ROADCOND), Light condition (LIGHTCOND). 

Example:
In the location (-122.32,47.70), there was an accident in 2013/03/27 and the driver was not under the influence 
of the drags and alcohol and the weather was overcast and the road was wet and that happened in daylight.
 All the previous information will be the input of our data. While the output of the model will be 2 which
 denotes to injuries.




Methodology section:
I analyzed the data and I have some comments:
•	Number of collisions decreased along with years i.e. number of collisions in 2005-2007 is greater than number of collisions in 2017-2019.
•	Most of the cases of the collisions were without the influence of the drugs and the alcohol where the percentage of collision under alcohol and drugs is 5.05%.
•	The weather is clear in most of the collision’s cases. But also, when the weather is raining and overcasting, there are some collisions due to the bad weather. 
•	The road condition is dry in most of the collision’s cases. But also, when the road is wet for some reason i.e. oil and rain, there are some collisions. 
•	Most of the collisions happened in the daylight but there are some cases happened at night where there were lights. There are some collisions happened in unknown situations and dusk and then dawn. 
•	Finally, most of the cases are property collisions not injuries but the percentage of the injuries collisions represents 43.71%. 

Results section:
•	I selected K-nearest neighbor which is considered as supervised machine learning and it classifies the collisions based on the severity whether it is a property or injuries collisions. I selected 7 neighbors to decide on the test dataset and I used the Euclidean distance to calculate the distance between the points in the space. My model can classify the collisions of the test dataset accurately by 65.04%. 
•	I also selected another supervised algorithm to predict the collisions using logistic regression and my model can predict the severity of the collision precisely by 69.52%.   

Conclusion section:
I achieved a good result, but my model needs to be improved more by cleaning the data more or using a better algorithm such as neural network. 


