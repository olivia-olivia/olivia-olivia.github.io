---
layout: default
title: poemas
---

<div>
  <h3> todos, começando pelos mais recentes </h3>
</div>

<div id="index-posts">
  {% for post in site.posts %}
  <div id="post-short">
    <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
      <h4>{{post.title}}</h4>
    </a>
    <p>
      {% if post.excerpt %}
        {{ post.excerpt }}
      {% else %}
        {{ post.content }}
      {% endif %}
    </p>
  </div>
  {% endfor %}
</div>

=====

olá,

seja bem-vinda!

esse é um projeto de arquivamento, publicação e desenvolvimento de poemas.
está tudo muito no começo.

para enviar uma mensagem ou conversar comigo três jeitos:

<i class="fab fa-github"></i> issue ou pull request no  [GitHub](https://github.com/olivia-olivia/olivia-olivia.github.io)  
<i class="fas fa-envelope"></i> email pra oliviagj [arroba] prontonmail [ponto] com  
<i class="fab fa-twitter"></i> um oi lá no [twitter](http://twitter.com/oliviagj/)  

olivia

======

sobre publicação, edição, hospedagem da página, etc.

não sou programadora, mas tenho alguma familiaridade e facilidade com
tecnologia da informação. por enquanto, estou montando este site simples usando
[Jekyll](https://jekyllrb.com/) e [Github](https://github.com/) (inclusive Pages). no computador, pra fazer tudo funcionar, uso
sistema operacional [Fedora](https://getfedora.org/), [Firefox](https://firefox.com/) para navegar, [Atom](https://atom.io/) para mexer
nos arquivos, [Gitkraken](https://www.gitkraken.com/) para a interface com o GitHub.

estou disponível pra trocar
ideias sobre este processo. ganhar autonomia em relação aos meios de difusão
no processo de tornar públicas coisas que desenvolvo privadamente desde o século
passado.
