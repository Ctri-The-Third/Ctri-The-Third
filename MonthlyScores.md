---
layout : none

---



# {{site.data.MonthlyScoreLatest.ScoreTitle}}


<table>
<tr><th>Player Name</th><th>Average Score </th><th> Missions Played</th> </tr>
{% for Player in site.data.MonthlyScoreLatest.Player %}
<tr><td>{{Player.Name}}</td><td>{{Player.AverageScore}}</td><td>{{Player.MissionsPlayed}}</td></tr>
{% endfor %}
</table>

-----

## <small>How does this work?</small>

<small>An individual player games are available from [http://www.iplaylaserforce.com/](http://www.iplaylaserforce.com/). We query the scoreboard, and take note of the last 30 games played (ignoring things we've seen before)<br/> From all the games seen, we can then calculate the average score for a player.</small>

<small><br/> We only regularly check up on players we know about, so if you're new and play a lot, you might be missing!  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-9-1234". <br/>
Want excluded? Same as above!</small>