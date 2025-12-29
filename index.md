---
layout: default
title: Доктор Стафий | Эндокринолог-нутрициолог
---

<section id="hero" class="hero">
    <div class="container">
        <span class="badge-online">Приём онлайн</span>
        <h1 style="font-size: 3.5rem; margin: 20px 0;">Доктор Стафий</h1>
        <p style="font-size: 1.4rem; color: var(--primary); margin-bottom: 40px;">
            Стафий Диана Викторовна — Ваш эксперт в мире гормонального здоровья и осознанного питания.
        </p>
        <a href="#booking" class="btn-nav" style="padding: 20px 40px; font-size: 1.1rem; text-decoration: none;">Записаться онлайн</a>
    </div>
</section>

<section id="about">
    <div class="container">
        <div style="display: flex; gap: 50px; flex-wrap: wrap; align-items: center;">
            <div style="flex: 1; min-width: 300px;">
                <h2 style="font-size: 2.5rem;">О враче</h2>
                <p><b>Стафий Диана Викторовна</b> — врач-эндокринолог первой категории, нутрициолог. Стаж работы более 12 лет.</p>
                <p>Специализируюсь на лечении патологий щитовидной железы, сахарного диабета, ожирения и коррекции дефицитных состояний.</p>
            </div>
            <div style="flex: 1; min-width: 300px; background: var(--accent); height: 500px; border-radius: 20px; overflow: hidden;">
                 <img src="./images/doctor.png" alt="Диана Викторовна" style="width:100%; height:100%; object-fit: cover;">
            </div>
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
                <img src="{{ item.image | relative_url }}" 
                     alt="{{ item.title }}" 
                     class="diploma-image" 
                     itemprop="image">
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
    <div class="container">
        <h2 style="text-align: center;">Услуги и цены</h2>
        <div class="card-grid">
            <div class="card">
                <h3>Эндокринолог</h3>
                <p>Первичная консультация, осмотр, план диагностики.</p>
                <p><b>10 000 ₸</b></p>
            </div>
            <div class="card">
                <h3>Нутрициолог</h3>
                <p>Разбор рациона, восполнение дефицитов витаминов.</p>
                <p><b>15 000 ₸</b></p>
            </div>
            <div class="card">
                <h3>Повторный прием</h3>
                <p>Коррекция терапии по результатам анализов.</p>
                <p><b>7 000 ₸</b></p>
            </div>
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

            <iframe 
                src="https://calendar.google.com/calendar/appointments/schedules/AcZssZ2i5tRlXYaJ8xwBVwlNWhMC_qlRVYVaD38cEBtIHm9Y6tfuqlr7fghSu_O610_o7RjaenYaAW40?gv=true" 
                style="border: 0" 
                width="100%" 
                height="700" 
                frameborder="0">
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
                    <div style="width: 45px; height: 45px; background: var(--accent-light); border-radius: 50%; display: flex; align-items: center; justify-content: center; color: var(--primary-dark); font-weight: bold;">
                        {{ review.name | slice: 0 }}
                    </div>
                    <div>
                        <span class="author-name" itemprop="author">{{ review.name }}</span>
                        <div style="font-size: 0.85rem; color: #99aaaa;">Пациент клиники</div>
                    </div>
                </div>

                <meta itemprop="datePublished" content="{{ review.date }}">
                <div itemprop="reviewRating" itemscope itemtype="https://schema.org/Rating" style="display:none;">
                    <meta itemprop="ratingValue" content="5">
                </div>
            </div>
            {% endfor %}
        </div>

        <div style="text-align: center; margin-top: 60px;">
            <a href="https://www.instagram.com/{{ site.author.instagram }}/" target="_blank" class="cta-button" style="background: white; color: var(--primary-dark); border: 2px solid var(--accent-mint);">
                Читать все отзывы в Instagram
            </a>
        </div>
    </div>
</section>

<section id="map">
    <div class="container">
        <h2>Где я принимаю</h2>
        <p>г. Петропавловск, ул. Ауэзова 133</p>
        <iframe src="https://yandex.kz/maps/org/doktor_stafiy/96035534355/?ll=69.151413%2C54.891331&z=11" width="100%" height="400" frameborder="0" style="border-radius: 15px;"></iframe>
    </div>
    
</section>
