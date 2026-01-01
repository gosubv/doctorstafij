---
layout: default
title: Доктор Стафий | Эндокринолог-нутрициолог
---

<section id="hero" class="hero">
    <div class="container">
        <span class="badge-online">Консультация в клинике и онлайн</span>
        <h1 style="font-size: 3.5rem; margin: 20px 0;">Доктор Стафий</h1>
        <p style="font-size: 1.4rem; color: var(--primary); margin-bottom: 40px;">
            Стафий Диана Викторовна — Ваш эксперт в мире гормонального здоровья и осознанного питания.
        </p>
        <a href="#booking" class="btn-nav" style="padding: 20px 40px; font-size: 1.1rem; text-decoration: none;">Онлайн запись на консультацию</a>
    </div>
</section>

<section id="about" class="about-section">
    <div class="container">
        
        <div class="about-hero">
            <div class="about-image">
                <img src="{{ '/assets/img/doctor.png' | relative_url }}" alt="Стафий Диана Викторовна" class="doctor-img glass-panel">
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

<section id="certificates" style="background: #ffffff; padding: 80px 0;">
    <div class="container">
        <div style="display: flex; justify-content: space-between; align-items: flex-end; margin-bottom: 30px;">
            <div>
                <h2 style="margin-bottom: 10px;">Сертификаты и дипломы</h2>
                <p>Подтвержденная квалификация и постоянное обучение</p>
            </div>
            <div style="color: var(--accent-mint); font-size: 0.9rem; font-weight: bold;">
                Листайте вправо →
            </div>
        </div>

        <div class="diploma-carousel" itemscope itemtype="https://schema.org/EducationalOccupationalCredential">
            {% for item in site.data.diplomas %}
                <div class="diploma-card">
                    <img src="{{ item.image | relative_url }}" alt="{{ item.title }}" class="diploma-image" itemprop="image">
                    <div class="diploma-info">
                        <p itemprop="name">{{ item.title }}</p>
                    </div>
                </div>
            {% endfor %}
        </div>
        
        <p style="text-align: center; font-size: 0.8rem; color: #99aaaa; margin-top: 20px;">
            * Нажмите и удерживайте изображение, чтобы увеличить его
        </p>
    </div>
</section>

<section id="services" style="background: #f0f7f5;">
    <div class="container price-section">
        <h2 class="section-title" style="text-align: center;">Услуги и цены</h2>
        <div class="card-grid glass-panel">
            {% for item in site.data.services %}
                <div class="card price-item">
                    <h3>{{ item.title }}</h3>
                    <p>{{ item.text }}</p>
                    <span class="price-val"><p><b>{{ item.price }}</b></p></span>
                </div>
            {% endfor %}
        </div>
    </div>
</section>

<section id="blog" class="blog-section">
    <div class="container">
        <div style="display: flex; justify-content: space-between; align-items: flex-end; margin-bottom: 40px; flex-wrap: wrap; gap: 20px;">
            <div>
                <h2 style="font-size: 2.8rem; margin: 0;">Блог эксперта</h2>
                <p style="margin-top: 10px; color: #667e7e;">Актуальные темы эндокринологии и нутрициологии из моего Instagram</p>
            </div>
            <a href="{{ site.author.instagram_url }}" target="_blank" class="cta-button" style="background: transparent; border: 2px solid var(--accent-mint); color: var(--primary-dark);">
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

<section id="booking" style="background: linear-gradient(180deg, #f0f7f5 0%, #ffffff 100%); padding: 100px 0;">
    <div class="container">
        <div style="text-align: center; max-width: 800px; margin: 0 auto 50px auto;">
            <h2 style="font-size: 2.5rem; margin-bottom: 20px;">Запись на консультацию</h2>
            <p style="font-size: 1.1rem; color: #4a6363;">
                Выберите удобный тип приема и время в календаре ниже. После успешной записи вы получите подтверждение на указанную электронную почту.
            </p>
        </div>

        <div class="booking-container" style="background: white; border-radius: 20px; box-shadow: 0 15px 45px rgba(26, 77, 77, 0.08); overflow: hidden; border: 1px solid var(--accent-light);">
            <div style="background: var(--primary-dark); color: white; padding: 15px 30px; font-size: 0.9rem; display: flex; align-items: center; gap: 10px;">
                <span style="background: var(--accent-mint); width: 8px; height: 8px; border-radius: 50%;"></span>
                Выберите дату и доступный временной слот:
            </div>

            <iframe src="https://calendar.google.com/calendar/appointments/schedules/AcZssZ2i5tRlXYaJ8xwBVwlNWhMC_qlRVYVaD38cEBtIHm9Y6tfuqlr7fghSu_O610_o7RjaenYaAW40?gv=true" style="border: 0" width="100%" height="700" frameborder="0">
            </iframe>
        </div>

        <div style="text-align: center; margin-top: 30px;">
            <p style="font-size: 0.9rem; color: #99aaaa;">
                Если у вас возникли вопросы по записи, вы можете написать на <a href="mailto:{{ site.email }}" style="color: var(--primary-dark); font-weight: 600;">{{ site.email }}</a>
            </p>
        </div>
    </div>
</section>

<section id="reviews" style="background-color: #fbfdfd;">
    <div class="container">
        <div style="text-align: center; margin-bottom: 50px;">
            <h2 style="font-size: 2.8rem;">Отзывы пациентов</h2>
            <div style="width: 60px; height: 3px; background: var(--accent-mint); margin: 20px auto;"></div>
        </div>

        <div class="reviews-grid">
            {% for review in site.data.reviews limit:6 %}
                <div class="review-card" itemscope itemtype="https://schema.org/Review">
                    <div class="review-stars">
                        {% for i in (1..5) %}★{% endfor %}
                    </div>
                
                    <div class="review-text" itemprop="reviewBody">
                        {{ review.text }}
                    </div>

                    <div class="review-info">
                        <span class="author-name" itemprop="author">{{ review.name }}</span>
                    </div>

                    <meta itemprop="datePublished" content="{{ review.date }}">
                    <div itemprop="reviewRating" itemscope itemtype="https://schema.org/Rating" style="display:none;">
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
        <p>{{ site.author.address }}</p>
        <iframe src="https://yandex.ru/map-widget/v1/?z=12&ol=biz&oid=96035534355" width="100%" height="400" frameborder="0" style="border-radius: 15px;"></iframe>
    </div>
</section>
