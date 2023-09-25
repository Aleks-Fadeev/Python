# Prediction dealers revenue.

**prediction.ipynb** - code  

**Task description.**  
The telecom operator sells a certain number of SIM cards to partner companies (dealers) on a monthly basis.    
Dealers sell SIM cards to users.    
Depending on the users' expenses, the dealer's remuneration is calculated:
- if the user has not entered personal data, the reward accumulates in potential; 
- if the user spent less money than the initial balance, the reward is entered into the potential from the initial balance; if the user spent more money than the initial balance, but less than the "threshold", the reward is paid from the difference between the total expenses and the initial balance; 
- if the user has spent more money than the "threshold" - the reward is paid as a percentage of spending per month, the potential and potential from the initial balance are added.

Each dealer and tariff group has its own monitoring period (the period during which remuneration payments are made). 
