---
title: CAPITULO 10
layout: post
permalink: /why/
background: '#0a5'

slides:
 - title: TIPOS DE ERRORES
   slide-data: ERROR DE BIT, cuando uno o mas bits cambian de valor durante la transmision, Errores por ráfagas, Cuando varios bits consecutivos son afectados.
    

 - title: METODOS DE DETECCION DE ERRORES
   slide-data: PARIDAD, añador un bit para que el numero total de bits 1 sea par o impar, CHEQUEO DE REDUNDANCIA CICLICA CRC, usa divisiones polinomicas para detectar errores en bloques de datos, siendo muy eficaz en la deteccion de errores multiples, CHECKSUM, suma de los valores de segmentos de datos y envia el resultado junto con los datos

   background: '#05a'
   
 - title: METODOS DE CORRECCION DE ERRORES
   slide-data: CORRECCION DE ERRORES HACIA ADELANTE FEC, permite corregir errores sin retransmision, usando redundancia en los datos, CODIGOS DE HAMMING, permite detectar y corregir errores de un solo bit mediante el uso de bits de paridad en posiciones especificas
   background: '#e74c3c'
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
        <h1>{{slide.title}}</h1>{{ slide.slide-data }}

</section>               
{% endfor %}
    
