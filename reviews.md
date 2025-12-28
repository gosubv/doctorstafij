---
layout: default
title: Отзывы
---

# Отзывы пациентов

{% for review in site.data.reviews %}
<div class="review">
  <strong>{{ review.name }}</strong> ({{ review.date }})  
  <p>{{ review.review }}</p>
</div>
{% endfor %}
