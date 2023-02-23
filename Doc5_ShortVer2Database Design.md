User Table:

user_id (integer, primary key)  
name (string)  
email (string)  
date_of_birth (date)  
weight (float)  
height (float)  
medical_conditions_id (integer, foreign key)  
...  
Medical Conditions Table:  
  
medical_condition_id (integer, primary key)  
name (string)  
description (text)  
...  
Activities Table:  

activity_id (integer, primary key)  
name (string)  
type (string)  
intensity_level (integer)  
...  
Foods Table:  
  
food_id (integer, primary key)  
name (string)  
category (string)  
calories (float)  
protein (float)  
carbohydrates (float)  
fats (float)   
...  
Recipes Table:   

recipe_id (integer, primary key)  
name (string)  
preparation_instructions (text)  
...  
Recipe Ingredients Table:  

recipe_ingredient_id (integer, primary key)  
recipe_id (integer, foreign key)  
food_id (integer, foreign key)  
quantity (float)  
...  
Beverages Table:  

beverage_id (integer, primary key)  
name (string)  
volume (float)    
calories (float)  
...   
Sweets Table:  
  
sweet_id (integer, primary key)  
name (string)  
size (string)   
calories (float)  
...  
User Medical Conditions Table:  
  
user_medical_condition_id (integer, primary key)  
user_id (integer, foreign key)  
medical_condition_id (integer, foreign key)   
...   
Nutrient Intake Table:  
  
nutrient_intake_id (integer, primary key)  
user_id (integer, foreign key)  
meal_id (integer, foreign key)  
nutrient_id (integer, foreign key)  
quantity (float)   
...  
User Activities Table:  
  
user_activity_id (integer, primary key)  
user_id (integer, foreign key)   
activity_id (integer, foreign key)  
date (date)  
duration (float)  
...  
User Beverages Table:  
  
user_beverage_id (integer, primary key)  
user_id (integer, foreign key)  
beverage_id (integer, foreign key)  
date (date)  
volume (float)  
...  
User Sweets Table:  
  
user_sweet_id (integer, primary key)  
user_id (integer, foreign key)  
sweet_id (integer, foreign key)  
date (date)  
quantity (float)  
...  
Meal Table:  
   
meal_id (integer, primary key)  
name (string)   
portion_size (float)  
...  
Food Preparation Table:  
  
food_preparation_id (integer, primary key)  
food_id (integer, foreign key)   
cooking_method (string)  
seasonings_or_sauces (text)  
...  
Daily Input Table:   
  
daily_input_id (integer, primary key)  
user_id (integer, foreign key)  
date (date)  
activity_id (integer, foreign key)  
activity_duration (float)  
beverage_id (integer, foreign key)  
beverage_volume (float)  
sweet_id (integer, foreign key)  
sweet_quantity (float)  
meal_id (integer, foreign key)  
meal_portion_size (float)  
...  
Weekly Summary Table:  
  
weekly_summary_id (integer, primary key)  
user_id (integer, foreign key)  
week_number (integer)  
activity_duration_total (float)  
beverage_volume_total (float)  
sweet_quantity_total (float)  
meal_portion_size_total (float)  
...  
User Notification Table:  

user_notification_id (integer, primary key)  
user_id (integer, foreign key)  
notification_date (date)  

![1](https://user-images.githubusercontent.com/124771643/220810545-983d3113-34bf-4387-9b96-eebccd8db006.png)
![2](https://user-images.githubusercontent.com/124771643/220810551-4616fda6-b113-420f-b031-2536f11b502a.png)
![3](https://user-images.githubusercontent.com/124771643/220810563-a322a551-72e6-4417-8dd5-c383806e293c.png)
![4](https://user-images.githubusercontent.com/124771643/220810611-ee7f4b25-de41-44e0-a462-d6a903a9aecc.png)
![5](https://user-images.githubusercontent.com/124771643/220810614-3d433bad-7341-411c-8a5d-489ccf762c84.png)
![6](https://user-images.githubusercontent.com/124771643/220810618-5e030ce0-5e5b-4aca-b080-9966674fa296.png)
![7](https://user-images.githubusercontent.com/124771643/220810620-f97208c6-cda9-455d-b01c-4bcfa1b3b5f4.png)
![8](https://user-images.githubusercontent.com/124771643/220810634-d1bd0ef6-92fe-454e-a21f-ef85cb8ad3ac.png)
