---
layout : LaserSplash
permalink: /7-9/LastYear
URLPrefix: '/7-9'
---
# testing
**Hello World**, this is my first page. I hope you like it.
<b>testing testing </b>
<div class = "container">
  <div class = "row">
    <div class = "col-sm-6">
        <table class = "AnnualTop3s" style = "border-radius:10px; margin:0px">
        {% for Month in site.data.7-9-AnnualTop3s %} 
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
    </div>
    <div class = "col-sm-6">
        <div class = "genericWrapper genericWrapperOffset LaserCardWrapper7-9"> 
        Games Played
        </div>
        <div class = "genericWrapper LaserCardWrapper7-9"> 
        Gains and Losses
        </div>
        <div class = "genericWrapper genericWrapperOffset LaserCardWrapper7-9"> 
        Referrals and Welcomers
        </div>
    </div>
