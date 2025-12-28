---
layout: default
title: Отзывы
---

# Отзывы пациентов

{% for review in site.data.reviews %}
<div class="review-card">
  <strong>{{ review.name }}</strong>
  <span>{{ review.date }}</span>
  <p>{{ review.review }}</p>
</div>
{% endfor %}
