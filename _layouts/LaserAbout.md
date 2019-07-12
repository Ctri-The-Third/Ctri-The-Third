<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">

    {%- include head_card.html -%}

  <body>


{%- include header.html -%}
    
    <main class="page-content" aria-label="Content">
    
      <div class="wrapper HarbingerBack">
        <div class="CentralBlock" style =  "background-color: rgba(0, 0, 0, 0.4); padding:10px; border-radius:20px;"  >

          {{ content }}
        </div>
      </div>
    </main>

    {%- include footer.html -%} 

  </body>

</html>
