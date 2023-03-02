# Variables= (must/optional) + (update oftenly/weekly/once)  
----------------------------------------------------------------------------
Meals today & Cooking method (Raw food types and amount) & Nutrient interactions	
** Ask users how they prepare each food before they cook	
** Ask users what they eat today (portion/how they cook). 

----------------------------------------------------------------------------
Medical conditions and medications,Age and life stage.  [USER CONDITION]
** Age, weight, height (short/normal/tall/cm/ft), body physique (little/standard/heavily/very----fat/lean/muscular/thin) 
** Genetic condition (optional) 

----------------------------------------------------------------------------
Lifestyle (how often you exercise)	
** ask how often and what beverages they drink	
** ask how and how often they exercise/ do heavy physical activity	
** ask do they cannot sleep oftenly	
** ask them about how often they eat sweets/cookies outside meals.

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
*	P2:Maria hopes to ensure your healthiness as accurate as possible (NL) So Maria prepared this section to ensure that Maria understand more about your nutrients intake (NP)	 
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
4) To be filled by user (optional)  
5) How long the dish is cooked for each style    
  
----------------------------------------------------------------------------
Medical conditions and medications,Age and life stage.  
** Age, weight, height (short/normal/tall/cm/ft), body physique ([little/standard/heavily/very]----[fat/lean/muscular])  
** Genetic condition (optional)    

##  Section about medical conditions, medical treatment , age, life stage (User condition)( Tag: SAUC )    
## Variables about users' medical condition (tag: VAUC )  
1) Birth Date=(age+life stage ): Enter once, update every year 
2) Age Now ( Update every year )
3) Life stage ( infant , child , .... ) 
4) Medicines / medical treatment taking  
  * Amount of medicine , time length, type of treatment    
5) Diseases: 
  * Types: Sleeping problem...  
  * Level: X times per X  [unit: days/weeks/months ] 
6) Menopause? 
7) Biological gender  
8) Weight 
9) Height(short/normal/tall/cm/ft)   
10) Body physique (little/standard/heavily/very----fat/lean/muscular)  
11) Genetic condition 
12) To be filled by user (optional)

----------------------------------------------------------------------------
Lifestyle (how often you exercise)	
** ask how often and what beverages they drink	
** ask how and how often they exercise/ do heavy physical activity	
** ask them about how often they eat sweets/cookies outside meals.  

##  Section about Lifestyle( Tag: SAL ) 
For physical activities, the level of it might be different daily.  
Hence, the app might needs to have versions of Daily vs Regularly   
## Variables about Lifestyle(tag: VAL ) 
Regularly / weekly version:  
1)Drinkings:  
  * Drinked beverages' types 
  * Volume of drinked beverage: whole/half/1/4 of  X [unit: tin or (X milli-liter) ] 
  * How often drinking the beverages (update weekly) 
  * To be filled by user (optional)
2) Physical activities:   
  * Types of physical activities: Yoga/Exercise:back-muscle...abs...leg /carry loads  
  * Level/weights of the activity: X of  [unit:kg/pounds]  
  * Time length per 1 continous activity: X [unit:hours+ X minutes ] 
  * Total time length doing the activity: X  [unit:hours/day/week/month/year/decade]  
  * To be filled by user (optional)
3)  Sweets & snacks outside meals 
  * Types 
  * Size 
  * Volume: whole/half/1/4 of X  [unit: pieces]  
  * How often eating: X times per X days/weeks/months  (update weekly) 
  * To be filled by user (optional)
________________________________________________________________________
Daily version:  
1)Drinkings:   
  * Drinked beverages' types 
  * Volume of drinked beverage: whole/half/1/4 of  X [unit: tin or (X milli-liter) ] 
  * To be filled by user (optional)
2) Physical activities:   
  * Types of physical activities: Yoga/Exercise:back-muscle...abs...leg /carry loads  
  * Level/weights of the activity: X of  [unit:kg/pounds]  
  * Time length per 1 continous activity: X [unit:hours, X minutes ] 
  * Total time length doing the activity:  [unit:X  hours, Y minutes]  
  * To be filled by user (optional)
3)  Sweets & snacks outside meals 
  * Types 
  * Size 
  * Volume: whole/half/1/4 of X  [unit: pieces]  
  * To be filled by user (optional)  

________________________________________________________________________  
Section about User's ACCOUNT Profile ( FOR ACCOUNT LOGIN & REGISTRATION & As secured PROFILE ) (SAAP)
1) account name  
2) account password  
3) email address  
4) phone number  
5) 2nd phone number ( optional for user to input )  
6) Meal members ( let users choose 0 or more accounts as members who dine together )  
7) Current region ( confirm ip / mac address for anti-hacking )
 _______________________________________________________________________  

Weekly same type physical activities = sum of time length of same type physical activities in daily version.  
Weekly volume of drinked beverages= sum of volume of drinked beverages in daily version.  
Weekly volume of eaten sweets/cookies= sum of volume of eaten sweets/cookies in daily version.  
1 dish of meal= sum of portion of 1 dish per meal eaten by each group of table_member  
____________________________________________________    
Since weekly version exists, user's input in daily version is optional. Just that daily version provides more accurate data.  
If [sum of daily version's data values] != [weekly version's data value], [daily version's data values] has higher priority.  
App will notify users that the data values of betwen two versions is different.   	

( OPTIONAL FIELDS )  
1) DAILY VERSIONS' DATA  
2) PREPARE FOODS' METHOD
3) MEDICAL CONDITIONS & treatments
4) Snacks & Sweets outside meals  

USERS ALLOWED TO EDIT THEIR DATA / PROFILE INCLUDING PASSWORD AFTER authentication . Edit in profile could affect the status of the other accounts who dine together so that  nutrients intake per account in the same group is updated automatically . 
