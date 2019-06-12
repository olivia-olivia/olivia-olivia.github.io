---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: info
---

para ler os poemas, navegue nos títulos de coleção acima ou direto no listão
(nem tão ão) de todos os poemas, [abaixo](#todos-os-poemas).

para enviar uma mensagem ou conversar comigo três jeitos:
- Issue ou pull request no [GitHub](https://github.com/olivia-olivia/olivia-olivia.github.io)
- Email pra oliviagj [arroba] prontonmail [ponto] com
- Um oi lá no [twitter](http://twitter.com/oliviagj/)


esse é um projeto de arquivamento, publicação e desenvolvimento de poemas.
está tudo muito no começo. não sou programandora, mas tenho alguma familiaridade
e facilidade com tecnologia da informação. por enquanto, estou montando este
site simples usando Jekyll e Github (inclusive Pages). no computador, pra fazer
tudo funcionar, uso sistema operacional Fedora (versão 30), Firefox para
navegar, Atom para mexer nos arquivos, Gitkraken para a interface com o GitHub.

aos poucos vou adicionar links para esses recursos e estou disponível pra trocar
ideias sobre este processo. ganhar autonomia em relação aos meios de difusão
no processo de tornar públicas coisas que desenvolvo privadamente desde o século
passado. seja bem-vinda.

olivia

======

## todos os poemas

{% for post in site.posts %}
  <div id="post-short">
    <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
      <h3>{{post.title}}</h3>
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
