<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">

    {%- include head_card.html -%}

  <body>

    <div class = headerGradient  >
      <div class = "navBar">
        <ul class = navbarList >
          <li> <a class = "navBar" href = "/MonthlyScores"> Monthly Scores </a></li>
          <li> <a class = "navBar" href = "/StarQuality"> Star Quality </a> </li>
          <li> <a class = "navBar" href = "/Overachievers"> Overachievers </a> </li>
          <li> <a class = "navBar" href = "/HeadToHeads"> Head to Head </a> </li> 
        </ul>
      </div>
    </div>
    
    <main class="page-content" aria-label="Content">
    
      <div class="wrapper HarbingerBack">
        <div class="CentralBlock">
          {{ content }}
        </div>
      </div>
    </main>

    {%- include footer.html -%} 

  </body>

</html>
