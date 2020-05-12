---
layout: page
title: Recursos
orden: 3
---

<p class="message">
  Se puede dejar de lado la identidad nacional es un sistema politico, y en vez defender el bienestar comun,
  sin tocar la identidad.
</p>  

# Personas

- [Tomas Perez Vejo](https://inah.academia.edu/TomasPerezVejo)
- [Alejandra B Osorio](https://alejandraosorio.academia.edu/)
- [François-Xavier Guerra](https://es.wikipedia.org/wiki/Fran%C3%A7ois-Xavier_Guerra)
- [Jaime Rodríguez Ordóñez](https://es.wikipedia.org/wiki/Jaime_Rodr%C3%ADguez_Ord%C3%B3%C3%B1ez)
- [Regina Grafe](https://www.eui.eu/DepartmentsAndCentres/HistoryAndCivilization/People/Professors/Grafe)
- [Carlos Marichal](https://carlosmarichal.colmex.mx/)
- [Horst Pietschmann](https://uni-hamburg.academia.edu/HorstPietschmann)
- [Ricardo Hausmann](https://www.hks.harvard.edu/faculty/ricardo-hausmann)
- [Cesar Hidalgo](https://chidalgo.com/)
- [Ha-Joon Chang](http://hajoonchang.net/)
- [Erik S. Reinert](https://en.wikipedia.org/wiki/Erik_S._Reinert)


Journals

- [Laboratory of Agent-Based Social Simulation](http://labss.istc.cnr.it/)
- [Computational Social Science Society of the Americas](https://computationalsocialscience.org/)
- [European Social Simulation Association (ESSA)](http://www.essa.eu.org/)
- [Real Hacienda Colmex](https://realhacienda.colmex.mx/)
- [Plaza de armas](http://www.plazadearmas.tv/debate.htm)
- [Historia de Mexico](https://historiamexicana.colmex.mx/)
- [Biblioteca Digital del Pensamiento Novohispano](http://www.bdpn.unam.mx/)
- [The Harvard Atlas of Economic Complexity](https://atlas.cid.harvard.edu/)
- [The Observatory of Economic Complexity](https://oec.world/en/)
- [New Things Under the Sun](https://mattsclancy.substack.com/)

<ul>
{% for cat in site.categories %}
<li>
  <a href="#{{ cat[0] }}"> {{ cat[0] }} ({{ cat[1].size }})</a>
  </li>
{% endfor %}
</ul>

{% for cat in site.categories %}
  <h2 id="{{ cat[0] }}">{{ cat[0] }} </h2>
  <ul>
    
    {% for post in cat[1] reversed %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}

  </ul>
{% endfor %}