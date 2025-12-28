---
layout: page
title: "Отзывы"
---

# Отзывы пациентов

{% for review in site.data.reviews %}
<div class="review-card">
> **{{ review.name }}**  
> {{ review.text }}

{% endfor %}
