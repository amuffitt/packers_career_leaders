# Background

As a Green Bay Packer fan, I'm not only interested in following the team every year but also wanting to learn more about the team's history including both past and current players.  I thought it would be interesting to see the team's career leaders in passing yards, rushing yards, and receiving yards.  However, instead of just looking at a static final list which can easily be seen anywhere, I thought it would be interesting to show the top career leaders as of each year to see how they changed. Watching players visually fall on and off the list as the years progress gives a good historical sense of the team's stars over time, and seeing just how players like Brett Favre ascended and dominated the team record books is pretty dramatic.

Once the data was assembled into an Excel file, the year by year animation was done in Python and  utilized Matplotlib's 'funcanimation' which effectively plays a slideshow of each year's statistical leaders.  

# Dataset

The data came from Packers.com season by season player stats logs (ex: https://www.packers.com/team/stats/2018/REG ) and 'years played' came from various player Internet lookups - mostly ESPN. This info was put into an Excel file for further analysis in both Excel and Python.  There are 3 different files/datasets - passing, rushing, and receiving. All 3 encompass data from the 1930's to 2019 (the last year played at the time of this project).

# Files

**Excel files** - Packers_Top_PassingYds.xlsx, Packers_Top_Rushing Yds.xlsx, and Packers_Top_ReceivingYds.xlsx .  These contain the top 10 players (from a related yards standpoint) for each year.  Columns are Year, Player, Yards, and Years Played.  These are the final 'clean" files.   Prior to this, Excel formulas were used for cumulative yds (although I later learned how to do this in Python using cumsum()) , top 10 utlized Excel Pivot Tables, and adding Years Played in each player column used Vlookup.

**Jupyter Notebook files** - Packers Passing Yards.ipynb, Packers Rushing Yards.ipynb, Packers Receiving Yards.ipynb .  These all show the same basic steps with different data.  At a high level, they involve create a dataframe from the excel file, manipulating that dataframe, showing bar graphs for the top players each year, creating a dynamic color array to ensure each player's bar is a different color (over time), and animating each year as a 'slideshow' using funcanimation in Matplotlib.  

Note: To keep the  Notebook file size lower and ensure easy viewability outside of Jupyter notebook, the animation player code is shown but commented out and replaced with a recorded video gif of the the animation.  

Here are easy-to-view links to each Notebook file in NBViewer:

Packers Passing  https://nbviewer.jupyter.org/github/amuffitt/packers_career_leaders/blob/master/Packers%20Passing%20Yards.ipynb

Packers Rushing https://nbviewer.jupyter.org/github/amuffitt/packers_career_leaders/blob/master/Packers%20Rushing%20Yards.ipynb

Packers Receiving  https://nbviewer.jupyter.org/github/amuffitt/packers_career_leaders/blob/master/Packers%20Receiving%20Yards.ipynb


