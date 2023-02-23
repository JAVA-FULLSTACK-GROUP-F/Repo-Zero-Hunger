----------------------------------------------------------------------------
Meals today & Cooking method (Raw food types and amount) & Nutrient interactions	
** Ask users how they prepare each food before they cook	
** Ask users what they eat today (portion/how they cook). 
## Variables about meals (tag: VAM )
* Who eats
*	Types of food	 
*	Weight of food	 
*	Types of ingredients	
*	Weight of ingredients	
*	For how many people? (To be reference of weights of food & ingredients PER person)	
*	Portion of every people take 
*	To be filled by user  


## Section about who eats ( tag: SAWE)
One family has different individuals. But individuals are in a group (family).  
1 meal for 1 family = 1 meal for many individuals
Hence, the app should know the nutrients intake of every people, by knowing  [meal of 1 family]
### Variables of individual/who eats:  
* Members of the meal (who eats the meals)  
    
Result:   
Amount and types of nutrients intake by each person  
Interactions among nutrients  

*Many individuals may belong to 1 unit of family. Hence, there may be different accounts for the same meal. Synchronisation is needed for this.   

## Section about food preparation (tag: SAFP )
### Every [same dish] only needed to be asked about [preparation's method] to them [once.] (optional because information can be searched by app through Internet?)	
Because the methods are always the same.	
But the variable can be edited.
Hence, the question at the frontend will be like this:
#  	
Display:	
*	P1:(First time open):	Nice to meet you!(then Next Line= NL) I'm Maria the app assistant	(then Next page= NP)	
**	Make user [tap] the screen to continue [to next page]. For example:	a part of screen [lights up repetitively]. 
*	P2:Maria hopes to ensure your healthiness as accurate as possible (NL) So Maria prepared this section to ensure that Maria understand more about your daily nutrients intake (NP)	 
*	P3: You just need to do ONCE! You may UPDATE this by clicking THIS... (enter instruction/skip instruction)  
*	P4:	(User enter information, app search the database/internet to obtain the nutriton value) 
  
## Section about cooking's method  (tag: SACM ) 
There are different types of cooking method for same raw food.  
  For example: Chicken can be steamed, grilled, baked.... 
So, the food itself can be categorized as:  
## Variables about cooking's method (tag: VACM )  
1) Cooking style: grill, steam, bake  
2) Raw main ingredient:chicken, insects, cow  
3) Portion: 1, 1/2, 1/4 of X [unit: dish/plate/bowl]  
4) How long the dish is cooked for each style 
5) To be filled by user       
    
    
    BY GPT:
CREATE TABLE Meals (  
meal_id INT PRIMARY KEY,  
meal_date DATE,  
meal_type VARCHAR(50),  
meal_weight FLOAT,  
ingredient_type VARCHAR(50),  
ingredient_weight FLOAT,  
number_of_people INT,  
portion FLOAT  
); 
  
CREATE TABLE Food_Preparation (  
food_id INT PRIMARY KEY,  
food_type VARCHAR(50),  
preparation_method VARCHAR(50),  
cooked_time FLOAT  
);  
  
CREATE TABLE Individuals (  
individual_id INT PRIMARY KEY,   
meal_id INT,    
name VARCHAR(50),  
nutrient_intake VARCHAR(50),  
nutrient_interactions VARCHAR(50),   
FOREIGN KEY (meal_id) REFERENCES Meals(meal_id)  
);  
  This creates three tables:  
  
Meals: This table contains information about the meals,   
including their unique ID (meal_id), the date they were eaten (meal_date),  
the type of meal (meal_type),  
the total weight of the meal (meal_weight),  
the type of ingredient (ingredient_type),  
the weight of the ingredient (ingredient_weight),  
the number of people who ate the meal (number_of_people),  
and the portion size (portion).  

Food_Preparation:  
This table contains information about the different types of food and their preparation methods,  
including their unique ID (food_id),  
the type of food (food_type),  
the preparation method (preparation_method),   
and the cooking time (cooked_time).      
  
Individuals:  
This table contains information about the individuals who ate the meal,  
including their unique ID (individual_id),  
the ID of the meal they ate (meal_id),  
their name (name),  
their nutrient intake (nutrient_intake),  
and any nutrient interactions they may have experienced (nutrient_interactions).  
The meal_id column is a foreign key that references the meal_id column in the Meals table.  

![MEALS](https://user-images.githubusercontent.com/124771643/220807910-edcc6aa6-57c7-4ef6-956b-c830ef85c265.png)
