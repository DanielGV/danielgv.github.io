---
layout: splash
title: Daniel Gomez villanueva
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/bio-photo.jpg
  actions:
    - label: "Download CV"
      url: "/assets/downloads/Daniel Gomez Villanueva.pdf"
  caption: ""
excerpt: "A software developer with passion for search"
type: center
---

## Experience

{% for experience in site.data.experience %}
### {{ experience.company }} - _{{ experience.position }}_
*{{ experience.timeline }}*

{{ experience.description }}
> {{ experience.tags }}
{% endfor %}

## Smaller consultant projects

{% for experience in site.data.consultancy %}
### {{ experience.company }} - _{{ experience.position }}_
{{ experience.description }}
> {{ experience.tags }}

{% endfor %}

## Studies

{% for education in site.data.education %}

### {{ education.school }} - _{{ education.program }}_

{% comment %}
![{{ education.school }}]({{ education.logo }} "{{ education.school }}")
{% endcomment %}

*{{ education.timeline }}*

{{ education.description }}

> {{ education.courses }}

{% endfor %}

## Interests
I enjoy running, not for the sake of it, but as an outdoor activity and a way of discovering new places. My favourite places usually involve nature, be it small parks of large natural parks. National parks are indeed my favourite travelling destinations, but any new places are appreciated. Along new places come new cultures and food, I always try to taste and learn to cook different dishes with uncommon ingredients. I like playing both board games and videogames, especially focusing on new mechanics and solving puzzles. It is all about learning new stuff: new food, challenging puzzles or new technology though online courses or webinars.

## Training / Certifications

{% for certification in site.data.certifications %}
* {{ certification.cert }} - *{{ certification.time }}* {% if certification.link %} [See certificate]({{ certification.link }})  {% endif %} {% endfor %}

## Publications
[Problem with SSL subject matching in Apache’s HttpClient](https://medium.com/pricerunner-tech/problem-with-ssl-subject-matching-in-apaches-httpclient-48b196931772) - Pricerunner Blog post

[Relevance in the wild](https://www.slideshare.net/lucidworks/relevance-in-the-wild-daniel-gomez-vilanueva-findwise) - [Recording](https://www.youtube.com/watch?v=Tf3tEn1bZfM) - 
Lucene/Solr Revolution 2017

[Solr vs Elastic](https://findwise.com/blog/solr-or-elasticsearch/) - Findwise Blog post

## Languages

{% for language in site.data.languages %}
* {{ language.flag }} {{ language.lang }} - {{ language.level }} {% endfor %}