---
layout: default
title: Доктор Стафий | Эндокринолог-нутрициолог
---

<section id="hero" class="hero">
    <div class="container">
        <span class="badge-online">Консультация в клинике и онлайн</span>
        <h1 class="hero-title">Доктор Стафий</h1>
        <p class="hero-subtitle">
            Стафий Диана Викторовна — Ваш эксперт в мире гормонального здоровья и осознанного питания.
        </p>
        <a href="#booking" class="btn-nav hero-btn">Запись на консультацию</a>
    </div>
</section>

<section id="about" class="about-section">
    <div class="container">
        
        <div class="about-hero">
            <div class="about-image">
                <img src="{{ '/assets/img/doctor_02.png' | relative_url }}" alt="Стафий Диана Викторовна" class="doctor-img" />
                <div class="experience-badge glass-panel">
                    <span class="years">14+</span>
                    <span class="exp-text">лет практики</span>
                </div>
            </div>

            <div class="about-content">
                <h2 class="section-title">Стафий Диана Викторовна</h2>
                <p class="subtitle">Эндокринолог • Интегративный нутрициолог</p>
                
                <div class="bio-text">
                    <p>Мой путь в медицине начался в 2011 году после окончания <strong>Медицинского университета г. Астана</strong>. За годы клинической практики я поняла, что гормональное здоровье требует не только точных лекарственных назначений, но и глубокой работы с образом жизни.</p>
                    <p>Получив специализацию по <strong>интегративной нутрициологии в Академии интегративной нутрициологии PRO-ЗДОРОВЬЕ</strong>, я интегрировала методы коррекции питания в классическую эндокринологию. Это позволяет моим пациентам добиваться устойчивых результатов в лечении метаболических нарушений и патологий щитовидной железы.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="specializations" class="spec-section">
    <div class="container">
        <h2 class="section-title">Направления работы</h2>
        <div class="spec-grid">
            {% for item in site.data.specializations %} 
                <div class="spec-card">
                    <div class="spec-icon-wrapper">{{ item.icon }}</div>
                    <h3>{{ item.title }}</h3>
                    <p>{{ item.text }}</p>
                </div>
            {% endfor %}
        </div>
    </div>
</section>

<section id="certificates" class="certificates-section">
    <div class="container">
        <div class="certificates-header">
            <div>
                <h2 class="certificates-title">Сертификаты и дипломы</h2>
                <p>Подтвержденная квалификация и постоянное обучение</p>
            </div>
            <div class="certificates-nav">
                <button class="cert-nav-btn" onclick="document.querySelector('.diploma-carousel').scrollBy({left: -320, behavior: 'smooth'})">←</button>
                <button class="cert-nav-btn" onclick="document.querySelector('.diploma-carousel').scrollBy({left: 320, behavior: 'smooth'})">→</button>
            </div>
        </div>

        <div class="diploma-carousel" itemscope itemtype="https://schema.org/EducationalOccupationalCredential">
            {% for item in site.data.diplomas %}
                <div class="diploma-card">
                    <input type="checkbox" id="zoom-{{ forloop.index }}" class="zoom-toggle">
                    <label for="zoom-{{ forloop.index }}" class="diploma-img-wrapper">
                        <img src="{{ item.image | relative_url }}" alt="{{ item.title }}" class="diploma-image" itemprop="image">
                    </label>
                    <div class="diploma-info">
                        <p itemprop="name">{{ item.title }}</p>
                    </div>
                </div>
            {% endfor %}
        </div>
        
    </div>
</section>

<section id="services" class="services-section">
    <div class="container price-section">
        <h2 class="section-title services-title">Виды консультаций</h2>
        <div class="card-grid">
            {% for item in site.data.services %}
                <div class="card price-item">
                    <h3>{{ item.title }}</h3>
                    <span>{{ item.text }}</span>
                    <span class="price-val"><p><b>{{ item.duration }}</b></p></span>
                    <span class="price-val"><p><b>{{ item.price }}</b></p></span>
                    <span class="price-val"><p><b>{{ item.price_online }}</b></p></span>
                    <span class="price-val"><p><b>{{ item.price_repeating }}</b></p></span>
                    <span class="price-val"><p><b>{{ item.paying }}</b></p></span>
                    <span class="price-val">
                        <div><a href='https://wa.me/{{ site.author.phonewhatsapp }}?text=Здравствуйте!%20Хочу%20записаться%20на%20консультацию {{ item.button_text }}.' class='cta-button btn-whatsapp' target='_blank'>
                        {% include whatsapp.html %}
                        Записаться на консультацию {{ item.button_text }}</a></div>
                    </span>
                </div>
            {% endfor %}
        </div>
    </div>
