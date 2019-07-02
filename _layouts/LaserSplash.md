<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">

    {%- include head_card.html -%}

  <body>

    <div class = headerGradient  >
    
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
