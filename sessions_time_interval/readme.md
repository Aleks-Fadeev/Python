# Determine the time intervals during which the peak load was observed on the site.  
Сonsider the load of the site at some point in time T to be peak, if at that moment the maximum number of user sessions for the entire observation period was opened.
A user session is a continuous period of time during which a user is active on the site. A user session opens at the moment when a user who has come to the site for the first time (or has been absent from the site for a long time) performs any action, for example, loads a page with a product catalog. The session continues as long as the user performs some actions on the site, and closes when a period of time equal to 30 minutes has passed since the last user action - the so—called inactivity period. Each new user action on the site updates the moment of time from which the period of inactivity of the user is counted. If the user performs some action on the site again after the end of the session, this action will open a new session of this user.  

**sessions_time_interval.ipynb** - code  
**data.csv** - data for sessions_time_interval.ipynb
