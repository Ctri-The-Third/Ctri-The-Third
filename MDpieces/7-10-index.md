---
layout : LaserSplash
permalink: /7-10/
URLPrefix: '/7-10'
---

<div class = "LaserCardWrapper LaserCardWrapperGold  col-lg-12">
    <div class = "LaserCardContent">
        <div class = "row container-fluid">
            <div class = "LaserCardNames col-sm-3"> 
                <h1> {{site.data.7-10-playerBlob.GoldenPlayer.PlayerName}} </h1> 
            </div>
            <div class = "LaserCardNames col-sm-9"> <h2> {{site.data.7-10-playerBlob.GoldenPlayer.SkillLevelName}} of 
                {{site.data.7-10-playerBlob.GoldenPlayer.HomeArenaTrunc}} </h2> 
            </div>
        </div>
        <div class = "row container-fluid">
            <div class = "LaserCardBlock col-sm-6" >
                <b>This month</b> <hr/> 
                Games: {{site.data.7-10-playerBlob.GoldenPlayer.MonthlyGamesPlayed}} games <br/>
                Average Stars: {{site.data.7-10-playerBlob.GoldenPlayer.StarQuality}} stars <br/><p>
                {%unless site.data.7-10-playerBlob.GoldenPlayer.GGName == blank%}<b>Game of the Month:</b>{{site.data.7-10-playerBlob.GoldenPlayer.PlayerName}} played a game of {{site.data.7-10-playerBlob.GoldenPlayer.GGName}}, coming {{site.data.7-10-playerBlob.GoldenPlayer.GGRank}} and defeating {{site.data.7-10-playerBlob.GoldenPlayer.GGVanq1}}, {{site.data.7-10-playerBlob.GoldenPlayer.GGVanq2}}, {{site.data.7-10-playerBlob.GoldenPlayer.GGVanq3}}, and {{site.data.7-10-playerBlob.GoldenPlayer.GGVanq4}} for {{site.data.7-10-playerBlob.GoldenPlayer.GGStars}} {% endunless %}</p>
                <p><b>Claim to Fame:</b> Gold star! {{site.data.7-10-playerBlob.GoldenPlayer.PlayerName}} beat the most other members this month.
                <br/></p> 
            </div>
            <div class = "LaserCardBlock col-sm-6" >
                <b>All time</b> <hr/>
                Achievements: {{site.data.7-10-playerBlob.GoldenPlayer.Achievements}} <br/>
                Rarest Achievement: {{site.data.7-10-playerBlob.GoldenPlayer.GAName}} <p>
                "{{site.data.7-10-playerBlob.GoldenPlayer.GADesc}}"  </p><p>
                {{site.data.7-10-playerBlob.GoldenPlayer.GAOthers}} this achievement!  </p>
            </div>
        </div>
    </div>
</div>

<div class = "LaserCardWrapper LaserCardWrapperSilver  col-lg-12">
    <div class = "LaserCardContent">
        <div class = "row container-fluid">
            <div class = "LaserCardNames col-sm-3">
                <h1> {{site.data.7-10-playerBlob.SilverPlayer.PlayerName}} </h1> 
            </div>
            <div class = "LaserCardNames col-sm-9"> <h2> {{site.data.7-10-playerBlob.SilverPlayer.SkillLevelName}} of 
                {{site.data.7-10-playerBlob.SilverPlayer.HomeArenaTrunc}} </h2> 
            </div>
        </div>
        <div class = "row container-fluid">
            <div class = "LaserCardBlock col-sm-6" >
                <b>This month</b> <hr/> 
                Games: {{site.data.7-10-playerBlob.SilverPlayer.MonthlyGamesPlayed}} games <br/>
                Average Stars: {{site.data.7-10-playerBlob.SilverPlayer.StarQuality}} stars <br/><p>
                {%unless site.data.7-10-playerBlob.SilverPlayer.GGName == blank%}<b>Game of the Month:</b>{{site.data.7-10-playerBlob.SilverPlayer.PlayerName}} played a game of {{site.data.7-10-playerBlob.SilverPlayer.GGName}}, coming {{site.data.7-10-playerBlob.SilverPlayer.GGRank}} and defeating {{site.data.7-10-playerBlob.SilverPlayer.GGVanq1}}, {{site.data.7-10-playerBlob.SilverPlayer.GGVanq2}}, {{site.data.7-10-playerBlob.SilverPlayer.GGVanq3}}, and {{site.data.7-10-playerBlob.SilverPlayer.GGVanq4}} for {{site.data.7-10-playerBlob.SilverPlayer.GGStars}} {% endunless %}</p>
                <p><b>Claim to Fame:</b> Silver star! {{site.data.7-10-playerBlob.SilverPlayer.PlayerName}} beat the second most other members this month.
                <br/></p> 
            </div>
            <div class = "LaserCardBlock col-sm-6" >
                <b>All time</b> <hr/>
                Achievements: {{site.data.7-10-playerBlob.SilverPlayer.Achievements}} <br/>
                Rarest Achievement: {{site.data.7-10-playerBlob.SilverPlayer.GAName}} <p>
                "{{site.data.7-10-playerBlob.SilverPlayer.GADesc}}"  </p><p>
                {{site.data.7-10-playerBlob.SilverPlayer.GAOthers}} this achievement!  </p>
            </div>
        </div>
    </div>
