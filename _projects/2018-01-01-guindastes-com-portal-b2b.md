---
title: "Portal B2B of Construction Companies in Brazil"
layout: page
excerpt: "Companies, equipments in one place"
tags: [Algolia, PHP, MySQL, Laravel, Codeigniter]
work: "PHP"
---

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/guindastesSearch.png){: .align-center}

## Guindastes.com ##

A web portal that connects construction machinery companies to their clientes, displaying their equipments in the main search of the site. 

Right now is being refactoring to implement an amazin Search Engine written in C++ called Algolia which enable us to offer a better user experience in the way we display the equipments and also the services that the companies offer. 

The search apply indexes and algorithms to rank the search according to the terms the user searched filtering down to the most relevant to the user bringing not only what he exactly searched but thouse results that may be similar or have some relation to what the user search, as also, give the oportunity to find out data inside products, companies profiles and equipments descriptions, making larger the spectrum of information available to the user, helping find the right equipment and company to user's job.

The project was made using PHP7 Codeigniter initially, then moved to Laravel, connecting two databases, one internal in Oracle and another one in the cloud using MySQL. We moved from a monolithic structure to a descentralized one adopting a MicroService Architecture by using REST APIs and separating concerns on a lower level.