---
layout: default
title: Доктор Стафий — эндокринолог и нутрициолог
---

<!-- HERO -->
<section id="hero" class="hero">
  <div class="container">
    <span class="badge-online">Консультация онлайн и в клинике</span>
    <h1>Доктор Стафий</h1>
    <p class="hero-subtitle">
      Стафий Диана Викторовна — эксперт в гормональном здоровье и осознанном питании
    </p>
    <a href="#booking" class="btn-primary">Записаться на консультацию</a>
  </div>
</section>

<!-- ABOUT -->
<section id="about" class="about-section">
  <div class="container about-grid">
    <div class="about-image">
      <img src="{{ '/assets/img/doctor.png' | relative_url }}"
           alt="Стафий Диана Викторовна"
           class="glass-panel">
      <div class="experience-badge glass-panel">
        <strong>14+</strong>
        <span>лет практики</span>
      </div>
    </div>

    <div class="about-content glass-panel">
      <h2>Стафий Диана Викторовна</h2>
      <p class="subtitle">Эндокринолог • Клинический нутрициолог</p>

      <p>
        Мой путь в медицине начался в 2011 году после окончания
        <strong>Медицинского университета г. Астана</strong>.
        Я работаю на стыке доказательной эндокринологии и нутрициологии,
        помогая пациентам достигать устойчивых результатов.
      </p>

      <a href="#booking" class="btn-primary">Записаться</a>
    </div>
  </div>
</section>

<!-- SPECIALIZATIONS -->
<section id="specializations" class="spec-section">
  <div class="container">
    <h2>Направления работы</h2>

    <div class="spec-grid">
      <div class="spec-card">
        <div class="spec-icon">🦋</div>
        <h3>Щитовидная железа</h3>
        <p>Гипотиреоз, АИТ, тиреотоксикоз, узловые образования</p>
      </div>

      <div class="spec-card">
        <div class="spec-icon">🩸</div>
        <h3>Диабетология</h3>
        <p>Диабет 1 и 2 типов, инсулинорезистентность</p>
      </div>

      <div class="spec-card">
        <div class="spec-icon">⚖️</div>
        <h3>Метаболизм и вес</h3>
        <p>Ожирение, метаболический синдром, гормональные причины</p>
      </div>

      <div class="spec-card">
        <div class="spec-icon">🤰</div>
        <h3>Беременность и ГСД</h3>
        <p>Эндокринологическое сопровождение беременности</p>
      </div>

      <div class="spec-card">
        <div class="spec-icon">🧬</div>
        <h3>Нутрициология</h3>
        <p>Дефициты витаминов и минералов, остеопороз</p>
      </div>

      <div class="spec-card">
        <div class="spec-icon">🧠</div>
        <h3>Сложные патологии</h3>
        <p>Гипофиз, пролактиномы, редкие эндокринные нарушения</p>
      </div>
    </div>
  </div>
</section>

<!-- CERTIFICATES -->
<section id="certificates" class="cert-section">
  <div class="container">
    <h2>Сертификаты и дипломы</h2>

    <div class="diploma-carousel">
      {% for item in site.data.diplomas %}
      <div class="diploma-card">
        <img src="{{ item.image | relative_url }}"
             alt="{{ item.title }}">
        <p>{{ item.title }}</p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- SERVICES -->
<section id="services" class="price-section">
  <div class="container">
    <h2>Услуги и цены</h2>

    <div class="price-grid">
      <div class="price-card glass-panel">
        <h3>Эндокринолог</h3>
        <p>Первичный приём и диагностика</p>
        <strong>10 000 ₸</strong>
      </div>

      <div class="price-card glass-panel">
        <h3>Нутрициолог</h3>
        <p>Коррекция питания и дефицитов</p>
        <strong>15 000 ₸</strong>
      </div>

      <div class="price-card glass-panel">
        <h3>Повторный приём</h3>
        <p>Коррекция лечения</p>
        <strong>7 000 ₸</strong>
      </div>
    </div>
  </div>
</section>

<!-- BLOG -->
<section id="blog" class="blog-section">
  <div class="container">
    <h2>Блог эксперта</h2>

    <div class="blog-grid">
      {% for post in site.data.insta_feed limit:3 %}
      <a href="{{ post.link }}" target="_blank" class="blog-card">
        <span class="category">{{ post.category }}</span>
        <h3>{{ post.title }}</h3>
        <span class="blog-link">Смотреть в Instagram →</span>
      </a>
      {% endfor %}
    </div>
  </div>
</section>

<!-- BOOKING -->
<section id="booking" class="booking-section">
  <div class="container">
    <h2>Запись на консультацию</h2>

    <iframe
      src="https://calendar.google.com/calendar/appointments/schedules/AcZssZ2i5tRlXYaJ8xwBVwlNWhMC_qlRVYVaD38cEBtIHm9Y6tfuqlr7fghSu_O610_o7RjaenYaAW40?gv=true"
      width="100%" height="700" frameborder="0">
    </iframe>
  </div>
</section>

<!-- REVIEWS -->
<section id="reviews" class="reviews-section">
  <div class="container">
    <h2>Отзывы пациентов</h2>

    <div class="reviews-grid">
      {% for review in site.data.reviews limit:6 %}
      <div class="review-card glass-panel">
        <div class="review-stars">★★★★★</div>
        <p>{{ review.text }}</p>
        <strong>{{ review.name }}</strong>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- MAP -->
<section id="map" class="map-section">
  <div class="container">
    <h2>Где я принимаю</h2>
    <p>г. Петропавловск, ул. Ауэзова 133</p>

    <iframe
      src="https://yandex.ru/map-widget/v1/?z=12&ol=biz&oid=96035534355"
      width="100%" height="400" frameborder="0"
      style="border-radius:16px;">
    </iframe>
  </div>
</section>