</div>


<div class = "LaserCardWrapper LaserCardWrapperBronze  col-lg-12">
    <div class = "LaserCardContent">
        <div class = "row container-fluid">
            <div class = "LaserCardNames col-sm-3">
                <h1> {{site.data.7-10-playerBlob.BronzePlayer.PlayerName}} </h1> 
            </div>
            <div class = "LaserCardNames col-sm-9"> <h2> {{site.data.7-10-playerBlob.BronzePlayer.SkillLevelName}} of 
                {{site.data.7-10-playerBlob.BronzePlayer.HomeArenaTrunc}} </h2> 
            </div>
        </div>
        <div class = "row container-fluid">
            <div class = "LaserCardBlock col-sm-6" >
                <b>This month</b> <hr/> 
                Games: {{site.data.7-10-playerBlob.BronzePlayer.MonthlyGamesPlayed}} games <br/>
                Average Stars: {{site.data.7-10-playerBlob.BronzePlayer.StarQuality}} stars <br/><p>
                {%unless site.data.7-10-playerBlob.BronzePlayer.GGName == blank%}<b>Game of the Month:</b>{{site.data.7-10-playerBlob.BronzePlayer.PlayerName}} played a game of {{site.data.7-10-playerBlob.BronzePlayer.GGName}}, coming {{site.data.7-10-playerBlob.BronzePlayer.GGRank}} and defeating {{site.data.7-10-playerBlob.BronzePlayer.GGVanq1}}, {{site.data.7-10-playerBlob.BronzePlayer.GGVanq2}}, {{site.data.7-10-playerBlob.BronzePlayer.GGVanq3}}, and {{site.data.7-10-playerBlob.BronzePlayer.GGVanq4}} for {{site.data.7-10-playerBlob.BronzePlayer.GGStars}} {% endunless %}</p>
                <p><b>Claim to Fame:</b> Bronze star! {{site.data.7-10-playerBlob.BronzePlayer.PlayerName}} beat the third most other members this month.
                <br/></p> 
            </div>
            <div class = "LaserCardBlock col-sm-6" >
                <b>All time</b> <hr/>
                Achievements: {{site.data.7-10-playerBlob.BronzePlayer.Achievements}} <br/>
                Rarest Achievement: {{site.data.7-10-playerBlob.BronzePlayer.GAName}} <p>
                "{{site.data.7-10-playerBlob.BronzePlayer.GADesc}}"  </p><p>
                {{site.data.7-10-playerBlob.BronzePlayer.GAOthers}} this achievement!  </p>
            </div>
        </div>
    </div>
</div>