</section>

<section id="consultation-details" class="consultation-section">
    <div class="container">
        <div class="consultation-notice">
            <h3>⚠ Обратите внимание!</h3>
            <p>Консультация эндокринолога - это лечение заболеваний эндокринной системы. Здесь проводится беседа, назначение плана диагностики и лечения.</p>
            <p>На этом приёме не проводится глубокий разбор анализов по железу, витаминам, холестерину и другим биохимическим показателям. Эти вопросы относятся к компетенции терапевта, гематолога или к превентивному приёму, где подробно разбираются все базовые анализы, дефициты и составляется индивидуальная схема коррекции.</p>
            <p>📌 Если вы хотите обсудить именно такие результаты анализов и получить комплексный план для организма в целом — пожалуйста, запишитесь  консультацию эндокринолога- нутрициолога.</p>
            <p>Благодарю за понимание! Буду рада Вас видеть 😊</p>
        </div>
    </div>
</section>

<section id="blog" class="blog-section">
    <div class="container">
        <div class="blog-header">
            <div>
                <h2 class="blog-title">Блог эксперта</h2>
                <p class="blog-subtitle">Актуальные темы эндокринологии и нутрициологии из моего Instagram</p>
            </div>
            <a href="{{ site.author.instagram_url }}" target="_blank" class="cta-button blog-cta">
                Все публикации
            </a>
        </div>

        <div class="blog-grid">
            {% for post in site.data.insta_feed limit:3 %}
                <a href="{{ post.link }}" target="_blank" class="blog-card">
                    <div>
                        <div class="category">{{ post.category }}</div>
                        <h3>{{ post.title }}</h3>
                    </div>
                    <div class="blog-link">
                        Смотреть в Instagram 
                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.25 29 29 0 0 0-.46-5.33z"></path><polygon points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02"></polygon></svg>
                    </div>
                </a>
            {% endfor %}
        </div>
    </div>
</section>

