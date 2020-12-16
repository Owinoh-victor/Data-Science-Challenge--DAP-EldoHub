### Data-Science-Challenge--DAP-EldoHub
This is my solution for the EldoHub DAP data science challenge 

## The Challenge

Consider a dataset providing information on the functionality of infrastructure resources, for each water point it includes the name of the village it is in and its functional state. Implement a data processing module in python which takes a dataset URL as input and returns:
 -	The number of water points that are functional,
 - The number of water points per community,
 - The rank for each community by the percentage of broken water points.
 
 @Dataset URL
 
 Data: https://raw.githubusercontent.com/onaio/ona-tech/master/data/water_points.json
 
 ### MY SOLUTION
 
 # Introduction
 
 As a Data Scientist and AI programmer, you do most of the works on the JSON data. You usually fetch the JSON data from a particular URL and visualizes it. But traversing into a JSON data is always a challenging task especially for beginners.
 
 The full-form of JSON is JavaScript Object Notation. It means that a script (executable) file which is made of text in a programming language, is used to store and transfer the data. Python supports JSON through a built-in package called json. To use this feature, we import the json package in Python script. The text in JSON is done through quoted string which contains value in key-value mapping within . It is similar to the dictionary in Python. JSON shows an API similar to users of Standard Library marshal and pickle modules and Python natively supports JSON features.
 
 -Initially, I use pandas library which provides an inbuilt function (pd.read_json()) to read the json file
 -Then convert the json file into pandas data frame using the function DataFrame (At this point am ready to use my dataset to analysis)
 - The  water point dataset that contains many columns, the relevant ones are:
         -communities villages 
         -water functioning
         
  # 1. Number of Functional Water Point
  
  ![4](https://github.com/Owinoh-victor/Data-Science-Challenge--DAP-EldoHub/blob/main/screenshots/4.JPG)
  functioning           590
  **************************
  
  broken                 40
  
  abandoned              36
  
  newly_constructed      28
  
  under_construction     16
  
  na_dn                   2

NB: 590 Water point are functioning

# 2. Number of Water Points per Community

![1](https://github.com/Owinoh-victor/Data-Science-Challenge--DAP-EldoHub/blob/main/screenshots/1.JPG)

![2](https://github.com/Owinoh-victor/Data-Science-Challenge--DAP-EldoHub/blob/main/screenshots/2.JPG)
                      
                      
  # 3. Community Ranking     
  

![3](https://github.com/Owinoh-victor/Data-Science-Challenge--DAP-EldoHub/blob/main/screenshots/3.JPG)

# 4. Conclusion

High percentage of the water points are functional and few are brocken.

A good number are either abandoned or under construction or newly_constructed

Google Collab  Notebook:  https://colab.research.google.com/drive/1R47uK41R-oqj7dSemaw1baOHSfgov8jT?usp=sharing




