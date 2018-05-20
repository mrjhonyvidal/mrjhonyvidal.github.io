---
title: "Building a Test-Driven REST Subscription API"
layout: page
excerpt: "Using best practices"
last_modified_at: 2017-12-06 00:00:00 
tags: [test-driven, rest, laravel]
---

## Still preparing the post and files...

## What we will build? ##

We're going to build a Subscription System API for Online Services using [REST](https://spring.io/understanding/REST) and PHP Laravel 5.6.

The API will implement different Payment Gateways like (Stripe and PayPal), it contains User Authentication and Registration using OAuth - JWT protocol for security. 

The code source and online API can be found in [GitHub](https://github.com/elephwebb/laravel-test-driven-rest-api) and you can contribute if you want.

Here is the [KANBAN](https://trello.com/b/FVryIUaW) of the project.

## Quick Summary ##

- [Toolbelt](#toolbelt)
- [Introduction](#introduction)
- [Define Business Model](#business-model)
- [Requirements with KanBan](#requirements) 
- [API Endpoints](#rest-api-endpoints)
- [Design API](#design-api)
- [Pre Testing the API](#pre-testing-the-api)
- [Development Environment](#development-environment)
- [Git Workflow](#git-workflow)
- [Code](#code)
- [Push Always](#push-always)
- [Deploy](#deploy)
- [Measure](#measure)

We will in future split the section [Code](#code) in small chunks for better readability.


## ToolBelt ##

- GIT, Varnish AND/OR [Docker](http://laradock.io/) - Development Environment
- PHP Laravel, OOP, SOLID, Design Patterns
- APIRY for API Design and Tests
- Postman / SoapUI for simple tests on endpoints
- TravisCI for Continous Integration
- Loader.io for benchmark
- Heroku to publish our API


We will pre-built the API Schema and Docs using [APIRY](https://apiary.io/) before write a single line of code, mapping our business model/rules to the schema.

Basically the idea is to document the Endpoints using a standard so it's easier to design, test and colaborate with others developers, so it's clear what the API does or not without spend time write down software to implement it. It's important spend some time think what we want to accomplish, what we want to build. 

That is our first move toward a **better code** and **client happiness**.

After that we will dive in actually develop it with tests and Laravel best practices in mind to detect errors and behaviors quickly, use SOLID principles and Design Patterns to build an application that can scale.

Push the code with GIT to TravisCI which will automate some tests before deploy to our server, in our case, Heroku.

To monitor the perfomance of our API we will use [Loader.io](https://loader.io/).

We will use [Postman](https://www.getpostman.com/) to check the responses from the API, we also will try out [SoapUI](https://www.soapui.org/).


## Introduction

First of all, why would you like to build an API, it's crucial to understand the reason behind and why it's so popular nowadays. 

It follows a software architecture called [Micro Services](https://martinfowler.com/articles/microservices.html). 

> <cite>In short, the microservice architectural style [1] is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweight mechanisms, often an HTTP resource API. [Martin Fowler](https://martinfowler.com/) and [James Lewis](https://twitter.com/boicy)</cite>

Not get in too much detail about it and focus on the practical side of code using a test-driven aproach as a key factor inside the [Agile Methodology](http://agilemanifesto.org/principles.html).

I definetly advice take a look at [HTTP API Designs](https://geemus.gitbooks.io/http-api-design/content/en/) for more information.

As Phil Sturgeon suggest in his book [Building APIs you don't hate](https://www.amazon.com/?afiliate_program=jhonyvidal).

Define the API endpoints even if in a piece of paper (or initially)

- [ ] [Business Model](#business-model)
- [ ] [API Endpoints](#api-endpoints)




## Business Model ##


## REST API Endpoints ##



## Requirements ##



## Design Api ##





## Pre Testing The Api ##







## Development Environment ##






## Git Workflow ##






## Code ##


```php
namespace App;

use Laravel\Passport\HasApiTokens;
use Illuminate\Notifications\Notifiable;
use Illuminate\Foundation\Auth\User as Authenticatable;

class User extends Authenticatable
{
    use HasApiTokens, Notifiable;
}
```



## Push Always ##




## Deploy ##




## Measure ##

