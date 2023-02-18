# BY ChatGPT	
Doc5_Database Design.md:	
![MT](https://user-images.githubusercontent.com/124771643/219880436-4145cfba-3074-49c3-a3f8-8852caf073d4.png)
![MDT](https://user-images.githubusercontent.com/124771643/219880470-13879afd-3d3d-4990-b0e7-b0eba090d73f.png)
![FT](https://user-images.githubusercontent.com/124771643/219880489-77710497-9173-4ece-866f-69e148e701e2.png)
![MTT](https://user-images.githubusercontent.com/124771643/219881024-3c819667-e2a7-49d0-b0d1-c16e452d519e.png)
![DT](https://user-images.githubusercontent.com/124771643/219881026-9d34f43c-4675-4c53-967c-6b77154fb7a1.png)
![RT](https://user-images.githubusercontent.com/124771643/219880968-61fc66b8-2572-4b63-bf5e-527e49f7ecf2.png)
![ST](https://user-images.githubusercontent.com/124771643/219880970-94a8297a-7515-4d54-9d38-de1d9f9763c6.png)
![NT](https://user-images.githubusercontent.com/124771643/219880972-68a2f181-90a3-42d6-af7f-633a57a91b12.png)
![GT](https://user-images.githubusercontent.com/124771643/219880976-db28f088-5be0-42f0-b42b-0c7fdf51a920.png)
![AT](https://user-images.githubusercontent.com/124771643/219880980-9a996c2d-7476-4be8-a036-5b7899bd6ce9.png)
![UT](https://user-images.githubusercontent.com/124771643/219881128-3ecf6939-a27a-4282-94f0-b4ae4e3184da.png)


## Database Design for Nutritional Monitoring and Tracking System	
Tables	
	Users Table (UT)	
Column Name	Data Type	Description	
user_id	int	Unique identifier for the user	
username	varchar(255)	User's username	
password	varchar(255)	User's password	
email	varchar(255)	User's email	
date_of_birth	date	User's date of birth	
biological_gender	varchar(10)	User's biological gender	
height	float	User's height	
weight	float	User's weight	
body_fat	float	User's body fat percentage	
body_type	varchar(20)	User's body type (e.g. lean, muscular)	
genetic_condition	varchar(255)	User's genetic condition	
created_at	datetime	Timestamp of when the user's account was created	
updated_at	datetime	Timestamp of when the user's account was last updated	
	Meals Table (MT)	
Column Name	Data Type	Description	
meal_id	int	Unique identifier for the meal	
user_id	int	Foreign key referencing the user who consumed the meal	
date	date	Date when the meal was consumed	
total_calories	float	Total calories of the meal	
total_fat	float	Total fat of the meal	
total_protein	float	Total protein of the meal	
total_carbohydrates	float	Total carbohydrates of the meal	
created_at	datetime	Timestamp of when the meal was added	
updated_at	datetime	Timestamp of when the meal was last updated	
	Meal Details Table (MDT)	
Column Name	Data Type	Description	
meal_detail_id	int	Unique identifier for the meal detail	
meal_id	int	Foreign key referencing the meal the detail belongs to	
food_id	int	Foreign key referencing the food consumed in the meal	
serving_size	float	The serving size of the food consumed in the meal	
calories	float	Calories of the food consumed in the meal	
fat	float	Fat of the food consumed in the meal	
protein	float	Protein of the food consumed in the meal	
carbohydrates	float	Carbohydrates of the food consumed in the meal	
created_at	datetime	Timestamp of when the meal detail was added	
updated_at	datetime	Timestamp of when the meal detail was last updated	
	Foods Table (FT)	
Column Name	Data Type	Description	
food_id	int	Unique identifier for the food	
name	varchar(255)	Name of the food	
serving_size	float	Serving size of the food	
calories	float	Calories of the food	
fat	float	Fat of the food	
protein	float	Protein of the food	
carbohydrates	float	Carbohydrates of the food	
created_at	datetime	Timestamp of when the food was added	
updated_at	datetime	Timestamp of when the food was last updated	
	Meal Types Table (MTT)	
Column Name	Data Type	Description	
meal_type_id	int	Unique identifier for the meal type	
name	varchar(255)	Name of the meal type	
created_at	datetime	Timestamp of when the meal type was added	
updated_at	datetime	Timestamp of when the meal type was last updated			
	Meal Type Details Table (MTDT)	
Column Name	Data Type	Description		
allergens	text	A comma-separated list of common allergens contained in the meal type, such as "milk, eggs, soy, wheat, nuts, etc."	
calories	integer	The number of calories in the meal type.	
price	decimal	The price of the meal type in the local currency.	
created_at	datetime	The date and time when the meal type was added to the system.	
updated_at	datetime	The date and time when the meal type was last updated in the system.	

Note: The created_at and updated_at columns are commonly used in database systems to keep track of when a record was created and last updated. They can be useful for auditing and troubleshooting purposes.

Activity Table (AT)
Column Name Data Type Description
activity_id int Unique identifier for the activity
user_id int Foreign key referencing the user who performed the activity
activity_name varchar(255) Name of the activity
date date Date when the activity was performed
time time Time when the activity was performed
duration float Duration of the activity in minutes
calories_burned float Calories burned during the activity

Goals Table (GT)
Column Name Data Type Description
goal_id int Unique identifier for the goal
user_id int Foreign key referencing the user who set the goal
goal_type varchar(255) Type of the goal (e.g. weight loss, muscle gain)
start_date date Start date of the goal
target_date date Target date to achieve the goal
target_value float Target value for the goal

Nutrients Table (NT)
Column Name Data Type Description
nutrient_id int Unique identifier for the nutrient
food_id int Foreign key referencing the food the nutrient is associated with
nutrient_name varchar(255) Name of the nutrient
serving_size float Serving size of the food in grams
amount_per_serving float Amount of the nutrient per serving in milligrams

Supplements Table (ST)
Column Name Data Type Description
supplement_id int Unique identifier for the supplement
user_id int Foreign key referencing the user who takes the supplement
supplement_name varchar(255) Name of the supplement
dosage float Dosage of the supplement
frequency varchar(20) Frequency of use (e.g. daily, weekly)

Recipes Table (RT)
Column Name Data Type Description
recipe_id int Unique identifier for the recipe
user_id int Foreign key referencing the user who created the recipe
recipe_name varchar(255) Name of the recipe
ingredients text Ingredients of the recipe
instructions text Instructions for making the recipe
total_calories float Total calories of the recipe
total_fat float Total fat of the recipe
total_protein float Total protein of the recipe
total_carbohydrates float Total carbohydrates of the recipe

Diary Table (DT)
Column Name Data Type Description
diary_id int Unique identifier for the diary entry
user_id int Foreign key referencing the user who made the entry
date date Date of the diary entry
meal_entries text Entries for meals consumed during the day
activity_entries text Entries for activities performed during the day
supplement_entries text Entries for supplements taken during the day
notes text Additional notes for the day



