                                                            Design Milestone for Bot
                                                            
BOT OF CHOICE: FocusBot “Help community members be productive”

----Help community members be productive, e.g. recommending open task to worker, or recommending best workers to task

----Help to identify potential players, e.g. “cheap talker[1]”, “collusion[2]”

----Provide productivity aids, such as daily reminders, new task alert, new competitor alert, mute incoming notifications, etc. to a community member.


PROBLEM STATEMENTS:

---- The problem that the FocusBot helps to alleviate is insufficient productivity and focus. It helps the community members be more productive in their work by recommending open tasks to the worker or recommending the best worker to work on a single task. The intention of the bot is to cut down on downtime and tasks that are considered to be “unfocused” and to help improve productivity. This helps save the team time and keeps the members on track to do better work.

BOT DESCRIPTION:

----Our focus bot will help community members be productive, e.g. recommending open tasks to workers, or recommending best workers to task. In addition, it’ll help to identify potential players, e.g. “cheap talker”, “collusion”. Finally, it’ll also provide productivity aids, such as daily reminders, new task alert, new competitor alert, etc. to a community member.
    The bot will both provide analytical reports of user 
    “Do your work, stop being lazy!” - the bot
    
USE CASES:

Use Case 1: Review current task
Precondition: Have a current task selected
Main Flow: User clicks on the current tasks [S1]. User will be given a list of all their current task to choose from [S2]. Bot will display what the current task is and gives more in depth information on it, including other people who have been working on it [S3]. 
Subflows:
[S1] There is a button to click to open the current task if they have one.
[S2] User will be given a list of their current task based on date and also importance with the option to star the important task
[S3] The bot will display the details on the task to the user
Alternative Flows: There is no current task so the user is prompted to select one.

Use Case 2: Set a Daily Reminder
Precondition: None
Main Flow: User goes to the daily reminders to set up a new one[S1]. User will be prompted with a stickies-like interface to write a note [S2]. The bot will display the daily reminder the next day the user starts up their computer [S3]. 
Subflows:
[S1] The user will go to the daily reminders interface where they can choose a recurring reminder or a one time one.
[S2] The user will put in the desired note to remind themselves with.
[S3] The bot will display the data at either a desired time the next day or at startup of the system.
Alternative Flows: [E1] User exits the daily reminder interface. [E2] The user deletes a daily reminder.


DESIGN SKETCHES:


![Capture1115](https://user-images.githubusercontent.com/33581164/77868837-8bdd5880-720a-11ea-8bd6-bbd98d31d9e5.JPG)
![Capture1116](https://user-images.githubusercontent.com/33581164/77868850-9861b100-720a-11ea-99f3-834e4d5b5bb4.JPG)

ARCHITECTURE DESIGN:

![Capture1113](https://user-images.githubusercontent.com/33581164/77868890-b4655280-720a-11ea-8e9f-bdcdf3342c33.JPG)

   For the first diagram the user is of course the person who utilizes the bot. The channel converter connects what the user inputs into the bot. The app services connect the focus bot through the network. Then the channel is going to be Discord where the bot will also be. The bot will utilize a SQL database. Ideally there will also be an application insight to see how the FocusBot is running and detecting efficient usage.

![Capture1114](https://user-images.githubusercontent.com/33581164/77868995-09a16400-720b-11ea-91ed-c83da61dd8c2.JPG)

  The second diagram shows the individual components of the bot. The focus bot can get member data and show member data, this is used for the interaction between the focus bot and the user, which is the community member. The communtiy member can has a username, which is a string and a id, which is also a string. The community member also has loyalty points, which is a double, this helps the focus bot get more people to be productive because it shows how productive other community members have been. The loyalty points can be established from the productivity history of each community member. 
  
  The bot also has an established job, which can show the job role and get the job role. The suggestions part of the diagram is basically what is being displayed to the communty member. The focus bot can display the current job, display the reminder set by the community member, display a to-do list of tasks for the community member, and also display a detailed information on each indivual task.
  
