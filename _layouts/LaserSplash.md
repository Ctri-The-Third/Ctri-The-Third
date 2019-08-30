<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
{%- include head_card.html -%}
  <body>
    <div class = headerGradient  >
    {%- include navbar.html -%}
    </div>
    <main class="page-content container-fluid" aria-label="Content">
      <div class="wrapper HarbingerBack col-xs-12" style = "background-image:url('../assets/images/{{ page.URLPrefix | default: '' }}logoback.png')">
        <div class ="col-md-3" style = ""></div>
        <div class="col-md-6" style = "">
          {{ content }}
        </div>
        <div class ="col-md-3" style = ""> </div>
      </div>
    </main>

    {%- include footer.html -%} 

  </body>

</html>
