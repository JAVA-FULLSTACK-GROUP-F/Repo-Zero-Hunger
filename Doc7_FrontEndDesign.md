Doc7_FrontEndDesign (hope you guys make this doc suitable for .md format as possible )
And try to ensure space before and after the words so that it is easy to ctrl-f the word in future.

Non-Public-View Interface Description :  
* Token is injected.  ( action to allow users access app )
* Load-balancing ( to simultaneously handle lots of users )   
* ip or mac address tracking ( to prevent hacking )  
* when suddenly no internet connection , data and app is safe  
* cache in phone  

Public-View Interface Description ( html settings ) :  
All pages :  
* If possible , a single-line-text bar that shows moving text such as interesting trivia is placed on top of app page .  
* Art is comfortable for general society .  
* All users can easily understand what the app is saying .  
* Allow the user to quickly go to another page by tapping the menu bar created inside java programming  ( except for page 1 because user haven’t login )  
    
Public-View Pages :  
Page 0 : Wallpaper
Page 1 : Login ( go to page 2 ) , register ( go to page 2 ) , preview , 
Page 2 : Profile ( Info about users themselves , other account eat same meal )  
Page 3A : Today meals / dishes      
Page 3B :  This week meals / dishes
Page 4 : Food processing / preparation  
Page 5 : Medical record ( include weight … )  
Page 6A : Today Snack & Drinks  
Page 6B : This week Snack & Drinks  
Page 7A : Today Exercise  
Page 7B : This week Exercise  
Final : Result & advice  
Extra : Game reward  
 
# page 0 : Wallpaper   
* First page that opened when the app is opened.    
* Purely to make the app look cool.   

# page 1 ( maybe For once only ) :  
* First page occur after Wallpaper   
* Allow users to roughly experience / preview the app without login / sign up  
 ( less features shown hence less accuracy in result, or data are auto-filled and result is shown quickly )  
* Allows users to click to redirect to register ( sign up ) page  
* Logo is placed on the upper part of the app's page.  
* Allow users login. ( By entering something to prove their identity . After users login, a simple quest to users to increase security ).  
ALSO , the ip or mac address is checked and asks users to check / validate the login if the ip or mac is different from the previous login's address .     
   Method 1: 
   * Users just click to link the Internet ( Google / Microsoft .... ) account with the app itself .  
   
   Method 2:  
   * User enters password (allow password to be auto-filled )  
   * also enters string type input ( allow the string input to be auto-filled )
   * or click pictures to authenticate identity   


Game :  
* prize / award is given if conditions are complied .    

After the user clicks to login from p1 , the user goes to p2 .    
# Page 2 : Profile ( Info about users themselves , other account eat same meal )   
  
Gender  
BirthDate        
Weight         
Height  
Physique type   
Menopause  
Medical_conditions_id :    
Disease type     
Disease severity  
Treatment type  
Treatment type length  
Genetic condition     
Description  

 
