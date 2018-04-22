# Elon-Moist

Project Overview

Elon Moist is an automatic plant moisturiser. Using a moisture probe, the system will determine the moisture content of a plant’s soil and decide whether water should be added to the plant or not. Using these statistics, the system operates a water pump which automatically adds water to the plant, when required.

The inspiration of the project begins with the notion to automate everything. As the world is progressing, more and more things are being automated, which gives the rest of society time and ability to focus on other aspects of life. With this idea, we decided that we would create a project with the Omega that would further reaffirm this concept. By creating an automatic plant waterer, the time that a human being would have spent doing this menial task can now be used to work on lab 9.

Further adding to the previous concept of the direction that society is headed, one of the new major technological advances in our era is Artificial Intelligence. Ideally, we would have liked to be able to implement a machine learning aspect in our program. Instead of constantly running the omega and checking moisture content (when we know it doesn’t need to be watered based on past readings), we would have wanted the program to look at the past readings and determine a pattern (on its own) of these readings. Using that pattern, the Omega would then create its own moisture reading cycle. This would make the system more efficient and reduce the waste of computation power.

Compared to what we wanted the project to do in a perfect world, our system does not have a machine learning component implemented in the design. The reason is because a machine learning complex algorithm is very complex and identifying a classifier type would be very difficult. In the end result, we created a standard smart plant waterer. This is the subset of the initial goal that we were able to achieve.

As stated in our proposal, our project reads moisture from a sensor. Using this data, it computes statistics and writes them in a file. Our product also determines if the plant requires water and if it does, water the plant.

System Design

The design of the system will be split into its hardware components and its software components.

Hardware Components
-       Omega 2
-       Onion Arduino Dock for Omega2
-       Water Pump
-       Moisture Sensor
-       Water Supply
-       Relay Expansion Board
-       Wires
-       6V AA battery Pack

Software Components
In terms of software, the program reads the moisture values from the moisture sensor and writes them in a file every hour. Then, it reads the values from that file and converts that data into integers. After, the program finds the minimum and maximum values of moisture. It also computes the average moisture as well as the standard deviation. Afterwards, theses statistics are written in a file. Finally, based on the average value of moisture, the program determines if the plant requires water and if so, activates the pump to the send water.




