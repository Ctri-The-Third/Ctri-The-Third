---
layout : LaserTable
title : Monthly Scores in Standard Games
---

#### {{site.data.MonthlyScoreLatest.ScoreTitle}}

{% for Match in site.data.HeadToHeads.Match %}
<div class = "h2hBox" >
    <div class = "h2hContent" >
        <div class = "h2hPlayer1">
            
                <h1>{{Match.Player1Name}}</h1>
                <h2>{{Match.Player1Score}}</h2>
            
        </div>
        <div class = "h2hCentre" >
            <p style = "vertical-align:center; line-height:14pt; margin:0px;">
                <small>{{Match.GameDate}}</small>
                <h1>VS</h1>
            </p>
        </div>
        <div class = "h2hPlayer2" >
            
                <h1>{{Match.Player2Name}}</h1>
                <h2>{{Match.Player2Score}}</h2>
            
        </div>
    </div>
</div>
{% endfor %}

-----

## <small>How does this work?</small>

<small>An individual player's games are available from [http://www.iplaylaserforce.com/](http://www.iplaylaserforce.com/). We query the scoreboard, and take note of the last 30 games played (ignoring things we've seen before)<br/> From there, we can spot if there's only 2 players. <br/>
If the game only has two players, and is an Individual game. This won't eliminate <i>all</i> the games where players play against public, but it guarantees that players are not on the same team!</small>

<small>We only regularly check up on players we know about, so if you're new, you might be missing!  <br/>
Want included? Email me at [LaserForceStats@ctri.co.uk](mailto:LaserForceStats@ctri.co.uk), all I need is your member ID in the form "7-9-1234". <br/>
Want excluded? Same as above!</small>