<section id="booking" class="booking-section">
    <div class="container">
        <div class="booking-footer">
            <h2 class="booking-title">Запись на консультацию</h2>
            
            <div class="calendar-container">
                <p style="margin-bottom: 15px; opacity: 0.8;">График консультаций на ближайшие недели:</p>

                <div id="calendar-ribbon" class="calendar-ribbon">
                    {% assign calendar_items = site.data.calendar %}
                    {% for item in calendar_items %}
                        {% assign date_str = item.date %}
                        
                        {% assign day_name_eng = date_str | date: "%a" %}
                        {% assign day_num = date_str | date: "%-d" %}
                        {% assign month_eng = date_str | date: "%b" %}
                        
                        {% case day_name_eng %}
                            {% when 'Mon' %}{% assign day_name_ru = 'Пн' %}
                            {% when 'Tue' %}{% assign day_name_ru = 'Вт' %}
                            {% when 'Wed' %}{% assign day_name_ru = 'Ср' %}
                            {% when 'Thu' %}{% assign day_name_ru = 'Чт' %}
                            {% when 'Fri' %}{% assign day_name_ru = 'Пт' %}
                            {% when 'Sat' %}{% assign day_name_ru = 'Сб' %}
                            {% when 'Sun' %}{% assign day_name_ru = 'Вс' %}
                        {% endcase %}
                        
                        {% case month_eng %}
                            {% when 'Jan' %}{% assign month_ru = 'янв' %}
                            {% when 'Feb' %}{% assign month_ru = 'фев' %}
                            {% when 'Mar' %}{% assign month_ru = 'мар' %}
                            {% when 'Apr' %}{% assign month_ru = 'апр' %}
                            {% when 'May' %}{% assign month_ru = 'мая' %}
                            {% when 'Jun' %}{% assign month_ru = 'июн' %}
                            {% when 'Jul' %}{% assign month_ru = 'июл' %}
                            {% when 'Aug' %}{% assign month_ru = 'авг' %}
                            {% when 'Sep' %}{% assign month_ru = 'сен' %}
                            {% when 'Oct' %}{% assign month_ru = 'окт' %}
                            {% when 'Nov' %}{% assign month_ru = 'ноя' %}
                            {% when 'Dec' %}{% assign month_ru = 'дек' %}
                        {% endcase %}
                        
                        {% assign calendar_date = date_str | date: "%Y-%m-%d" %}
                        {% assign today_date = site.time | date: "%Y-%m-%d" %}

                        {% if item.is_off == true or calendar_date <= today_date %}
                            <div class="calendar-day day-off">
                                <div class="day-name">{{ day_name_ru }}</div>
                                <div class="day-number">{{ day_num }} {{ month_ru }}</div>
                                <span class="no-slot">Нет записи</span>
                                <span class="no-slot"></span>
                            </div>
                        {% else %}
                            <a href="https://wa.me/{{ site.author.phonewhatsapp }}?text=Здравствуйте!%20Хочу%20записаться%20на%20{% if item.is_online %}Онлайн{% endif %}%20консультацию.%20Желаемая%20дата:%20{{ day_num }}%20{{ month_ru }}." class="calendar-day available" target="_blank">
                                <div class="day-name">{{ day_name_ru }}</div>
                                <div class="day-number">{{ day_num }} {{ month_ru }}</div>
                                <span class="time-slot">{{ item.time }}</span>
                                <span class="time-slot">
                                    {% if item.is_online %}
                                        Онлайн
                                    {% else %}
                                        
                                    {% endif %}
                                </span>
                            </a>
                        {% endif %}
                    {% endfor %}
                </div>
            </div>

            <p class="booking-desc"><h3>Для вашего удобства я веду запись через WhatsApp.</h3></p><p><h3>Нажмите на интересующую Вас дату или нажмите кнопку ниже, чтобы начать чат:</h3></p>
            <div><a href="https://wa.me/{{ site.author.phonewhatsapp }}?text=Здравствуйте!%20Хочу%20записаться%20на%20консультацию." class="cta-button btn-whatsapp" target="_blank">
                {% include whatsapp.html %}
                Написать в WhatsApp
            </a></div>
        </div>
    </div>
</section>

<section id="reviews" class="reviews-section">
    <div class="container">
        <div class="reviews-header">
            <h2 class="reviews-title">Отзывы пациентов</h2>
            <div class="reviews-separator"></div>
        </div>

        <div class="reviews-grid">
            {% for review in site.data.reviews limit:6 %}
                <div class="review-card" itemscope itemtype="https://schema.org/Review">
                    <div class="review-stars">
                        {% for i in (1..review.rating) %}★{% endfor %}
                    </div>
                
                    <div class="review-text" itemprop="reviewBody">
                        {{ review.text }}
                    </div>

                    <div class="review-info">
                        <span class="author-name" itemprop="author">{{ review.name }}</span>
                    </div>

                    <meta itemprop="datePublished" content="{{ review.date }}">
                    <div itemprop="reviewRating" itemscope itemtype="https://schema.org/Rating" class="hidden-schema">
                        <meta itemprop="ratingValue" content="5">
                    </div>
                </div>
            {% endfor %}
        </div>
    </div>
</section>

<section id="map">
    <div class="container">
        <h2>Где я принимаю</h2>
        <p><h3>{{ site.author.address }}</h3></p>
        <iframe src="https://yandex.ru/map-widget/v1/?z=12&ol=biz&oid=18459114169" width="100%" height="400" frameborder="0" class="map-iframe"></iframe>
    </div>
</section>

<!-- Floating WhatsApp Button -->
<a href="https://wa.me/{{ site.author.phonewhatsapp }}?text=Здравствуйте!%20Хочу%20записаться%20на%20консультацию." class="whatsapp-float" target="_blank">
    {% include whatsapp.html %}
</a>

<script>
    document.addEventListener("DOMContentLoaded", function() {
        // Перемещаем кнопку в body, чтобы она не зависела от transform родительских секций
        const floatBtn = document.querySelector('.whatsapp-float');
        if (floatBtn) {
            document.body.appendChild(floatBtn);
        }
    });
</script>