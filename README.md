# Codefundo_Idea
Idea on Disaster Prediction for Microsoft Codefundo Contest

This project will primarily focus on Cyclone prediction rate in a given region and thus will help people to manage the upcoming the disaster or evacuate if necessary.
In non technical terms, cyclone tend to occur in places where pressure drops below a certain permitted value.So our algorithm will check on the data acquired from a metrological dataset , determine the average pressure of that region and within 100 miles of it and set a threshold accordingly for that area. So over a week or so , if the pressure (as one parameter) decreases below a set value, the user of our application will be messaged accordingly to take necessary measures against it . This wont require internet but will require a mobile connection . Also it will also message the names of safe regions where users can take shelter and constant uddate the data. People of all classes can avail the service provide they have a basic cell phone. The application needs to be registered just like another portal using a internet service,after that no need for internet , they will be notified.
To predict the cyclone we can use the past weather data samples using which we can create a regression model. The features we use for this model will be humidity, pressure, percipitation and some other factors. Suppose a cyclone has already hit a particular place we can predict its trajectory using regression. For this model we can use tensorflow library present in pyhton. But predicting the trajectory of cyclone will involve a lot of non-linearity and complexity so for its prediction we can use a recurrent neural networks model which takes the previous data into account to predict its subsequent movements. 
The data for the prediction of model should also employ the data from the past 50 years of wind directions in that area to predict which place will the cyclone move to next.Once this is done we can SMS to the residents in that area.
