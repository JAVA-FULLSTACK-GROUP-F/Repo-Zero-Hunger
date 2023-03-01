The combined list of database tables would include:  

User Table - This table would store information about each user, such as their name, email address, password, age now, date of birth and phone no.  

Meal Table - This table would store information about each meal, including the date and time it was consumed, the user who consumed it, and any notes about the meal (such as where it was consumed or who prepared it).  

Food Table - This table would store information about each food item, such as its name, category (e.g. protein, carbohydrate, fat), and nutritional information (calories, macronutrients, micronutrients).  

Recipe Table - This table would store information about each recipe, including its name, list of ingredients (which would link to the Food table), and preparation instructions.  

FoodPreparation Table - This table would store information about how each food item was prepared, including the cooking method and any seasonings or sauces used.  

Activity Table - This table would store information about each physical activity, including its name, type (e.g. cardio, strength training), and intensity level.  

Beverage Table - This table would store information about each beverage consumed, including its name, volume, and any additional ingredients (such as sugar or cream).  
  
Sweet/Cookie Table - This table would store information about each sweet or dessert consumed, including its name, size, and ingredients.  

MedicalConditions Table - This table would store information about any medical conditions or allergies that a user has, as well as any medications they are taking.   
condition_id (primary key)  
user_id (foreign key)  
condition_name  
severity (mild, moderate, severe)  
medication (optional)
weight
height
body physique
notes (optional)  
  
NutrientIntake Table - This table would store information about the nutrient intake for each meal, including the user who consumed the meal, the date and time of the meal, and the amounts of each nutrient consumed.  

UserActivity Table - This table would store information about the physical activities performed by each user, including the type, intensity level, and duration of each activity.  

UserBeverage Table - This table would store information about the beverages consumed by each user, including the type, volume, and frequency of consumption.  

UserSweet/Cookie Table - This table would store information about the sweets and desserts consumed by each user, including the type, size, and frequency of consumption.  

DailyInput Table - This table would store the user's daily input, including the date, the amount of time spent on each physical activity, the volume of each beverage consumed, the volume of each sweet/cookie consumed, and the portion size of each meal consumed.  

WeeklySummary Table - This table would store the user's weekly summary, including the week number, the total time spent on each physical activity, the total volume of each beverage consumed, the total volume of each sweet/cookie consumed, and the total portion size of each meal consumed.  

UserNotification Table - This table would store the notifications that the app sends to the user regarding any discrepancies between the daily input and weekly summary data values. It would include the date, the notification message, and a flag indicating whether the user has acknowledged the notification.    
  
build table considering that by knowing the conditions and activities of user, app analyse that and give advise about how food/nutrients should be intake by ysers
Based on the information you provided, I would suggest adding the following table to the database:  

NutrientAdvice: This table would store information about the recommended nutrient intake for each user, based on their medical conditions and physical activities. It would include fields such as the user ID, the date, the recommended calorie intake, and recommended daily amounts of each nutrient (e.g. protein, carbohydrates, fats, vitamins, minerals). The table could also include additional fields for tracking the user's progress towards meeting these recommendations over time.  

This table would be updated based on the user's input and any changes to their medical conditions or physical activities. The app could then use this information to provide personalized nutrition advice to the user, including recommendations for foods that are high in the nutrients they need and suggestions for meals and recipes that meet their specific dietary needs.  

By integrating this table into the app, users would have access to tailored nutrition advice that takes into account their unique health needs and lifestyle habits. This could help them to make more informed food choices and achieve their health and wellness goals more effectively.    
