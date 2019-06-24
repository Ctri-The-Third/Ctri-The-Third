---
layout : LaserSplash
layout : LaserCard
title: Player profile
---

<div class = "LaserCardWrapper">
<div class = "LaserCardNames">
<h2> {{site.data.playerBlob.SkillLevelName}} of  {{site.data.playerBlob.HomeArenaTrunc}} </h2>
</div>
<h1> {{site.data.playerBlob.PlayerName}} </h1>

<div class = "LaserCardBlock" >
<div class = "LaserCardPadding">
<b>This month</b> <hr/> 
Games: {{site.data.playerBlob.MonthlyGamesPlayed}} games <br/>
Average Stars: {{site.data.playerBlob.StarQuality}} stars <br/><p>
{{site.data.playerBlob.PlayerName}} played a game of {{site.data.playerBlob.GGName}}, coming {{site.data.playerBlob.GGRank}} and defeating {{site.data.playerBlob.GGVanq1}}, {{site.data.playerBlob.GGVanq2}}, {{site.data.playerBlob.GGVanq3}}, and {{site.data.playerBlob.GGVanq4}} for {{site.data.playerBlob.GGStars}} <br/></p>
</div></div>
<div class = "LaserCardBlock" >
<div class = "LaserCardPadding">
<b>All time</b> <hr/>
Achievements: {{site.data.playerBlob.Achievements}} <br/>
Rarest Achievemnt: {{site.data.playerBlob.GAName}} <p>
{{site.data.playerBlob.GADesc}}  </p><p>
{{site.data.playerBlob.GAOthers}}   </p>
</div></div>
</div>
