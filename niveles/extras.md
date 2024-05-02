---
layout: page
permalink: /nivel/extras
comments: true
---


# JLPT Extras


<br>

---

<br>

Libros extras que se han recopilado a lo largo del tiempo.

<br>

---
<br>

## Libros de textos

---

<br>


{% for libro in site.data.nivel.ex %}
{% if libro.nombre %}
### **{{ libro.nombre }}** {% if libro.idioma %}({{libro.idioma}}){% endif %}

<br>

{{libro.descripcion}}

<br>

**Recursos**:

- Libro <a href="{{ '/view/' | relative_url }}?dato={{libro.link}}" class="text-info" target="_blank">[Abrir] </a>

{% if libro.workbook %}

- Workbook <a href="{{ '/view/' | relative_url }}?dato={{libro.workbook}}" class="text-info" target="_blank">[Abrir] </a>

{% endif %}

{% if libro.respuestas %}

- Respuestas <a href="{{ '/view/' | relative_url }}?dato={{libro.respuestas}}" class="text-info" target="_blank">[Abrir] </a>

{% endif %}

{% if libro.audio %}

- Audio <a href="{{ '/view/' | relative_url }}?dato={{libro.audio}}" class="text-info" target="_blank">[Abrir] </a>

{% endif %}

{% if libro.img %}
<br>
<div class="row justify-content-center">
    <div class="col-md-6">
      <img width="40%" src="{{libro.img}}" class="img-fluid">
    </div>
</div>
{% endif %}

<br>

---

{% endif %}
{% endfor %}

<br><br><br><br><br><br><br><br><br>

{% if page.comments %} 
<div id="disqus_thread"></div>
<script>
        /**
        *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
        *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables    */
        /*
        var disqus_config = function () {
        this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
        this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
        };
        */
    var disqus_config = function () {
        this.page.url = 'https://dokugakunihongo.github.io/';
        this.page.identifier = '';
        this.page.title = '';
    };
    (function() { // DON'T EDIT BELOW THIS LINE
      var d = document, s = d.createElement('script');
      s.src = 'https://dokugaku-nihongo.disqus.com/embed.js';
      s.setAttribute('data-timestamp', +new Date());
      (d.head || d.body).appendChild(s);
      })();
  </script>
  <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
{% endif %} 