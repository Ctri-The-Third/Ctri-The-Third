<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
    {%- include head_card.html -%}
  <body>
    <div class = headerGradient  >
    </div>
    <main class="page-content container-fluid" style = "margin-top:-50px;" aria-label="Content">
      <div class="wrapper HarbingerBack col-xs-12" >
          {{ content }}
      </div>
    </main>

    {%- include footer.html -%} 

  </body>

</html>
