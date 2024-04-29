---
layout: page
permalink: /nivel/extras
---


# Extras


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