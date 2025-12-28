---
layout: page
title: "Отзывы"
---

# Отзывы пациентов

{% for review in site.data.reviews %}

> **{{ review.name }}**  
> {{ review.date }}
> {{ review.text }}

{% endfor %}
