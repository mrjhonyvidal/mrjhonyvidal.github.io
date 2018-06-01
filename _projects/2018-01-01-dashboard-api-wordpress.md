---
title: "All-in one APIs Integration"
website: https://9dapps.com
layout: page
excerpt: "ZonaProp, OLX, MercadoLibre"
tags: [Wordpress, PHP, API, JSON]
work: "PHP"
---

The goal of this project was to create a Wordpress plugin using PHP that connects to three 

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/dashboardAPIs.png){: .align-center}

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/dashboardML.png){: .align-center}


![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/propertyDetail.png){: .align-center}

### Setting all the API Keys and Secrets in one place ###

As also the redirect OAUTH callbacks and also the automatically response system that some APIs like the one that MercadoLibre provides which allows us to catch automatically the questions made by our clients in the products we are selling, in this particularly case, real estate.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/settingsPlugin.png){: .align-center}

### Generate a XML to be exported ###

Generate a XML file automatically from the data inside the database in the format that OLX could read and enabled it always through a WP REST API endpoint

[WP REST Endpoint](https://www.globocenter.com.br/workana-qa/wp-json/isobrokers/api/v2/feed/olx)