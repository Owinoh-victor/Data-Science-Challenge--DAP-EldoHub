### Data-Science-Challenge--DAP-EldoHub
This is my solution for the EldoHub DAP data science challenge 

##The Challenge

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
  
  functioning           590
  **************************
  broken                 40
  abandoned              36
  newly_constructed      28
  under_construction     16
  na_dn                   2

NB: 590 Water point are functioning

# 2. Number of Water Points per Community

communities_villages  water_point_condition

************************************************************


Abanyeri              functioning               3
                      newly_constructed         1
                      ***************************************
                      
Akpari-yeri           functioning               3
                       ***************************************
                       
Alavanyo              functioning               2
                      abandoned                 1
                       ***************************************
                       
Arigu                 functioning               6
                      abandoned                 4
                      broken                    2
                       ***************************************
                       
                     
Badomsa               functioning              26
                      newly_constructed         1
                       ***************************************
                       
Bandem                functioning               4
                      broken                    2
                      newly_constructed         1
                       ***************************************
                       
Banyangsa             functioning               8
                      broken                    1
                      na_dn                     1
                       ***************************************
                       
                       
Bechinsa              functioning              26
Chanpolinsa           functioning               4
Chansa                functioning               9
Chondema              functioning               4
Dibisi                functioning               2
Dorinsa               functioning              13
                      newly_constructed         3
                      under_construction        1
                       ***************************************
                       
Fiisa                 functioning               5
Gaadem                functioning               2
Garigu                functioning               1
Gbaarigu              broken                    2
                      functioning               2
                      abandoned                 1
                      ***************************************
                      
Soo                   under_construction        1
Suik                  functioning               1
Tankangsa             functioning               4
                      newly_constructed         2
                       ***************************************
                       
                       
Tantala               functioning              16
                      abandoned                 4
                      broken                    1
                      under_construction        1
                       ***************************************
                       
Tuisa                 functioning               4
Vundema               functioning               3
                      broken                    2
Zangu-Vuga            functioning              10
                      abandoned                 3
Zanwara               functioning               6
                      broken                    2
                      abandoned                 1
                      under_construction        1
                       ***************************************
                       
Zogsa                 functioning               5
                      broken                    1
Zua                   functioning              20
                      abandoned                 4
                      under_construction        2
                      na_dn                     1
                      newly_constructed         1
                       ***************************************
                       
Zuedema               functioning              18
Zukpeni               abandoned                 3
                      functioning               2
                      broken                    1
                       ***************************************
                       
Zundem                functioning              29
                      under_construction        1
                      
                      
  # 3. Community Ranking     
  









