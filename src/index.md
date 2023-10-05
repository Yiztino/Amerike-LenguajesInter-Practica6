---
layout: base.njk
title: Blog de Yiztino/Luis Lemus
---

# {{ title }}

![Imagen de Luis]({{ '/static/img/YiztinoBanner.png' | url }})
- Un pequeño blog sobre cosas interesantes relacionadas a la filosofía, los videojuegos o el desarrollo de software interactivo ;D

[Conóceme]({{ '/acerca' | url }})


## Artículos de mi Blog

### Videojuegos con contenido útil


{% for videojuego in collections.videojuegos %}

- [{{videojuego.data.title}}]({{ videojuego.url | url }})

{% endfor %}

### Reflexiones sobre filosofía

{% for reflexionFilo in collections.reflexionesFilosofia %}

- [{{reflexionFilo.data.title}}]({{ reflexionFilo.url | url }})

{% endfor %}

### Mi contenido multimedia favorito 

{% for contenidoMulti in collections.contenidosMulti %}

- [{{contenidoMulti.data.title}}]({{ contenidoMulti.url | url }})

{% endfor %}

