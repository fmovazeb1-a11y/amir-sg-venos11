# amir-sg-venos11
amir-sg-venos11
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080b1c">
<title>AMIR SG | سیاره زهره</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;700;900&display=swap');

:root {
  --bg: #080b1c;
  --panel: #121831;
  --gold: #ffc77d;
  --orange: #ff784f;
  --white: #f5f6ff;
  --muted: #aab2d0;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Vazirmatn', sans-serif;
  color: var(--white);
  background:
    radial-gradient(ellipse at 80% 5%, #382448 0, transparent 35%),
    radial-gradient(ellipse at 10% 50%, #14264a 0, transparent 35%),
    var(--bg);
  line-height: 1.9;
  overflow-x: hidden;
}

a {
  color: inherit;
  text-decoration: none;
}

header {
  position: sticky;
  top: 0;
  z-index: 10;
  padding: 14px 6%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  background: #080b1ce8;
  border-bottom: 1px solid #ffffff15;
  backdrop-filter: blur(16px);
}

.logo {
  font-weight: 900;
  font-size: 1.3rem;
  color: var(--gold);
  letter-spacing: 1px;
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
  font-size: .9rem;
}

nav a {
  color: var(--muted);
  transition: .25s;
}

nav a:hover {
  color: var(--gold);
}

.hero {
  min-height: 86vh;
  padding: 70px 7%;
  display: grid;
  grid-template-columns: 1.1fr .9fr;
  align-items: center;
  gap: 35px;
}

.eyebrow {
  color: var(--gold);
  font-size: .9rem;
  letter-spacing: 2px;
  font-weight: 700;
}

h1 {
  font-size: clamp(2.6rem, 7vw, 5.5rem);
  line-height: 1.25;
  margin: 15px 0;
  font-weight: 900;
}

h1 span {
  background: linear-gradient(90deg, #ffe3a8, #ff875e);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.hero p {
  color: var(--muted);
  max-width: 590px;
  margin-bottom: 25px;
}

.actions {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

.btn {
  display: inline-block;
  padding: 11px 21px;
  border-radius: 12px;
  font-weight: 700;
  border: 1px solid #ffffff24;
  transition: .25s;
  cursor: pointer;
  font-family: inherit;
  font-size: .95rem;
}

.btn-primary {
  color: #24140d;
  background: linear-gradient(110deg, #ffe0a1, #ff895d);
  border: none;
}

.btn:hover {
  transform: translateY(-3px);
}

.planet-stage {
  min-height: 370px;
  display: grid;
  place-items: center;
  position: relative;
}

.planet {
  width: min(66vw, 310px);
  aspect-ratio: 1;
  border-radius: 50%;
  position: relative;
  background:
    radial-gradient(ellipse at 28% 23%, #fff0c4 0, transparent 13%),
    repeating-linear-gradient(
      165deg,
      #dba36b 0 12px,
      #f1c48b 13px 22px,
      #b87850 23px 30px,
      #f6d5a0 31px 42px
    );
  box-shadow:
    inset -35px -25px 65px #351a23cc,
    inset 12px 10px 35px #fff3cf99,
    0 0 50px #ffad6860,
    0 0 110px #ff8d4b30;
  animation: float 6s ease-in-out infinite;
}

.planet::before {
  content: "";
  position: absolute;
  inset: -15px;
  border-radius: 50%;
  border: 1px solid #ffd8a72e;
  transform: rotate(-24deg) scaleY(.25);
}

.planet::after {
  content: "";
  position: absolute;
  inset: 8%;
  border-radius: 50%;
  background: linear-gradient(110deg, transparent 35%, #351b2b55 90%);
}

.orbit {
  position: absolute;
  width: 360px;
  max-width: 95%;
  aspect-ratio: 1;
  border: 1px solid #ffd39c32;
  border-radius: 50%;
  transform: rotate(-25deg) scaleY(.36);
}

.orbit-dot {
  position: absolute;
  width: 10px;
  height: 10px;
  top: 18%;
  left: 17%;
  border-radius: 50%;
  background: var(--gold);
  box-shadow: 0 0 20px var(--gold);
}

@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-15px); }
}

.section {
  padding: 75px 7%;
}

.section-heading {
  text-align: center;
  margin-bottom: 35px;
}

.section-heading h2 {
  font-size: clamp(1.7rem, 4vw, 2.7rem);
  margin-bottom: 8px;
}

.section-heading p {
  color: var(--muted);
}

.cards {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 15px;
}

.card {
  background: linear-gradient(145deg, #171e3b, #0d1228);
  border: 1px solid #ffffff12;
  border-radius: 20px;
  padding: 23px;
  transition: .3s;
}

.card:hover {
  transform: translateY(-5px);
  border-color: #ffc77d65;
}

.stat-number {
  color: var(--gold);
  font-size: 1.7rem;
  font-weight: 900;
  direction: ltr;
  text-align: right;
}

.card h3 {
  margin: 5px 0;
}

.card p {
  color: var(--muted);
  font-size: .92rem;
}

.two-columns {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 22px;
  align-items: stretch;
}

.info-panel {
  padding: 28px;
  background: #121831c9;
  border: 1px solid #ffffff12;
  border-radius: 22px;
}

.info-panel h3 {
  color: var(--gold);
  margin-bottom: 12px;
}

.info-panel p {
  color: var(--muted);
  margin-bottom: 12px;
}

.fact-list {
  list-style: none;
}

.fact-list li {
  padding: 9px 0;
  border-bottom: 1px solid #ffffff12;
}

.fact-list li::before {
  content: "✦ ";
  color: var(--gold);
}

.highlight {
  color: var(--gold);
  font-weight: 700;
}

.comparison {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 20px;
}

.comparison button {
  background: #171e3b;
  color: var(--white);
  border: 1px solid #ffffff20;
  border-radius: 10px;
  padding: 10px 18px;
  cursor: pointer;
  font-family: inherit;
}

.comparison button.active {
  background: var(--gold);
  color: #21150d;
}

.compare-result {
  max-width: 650px;
  margin: auto;
  text-align: center;
  padding: 25px;
  border-radius: 20px;
  background: #121831;
  border: 1px solid #ffffff12;
}

.compare-result h3 {
  color: var(--gold);
  margin-bottom: 8px;
}

.timeline {
  max-width: 760px;
  margin: auto;
  border-right: 2px solid #ffc77d66;
  padding-right: 25px;
}

.timeline-item {
  position: relative;
  padding: 0 10px 28px 0;
}

.timeline-item::before {
  content: "";
  position: absolute;
  right: -33px;
  top: 10px;
  width: 13px;
  height: 13px;
  border-radius: 50%;
  background: var(--gold);
  box-shadow: 0 0 15px #ffc77d80;
}

.timeline-item h3 {
  color: var(--gold);
}

.timeline-item p {
  color: var(--muted);
}

.quiz {
  max-width: 700px;
  margin: auto;
  padding: 28px;
  background: #121831;
  border: 1px solid #ffffff15;
  border-radius: 22px;
}

.quiz-question {
  margin-bottom: 22px;
}

.quiz-question h3 {
  margin-bottom: 12px;
}

.quiz-option {
  display: block;
  width: 100%;
  text-align: right;
  margin: 8px 0;
  padding: 12px 15px;
  border-radius: 10px;
  color: var(--white);
  background: #1b2342;
  border: 1px solid #ffffff12;
  font-family: inherit;
  cursor: pointer;
}

.quiz-option:hover {
  border-color: var(--gold);
}

.quiz-option:disabled {
  cursor: default;
  opacity: .85;
}

#quiz-result {
  margin-top: 18px;
  color: var(--gold);
  font-weight: 700;
}

footer {
  padding: 30px 7%;
  text-align: center;
  color: var(--muted);
  border-top: 1px solid #ffffff12;
}

footer strong {
  color: var(--gold);
}

@media (max-width: 850px) {
  .hero {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .hero p {
    margin-inline: auto;
  }

  .actions {
    justify-content: center;
  }

  .planet-stage {
    min-height: 320px;
  }

  .cards {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .two-columns {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  header {
    align-items: flex-start;
    flex-direction: column;
  }

  nav {
    gap: 12px;
    font-size: .82rem;
  }

  .section {
    padding: 55px 5%;
  }

  .cards {
    grid-template-columns: 1fr;
  }

  .planet-stage {
    min-height: 270px;
  }

  .planet {
    width: 230px;
  }

  .quiz {
    padding: 18px;
  }
}
</style>
</head>

<body>
<header>
  <a class="logo" href="#home">AMIR SG ✦</a>
  <nav>
    <a href="#facts">اطلاعات</a>
    <a href="#climate">اقلیم</a>
    <a href="#compare">مقایسه</a>
    <a href="#missions">کاوش‌ها</a>
    <a href="#quiz">آزمون</a>
  </nav>
</header>

<main>
<section class="hero" id="home">
  <div>
    <div class="eyebrow">VENUS • THE MYSTERIOUS PLANET</div>
    <h1>زهره؛<br><span>جهنمی درخشان</span></h1>
    <p>
      درخشان‌ترین سیارهٔ آسمان شب، جهانی پوشیده از ابرهای ضخیم،
      با فشار خردکننده و دمایی که حتی از عطارد هم بیشتر است.
      به کاوش یکی از شگفت‌انگیزترین سیاره‌های منظومهٔ شمسی خوش آمدی!
    </p>
    <div class="actions">
      <a class="btn btn-primary" href="#facts">شروع کاوش 🚀</a>
      <a class="btn" href="#quiz">آزمون دانش فضایی</a>
    </div>
  </div>

  <div class="planet-stage" aria-label="تصویر گرافیکی سیاره زهره">
    <div class="orbit"><div class="orbit-dot"></div></div>
    <div class="planet"></div>
  </div>
</section>

<section class="section" id="facts">
  <div class="section-heading">
    <h2>پروندهٔ علمی زهره</h2>
    <p>اعداد کلیدی برای شناخت همسایهٔ درخشان زمین</p>
  </div>

  <div class="cards">
    <article class="card">
      <div class="stat-number">≈ 465°C</div>
      <h3>دمای سطح</h3>
      <p>دمای میانگین سطح زهره حدود ۴۶۵ درجهٔ سانتی‌گراد است.</p>
    </article>

    <article class="card">
      <div class="stat-number">≈ 12,104 km</div>
      <h3>قطر سیاره</h3>
      <p>اندازهٔ زهره به زمین نزدیک است و گاهی خواهر زمین نامیده می‌شود.</p>
    </article>

    <article class="card">
      <div class="stat-number">225 days</div>
      <h3>سال زهره</h3>
      <p>یک دور گردش زهره به دور خورشید حدود ۲۲۵ روز زمینی طول می‌کشد.</p>
    </article>

    <article class="card">
      <div class="stat-number">92 bar</div>
      <h3>فشار سطح</h3>
      <p>فشار جو در سطح زهره تقریباً ۹۲ برابر فشار جو زمین است.</p>
    </article>
  </div>
</section>
<section class="section" id="climate">
  <div class="section-heading">
    <h2>🔥 سفری به جهنم منظومهٔ شمسی</h2>
    <p>چرا زهره با وجود فاصلهٔ بیشتر از خورشید، از عطارد داغ‌تر است؟</p>
  </div>

  <div class="two-columns">
    <article class="info-panel">
      <h3>🌫️ جوّی که گرما را حبس می‌کند</h3>
      <p>
        جوّ زهره عمدتاً از دی‌اکسید کربن تشکیل شده است.
        ابرهای ضخیم آن نیز حاوی قطره‌های اسید سولفوریک هستند.
        این جوّ بسیار متراکم، گرما را به‌شدت در نزدیکی سطح نگه می‌دارد.
      </p>
      <ul class="fact-list">
        <li>بخش عمدهٔ جوّ: دی‌اکسید کربن</li>
        <li>ابرهای ضخیم حاوی اسید سولفوریک</li>
        <li>اثر گلخانه‌ای بسیار شدید</li>
        <li>فشار سطح: حدود ۹۲ برابر زمین</li>
      </ul>
    </article>

    <article class="info-panel">
      <h3>🌡️ سطحی با شرایط افراطی</h3>
      <p>
        دمای سطح زهره در سراسر سیاره بسیار بالاست.
        این دما برای ذوب سرب کافی است و بیشتر فضاپیماهای
        فرودآمده بر سطح آن فقط مدت کوتاهی دوام آورده‌اند.
      </p>
      <ul class="fact-list">
        <li>دمای سطح: حدود ۴۶۵ درجهٔ سانتی‌گراد</li>
        <li>آب مایع پایدار روی سطح وجود ندارد</li>
        <li>بادهای جوّی در ارتفاعات می‌توانند بسیار سریع باشند</li>
        <li>چرخش سیاره به دور محور خود بسیار آهسته است</li>
      </ul>
    </article>

    <article class="info-panel">
      <h3>🌪️ روزی طولانی و عجیب</h3>
      <p>
        زهره در جهت مخالف بسیاری از سیاره‌های منظومهٔ شمسی
        می‌چرخد؛ به این نوع چرخش، چرخش پس‌گرد می‌گویند.
      </p>
      <p>
        یک دور چرخش زهره به دور محور خودش حدود ۲۴۳ روز زمینی
        طول می‌کشد؛ یعنی حتی از سال زهره، که حدود ۲۲۵ روز است،
        طولانی‌تر است!
      </p>
    </article>

    <article class="info-panel">
      <h3>🪨 سطح و ساختار داخلی</h3>
      <p>
        زهره یک سیارهٔ سنگی است. سطح آن شامل دشت‌های آتشفشانی،
        کوهستان‌ها، دهانه‌های برخوردی و ساختارهای زمین‌شناختی
        گوناگون است.
      </p>
      <p>
        دانشمندان شواهد فراوانی از فعالیت آتشفشانی گذشته پیدا
        کرده‌اند و بررسی می‌کنند که آیا برخی آتشفشان‌ها هنوز
        فعال‌اند یا نه.
      </p>
    </article>
  </div>
</section>

<section class="section" id="compare">
  <div class="section-heading">
    <h2>🌍 زهره در برابر همسایه‌ها</h2>
    <p>روی هر دکمه بزن تا اطلاعات سیاره تغییر کند.</p>
  </div>

  <div class="comparison">
    <button class="active" data-planet="venus" onclick="showPlanet('venus', this)">
      زهره
    </button>
    <button data-planet="earth" onclick="showPlanet('earth', this)">
      زمین
    </button>
    <button data-planet="mercury" onclick="showPlanet('mercury', this)">
      عطارد
    </button>
  </div>

  <div class="compare-result" aria-live="polite">
    <h3 id="compare-name">سیارهٔ زهره</h3>
    <p id="compare-description">
      زهره دومین سیاره از خورشید است و به دلیل اثر گلخانه‌ای
      شدید، داغ‌ترین سطح را در میان سیاره‌های منظومهٔ شمسی دارد.
    </p>
    <div class="cards" style="margin-top:20px; text-align:right">
      <article class="card">
        <div class="stat-number" id="compare-temp">465°C</div>
        <h3>دمای سطح</h3>
      </article>
      <article class="card">
        <div class="stat-number" id="compare-year">225 روز</div>
        <h3>طول سال</h3>
      </article>
      <article class="card">
        <div class="stat-number" id="compare-moons">۰</div>
        <h3>تعداد قمر</h3>
      </article>
      <article class="card">
        <div class="stat-number" id="compare-distance">108.2 میلیون km</div>
        <h3>فاصلهٔ میانگین از خورشید</h3>
      </article>
    </div>
  </div>
</section>

<script>
const planetData = {
  venus: {
    name: "سیارهٔ زهره",
    description:
      "زهره دومین سیاره از خورشید است و به دلیل اثر گلخانه‌ای شدید، داغ‌ترین سطح را در میان سیاره‌های منظومهٔ شمسی دارد.",
    temp: "465°C",
    year: "225 روز",
    moons: "۰",
    distance: "108.2 میلیون km"
  },

  earth: {
    name: "سیارهٔ زمین",
    description:
      "زمین سومین سیاره از خورشید است. وجود آب مایع پایدار روی سطح و شرایط مناسب، آن را به تنها جهان شناخته‌شدهٔ دارای حیات تبدیل کرده است.",
    temp: "حدود 15°C",
    year: "365 روز",
    moons: "۱",
    distance: "149.6 میلیون km"
  },

  mercury: {
    name: "سیارهٔ عطارد",
    description:
      "عطارد نزدیک‌ترین سیاره به خورشید است. چون جوّ قابل‌توجهی برای نگه‌داشتن گرما ندارد، اختلاف دمای شب و روز آن بسیار زیاد است.",
    temp: "حدود 167°C",
    year: "88 روز",
    moons: "۰",
    distance: "57.9 میلیون km"
  }
};

function showPlanet(planet, button) {
  const data = planetData[planet];

  document.getElementById("compare-name").textContent = data.name;
  document.getElementById("compare-description").textContent = data.description;
  document.getElementById("compare-temp").textContent = data.temp;
  document.getElementById("compare-year").textContent = data.year;
  document.getElementById("compare-moons").textContent = data.moons;
  document.getElementById("compare-distance").textContent = data.distance;

  document.querySelectorAll(".comparison button").forEach(function (item) {
    item.classList.remove("active");
  });

  button.classList.add("active");
}
</script>
<section class="section" id="missions">
  <div class="section-heading">
    <h2>🛰️ تاریخچهٔ کاوش زهره</h2>
    <p>از نخستین ملاقات‌های فضایی تا مأموریت‌های مدرن</p>
  </div>

  <div class="timeline">
    <article class="timeline-item">
      <h3>۱۹۶۲ — مارینر ۲</h3>
      <p>
        فضاپیمای مارینر ۲ ناسا از کنار زهره عبور کرد و نخستین
        مأموریت موفق برای بررسی یک سیاره از فاصلهٔ نزدیک بود.
      </p>
    </article>

    <article class="timeline-item">
      <h3>۱۹۷۰ — ونرا ۷</h3>
      <p>
        کاوشگر ونرا ۷ شوروی روی زهره فرود آمد و نخستین داده‌های
        ارسال‌شده از سطح یک سیارهٔ دیگر را به زمین فرستاد.
      </p>
    </article>

    <article class="timeline-item">
      <h3>۱۹۷۵ — ونرا ۹</h3>
      <p>
        ونرا ۹ تصاویر سطح زهره را به زمین فرستاد و شناخت دانشمندان
        از محیط سخت این سیاره را افزایش داد.
      </p>
    </article>

    <article class="timeline-item">
      <h3>۱۹۹۰ — ماژلان</h3>
      <p>
        فضاپیمای ماژلان با استفاده از رادار، نقشه‌های دقیقی از
        سطح زهره تهیه کرد؛ زیرا ابرهای ضخیم اجازهٔ مشاهدهٔ مستقیم
        سطح با دوربین معمولی را نمی‌دهند.
      </p>
    </article>

    <article class="timeline-item">
      <h3>۲۰۰۶ — ونوس اکسپرس</h3>
      <p>
        مأموریت آژانس فضایی اروپا جو، ابرها و ویژگی‌های آب‌وهوایی
        زهره را بررسی کرد.
      </p>
    </article>

    <article class="timeline-item">
      <h3>۲۰۱۵ — آکاتسوکی</h3>
      <p>
        فضاپیمای ژاپنی آکاتسوکی پس از ورود به مدار زهره، جوّ و
        الگوهای گردش بادهای این سیاره را مطالعه کرد.
      </p>
    </article>
  </div>
</section>

<section class="section" id="quiz">
  <div class="section-heading">
    <h2>🧠 آزمون دانش فضایی</h2>
    <p>به سه پرسش پاسخ بده و امتیازت رو ببین!</p>
  </div>

  <div class="quiz">
    <div class="quiz-question" data-answer="1">
      <h3>۱. دمای سطح زهره تقریباً چقدر است؟</h3>

      <button class="quiz-option" onclick="answerQuestion(this, 0)">
        حدود ۱۵ درجهٔ سانتی‌گراد
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 1)">
        حدود ۴۶۵ درجهٔ سانتی‌گراد
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 2)">
        حدود منفی ۱۰۰ درجهٔ سانتی‌گراد
      </button>
    </div>

    <div class="quiz-question" data-answer="2">
      <h3>۲. کدام گاز بخش عمدهٔ جوّ زهره را تشکیل می‌دهد؟</h3>

      <button class="quiz-option" onclick="answerQuestion(this, 0)">
        اکسیژن
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 1)">
        نیتروژن
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 2)">
        دی‌اکسید کربن
      </button>
    </div>

    <div class="quiz-question" data-answer="0">
      <h3>۳. کدام فضاپیما نقشه‌های راداری مهمی از سطح زهره تهیه کرد؟</h3>

      <button class="quiz-option" onclick="answerQuestion(this, 0)">
        ماژلان
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 1)">
        هابل
      </button>

      <button class="quiz-option" onclick="answerQuestion(this, 2)">
        وویجر ۱
      </button>
    </div>

    <p id="quiz-result" aria-live="polite">
      هنوز به پرسش‌ها پاسخ ندادی. موفق باشی! 🌟
    </p>

    <button class="btn btn-primary" onclick="resetQuiz()">
      🔄 شروع دوباره
    </button>
  </div>
</section>

<section class="section">
  <div class="info-panel" style="text-align:center">
    <div class="eyebrow">THE UNIVERSE IS WAITING</div>
    <h2 style="margin:10px 0">هر سیاره، یک دنیای تازه 🌌</h2>
    <p>
      مطالعهٔ زهره به ما کمک می‌کند اثر گلخانه‌ای، تحول جوّ سیارات
      و تفاوت جهان‌های سنگی منظومهٔ شمسی را بهتر بشناسیم.
      هنوز پرسش‌های زیادی دربارهٔ گذشته و آیندهٔ این سیاره وجود دارد.
    </p>
  </div>
</section>
</main>

<footer>
  <p>
    ساخته‌شده با علاقه به علم و فضا توسط
    <strong>AMIR SG</strong>
  </p>
  <p>پروژهٔ پژوهشی سیارهٔ زهره | پایهٔ هفتم</p>
  <p>© 2026 AMIR SG — Venus Research Project</p>
</footer>

<script>
let quizScore = 0;
let answeredQuestions = 0;

function answerQuestion(button, selectedAnswer) {
  const question = button.closest(".quiz-question");

  if (question.dataset.answered === "true") {
    return;
  }

  question.dataset.answered = "true";

  const correctAnswer = Number(question.dataset.answer);
  const options = question.querySelectorAll(".quiz-option");

  options.forEach(function (option) {
    option.disabled = true;
  });

  if (selectedAnswer === correctAnswer) {
    quizScore++;

    button.style.borderColor = "#70e1a1";
    button.style.background = "#164634";

    question.insertAdjacentHTML(
      "beforeend",
      '<p style="color:#70e1a1;margin-top:8px">✅ آفرین! پاسخ درست بود.</p>'
    );
  } else {
    button.style.borderColor = "#ff7777";
    button.style.background = "#51252e";

    options[correctAnswer].style.borderColor = "#70e1a1";
    options[correctAnswer].style.background = "#164634";

    question.insertAdjacentHTML(
      "beforeend",
      '<p style="color:#ffb1b1;margin-top:8px">❌ این پاسخ درست نبود؛ پاسخ صحیح با رنگ سبز مشخص شده.</p>'
    );
  }

  answeredQuestions++;

  const result = document.getElementById("quiz-result");

  if (answeredQuestions < 3) {
    result.textContent =
      "تا اینجا " + answeredQuestions +
      " پرسش از ۳ پرسش رو جواب دادی.";
  } else {
    let message = "";

    if (quizScore === 3) {
      message = "عالی بود! تو یک کاوشگر حرفه‌ای هستی! 🚀";
    } else if (quizScore === 2) {
      message = "خیلی خوب بود! فقط یک نکته رو مرور کن. 🌟";
    } else if (quizScore === 1) {
      message = "شروع خوبی بود! با مطالعه بیشتر بهتر می‌شی. 💪";
    } else {
      message = "وقتشه دوباره مطالب سایت رو مرور کنی! 📚";
    }

    result.textContent =
      "امتیاز نهایی: " + quizScore + " از ۳ — " + message;
  }
}

function resetQuiz() {
  quizScore = 0;
  answeredQuestions = 0;

  document.querySelectorAll(".quiz-question").forEach(function (question) {
    delete question.dataset.answered;

    question.querySelectorAll(".quiz-option").forEach(function (option) {
      option.disabled = false;
      option.style.borderColor = "";
      option.style.background = "";
    });

    question.querySelectorAll("p").forEach(function (paragraph) {
      paragraph.remove();
    });
  });

  document.getElementById("quiz-result").textContent =
    "هنوز به پرسش‌ها پاسخ ندادی. موفق باشی! 🌟";
}
</script>

</body>
</html>