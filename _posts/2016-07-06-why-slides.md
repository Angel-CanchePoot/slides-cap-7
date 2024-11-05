---
title: CAPITULO 10
layout: post
permalink: /why/
background: '#0a5'

slides:
 - title: TIPOS DE ERRORES
   slide-data: ERROR DE BIT, cuando uno o mas bits cambian de valor durante la transmision, Errores por ráfagas, Cuando varios bits consecutivos son afectados.
    

 - title: METODOS DE DETECCION DE ERRORES
   slide-data: PARIDAD, añador un bit para que el numero total de bits 1 sea par o impar, CHEQUEO DE REDUNDANCIA CICLICA CRC, usa divisiones polinomicas para detectar errores en bloques de datos, siendo muy eficaz en la deteccion de errores multiples

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
    
