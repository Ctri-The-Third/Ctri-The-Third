<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
  {%- include head.html -%}
  <script src = "/assets/js/BreakdownScripts.js"></script>
  <script src = "/assets/js/jquery-3.4.1.min.js"></script>
  
  <body>
    {%- include header.html -%}  
    <main class="page-content" aria-label="Content">
      <div class="wrapper">
        <div class="CentralBlock">
          {{ content }}
        </div>
      </div>
    </main>
    {%- include footer.html -%} 

  </body>

</html>
