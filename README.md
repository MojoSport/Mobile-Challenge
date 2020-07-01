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

Build an app that displays and functions as a sports activity timer. The activity timer displays the current activities being performed, the time left on those activities and what activities are next.

### Basic Requirements

1. The UI should display the time left for the current activity that is counting down
1. The UI should display the current activities (eg. name, instructor) that are counting down
1. The UI should display the next activities (eg. name, instructor) to be timed
1. The activity timer can be paused.
2. The activity timer can be unpaused.
3. The activity timer can be stopped. Stopped the timer advances it to the next activity and re-starts the timer. 
1. When the activity timer reaches 0, advance to the next activity and start the countdown timer for that activity.
1. Stopping the current activity advances the timer to the next activity and re-starts the countdown timer.

## Data

Mock json data can be found here ([mock.json](mock.json)) to populate the list of activites.

* The mock data includes an array of **activities**. 
* Each activity should display a countdown timer based on its **durationSeconds**. 
* The activity **order** determines the order activities should be performed. Activities that have the same **order** are to be performed at the same time.
	* If multiple activities have an order of 2, for example, the timer should countdown for the first activity, then the second activity, etc until moving on to order 3 activit(es). This is the equivalent of running multiple activities at the same time and then having players switch groups.

## UI

Here are some example mockups of each potential state. Feel free to use them as a guide. 

| Single Current Activity  | Multiple Current Activities |
| ------------- | ------------- |
| <img src="examples/Single Activity.png" height="500" border="1px solid"> | <img src="examples/Multiple Activities.png" height="500" border="1px solid"> |


| Paused State  | Completed State |
| ------------- | ------------- |
| <img src="examples/Stopped State.png" height="500" border="1px solid">  | <img src="examples/Completed State.png" height="500" border="1px solid">
