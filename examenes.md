---
layout: page
permalink: /examenes/
---

# Exámenes del JLPT Noken (日本語能力試験)

<br>

---

<br>

 Estos exámenes anteriores son recursos útiles para aquellos que desean practicar y prepararse para el JLPT, ya sea comenzando desde los niveles básicos o aspirando a niveles más avanzados de competencia en japonés.

<br>

<div class="container">
  <div class="row justify-content-center">
    <div class="col-md-6">
      <img src="/img/jlpt.jpg" alt="Descripción de la imagen" class="img-fluid">
    </div>
  </div>
</div>


<br>

---

<br>

### Niveles: 

<br>

**Hojas para responder**

{% for youshi in site.data.examenes.youshi %}

- {{youshi.lvl}} <a href="{{youshi.link}}" class="fuente text-info" target="_blank"> [Abrir]</a> 

{% endfor %}

<br>

### Lista: 

<br>

<div id="accordion">
    <div class="card acordeon border">
    <div class="card-header" id="heading5">
      <h5 class="mb-0">
        <button class="btn btn-link fuente n5" data-toggle="collapse" data-target="#collapse5" aria-expanded="true" aria-controls="collapse5">
          N5 (初級者)
        </button>
      </h5>
    </div>
    <div id="collapse5" class="collapse show" aria-labelledby="heading5 data-parent=" data-parent="#accordion">
      <div class="card-body">
          {% include examenes.html titulo="Examenes" examenes=site.data.examenes.n5 %}
      </div>
    </div>
  </div>
    <div class="card acordeon border">
    <div class="card-header" id="heading4">
      <h5 class="mb-0">
        <button class="btn btn-link fuente n4" data-toggle="collapse" data-target="#collapse4" aria-expanded="false" aria-controls="collapse4">
          N4 (初級者~中級者)
        </button>
      </h5>
    </div>
    <div id="collapse4" class="collapse" aria-labelledby="heading4" data-parent="#accordion">
      <div class="card-body">
            {% include examenes.html titulo="Examenes" examenes=site.data.examenes.n4 %}
      </div>
    </div>
  </div>
  <div class="card acordeon border">
    <div class="card-header" id="heading3">
      <h5 class="mb-0">
        <button class="btn btn-link fuente n3" data-toggle="collapse" data-target="#collapse3" aria-expanded="false" aria-controls="collapse3">
          N3 (中級者):
        </button>
      </h5>
    </div>
    <div id="collapse3" class="collapse" aria-labelledby="heading3" data-parent="#accordion">
      <div class="card-body">
            {% include examenes.html titulo="Examenes" examenes=site.data.examenes.n3 %}
      </div>
    </div>
  </div>
  <div class="card acordeon border">
    <div class="card-header" id="heading2">
      <h5 class="mb-0">
        <button class="btn btn-link collapsed fuente n2" data-toggle="collapse" data-target="#collapse2" aria-expanded="false" aria-controls="collapse2">
          N2 (中級者~上級者)
        </button>
      </h5>
    </div>
    <div id="collapse2" class="collapse" aria-labelledby="heading2" data-parent="#accordion">
      <div class="card-body">
            {% include examenes.html titulo="Examenes" examenes=site.data.examenes.n2 %}
      </div>
    </div>
  </div>
  <div class="card acordeon border">
    <div class="card-header" id="headingThree">
      <h5 class="mb-0">
        <button class="btn btn-link collapsed fuente jyokyu" data-toggle="collapse" data-target="#collapse1" aria-expanded="false" aria-controls="collapse1">
          N1 (上級者)
        </button>
      </h5>
    </div>
    <div id="collapse1" class="collapse" aria-labelledby="heading1" data-parent="#accordion">
      <div class="card-body">
            {% include examenes.html titulo="Examenes" examenes=site.data.examenes.n1 %}
      </div>
    </div>
  </div>
</div>

