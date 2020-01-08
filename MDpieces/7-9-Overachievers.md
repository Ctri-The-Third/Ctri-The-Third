---
layout : LaserTable
title : Achievement points 
permalink: /7-9/Overachievers
URLPrefix: '/7-9'
Description: "Current Month's ranking of players with the most local achievements:  Funstation Edinburgh"
---



#### {{site.data.7-9-Achievements.ScoreTitle}}

<table class = "ScoreTable">
<tr><th>Player Name</th><th>Local Achievements<br/>Completed </th><th colspan = "2"> Rarest Achievmenent <br/>(others with it)</th> </tr>
{% for Player in site.data.7-9-Achievements.Player %}
<tr><td>{{Player.Name}}</td><td class = "number"> {{Player.AchievementsCompleted}}</td><td class = "number">{{Player.RarestAchievement}}</td><td class = "SmallBrightNumber">{{Player.OthersWith}}</td></tr>
{% endfor %}
</table>

-----

## <small>How does this work?</small>

<small>One of the neat things that LaserForce does is have achievements. You can see individual players achievements on [http://www.iplaylaserforce.com/](http://www.iplaylaserforce.com/). We query the scoreboard, and it tells us two things. </small>
1. <small> it gives us a huge list of all the achievements that the player has visibility of. The same list that shows up when you query your progress on the leaderboard in an arena.
2. <small> it gives us a number marked "Score". We've worked out this number is 1000 points for each completed local **and global** achievement. It also takes your percentage progress to an achievement completion as a fraction of 1000. For example, if I got 99/100 on the achievement to get 100% accuracy, I'll have an 990 extra points in my score, but wont have that achievement completed.

<small>Because of how heavy achievements are on the Laserforce Scoreboard, we keep track of fewer players.  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-9-1234". <br/>
Want excluded? Same as above!</small>