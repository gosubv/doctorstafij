---
layout: default
title: Доктор Стафий | Эндокринолог и нутрициолог
---

<section class="hero">
    <div class="container">
        <div class="badge-online">Доступна онлайн-консультация</div>
        <h1>Доктор Стафий</h1>
        <p style="font-size: 1.2rem; max-width: 700px; margin: 0 auto 30px;">
            Системный подход к здоровью: эндокринология, диетология и функциональная нутрициология в Петропавловске.
        </p>
        <a href="{{ site.baseurl }}/booking/" class="cta-button">Записаться на прием</a>
    </div>
</section>

<section id="services" style="padding: 60px 0;">
    <div class="container">
        <h2 style="text-align: center; margin-bottom: 40px;">Виды приемов</h2>
        <div class="grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px;">
            <div class="card">
                <h3>Первичный прием эндокринолога</h3>
                <p>Полный разбор жалоб, осмотр, интерпретация анализов и постановка диагноза.</p>
                <strong>Цена: от 10 000 ₸</strong>
            </div>
            <div class="card">
                <h3>Консультация нутрициолога</h3>
                <p>Разбор дефицитов, коррекция рациона, подбор нутрицевтической поддержки.</p>
                <strong>Цена: от 12 000 ₸</strong>
            </div>
            <div class="card">
                <h3>Повторный прием</h3>
                <p>Контроль динамики лечения и коррекция терапии.</p>
                <strong>Цена: от 7 000 ₸</strong>
            </div>
        </div>
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

<section id="map" style="padding: 60px 0;">
    <div class="container">
        <h2>Контакты и проезд</h2>
        <p>г. Петропавловск, ул. Ауэзова 133, Магия Рук</p>
        <div style="border-radius: 15px; overflow: hidden; border: 2px solid var(--accent-light);">
            <iframe src="https://yandex.ru/map-widget/v1/?ll=69.1389,54.8631&z=16&text=Петропавловск,Ауэзова,133" width="100%" height="450" frameborder="0"></iframe>
        </div>
    </div>
</section>
