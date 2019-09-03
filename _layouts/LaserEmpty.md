<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
    {%- include head_card.html -%}
  <body class = "" style = "">
    <div class = headerGradient  >
    </div>
    <div class="wrapper HarbingerBack col-xs-12 " style = "height:100%; " >
    <main class="page-content container-fluid " style = "margin-top:-50px;" aria-label="Content">
          {{ content }}  
    </main>
    </div>
    {%- include footer.html -%} 

  </body>

</html>