<div class = "LaserCardWrapper LaserCardWrapperOther  col-lg-12">
    <div class = "LaserCardContent">
        <div class = "row container-fluid">
            <div class = "LaserCardNames col-sm-3">
                <h1> {{site.data.7-10-playerBlob.OtherPlayer1.PlayerName}} </h1> 
            </div>
            <div class = "LaserCardNames col-sm-9"> <h2> {{site.data.7-10-playerBlob.OtherPlayer1.SkillLevelName}} of 
                {{site.data.7-10-playerBlob.OtherPlayer1.HomeArenaTrunc}} </h2> 
            </div>
        </div>
        <div class = "row container-fluid">
            <div class = "LaserCardBlock col-sm-6" >
                <b>This month</b> <hr/> 
                Games: {{site.data.7-10-playerBlob.OtherPlayer1.MonthlyGamesPlayed}} games <br/>
                Average Stars: {{site.data.7-10-playerBlob.OtherPlayer1.StarQuality}} stars <br/><p>
                {%unless site.data.7-10-playerBlob.OtherPlayer1.GGName == blank%}<b>Game of the Month:</b>{{site.data.7-10-playerBlob.OtherPlayer1.PlayerName}} played a game of {{site.data.7-10-playerBlob.OtherPlayer1.GGName}}, coming {{site.data.7-10-playerBlob.OtherPlayer1.GGRank}} and defeating {{site.data.7-10-playerBlob.OtherPlayer1.GGVanq1}}, {{site.data.7-10-playerBlob.OtherPlayer1.GGVanq2}}, {{site.data.7-10-playerBlob.OtherPlayer1.GGVanq3}}, and {{site.data.7-10-playerBlob.OtherPlayer1.GGVanq4}} for {{site.data.7-10-playerBlob.OtherPlayer1.GGStars}} {% endunless %}</p>
                <p><b>Claim to Fame:</b> {{site.data.7-10-playerBlob.OtherPlayer1.PlayerName}} got the highest average score of the month in standard missions!


                <br/></p> 
            </div>
            <div class = "LaserCardBlock col-sm-6" >
                <b>All time</b> <hr/>
                Achievements: {{site.data.7-10-playerBlob.OtherPlayer1.Achievements}} <br/>
                Rarest Achievement: {{site.data.7-10-playerBlob.OtherPlayer1.GAName}} <p>
                "{{site.data.7-10-playerBlob.OtherPlayer1.GADesc}}"  </p><p>
                {{site.data.7-10-playerBlob.OtherPlayer1.GAOthers}} this achievement!  </p>
            </div>
        </div>
    </div>
</div>

<div class = "LaserCardWrapper LaserCardWrapperOther  col-lg-12">
    <div class = "LaserCardContent">
        <div class = "row container-fluid">
            <div class = "LaserCardNames col-sm-3">
                <h1> {{site.data.7-10-playerBlob.OtherPlayer2.PlayerName}} </h1> 
            </div>
            <div class = "LaserCardNames col-sm-9"> <h2> {{site.data.7-10-playerBlob.OtherPlayer2.SkillLevelName}} of 
                {{site.data.7-10-playerBlob.OtherPlayer2.HomeArenaTrunc}} </h2> 
            </div>
        </div>
        <div class = "row container-fluid">
            <div class = "LaserCardBlock col-sm-6" >
                <b>This month</b> <hr/> 
                Games: {{site.data.7-10-playerBlob.OtherPlayer2.MonthlyGamesPlayed}} games <br/>
                Average Stars: {{site.data.7-10-playerBlob.OtherPlayer2.StarQuality}} stars <br/><p>
                {%unless site.data.7-10-playerBlob.OtherPlayer2.GGName == blank%}<b>Game of the Month:</b>{{site.data.7-10-playerBlob.OtherPlayer2.PlayerName}} played a game of {{site.data.7-10-playerBlob.OtherPlayer2.GGName}}, coming {{site.data.7-10-playerBlob.OtherPlayer2.GGRank}} and defeating {{site.data.7-10-playerBlob.OtherPlayer2.GGVanq1}}, {{site.data.7-10-playerBlob.OtherPlayer2.GGVanq2}}, {{site.data.7-10-playerBlob.OtherPlayer2.GGVanq3}}, and {{site.data.7-10-playerBlob.OtherPlayer2.GGVanq4}} for {{site.data.7-10-playerBlob.OtherPlayer2.GGStars}} {% endunless %}</p>
                <p><b>Claim to Fame:</b> {{site.data.7-10-playerBlob.OtherPlayer2.PlayerName}} Has the most achievements from everyone not already here.
                <br/></p> 
            </div>
            <div class = "LaserCardBlock col-sm-6" >
                <b>All time</b> <hr/>
                Achievements: {{site.data.7-10-playerBlob.OtherPlayer2.Achievements}} <br/>
                Rarest Achievement: {{site.data.7-10-playerBlob.OtherPlayer2.GAName}} <p>
                "{{site.data.7-10-playerBlob.OtherPlayer2.GADesc}}"  </p><p>
                {{site.data.7-10-playerBlob.OtherPlayer2.GAOthers}} this achievement!  </p>
            </div>
        </div>
    </div>
</div>
