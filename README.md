Final Project Explanation

Overview:
This is a simulated FIFA 2022 Worldcup virtual bracket. The user can go through an infinite number of winning possibilities. Or the user can choose which teams qualify for the bracket and use this program to keep track of the games and scores until the very end where it will keep track of 1st 2nd and 3rd place for them.

CLASSES------------------------------------------------------

Teams class:
Fields for name rank and score of each team with proper getters and setters for each variable.

Group Stage class:
Made  a String array of all 32 teams in the world cup split into 8 groups.
Used Math.Random to choose which 2 teams advance from each group. 
I then printed all the team names vertically onto the “GroupWinners.txt” file. Made it so that each time the class was run, the teams were renewed so that there can be a variety of different outcomes. 

Game Class:
This is where the bulk of the code and inner workings reside. Have fields for game Number, team1 and team2 and a VBox that will hold these two teams and a submit button.
Also have a constructor for each field variable.	
Different very simple return functions that return either team 1 or team 2 based on user score input.
Each match happens in a VBox with each team having its own HBox.
Try catch data validation to make sure user enters integers for scores, allows re-entry until user gets it right.
There are 2 cases, one where the teams tie and one where one team wins. For the tie, the two teams will have a penalty shootout where the user is prompted to re-enter scores for said penalties.
I have an Alert at the end of the program where it displays a new window congratulating the winner and listing the top 3 teams.
The names will display TBD (to be determined) until a team advance to the next round.

GUI class:
GUI class sets up the scene and panels for user interface .
The entire GUI is a borderPane.
There is a VBox on the left side and a huge HBox at the center. 
The huge HBox contains multiple VBoxes. 
Each VBox contains multiple games according to its column position.

Main Class:
Reads in the previously mentioned “Groupwinner.txt” file containing 16 teams. Assigns rating based on numerical order.
---------------------------------------------------------------------------

Challenges:
It really took me a long time and hours upon hours of research and videos to figure out how to do certain things. Incorporating reading in files was hard for me.
Figuring out how to build the GUI was a nightmare. I tried not to rely on scene builder and used a lot of online resources especially for the styling.
It was basically an inception of h boxes and v boxes and border panes.
Figuring out how to display the winners in a new window interacting with the previous window was tough and I have used many online resources to help with that.
Surprisingly enough Styling probably gave me the hardest time and I still am not extremely happy with how it looks style-wise.
I was trying to have a background for the bracket but just couldn’t crack it.


Incorporation:
Have multiple classes, one for teams, one for group stage, one for the games and then of course a main one to run everything. The game class is a composition of the team’s class.
I have it to where when I press run it asks whether I want to run the group stage class which would randomize the teams in the file, or the main class which would run the tournament using the existing teams in said text file.
There are two main GUI windows, one for the tournament where the user will input all the scores and one for the winners display where it congratulates the winner and lists the runner ups. There are minor windows also called “alerts” and those handle all the data validation. Like having a tie breaker for teams with the same score and an error message for non-integer entries for scores.


