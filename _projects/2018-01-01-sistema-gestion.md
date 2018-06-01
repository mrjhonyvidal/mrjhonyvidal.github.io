---
title: "Sistema de Gestión Portuaria"
layout: page
excerpt: "PHP, Javascript, MySQL"
tags: [JSON, AJAX, PHP7, OOP, MVC]
work: "PHP"
---
![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/cuencaLogin.png){: .align-center}

Cuenca SIS is an internal management system used to manage documents related to commodities imported at Argentina seaports.

It's created using PHP7, MVC patterns, Javascript and MySQL.

You can check out a [demo](https://fierce-lake-26418.herokuapp.com/){:target="_blank"} hosted in Heroku.

**Notice: Images Scanned Upload, TCPDFs generation are disabled in Heroku**

SYSAdmin
Login: CUIT: 99-99999999-9
Password: gestion

Client (Only can see his data)
Login: CUIT: 44-44444444-4
Password: gestion


Features:

- Massive Import from CSV to Database;
- Multi-tenant Client and User
- PDF Report individual
- PDF Report All
- CSV Report
- Dynamic Datatable with Search Capabilitie in All Modules
- Email Sending using Sendgrid API
- CUIT checking and Input-Masking
- Validations to avoid repeated CUIT and File Number ID on CSV Import and CRUDs
- Password Encryption using last standards and practices
- File Upload checking file size, reducing image and checking type
- Multi Image Scanned Upload reducing image size to A4, 72ddi

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/importacionCSVConExito.png){: .align-center}

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/cuencaFicha.png){: .align-center}

### Reporte PDF con imágenes escaneadas ##

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/pdfCartaPorte.png){: .align-center}

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/cuencaSisReporte.png){: .align-center}

