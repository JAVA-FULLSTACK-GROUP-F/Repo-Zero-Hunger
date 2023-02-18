# BY ChatGPT	
Doc5_Database Design.md:	

Database Design for Nutritional Monitoring and Tracking System	
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
