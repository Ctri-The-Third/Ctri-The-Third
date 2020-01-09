---
layout : LaserTable
title : Monthly Scores in Standard Games
permalink: /7-8/MonthlyScores
URLPrefix: '/7-8'
Description: "Current Month's average scores for members in Standard Games only:  LaserZone Huddersfield"

---

#### {{site.data.7-8-MonthlyScore.ScoreTitle}}

<table class="ScoreTable" >
<tr><th>Player Name</th><th colspan = "2">Average Score </th><th> Missions Played</th> </tr>
{% for Player in site.data.7-8-MonthlyScore.Player %}
<tr><td>{{Player.Name}}</td><td class = "number"> {{Player.AverageScore}} </td><td class = "SmallBrightNumber">  {{Player.ChangeInScore}} </td><td class = "number"> {{Player.MissionsPlayed}} </td></tr>
{% endfor %}
</table>

-----

## <small>How does this work?</small>

<small>An individual player's games are available from [http://www.iplaylaserforce.com/](http://www.iplaylaserforce.com/). We query the scoreboard, and take note of the last 30 games played (ignoring things we've seen before)<br/> From all the games seen, we can then calculate the average score for a player.</small>

<small>We only regularly check up on players we know about, so if you're new and play a lot, you might be missing!  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-8-1234". <br/>
Want excluded? Same as above!</small>