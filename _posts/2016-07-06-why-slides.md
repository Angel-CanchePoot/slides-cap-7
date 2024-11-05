---
title: CAPITULO 10
layout: post
permalink: /why/
background: '#0a5'

slides:
 - title: TIPOS DE ERRORES
   slide-data: ERROR DE BIT, cuando uno o mas bits cambian de valor durante la transmision!
   slide-data: ERRORES POR RAFAGAS, cuando varios bits consecutivos son afectados
    
 - title: Another reason to use webjeda slides    
   slide-data: It is very easy to apply different themes, background colors and images to slides.
   background: '#05a'
   
 - title: Is it free to use?
   slide-data: Absolutely. All credits should go to Hakim El Hattab for creating revealjs.
   background: '#e74c3c'
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
        <h1>{{slide.title}}</h1>{{ slide.slide-data }}

</section>               
{% endfor %}
    
