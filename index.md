---
layout: default
---

<div class="home">

  <h4>Olá, eu sou Bruno Duarte, um desenvolvedor mobile e web morando em São Paulo, Brasil. Abaixo você pode ver alguns projetos em que estou trabalhando. Caso você queira saber mais sobre mim, <a href="/sobre/" class="page-link">clique aqui.</a></h4>

  <br><br>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h1>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h1>
        <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>