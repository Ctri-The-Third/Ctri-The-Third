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