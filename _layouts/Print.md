<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: "en" }}">
  <head>
    <link rel="stylesheet" href="{{ "/assets/css/print.css" | relative_url }}">
  </head>
  <body>
    <main class="page-content container-fixed" aria-label="Content">        
      {{ content }}
    </main>
  </body>
</html>
