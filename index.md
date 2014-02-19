---
layout: default
---

<p class="message">
El servei de “Hosting” de Bibtic consisteix en l’allotjament de pàgines web en un servidor sobre plataforma Linux, amb un directori reservat per a l’usuari on es pot accedir mitjançant un sistema de transferència de fitxers segur (ftp) i amb un panel de control accessible via navegador. Amb un suport tècnic proper i de qualitat.
</p>

<hr id="plans">

<div class="posts list-posts list-plans">
  <h1>Plans d'Allotjament</h1>
  <small>
  L’espai en disc que s’ofereix condiciona la tarifa del mateix. L’espai en disc és el total entre l’ocupat pels fitxers al directori del domini, la bústia de correu electrònic i l’ocupat per les bases de dades que l’usuari disposi. 
  </small>
  {% for post in site.categories.plans %}
  <div class="post post-plan">
    <h2>{{ post.title }}</h2>

    <span class="post-description">{{ post.description }}</span>

    {{ post.content }}
    <span class="post-price">{{ post.price }}</span>
  </div>
  {% endfor %}
</div>

<hr id="dominis">

<div class="posts list-posts list-domains">
  <h1>Dominis</h1>
  {% for post in site.categories.dominis %}
  <div class="post">
    <h2>{{ post.title }}</h2>
    <span class="post-description">{{ post.description }}</span>
    {{ post.content }}
  </div>
  {% endfor %}
</div>

<hr id="serveis">

<div class="posts list-posts list-plans">
  <h1>Altres Serveis</h1>
  {% for post in site.categories.serveis %}
  <div class="post">
    <h2>{{ post.title }}</h2>

    <span class="post-description">{{ post.description }}</span>

    {{ post.content }}
    <br>
    <span class="post-price">{{ post.price }}</span>
  </div>
  {% endfor %}
</div>

<hr id="contacte">
  <h1>Contacte</h1>
  <p>Pot contactar amb BibticHosting a l'email [{{ site.email }}](mailto:{{ site.email }}) o a [twitter](http://twitter.com/bibtic).</p>

<hr>