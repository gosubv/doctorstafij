---
layout: default
title: Главная
---

<section class="hero">
    <div class="container">
        <span class="badge-online">● Приём онлайн доступен</span>
        <h1>Стафий Диана Викторовна</h1>
        <p>Врач эндокринолог первой категории, нутрициолог с 12-летним стажем.</p>
        <a href="{{ site.baseurl }}/booking/" class="btn-primary">Записаться на прием</a>
    </div>
</section>

<div class="container">
    <section id="services">
        <h2>Виды консультаций</h2>
        <div class="grid">
            <div class="card">
                <h3>Эндокринология</h3>
                <p>Первичный прием: диагностика щитовидной железы, обмена веществ.</p>
            </div>
            <div class="card">
                <h3>Нутрициология</h3>
                <p>Составление плана питания, коррекция дефицитов витаминов и минералов.</p>
            </div>
            <div class="card">
                <h3>Повторный прием</h3>
                <p>Анализ результатов обследования и корректировка терапии.</p>
            </div>
        </div>
    </section>

    <section id="how-it-works">
        <h2>Как проходит прием</h2>
        <div itemscope itemtype="https://schema.org/HowTo">
            <div itemprop="step"><b>1. Сбор жалоб:</b> Подробное обсуждение состояния здоровья и симптомов.</div>
            <div itemprop="step"><b>2. Осмотр:</b> Оценка состояния кожных покровов, щитовидной железы, измерение давления.</div>
            <div itemprop="step"><b>3. Анализ:</b> Изучение имеющихся анализов или назначение новых.</div>
            <div itemprop="step"><b>4. План:</b> Выдача рекомендаций по лечению и образу жизни.</div>
        </div>
    </section>

    <section id="reviews">
        <h2>Отзывы пациентов</h2>
        <div class="grid">
            {% for i in (1..6) %}
            <div class="card" itemprop="review" itemscope itemtype="https://schema.org/Review">
                <div itemprop="reviewRating" itemscope itemtype="https://schema.org/Rating">
                    <meta itemprop="ratingValue" content="5">⭐⭐⭐⭐⭐
                </div>
                <p itemprop="reviewBody">Благодарю Диану Викторовну за профессионализм. Очень грамотный подход к лечению!</p>
                <strong itemprop="author">Пациент {{ i }}</strong>
            </div>
            {% endfor %}
        </div>
    </section>

    <section id="location">
        <h2>Как нас найти</h2>
        <p>{{ site.author.address }}</p>
        <div style="width: 100%; height: 400px; background: #eee; border-radius: 15px; overflow: hidden;">
            <iframe src="https://yandex.ru/map-widget/v1/?ll=69.1389,54.8631&z=16&text=Петропавловск,Ауэзова,133" width="100%" height="400" frameborder="0"></iframe>
        </div>
    </section>
</div>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Physician",
  "name": "Стафий Диана Викторовна",
  "image": "{{ site.url }}{{ site.baseurl }}/assets/img/photo.jpg",
  "description": "{{ site.description }}",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "ул. Ауэзова 133",
    "addressLocality": "Петропавловск",
    "addressCountry": "KZ"
  },
  "url": "{{ site.url }}{{ site.baseurl }}",
  "telephone": "{{ site.author.phone }}",
  "priceRange": "$$",
  "hasCredential": {
    "@type": "EducationalOccupationalCredential",
    "credentialCategory": "Диплом врача, сертификат эндокринолога"
  }
}
</script>
