---
title: "Portal B2B of Construction Companies in Brazil"
layout: page
excerpt: "Companies, equipments in one place"
tags: [Algolia, PHP, MySQL, Laravel, Codeigniter]
work: "PHP"
---
<a href="http://www.guindastes.com" target="_blank">Guindastes.com</a>

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/logonovo.jpg){: .align-center}

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/guindastesStats.png){: .align-center}

A web portal that connects construction machinery companies to their clientes, displaying their equipments in the main search of the site. 

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/guindastesSearch.png){: .align-center}

Right now the website is being refactored to implement an amazing Search Engine written in C++ called Algolia which enables us to offer a better user experience in the way we display the equipment and also the services that the companies offer.


The search applies indexes and algorithms to rank the search (quite like ElasticSearch/Lucene) according to the terms the user searched filtering down to the most relevant to the user. Bringing not only the exact word/term searched but those results that may be similar or have some relation to what the user searched.


It also allows us to find out data inside products, companies profiles and equipment descriptions, making larger the spectrum of information available to the user, helping find the equipment and company that best match the user needs.


The project was made using PHP7 Codeigniter initially, then moved to Laravel 5.*, connecting two databases, one internal in Oracle and another one in the cloud using MySQL. We moved from a monolithic structure to a decentralized one adopting a MicroService Architecture by using REST APIs and separating concerns on a lower level.

The whole frontend is being re-designed and refactored to use Vue.js/Vuex and best frontend tools like TailWind.css / PostCSS.
