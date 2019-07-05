<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">

    {%- include head_card.html -%}

  <body>

    <div class = headerGradient  >
    <div class = "navBar" >
    <table class = links>
      <tr><td> Average Scores </td>
        <td> <a href = "/MonthlyScores/">July</a> </td> 
        <td><a href = "/MonthlyScores/2019-06">June</a></td>
      </tr>
      <tr><td> Star players </td>
        <td> <a href = "/StarQuality/">July</a> </td> 
        <td><a href = "/StarQuality/2019-06">June</a></td>
      </tr>
      <tr><td colspan = "3"><center><a href = "Overachievers">Achievements</a></center></td></tr>
      </table>
    </div>
    </div>
    
    <main class="page-content" aria-label="Content">
    
      <div class="wrapper">
        <div class="CentralBlock">
          {{ content }}
        </div>
      </div>
    </main>

    <!-- {%- include footer.html -%}-->

  </body>

</html>
