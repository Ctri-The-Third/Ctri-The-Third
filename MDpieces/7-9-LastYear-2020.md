---
layout : LaserSplash-nocolums
permalink: /7-9/YearToDate
URLPrefix: '/7-9'
Description: 'Membership performance & gameplay stats for Funstation Edinburgh, 2020'

---
# Overview of regular members, for Funstation Edinburgh, 2020
<div class = "container" style = "margin-top:15px;">
  <div class = "row">
    <div class = "col-md-6">
        <table class = "AnnualTop3s" style = "border-radius:10px; margin:0px; height:300px;">
        {% for Month in site.data.7-9-AnnualTop3s-2020 %} 
            <tr> 
                <td class = "MonthHeader">{{Month.month}}</td> 
                <td class = "golden"><b>{{Month.players[0].playerName}}</b>
                    <br/><div class = "SmallBrightNumber"> {{Month.players[0].averageStars}} stars <br/> {{Month.players[0].gamePlayed}} games </div>
                </td>
                <td class = "silver"><b>{{Month.players[1].playerName}}</b>
                    <br/><div class = "SmallBrightNumber"> {{Month.players[1].averageStars}} stars <br/> {{Month.players[1].gamePlayed}} games </div>
                </td>
                <td class = "bronze"><b>{{Month.players[2].playerName}}</b>
                    <br/><div class = "SmallBrightNumber"> {{Month.players[2].averageStars}} stars <br/> {{Month.players[2].gamePlayed}} games </div>
                </td>
            </tr>
        {% endfor %}
        </table>
        <div class = "fluid-container" style = "padding-left:15px;padding-right:15px; margin-top:15px;">
            <div class = "row" >
                <div class = "col-sm-6 GainLossIcon " style = "background-image:url('/assets/images/add-group.svg'); border-radius:30px 15px 15px 15px; " > 
                    Welcomed Regular <br/>
                    <div class="sup">Someone who played their first game with an existing regular</div>
                    <b>{{site.data.7-9-AnnualMetrics-2020.referrals.newPlayers}}</b>
                </div>
                <div class = "col-sm-6 GainLossIcon" style = "background-image:url('/assets/images/friendly.svg'); border-radius: 15px; " > 
                    Welcomer<br/>
                    <div class="sup">Any existing regular present for another regular's first game</div>
                    <b>{{site.data.7-9-AnnualMetrics-2020.referrals.welcomers}}</b>
                </div>
            </div>
        </div>
    </div>
    <div class = "col-md-6">
        <div class = "genericWrapper genericWrapperOffset LaserCardWrapper7-9" id = "piechart" style = "height:300px; padding-left:10px; margin-top:0px; padding-right:10px; background-color:#000; overflow:hidden;"> 
        </div>
        <div class = "fluid-container" style = "padding-left:15px;padding-right:15px; margin-top:15px;">
            <div class = "row" >
                <div class = "col-sm-4 GainLossIcon " style = "background-image:url('/assets/images/log-in.svg'); border-radius:30px 15px 5px 15px; " > 
                    New Regular Players <br/>
                    <div class="sup">any L4+ players, or 15+ games played</div>
                    <b>{{site.data.7-9-AnnualMetrics-2020.playerCounts.newPlayers}}</b>
                </div>
                <div class = "col-sm-4 GainLossIcon" style = "background-image:url('/assets/images/team.svg'); border-radius:15px 15px 5px 5px; " > 
                    Active Regular Players<br/>
                    <div class="sup">includes new and players who went dormant</div>
                    <b>{{site.data.7-9-AnnualMetrics-2020.playerCounts.activePlayers}}</b>
                </div>
                <div class = "col-sm-4 GainLossIcon" style = "background-image:url('/assets/images/logout.svg'); border-radius: 15px 30px 15px 5px " > 
                    Regs Going Dormant<br/>
                    <div class="sup">not playing in the last 60 days of the year</div>
                    <b>{{site.data.7-9-AnnualMetrics-2020.playerCounts.churnedPlayers}}</b>
                </div>
            </div>
            <div class = "row">
                <div class = "col-sm-4 GainLossIcon GainLossNoIcon" style= "padding-top:30px; border-radius: 15px 5px 15px 30px"  > Average games played:
                <br/>
                <table class = MicroAggregate><tr><th>games</th><th>Regulars</th></tr>
                    {% for entry in site.data.7-9-AnnualMetrics-2020.regularsAggregateGames %} 
                    <tr><td>{{entry.caption}} </td><td>{{entry.players}}</td></tr>
                    {% endfor %}
                </table>
                </div>
                <div class = "col-sm-4 GainLossIcon GainLossNoIcon" style= "padding-top:30px; border-radius: 5px 5px 15px 15px"  > Average times visited:
                <br/>
                <table class = MicroAggregate><tr><th>visits</th><th>Regulars</th></tr>
                    {% for entry in site.data.7-9-AnnualMetrics-2020.regularsAggregateVisits %} 
                    <tr><td>{{entry.caption}} </td><td>{{entry.players}}</td></tr>
                    {% endfor %}
                </table>
                </div><div class = "col-sm-4 GainLossIcon GainLossNoIcon" style= "padding-top:11px; border-radius: 5px 15px 30px 15px"  > Number of weeks a member:
                <br/>
                <table class = MicroAggregate><tr><th>duration</th><th>Regulars</th></tr>
                    {% for entry in site.data.7-9-AnnualMetrics-2020.regularsAggregateRetention %} 
                    <tr><td>{{entry.caption}} </td><td>{{entry.players}}</td></tr>
                    {% endfor %}
                </table>
                </div>
            </div>
        </div>
    </div>
    </div>
  <div class = "row">
    <div class = "col-md-6">
        <h3 class = blackShadow> Brightest Stars of the year!</h3> 
        <div class = blackShadow> On average, who gained the most stars per game?</div>
        <table class="ScoreTable" style = "margin-left:0px;" >
        <tr><th style = "padding-left:5px;">Name</th><th><b>Avg. Stars per game</b> </th><th> Avg no. players </th><th> Average rank</th><th> games played </th> </tr>
        {% for Player in site.data.7-9-AnnualStars-2020.brightestStars %}
        <tr><td>{{Player.gamertag}}</td>
        <td class = "number"> <b>{{Player.averageStars}}</b> </td>
        <td class = "number"> {{Player.averageOpponents}} </td>
        <td class = "number"> {{Player.averageRank}} </td>
        <td class = "number"> {{Player.gamesPlayed}} </td>
        </tr>
        {% endfor %}
        </table>
    </div>
    <div class = "col-md-6">
        <h3 class = blackShadow> Biggest Stars of the year!</h3> 
        <div class = blackShadow> In total, who gained the most stars?</div>
        <table class="ScoreTable" style = "margin-left:0px;" >
        <tr><th style = "padding-left:5px;">Name</th><th><b>Total Stars earned</b> </th><th> Avg no. players </th><th> Average rank</th><th> games played </th> </tr>
        {% for Player in site.data.7-9-AnnualStars-2020.biggestStars %}
        <tr><td>{{Player.gamertag}}</td>
        <td class = "number"> <b>{{Player.averageStars}}</b> </td>
        <td class = "number"> {{Player.averageOpponents}} </td>
        <td class = "number"> {{Player.averageRank}} </td>
        <td class = "number"> {{Player.gamesPlayed}} </td>
        </tr>
        {% endfor %}
        </table>
    </div>

<script type="text/javascript">
var data = [{
  values: [],
  labels: [],
  pull: [],
  textfont: [],
  type: 'pie'
}];
{% for GameType in site.data.7-9-AnnualMetrics-2020.gamesPlayed %} 
    data[0].labels.push("{{GameType.gameName}}")
    data[0].values.push({{GameType.timesPlayed}})
{% endfor %}

var layout = {
    title:'Games Played by Regulars',
    paper_bgcolor:'rgba(0,0,0,0)',
    plot_bgcolor:'rgba(0,0,0,0)',
    font: {
        family: 'Courier New, monospace',
        size: 12,
        color: 'limegreen'
    },
    autosize: true,
    margin: {
        l: 25,
        r: 50,
        b: 50,
        t: 50,
        pad: 4
    }
};
Plotly.newPlot('piechart', data, layout, {displayModeBar: false, showLegend: false});
</script>
