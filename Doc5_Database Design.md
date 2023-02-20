# BY CHATGPT  

sql  
Copy code  
-- Create Users table  
CREATE TABLE Users (  
  user_id INT PRIMARY KEY,  
  username VARCHAR(50),
  password VARCHAR(50),
  gender VARCHAR(10),
  age INT,
  height FLOAT,
  weight FLOAT
);

-- Create Meals table
CREATE TABLE Meals (
  meal_id INT PRIMARY KEY,
  meal_name VARCHAR(50),
  user_id INT,
  FOREIGN KEY (user_id) REFERENCES Users(user_id)
);

-- Create Meal Details table
CREATE TABLE Meal_Details (
  meal_detail_id INT PRIMARY KEY,
  meal_id INT,
  recipe_id INT,
  portion FLOAT,
  FOREIGN KEY (meal_id) REFERENCES Meals(meal_id),
  FOREIGN KEY (recipe_id) REFERENCES Recipes(recipe_id)
);

-- Create Meal Type Details table
CREATE TABLE Meal_Type_Details (
  meal_type_detail_id INT PRIMARY KEY,
  user_id INT,
  meal_type VARCHAR(50),
  calories INT,
  protein FLOAT,
  carbs FLOAT,
  fat FLOAT,
  FOREIGN KEY (user_id) REFERENCES Users(user_id)
);

-- Create Supplements table
CREATE TABLE Supplements (
  supplement_id INT PRIMARY KEY,
  supplement_name VARCHAR(50),
  calories INT,
  protein FLOAT,
  carbs FLOAT,
  fat FLOAT
);

-- Create Recipes table
CREATE TABLE Recipes (
  recipe_id INT PRIMARY KEY,
  recipe_name VARCHAR(50),
  calories INT,
  protein FLOAT,
  carbs FLOAT,
  fat FLOAT
);

-- Create Diary table
CREATE TABLE Diary (
  diary_id INT PRIMARY KEY,
  user_id INT,
  date DATE,
  water INT,
  sweets INT,
  FOREIGN KEY (user_id) REFERENCES Users(user_id)
);

-- Create Activity table
CREATE TABLE Activity (
  activity_id INT PRIMARY KEY,
  user_id INT,
  activity_name VARCHAR(50),
  time FLOAT,
  FOREIGN KEY (user_id) REFERENCES Users(user_id)
);


Assuming that we want to use the daily data as the primary data source, but the weekly data can be used to fill in the gaps where the daily data is missing, we can modify the Diary table to include both daily and weekly data, and add a flag to indicate which one is being used:

sql
Copy code
-- Modify Diary table to include daily and weekly data
ALTER TABLE Diary
ADD daily_water INT,
ADD daily_sweets INT,
ADD daily_activity_time FLOAT,
ADD weekly_water INT,
ADD weekly_sweets INT,
ADD weekly_activity_time FLOAT,
ADD is_daily_data BOOLEAN;

-- Set default value for is_daily_data to true
ALTER TABLE Diary
ALTER COLUMN is_daily_data SET DEFAULT true;


To insert data into the Diary table, we can set the is_daily_data flag to true for daily data, and false for weekly data:

sql
Copy code
-- Insert daily data for user 1 on 2023-02-20
INSERT INTO Diary (user_id, date, water, sweets, daily_water, daily_sweets, is_daily_data)
VALUES (1, '2023-02-20', 1500, 50, 1500, 50, true);

-- Insert weekly data for user 1 for week ending on 2023-02-20
INSERT INTO Diary (user_id, date, water, sweets, weekly_water, weekly_sweets, is_daily_data)
VALUES (1, '2023-02-20', 10000, 250, 10000, 250, false);


To calculate the weekly data based on the daily data, we can use a query like this:

sql
Copy code
-- Calculate weekly water consumption for user 1
SELECT user_id, DATE_TRUNC
