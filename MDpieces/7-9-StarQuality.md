---
layout : LaserTable
title : Monthly Star Quality 
permalink: /7-9/StarQuality
URLPrefix: '/7-9'


---

#### {{site.data.7-9-StarQuality.ScoreTitle}}

<table class = "ScoreTable">
<tr><th>Player Name</th><th colspan = "2">Star Quality<br/>per game </th><th> Total Star<br/>Quality</th> <th style = "padding-left:30px;"  colspan = "2">Average<br/>Players</th><th  colspan = "2">Average<br/> Rank</th><th>Games <br/>Played</th></tr>
{% for Player in site.data.7-9-StarQuality.Player %}
<tr onclick = "showBreakdown({{Player.JSID}})" >
<td class = "clickable">{{Player.Name}}</td><td class = "number">{{Player.StarQualityPerGame}}</td><td class = "SmallBrightNumber"> {{Player.ChangeInSQPerGame}} </td><td class = "number">{{Player.TotalStarQuality}}</td><td style = "padding-left:30px;" class = "number">{{Player.AverageOpponents}}</td><td class = "SmallBrightNumber"> {{Player.ChangeInPlayers}}</td><td class = "number">{{Player.AverageRank}}</td><td class = "SmallBrightNumber"> {{Player.ChangeInRank}}</td><td class = "number">{{Player.gamesPlayed}}</td>
</tr>
{% endfor %}
</table>

Click a player's name to see where they got their stars from!
{% for Player in site.data.7-9-StarQuality.Player %}
<div id = "Breakdown_{{Player.JSID}}" class = "breakdownDiv">
<h2>Breakdown for {{Player.Name}}</h2>

<table> 
    <tr>
        <th>Game Name</th><th>rank</th><th>players</th><th>stars</th>
    </tr>
    {% for BreakdownGame in Player.breakdown %}
    <tr>
        <td>{{BreakdownGame.gameName}}</td>
        <td><center> {{BreakdownGame.rank}} </center></td>
        <td><center> {{BreakdownGame.totalPlayers}} </center></td>
        <td><center> {{BreakdownGame.starsForGame}} </center></td>
    </tr>
{% endfor %} </table>
</div>
{% endfor %}

<script>
    showBreakdown(0)
</script>
-----

## <small>How does this work?</small>

<small>Sometimes we're not interested in the average score - It's relatively easy for a good player to build that up playing against less skilled players. Let's assume we want to know more about the *quality* of the games a player has. How do we judge that? Well, we look at 3 criteria
1. <small>The number of other members they played (at the moment, that's basically anyone we know about)</small>
2. <small>How well they ranked against other members</small>
3. <small>How many games played</small>

<small> So lets say you only played 1 game against 4 other members. Including you, that's 5 players (5)<br/>
Then lets say you came last of the members (5th place). Your star quality would be 5. <br/>
However let's say you came second! We multiply your quality for that game by how well you did compared to everyone else: <br/>
5 divided by 2 = 2.5. We take your base of 5, and multiply it by 2.5 to get 12.5, nice!<br/>

<small>Now, if you keep that up for the month, that will be your average Star Quality.<br/> To work out your total, we take the average, and multiply it by the number of games. </small>

-----

<small><br/> We only regularly check up on players we know about, so if you're new and play a lot, you might be missing!  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-9-1234". <br/>
Want excluded? Same as above!</small>