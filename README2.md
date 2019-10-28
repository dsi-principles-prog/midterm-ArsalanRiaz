# UFC Data 

## Data Overview and Source

The UFC data is the list of every UFC fighter in the histroy of the organisation from 1993 to 2019. 

Each row contains the information about both fighters, fight details and the winner.

Each row include stats on the daemage done by the red fighter and the dameage done by the opponent of th red fighter.

The same is included for the blue fighter.

It includes all the stats from the previous fights but excludes the stats of the current fight

##### Data Source

The dataset is taken from the kaggle webiste.

Link: https://www.kaggle.com/rajeevw/ufcdata


## Identified Problem

We need to predict the fighter in which corner i.e. blue or red will win the fight. Since we have the all the stats of both

fighters excluding the current fight stats. Therefore, we can easily predict by using the variables in order to know which fighter will win

## Content


Each row is a compilation of both fighter stats. Fighters are represented by 'red' and 'blue' (for red and blue corner). So for instance, red fighter has the complied average stats of all the fights except the current one. The stats include damage done by the red fighter on the opponent and the damage done by the opponent on the fighter (represented by 'opp' in the columns) in all the fights this particular red fighter has had, except this one as it has not occured yet (in the data). Same information exists for blue fighter. The target variable is 'Winner' which is the only column that tells you what happened. Here are some column definitions:

## Column definitions:
R_ and B_ prefix signifies red and blue corner fighter stats respectively
_opp_ containing columns is the average of damage done by the opponent on the fighter
KD is number of knockdowns
SIG_STR is no. of significant strikes 'landed of attempted'
SIG_STR_pct is significant strikes percentage
TOTAL_STR is total strikes 'landed of attempted'
TD is no. of takedowns
TD_pct is takedown percentages
SUB_ATT is no. of submission attempts
PASS is no. times the guard was passed?
REV ???
HEAD is no. of significant strinks to the head 'landed of attempted'
BODY is no. of significant strikes to the body 'landed of attempted'
CLINCH is no. of significant strikes in the clinch 'landed of attempted'
GROUND is no. of significant strikes on the ground 'landed of attempted'
win_by is method of win
last_round is last round of the fight (ex. if it was a KO in 1st, then this will be 1)
last_round_time is when the fight ended in the last round
Format is the format of the fight (3 rounds, 5 rounds etc.)
Referee is the name of the Ref
date is the date of the fight
location is the location in which the event took place
Fight_type is which weight class and whether it's a title bout or not
Winner is the winner of the fight
Stance is the stance of the fighter (orthodox, southpaw, etc.)
Height_cms is the height in centimeter
Reach_cms is the reach of the fighter (arm span) in centimeter
Weight_lbs is the weight of the fighter in pounds (lbs)
age is the age of the fighter
title_bout Boolean value of whether it is title fight or not
weight_class is which weight class the fight is in (Bantamweight, heavyweight, Women's flyweight, etc.)
no_of_rounds is the number of rounds the fight was scheduled for
current_lose_streak is the count of current concurrent losses of the fighter
current_win_streak is the count of current concurrent wins of the fighter
draw is the number of draws in the fighter's ufc career
wins is the number of wins in the fighter's ufc career
losses is the number of losses in the fighter's ufc career
total_rounds_fought is the average of total rounds fought by the fighter
total_time_fought(seconds) is the count of total time spent fighting in seconds
total_title_bouts is the total number of title bouts taken part in by the fighter
win_by_Decision_Majority is the number of wins by majority judges decision in the fighter's ufc career
win_by_Decision_Split is the number of wins by split judges decision in the fighter's ufc career
win_by_Decision_Unanimous is the number of wins by unanimous judges decision in the fighter's ufc career
win_by_KO/TKO is the number of wins by knockout in the fighter's ufc career
win_by_Submission is the number of wins by submission in the fighter's ufc career
win_by_TKO_Doctor_Stoppage is the number of wins by doctor stoppage in the fighter's ufc career
Acknowledgements
Inspiration: https://github.com/Hitkul/UFC_Fight_Prediction Provided ideas on how to store per fight data. Unfortunately, the entire UFC website and fightmetric website changed so couldn't reuse any of the code.

Print Progress Bar: https://gist.github.com/aubricus/f91fb55dc6ba5557fbab06119420dd6a To display progress of how much download is complete in the terminal

# The Project contains three files. 

## Order to run

1. 10 - Import This file contains the import, tidy and cleaning and explore

2. 20 - Feature Engineering - Contains two functions 

3. 40 - Modelling, this is a pipelining functions from the df. Them select and passing it on the augmented df.
