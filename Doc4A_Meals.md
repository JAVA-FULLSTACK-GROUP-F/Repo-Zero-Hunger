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
*	Other   

## Section about who eats ( tag: SAWE)
One family has different individuals. But individuals are in a group (family).  
1 meal for 1 family = 1 meal for many individuals
Hence, the app should know the nutrients intake of every people, by knowing  [meal of 1 family]
### Variables of individual/who eats:
* Members of the meal (who eats the meals)

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
4) Other: User's clarification  
5) How long the dish is cooked for each style 
6) Other by user     
  
