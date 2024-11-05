---
title: CAPITULO 10
layout: post
permalink: /why/
background: '#0a5'

slides:
 - title: TIPOS DE ERRORES
   slide-data: ERROR DE BIT, cuando uno o mas bits cambian de valor durante la transmision, Errores por ráfagas, Cuando varios bits consecutivos son afectados.
    

 - title: METODOS DE DETECCION DE ERRORES
   slide-data: Paridad Añadir un bit extra para que el número total de bits "1" sea par o impar.
Chequeo de redundancia cíclica (CRC) Usa divisiones polinómicas para detectar errores en bloques de datos, siendo muy eficaz en la detección de errores múltiples.
Checksum Suma los valores de segmentos de datos y envía el resultado junto con los datos.
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
    
