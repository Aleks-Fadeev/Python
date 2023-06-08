# Determine the time intervals during which the peak load was observed on the site.  

**sessions_time_interval.ipynb** - code  
**data.csv** - data for sessions_time_interval.ipynb  

**Task description.**  
Сonsider the load of the site at some point in time T to be peak, if at that moment the maximum number of user sessions for the entire observation period was opened.
A user session is a continuous period of time during which a user is active on the site. A user session opens at the moment when a user who has come to the site for the first time (or has been absent from the site for a long time) performs any action, for example, loads a page with a product catalog. The session continues as long as the user performs some actions on the site, and closes when a period of time equal to 30 minutes has passed since the last user action - the so—called inactivity period. Each new user action on the site updates the moment of time from which the period of inactivity of the user is counted. If the user performs some action on the site again after the end of the session, this action will open a new session of this user.  

**Input**  
File log.txt in the SIM format with a header containing data about the actions performed by users on the site. The data strings have the following format:  
• userid — user ID;  
• timestamp — date and time of the event in ISO format;  
• action — the action performed by the user can take one of the following values:  
  mainpage — login to the main page of the site;  
	search — search for products in the catalog;  
	product — opening a page with a product card;  
	category — opening a page with a category card;  
	cart — the page for adding an item to the cart;  
	checkout — checkout;  
	confirmation — order confirmation;  
• value — the cost of the added product (for the cart event), or the order amount (for the checkout and confirmation events);
• testids — ids of the test samples in which the user is located.F  

**Output**  
The time intervals during which the maximum number of sessions was opened on the site for the entire period of time in the log.tsv file, one on each line.  
Each output line must contain two dates separated by a single space. 
