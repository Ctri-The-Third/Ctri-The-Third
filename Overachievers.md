---
layout : LaserTable

---

[<img src = "{{ "/assets/images/Harbinger_250.png " | relative_url }}" style = "width:90px; float:left; margin-top:-5px;" />]( / )

# {{site.data.AchievementsLatest.ScoreTitle}}
-----

<table>
<tr><th>Player Name</th><th>Achievement<br/> Points </th><th> Achievements<br/>Completed</th> </tr>
{% for Player in site.data.AchievementsLatest.Player %}
<tr><td>{{Player.Name}}</td><td>{{Player.AchievementScore}}</td><td>{{Player.AchievementsCompleted}}</td></tr>
{% endfor %}
</table>

-----

## <small>How does this work?</small>

<small>One of the neat things that LaserForce does is have achievements. You can see individual players achievements on [http://www.iplaylaserforce.com/](http://www.iplaylaserforce.com/). We query the scoreboard, and it tells us two things. </small>
1. <small> it gives us a huge list of all the achievements that the player has visibility of. The same list that shows up when you query your progress on the leaderboard in an arena.
2. <small> it gives us a number marked "Score". We're not exactly sure how this works, and want to do careful experimenting to see if we can figure out if:

   3. <small>Achievements have individual value, or if every achievement is worth the same (e.g. getting the level 6 achieve might be worth more than the level 2 one!)</small>  
   4. <small>if player progress toward an achievement counts (e.g. if I have 99% toward the "100% accuracy" achievement, do I get 99% of the achievement points?) </small>  

<small>Because of how heavy achievements are on the Laserforce Scoreboard, we keep track of fewer players.  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-9-1234". <br/>
Want excluded? Same as above!</small>