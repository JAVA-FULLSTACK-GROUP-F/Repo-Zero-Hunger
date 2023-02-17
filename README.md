#Thought Process-thoughts on how this group-project should be planned & developed
0) Analyse the topic-Zero Hunger, including the meaning & purposes behind Zero Hunger.
1) Select a title 
2) Analyse the title including how zero hunger can be solved through it. 
3) Imagine and determine how frontend should look like. 
4) Present to group on how frontend should be looked like.
5) Analyse the elements/objects that should be included, then build checklist about that
6) Check & confirm how the elements linked together, build logical-algorithm through it.
7) Determine what software features to be used.
8) Determine how the group collaborate
 8A) Determine the elements/variables types and names
 8B) determine the functions/methods to be added
 8C) determine how to implement security and plan to handle crash/software errors
 8D) determine how to add comment/documentation
  8D1) For example, sysout.print the current path at every beginning of a method/class. So that people easy to know where the program stop 
   Like sysout ("pubVC Main.(extend by) pubStrC Eater.M buyOnline"); //pub=public; V=void; C=class; M=method 
  8D2) Put explanations about the flow of the functions
9) Begin to setup files and codings & website, test running...
 9A) Original files/folders should be always kept.
X) Merge the codings/files of project. Then convert it to Android App
X1) Prepare for presentation if somebody dont need to code/do website setup


# Repo-Zero-Hunger

Personal understanding:
(definition: every people able to have edible food)	
 * definition of edible food: things that can be eaten, not poisoning, as clean as possible					
Food supplier: party that get the first-hand/unprocessed food material 
End-users: party that eat the food 

TYPES OF FOOD   TYPES OF FOOD   TYPES OF FOOD   TYPES OF FOOD   TYPES OF FOOD   TYPES OF FOOD   TYPES OF FOOD
/*from GPT:
Food materials can come from a variety of sources, including plants, animals, and fungi. 
Here are some general types of food materials and their origins:

Fruits and Vegetables: These are plant-based foods that come from various parts of the plant, 
including the seeds, roots, stems, leaves, and fruits. 
Some examples include apples, bananas, carrots, spinach, and broccoli.

Grains: Grains are the seeds of various grasses, 
and they are an important source of carbohydrates in many diets. 
Examples include wheat, rice, oats, and barley.

Meat and Poultry: These are animal-based foods that come from the muscle tissue of cows, pigs, chickens, and other animals.

Seafood: Seafood refers to a variety of edible aquatic animals, including fish, shellfish, and crustaceans.

Dairy Products: Dairy products are derived from the milk of cows, goats, sheep, and other animals. Examples include milk, cheese, and yogurt.

Nuts and Seeds: Nuts and seeds are plant-based foods that are high in healthy fats, protein, and fiber. Examples include almonds, cashews, peanuts, and sunflower seeds.

Fungi: Fungi are a separate kingdom of living organisms that include mushrooms, truffles, and yeasts. Some of these are edible and used in cooking.

These food materials can be obtained from a variety of sources, including farms, ranches, fisheries, and wild environments. They can also be processed and packaged into various forms, such as canned or frozen foods, baked goods, and snacks.
 */
/*      METHODS TO HARVEST  METHODS TO HARVEST  METHODS TO HARVEST  METHODS TO HARVEST  METHODS TO HARVEST
The methods used to harvest food materials depend on the type of food and its origin. 
Here are some common ways food materials are harvested:
Fruits and Vegetables: 
Many fruits and vegetables are harvested by (hand), 
often with the help of tools such as (knives, scissors, and clippers.) 
Some crops, such as strawberries, are harvested using special machines that pick the fruit (without damaging it).

Grains: Most grains are harvested using machines such as (combines), which (cut and thresh the grain)
In some cases, grains may be harvested by (hand using sickles or other hand tools).

Meat and Poultry: Livestock such as cows, pigs, and chickens are typically raised on farms and then 
slaughtered for meat. The animals are usually killed using humane methods and the 
meat is then processed and packaged for sale.

Seafood: Seafood can be harvested using a variety of methods, 
including fishing with (nets, traps, and hooks). 
(Aquaculture, or the farming) of fish and other seafood, is also a common method of harvesting seafood.

Dairy Products: Milk from cows, goats, and other animals is typically harvested using 
(specialized equipment that milks) the animals. The milk is then processed into various dairy products 
such as cheese and yogurt.

Nuts and Seeds: Nuts and seeds are often harvested by (hand using tools such as ladders and poles). 
Some crops, such as sunflower seeds, can be harvested using (machines).

Fungi: Mushrooms and other edible fungi are typically grown in a (controlled environment) and harvested (by hand).

In many cases, food materials are harvested using a combination of these methods. 
For example, some crops may be partially harvested by (hand and then finished using machines). 
 */
