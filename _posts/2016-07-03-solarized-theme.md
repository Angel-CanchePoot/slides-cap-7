---
title: Solarized Theme
layout: post
permalink: /solarized/
theme: solarized
 
slides:
 - title: TIPOS DE ERROES
   slide-data: ERRORES DE BITS, cuando uno o mas bits cabian su valor durantela transmision
   ERRORES POR RAFAGAS,  cuando varios bits consecutivos son ad¿fectados

 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: Slide 3
   slide-data: This is third slide

   
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
