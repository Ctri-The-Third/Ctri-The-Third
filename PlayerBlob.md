---
layout : none

---


# Mini profile.
This is the profile for {{site.data.playerBlob.basicInfo.centre[0].codename}}, who predominantly plays LaserForce at {{site.data.playerBlob.basicInfo.centre[0].name}}.



{% for centre in site.data.playerBlob.basicInfo.centre %}
<div class = "arenaBox" style = "border:1px solid blue; padding-left:5px; width:300px; float:left; overflow:auto;">
<pre>Centre name: {{centre.name}}
Missions played: {{centre.missions}}
Average score: {{centre.summary[0][4]  }}
Level : {% assign trueSkill = centre.skillLevelNum | plus: 1 %}{{trueSkill }}</pre></div>{% endfor %}
