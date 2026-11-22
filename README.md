<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Motive Academy</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: Arial, Helvetica, sans-serif; color: #1f2937; line-height: 1.6; background: #f9fafb; }
    .lang { position: absolute; top: 14px; right: 14px; display: flex; gap: 6px; }
    .lang button { border: 2px solid white; background: transparent; color: white; padding: 6px 12px; border-radius: 6px; cursor: pointer; font-weight: bold; }
    .lang button.active { background: white; color: #1d4ed8; }
    header { position: relative; background: #1d4ed8; color: white; text-align: center; padding: 80px 20px 64px; }
    header h1 { font-size: 2.6rem; margin-bottom: 10px; }
    header p { font-size: 1.2rem; opacity: 0.9; }
    .btn { display: inline-block; margin-top: 24px; background: white; color: #1d4ed8; padding: 12px 28px; border-radius: 8px; text-decoration: none; font-weight: bold; }
    section { max-width: 900px; margin: 0 auto; padding: 48px 20px; }
    h2 { color: #1d4ed8; margin-bottom: 20px; text-align: center; }
    .cards { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
    .card { background: white; border-radius: 12px; padding: 24px; box-shadow: 0 2px 8px rgba(0,0,0,0.08); }
    .card h3 { margin-bottom: 8px; color: #1d4ed8; }
    .contact { text-align: center; }
    .contact p { margin: 8px 0; font-size: 1.15rem; }
    .contact a { color: #1d4ed8; font-weight: bold; text-decoration: none; }
    footer { text-align: center; padding: 24px; color: #6b7280; font-size: 0.9rem; }
  </style>
</head>
<body>

  <header>
    <div class="lang">
      <button data-lang="en">EN</button>
      <button data-lang="ru">RU</button>
      <button data-lang="uz">UZ</button>
    </div>
    <h1>Motive Academy</h1>
    <p data-i18n="tagline"></p>
    <a class="btn" href="#contact" data-i18n="enroll"></a>
  </header>

  <section>
    <h2 data-i18n="aboutTitle"></h2>
    <p style="text-align:center;" data-i18n="aboutText"></p>
  </section>

  <section>
    <h2 data-i18n="coursesTitle"></h2>
    <div class="cards">
      <div class="card">
        <h3 data-i18n="c1t"></h3>
        <p data-i18n="c1d"></p>
      </div>
      <div class="card">
        <h3 data-i18n="c2t"></h3>
        <p data-i18n="c2d"></p>
      </div>
      <div class="card">
        <h3 data-i18n="c3t"></h3>
        <p data-i18n="c3d"></p>
      </div>
      <div class="card">
        <h3 data-i18n="c4t"></h3>
        <p data-i18n="c4d"></p>
      </div>
    </div>
  </section>

  <section id="contact" class="contact">
    <h2 data-i18n="contactTitle"></h2>
    <p><span data-i18n="phone"></span>: <a href="tel:+998933368050">+998 93 336 80 50</a></p>
    <p>Telegram: <a href="https://t.me/Motive_Academy_admin" target="_blank" rel="noopener">@Motive_Academy_admin</a></p>
  </section>

  <footer>&copy; 2026 Motive Academy</footer>

  <script>
    var T = {
      en: {
        tagline: "Learn with motivation. Reach your goals.",
        enroll: "Enroll Now",
        aboutTitle: "About Us",
        aboutText: "Motive Academy is a learning centre that helps students build knowledge and confidence with friendly teachers and a motivating atmosphere.",
        coursesTitle: "Our Courses",
        c1t: "General English", c1d: "Speaking, listening, reading, writing and grammar for all levels.",
        c2t: "IELTS", c2d: "Focused exam preparation with practice tests and proven strategies.",
        c3t: "Russian Language", c3d: "Learn to speak, read and write Russian with confidence.",
        c4t: "Mathematics", c4d: "School support and exam preparation, explained step by step.",
        contactTitle: "Contact Us",
        phone: "Phone"
      },
      ru: {
        tagline: "Учись с мотивацией. Достигай целей.",
        enroll: "Записаться",
        aboutTitle: "О нас",
        aboutText: "Motive Academy — учебный центр, который помогает ученикам обрести знания и уверенность благодаря дружелюбным преподавателям и мотивирующей атмосфере.",
        coursesTitle: "Наши курсы",
        c1t: "General English", c1d: "Разговорная речь, аудирование, чтение, письмо и грамматика для всех уровней.",
        c2t: "IELTS", c2d: "Целенаправленная подготовка к экзамену с пробными тестами и проверенными стратегиями.",
        c3t: "Русский язык", c3d: "Научитесь уверенно говорить, читать и писать по-русски.",
        c4t: "Математика", c4d: "Помощь по школьной программе и подготовка к экзаменам с пошаговыми объяснениями.",
        contactTitle: "Контакты",
        phone: "Телефон"
      },
      uz: {
        tagline: "Motivatsiya bilan o'rganing. Maqsadlaringizga erishing.",
        enroll: "Ro'yxatdan o'tish",
        aboutTitle: "Biz haqimizda",
        aboutText: "Motive Academy — samimiy o'qituvchilar va ilhomlantiruvchi muhit orqali o'quvchilarga bilim va ishonch beradigan o'quv markazi.",
        coursesTitle: "Kurslarimiz",
        c1t: "General English", c1d: "Barcha darajalar uchun gapirish, tinglash, o'qish, yozish va grammatika.",
        c2t: "IELTS", c2d: "Sinov testlari va samarali strategiyalar bilan imtihonga maqsadli tayyorgarlik.",
        c3t: "Rus tili", c3d: "Rus tilida ishonch bilan gapirish, o'qish va yozishni o'rganing.",
        c4t: "Matematika", c4d: "Maktab dasturi va imtihonlarga tayyorgarlik, bosqichma-bosqich tushuntirish bilan.",
        contactTitle: "Aloqa",
        phone: "Telefon"
      }
    };

    function setLang(l) {
      document.documentElement.lang = l;
      document.querySelectorAll("[data-i18n]").forEach(function (el) {
        el.textContent = T[l][el.getAttribute("data-i18n")];
      });
      document.querySelectorAll(".lang button").forEach(function (b) {
        b.classList.toggle("active", b.getAttribute("data-lang") === l);
      });
      try { localStorage.setItem("lang", l); } catch (e) {}
    }

    document.querySelectorAll(".lang button").forEach(function (b) {
      b.addEventListener("click", function () { setLang(b.getAttribute("data-lang")); });
    });

    var saved = "en";
    try { saved = localStorage.getItem("lang") || "en"; } catch (e) {}
    setLang(T[saved] ? saved : "en");
  </script>
</body>
</html>