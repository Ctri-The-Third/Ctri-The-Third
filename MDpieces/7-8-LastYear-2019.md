---
layout : LaserSplash-nocolums
permalink: /7-8/LastYear-2019
URLPrefix: '/7-8'
---
# Overview of regular members, for LaserZone Huddersfield, 2019
<div class = "container" style = "margin-top:15px;">
  <div class = "row">
    <div class = "col-md-6">
        <table class = "AnnualTop3s" style = "border-radius:10px; margin:0px; height:300px;">
        {% for Month in site.data.7-8-AnnualTop3s-2019 %} 
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
                    <b>{{site.data.7-8-AnnualMetrics-2019.referrals.newPlayers}}</b>
                </div>
                <div class = "col-sm-6 GainLossIcon" style = "background-image:url('/assets/images/friendly.svg'); border-radius: 15px; " > 
                    Welcomer<br/>
                    <div class="sup">Any existing regular present for another regular's first game</div>
                    <b>{{site.data.7-8-AnnualMetrics-2019.referrals.welcomers}}</b>
                </div>
            </div>
        </div>
    </div>
    <div class = "col-md-6">
        <div class = "genericWrapper genericWrapperOffset LaserCardWrapper7-8" id = "piechart" style = "height:300px; padding-left:10px; margin-top:0px; padding-right:10px; background-color:#000; overflow:hidden;"> 
        </div>
        <div class = "fluid-container" style = "padding-left:15px;padding-right:15px; margin-top:15px;">
            <div class = "row" >
                <div class = "col-sm-4 GainLossIcon " style = "background-image:url('/assets/images/log-in.svg'); border-radius:30px 15px 15px 15px; " > 
                    New Regular Players <br/>
                    <div class="sup">any L4+ players, or 15+ games played</div>
                    <b>{{site.data.7-8-AnnualMetrics-2019.playerCounts.newPlayers}}</b>
                </div>
                <div class = "col-sm-4 GainLossIcon" style = "background-image:url('/assets/images/team.svg'); border-radius:15px 15px 30px 15px; " > 
                    Active Regular Players<br/>
                    <div class="sup">includes new and players who went dormant</div>
                    <b>{{site.data.7-8-AnnualMetrics-2019.playerCounts.activePlayers}}</b>
                </div>
                <div class = "col-sm-4 GainLossIcon" style = "background-image:url('/assets/images/logout.svg'); border-radius: 15px; " > 
                    Regs Going Dormant<br/>
                    <div class="sup">not playing in the last 60 days of the year</div>
                    <b>{{site.data.7-8-AnnualMetrics-2019.playerCounts.churnedPlayers}}</b>
                </div>
            </div>
        </div>
    </div>

<script type="text/javascript">
var data = [{
  values: [],
  labels: [],
  pull: [],
  textfont: [],
  type: 'pie'
}];
{% for GameType in site.data.7-8-AnnualMetrics-2019.gamesPlayed %} 
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
