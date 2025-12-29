---
layout: default
---

<section class="hero">
  <div class="badge-online">Приём онлайн</div>
  <h1>Доктор Стафий</h1>
  <p>Эндокринолог, нутрициолог, эксперт в системном подходе к здоровью.</p>
  <a href="/booking/" class="cta-button">Записаться на консультацию</a>
</section>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Physician",
  "name": "Стафий Диана Викторовна",
  "image": "https://gosubv.github.io/doctorstafij/assets/img/photo.jpg",
  "medicalSpecialty": ["Endocrinology", "Nutritionist"],
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "ул. Ауэзова 133",
    "addressLocality": "Петропавловск",
    "addressCountry": "KZ"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "54.8631", 
    "longitude": "69.1389"
  },
  "url": "https://gosubv.github.io/doctorstafij/",
  "telephone": "+77XXXXXXXXX",
  "priceRange": "$$",
  "hasCredential": {
    "@type": "EducationalOccupationalCredential",
    "credentialCategory": "Диплом врача"
  }
}
</script>

<section id="services">
  <h2>Типы консультаций</h2>
  <div class="price-grid">
    <div class="card"><h3>Эндокринолог</h3><p>Первичный прием</p></div>
    <div class="card"><h3>Нутрициолог</h3><p>Коррекция дефицитов</p></div>
  </div>
</section>

<section id="reviews">
  {% for review in site.data.reviews %}
  <div class="review-box" itemprop="review" itemscope itemtype="https://schema.org/Review">
    <span itemprop="author">{{ review.name }}</span>
    <div class="stars">⭐⭐⭐⭐⭐</div>
    <p itemprop="reviewBody">{{ review.text }}</p>
  </div>
  {% endfor %}
</section>
