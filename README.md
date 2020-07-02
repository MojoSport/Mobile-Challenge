## MOJO's Quick Android Coding Challenge

Hi there! Here is a coding exercise to help us assess your technical skills. Please plan to spend no more than **2 hours** on this. We understand we may not be the only company asking for an exercise from you and want to be respectful of your time.

After 2 hours, please feel free to stop working. Explain what refactors, code organization, and/or enhancements you would have made with more time in the SOLUTION.md file.

If you have any questions at any point, please reach us via email.

## Submission
Please **clone** or **download** this repository and commit all your changes to a repository that can be shared with us. When you're done, send us an email with a link to your repository URL. We'll schedule a call to review your solution.

## Task

1. Clone or download this repository.
2. Create a *source* directory for your code.
3. In the *source* directory, please create an Android app that accomplishes the technical spec below.
4. Commit and Push your code to your repository.
5. Send us an email with a link to your respository URL.

# Technical spec
_____________

Build an app that displays and functions as a sports activity timer. The activity timer will be used by a sports coach to manage their practice so they know what activity (drill) is running and when the next activity(ies) start. The activity timer displays the current activities being performed, the time left on those activities and what activities are next. 

### Basic Requirements

1. The UI should display the time left for the current activity(ies) counting down.
1. The UI should display the current activity(ies) (eg. name, instructor) counting down.
1. The UI should display the next activity(ies) (eg. name, instructor) that will be up next.
1. The activity timer can be paused.
2. The activity timer can be unpaused.
3. The activity timer can be stopped. Stopping the timer should advance it to the next activity(ies) and re-start the timer. 
1. When the activity timer reaches 0, advance to the next activity(ies) and start the countdown timer for the next activity(ies).

## Data

Mock json data can be found here ([mock.json](mock.json)) to populate the list of activites.

* The mock data includes an array of **activities**. 
* Each activity should display a countdown timer based on its **durationSeconds**. 
* The activity **order** determines the order activities should be performed. 
* Activities that have the same **order** (and **durationSeconds**) are to be performed at the same time.
	*  This happens when a subset of players at practice perform one activity while another subset perform another activity simultaneously. At the end of the **durationSeconds**, the players switch activities before moving on to the next **order** in the **activities** array.
	*  For example, if multiple activities have an **order** of **2**, the timer would count down for **durationSeconds**, the players would switch activities and the timer would count down for **durationSeconds** again.

	

## UI

Here are some example mockups of each potential state. Feel free to use them as a guide. 

| Single Current Activity  | Multiple Current Activities |
| ------------- | ------------- |
| <img src="examples/Single Activity.png" height="500" border="1px solid"> | <img src="examples/Multiple Activities.png" height="500" border="1px solid"> |


| Paused State  | Completed State |
| ------------- | ------------- |
| <img src="examples/Stopped State.png" height="500" border="1px solid">  | <img src="examples/Completed State.png" height="500" border="1px solid">