/* 
(A)Food distribution(process):  (A)Food distribution(process):  (A)Food distribution(process):  (A)Food distribution(process):
1)harvesting, collect and put on vehicles for transportation
2)sorting,grading. 
2)transport the food and then process to prevent makanan rosak (This can include washing, chopping, blanching, canning, freezing, or drying.)
3)the processed food is then packed.
4)the packed food is then put onto the vehicles for further transportation
5)the packed food arrives the retailer/distributors(grocery stores, restaurants, and others)
6)the food is stored in storage site.
7)the food is sold to individuals
8)food is eaten

GPT:
Sorting and Grading: After harvest, many foods are sorted and graded to remove any damaged or defective items. 
This helps ensure that only high-quality food is packaged and sent to market.

Processing: Some foods may be processed after harvest to make them more palatable, 
safe to eat, or easier to store. This can include washing, chopping, blanching, canning, freezing, or drying.

Packaging and Transportation: Once the food is processed, 
it is often packaged in containers suitable for storage and transportation. 
This may include boxes, bags, cans, or other types of packaging. 
The food is then transported to markets and distribution centers.

Retail and Distribution: Food is typically sold through retail stores or distribution centers, 
where it is displayed for customers to purchase. 
This can include grocery stores, restaurants, and other food service establishments.

Preparation and Cooking: When the food is purchased by the consumer, 
it may be prepared and cooked in a variety of ways, depending on the type of food and personal preferences. 
This can include boiling, frying, grilling, baking, or microwaving.

Consumption: Finally, the food is eaten by the consumer. 
During digestion, the nutrients in the food are broken down and absorbed by the body, 
providing energy and nourishment.
(A)Food distribution(process):  (A)Food distribution(process):  (A)Food distribution(process):  (A)Food distribution(process):
 */

 /*
 GPT:   (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C)
how to ensure food safety and quality through 
automated tracking and monitoring of food production and distribution processes.	
1)CCPs, (hazard is identified and controlled before product is shipped)
2)Sensors, REAL-TIME (temperature, humidity, pH, and chemical composition.)
3)Automation:such as ingredient measurement, mixing, and packaging,
4)Using Data Analytics-collect vast amounts of data
5)Tracking and Tracing: track the movement of food products throughout the supply chain, 
from production to distribution to retail. 
6)Regulations: compliance with food safety regulations by monitoring critical parameters and 
providing documentation of compliance efforts.

1)Establishing Critical Control Points (CCPs): 
Critical control points are specific stages 
in the [production process] where [hazards] can be [identified] and [controlled]. 

By establishing CCPs and monitoring them using automated systems, 
food manufacturers can ensure that [potential hazards] are [detected and addressed] [before] the 
final product is [shipped]. 

[Production process][hazards][identified]&[controlled].
[Potential hazards] [detected & addressed] [before] [final product][shipped]. 

2)Using Sensor Technology: Sensors can be used to monitor a wide range of parameters, 
including temperature, humidity, pH, and chemical composition. 
By installing sensors throughout the production and distribution process, 
companies can collect real-time data that can be analyzed to detect potential quality and safety issues.

3)Implementing Automation: Automated systems can help to reduce the risk of human error, 
which is a common cause of food safety and quality issues. 
By automating tasks such as ingredient measurement, mixing, and packaging, companies can ensure that 
products are produced consistently and accurately.

4)Using Data Analytics: Automated systems can collect vast amounts of data, 
which can be analyzed using advanced data analytics techniques to identify trends and patterns. 
By analyzing this data, companies can detect potential issues and take action to prevent them from 
becoming major problems.

5)Tracking and Tracing: Automated systems can be used to 
track the movement of food products throughout the supply chain, 
from production to distribution to retail. 
This allows companies to quickly identify the source of any quality or safety issues and take action to 
address them.

6)Ensuring Compliance: Automated systems can help companies to ensure 
compliance with food safety regulations by monitoring critical parameters and 
providing documentation of compliance efforts.
(C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C) (C)
  */

/*
(D)Food Traceability and Transparency System: A software that tracks the journey of food from farm to table, 
providing transparency and accountability in the food supply chain.		

(E)Food Waste Reduction System: A software that helps reduce food waste by tracking food inventory, 
managing food waste disposal, and monitoring food waste reduction efforts.	
*/
