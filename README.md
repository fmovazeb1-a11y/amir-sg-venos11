# amir-sg-venos11
amir-sg-venos11

<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#0b0814">
<meta name="description" content="پروژه پژوهشی و تعاملی سیاره زهره، ساخته‌شده توسط AMIR SG">
<title>AMIR SG | کاوش در سیاره زهره</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;700;900&display=swap');

:root {
  --bg:#0b0814;
  --panel:#171225;
  --gold:#ffc27c;
  --orange:#ff704c;
  --text:#fff7f0;
  --muted:#c7bbd5;
  --line:#ffffff18;
}
* {box-sizing:border-box}
html {scroll-behavior:smooth;scroll-padding-top:100px}
body {
  margin:0;
  background:radial-gradient(ellipse at 80% 0%,#48203a55,transparent 40%),var(--bg);
  color:var(--text);
  font-family:'Vazirmatn',Tahoma,sans-serif;
  line-height:2;
}
a {color:var(--gold);text-decoration:none}
a:hover {text-decoration:underline}
button {font:inherit;cursor:pointer}
.progress {position:fixed;top:0;right:0;height:3px;width:0;background:linear-gradient(90deg,var(--orange),var(--gold));z-index:100}
header {position:sticky;top:0;z-index:50;background:#0b0814ed;backdrop-filter:blur(14px);border-bottom:1px solid var(--line)}
.nav {max-width:1120px;margin:auto;padding:12px 20px;display:flex;justify-content:space-between;align-items:center;gap:12px}
.logo {font-weight:900;font-size:20px;white-space:nowrap;color:var(--gold)}
nav {display:flex;flex-wrap:wrap;gap:14px;font-size:13px}
nav a {color:var(--muted)}
nav a:hover {color:var(--gold)}
.hero {max-width:1120px;margin:auto;padding:65px 22px;min-height:510px;display:grid;grid-template-columns:1.1fr .9fr;align-items:center;gap:30px}
.eyebrow {color:var(--gold);font-size:12px;font-weight:bold;letter-spacing:1px}
h1 {font-size:clamp(43px,7vw,76px);line-height:1.35;margin:12px 0}
.gradient {background:linear-gradient(100deg,#fff2d8,#ffb86c,#ff6948);color:transparent;background-clip:text;-webkit-background-clip:text}
.lead {color:var(--muted);max-width:590px}
.actions {display:flex;flex-wrap:wrap;gap:12px;margin-top:24px}
.btn {display:inline-block;border:1px solid var(--line);border-radius:12px;padding:9px 17px;color:var(--text);background:#21182d;font-weight:bold}
.btn.primary {background:linear-gradient(110deg,var(--gold),var(--orange));color:#241020;border:0}
.planet-wrap {min-height:320px;display:grid;place-items:center;position:relative;overflow:hidden}
.planet {width:min(64vw,270px);aspect-ratio:1;border-radius:50%;background:repeating-linear-gradient(160deg,#f4c18a 0 12px,#c47c59 16px,#f7d29b 27px,#a85d50 38px);box-shadow:inset -32px -20px 55px #321324bb,inset 10px 5px 25px #fff2b866,0 0 60px #ff824b35;animation:float 6s ease-in-out infinite}
.orbit {position:absolute;width:340px;height:120px;border:1px solid #ffc17a50;border-radius:50%;transform:rotate(-22deg)}
.star {position:absolute;color:var(--gold);animation:twinkle 2s infinite alternate}
@keyframes float {50%{transform:translateY(-12px)}}
@keyframes twinkle {to{opacity:.3}}
.stats {max-width:1050px;margin:0 auto 40px;padding:0 20px;display:grid;grid-template-columns:repeat(4,1fr);gap:12px}
.stat,.card,.fact,.quiz-box {background:linear-gradient(145deg,#1c162b,#110d1c);border:1px solid var(--line);border-radius:17px}
.stat {text-align:center;padding:16px 8px}
.stat strong {display:block;color:var(--gold);font-size:24px}
.stat span {color:var(--muted);font-size:12px}
section {max-width:1080px;margin:auto;padding:38px 22px}
.section-head {margin-bottom:22px}
h2 {font-size:clamp(26px,4vw,35px);margin:5px 0}
.section-head p,.muted {color:var(--muted)}
.grid {display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px}
.card {padding:20px;overflow-wrap:anywhere}
.card h3 {color:var(--gold);margin:5px 0 10px}
.card p {font-size:14px;color:var(--muted);margin-bottom:0}
.icon {font-size:28px}
.highlight {padding:25px;border:1px solid #ffb56b44;background:linear-gradient(120deg,#48233466,#171225);border-radius:18px}
.highlight strong {color:var(--gold)}
.table-wrap {overflow-x:auto;border-radius:12px}
table {width:100%;border-collapse:collapse;min-width:420px;font-size:13px}
th,td {border:1px solid var(--line);padding:10px;text-align:right}
th {background:#382138;color:var(--gold)}
td {background:#151020}
.fact-list {display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px}
.fact {padding:15px;font-size:14px}
.fact b {color:var(--gold)}
.quiz-box {padding:23px}
.option {display:block;width:100%;text-align:right;padding:11px 14px;margin:9px 0;border:1px solid var(--line);border-radius:10px;color:var(--text);background:#21192f}
.option:hover:not(:disabled) {border-color:var(--gold)}
.option:disabled {opacity:1;cursor:default}
#feedback {color:var(--gold);font-weight:bold;min-height:30px}
#result {font-size:19px;font-weight:bold;color:var(--gold)}
.small {font-size:12px;color:var(--muted)}
footer {margin-top:35px;border-top:1px solid var(--line);padding:28px 18px;text-align:center;color:var(--muted);font-size:13px}
footer strong {color:var(--gold)}
@media(max-width:740px) {
 .nav {align-items:flex-start;flex-direction:column}
 nav {gap:10px}
 .hero {grid-template-columns:1fr;padding-top:40px;gap:0}
 .planet-wrap {min-height:285px}
 .stats {grid-template-columns:repeat(2,1fr)}
 .grid {grid-template-columns:1fr}
 .fact-list {grid-template-columns:1fr}
}
@media(prefers-reduced-motion:reduce) {
 html {scroll-behavior:auto}
 .planet,.star {animation:none}
}
</style>
</head>

<body>
<div class="progress" id="progress"></div>

<header>
  <div class="nav">
    <a class="logo" href="#home">✦ AMIR SG</a>
    <nav aria-label="منوی اصلی">
      <a href="#intro">معرفی</a>
      <a href="#science">ویژگی‌ها</a>
      <a href="#compare">مقایسه</a>
      <a href="#missions">مأموریت‌ها</a>
      <a href="#quiz">آزمون</a>
      <a href="#sources">منابع</a>
    </nav>
  </div>
</header>

<main>
  <div class="hero" id="home">
    <div>
      <span class="eyebrow">ASTRONOMY • RESEARCH PROJECT</span>
      <h1>سفری به<br><span class="gradient">سیاره زهره</span></h1>
      <p class="lead">
        جهانی پوشیده از ابرهای ضخیم، با دمایی طاقت‌فرسا و
        فشاری بسیار زیاد؛ سیاره‌ای که اندازه‌اش به زمین
        شباهت دارد، اما محیط آن کاملاً متفاوت است.
      </p>
      <div class="actions">
        <a class="btn primary" href="#intro">شروع کاوش ←</a>
        <a class="btn" href="#quiz">🧠 آزمون فضانوردی</a>
      </div>
    </div>
    <div class="planet-wrap" role="img" aria-label="تصویرسازی گرافیکی سیاره زهره">
      <span class="star" style="top:12%;right:18%">✦</span>
      <span class="star" style="bottom:18%;left:13%">✧</span>
      <span class="star" style="top:28%;left:15%">·</span>
      <div class="orbit"></div>
      <div class="planet"></div>
    </div>
  </div>

  <div class="stats">
    <div class="stat"><strong>۴۶۵°C</strong><span>دمای تقریبی سطح</span></div>
    <div class="stat"><strong>۲۲۵ روز</strong><span>یک سال زهره</span></div>
    <div class="stat"><strong>۱۲٬۱۰۴</strong><span>قطر به کیلومتر</span></div>
    <div class="stat"><strong>۹۲ برابر</strong><span>فشار تقریبی جو زمین</span></div>
  </div>

  <section id="intro">
    <div class="section-head">
      <span class="eyebrow">01 / INTRODUCTION</span>
      <h2>زهره چه سیاره‌ای است؟</h2>
      <p>همسایه زمین؛ اما با شرایط محیطی بسیار متفاوت.</p>
    </div>
    <div class="grid">
      <article class="card">
        <div class="icon">✨</div>
        <h3>ستاره شامگاهی؟</h3>
        <p>زهره ستاره نیست؛ سیاره‌ای است که به دلیل درخشندگی زیاد، گاهی پس از غروب یا پیش از طلوع خورشید دیده می‌شود.</p>
      </article>
      <article class="card">
        <div class="icon">🔥</div>
        <h3>داغ‌ترین سیاره</h3>
        <p>زهره از عطارد داغ‌تر است. جو ضخیم و سرشار از دی‌اکسید کربن، گرما را به‌شدت در نزدیکی سطح نگه می‌دارد.</p>
      </article>
      <article class="card">
        <div class="icon">🌍</div>
        <h3>دوقلوی زمین؟</h3>
        <p>اندازه و ساختار کلی زهره به زمین شباهت دارد؛ اما شرایط سطح آن برای انسان بسیار نامناسب است.</p>
      </article>
    </div>
  </section>

  <section id="science">
    <div class="section-head">
      <span class="eyebrow">02 / SCIENTIFIC DATA</span>
      <h2>پرونده علمی زهره</h2>
      <p>ویژگی‌های فیزیکی، جوی و مداری این سیاره.</p>
    </div>
    <div class="grid">
      <article class="card">
        <div class="icon">🌡️</div>
        <h3>دمای سطح</h3>
        <p>دمای متوسط سطح نزدیک به ۴۶۵ درجه سانتی‌گراد است؛ به‌اندازه‌ای گرم که سرب در آن ذوب می‌شود.</p>
      </article>
      <article class="card">
        <div class="icon">☁️</div>
        <h3>جو سیاره</h3>
        <p>جو زهره عمدتاً از دی‌اکسید کربن تشکیل شده و ابرهای آن حاوی قطرات اسید سولفوریک هستند.</p>
      </article>
      <article class="card">
        <div class="icon">🧭</div>
        <h3>چرخش وارونه</h3>
        <p>زهره برخلاف جهت چرخش بیشتر سیاره‌های منظومه شمسی می‌چرخد.</p>
      </article>
      <article class="card">
        <div class="icon">🕒</div>
        <h3>روز طولانی</h3>
        <p>یک چرخش کامل زهره نسبت به ستارگان حدود ۲۴۳ روز زمینی طول می‌کشد.</p>
      </article>
      <article class="card">
        <div class="icon">🪨</div>
        <h3>سطح سنگی</h3>
        <p>زهره سیاره‌ای سنگی است که دشت‌ها، کوهستان‌ها، دهانه‌ها و ساختارهای آتشفشانی دارد.</p>
      </article>
      <article class="card">
        <div class="icon">☀️</div>
        <h3>فاصله از خورشید</h3>
        <p>میانگین فاصله زهره از خورشید حدود ۱۰۸ میلیون کیلومتر است.</p>
      </article>
    </div>
  </section>

  <section id="surface">
    <div class="section-head">
      <span class="eyebrow">03 / EXTREME WORLD</span>
      <h2>چرا زهره این‌قدر داغ است؟</h2>
    </div>
    <div class="highlight">
      <p>
        جو بسیار ضخیم زهره عمدتاً از دی‌اکسید کربن تشکیل شده است.
        این گاز بخش زیادی از گرمای خروجی سطح را در سامانه جو نگه
        می‌دارد و اثر گلخانه‌ای بسیار شدیدی ایجاد می‌کند.
      </p>
      <p><strong>فشار شگفت‌انگیز:</strong> فشار سطح زهره حدود ۹۲ برابر فشار جو زمین در سطح دریاست.</p>
      <p><strong>ابرهای اسیدی:</strong> ابرهای زهره قطرات اسید سولفوریک دارند؛ اما این ابرها به معنای وجود اقیانوس اسید روی سطح نیستند.</p>
      <p><strong>زندگی انسان:</strong> دما، فشار و ترکیبات شیمیایی محیط، زندگی مستقیم روی سطح زهره را با فناوری کنونی بسیار دشوار می‌کنند.</p>
    </div>
  </section>

  <section id="compare">
    <div class="section-head">
      <span class="eyebrow">04 / PLANET COMPARISON</span>
      <h2>زهره در برابر زمین</h2>
      <p>دو سیاره سنگی با اندازه نزدیک، اما محیطی متفاوت.</p>
    </div>
    <div class="table-wrap">
      <table>
        <thead><tr><th>ویژگی</th><th>زهره</th><th>زمین</th></tr></thead>
        <tbody>
          <tr><td>قطر تقریبی</td><td>۱۲٬۱۰۴ کیلومتر</td><td>۱۲٬۷۴۲ کیلومتر</td></tr>
          <tr><td>مدت سال</td><td>۲۲۵ روز زمینی</td><td>۳۶۵٫۲۵ روز</td></tr>
          <tr><td>چرخش نسبت به ستارگان</td><td>حدود ۲۴۳ روز</td><td>حدود ۲۳ ساعت و ۵۶ دقیقه</td></tr>
          <tr><td>دمای متوسط سطح</td><td>حدود ۴۶۵°C</td><td>حدود ۱۵°C</td></tr>
          <tr><td>قمر طبیعی</td><td>ندارد</td><td>ماه</td></tr>
          <tr><td>گاز غالب جو</td><td>دی‌اکسید کربن</td><td>نیتروژن</td></tr>
        </tbody>
      </table>
    </div>
    <p class="small">اعداد تقریبی‌اند و ممکن است با روش اندازه‌گیری و مرجع علمی اندکی تفاوت داشته باشند.</p>
  </section>

  <section id="missions">
    <div class="section-head">
      <span class="eyebrow">05 / SPACE EXPLORATION</span>
      <h2>کاوشگران زهره</h2>
      <p>فضاپیماها چگونه رازهای این جهان را آشکار کردند؟</p>
    </div>
    <div class="grid">
      <article class="card">
        <div class="icon">🚀</div>
        <h3>مارینر ۲ — ۱۹۶۲</h3>
        <p>نخستین فضاپیمایی بود که با موفقیت از کنار سیاره‌ای دیگر گذر کرد؛ مقصد آن زهره بود.</p>
      </article>
      <article class="card">
        <div class="icon">🛰️</div>
        <h3>ونرا ۷ — ۱۹۷۰</h3>
        <p>نخستین فضاپیمایی بود که با موفقیت روی زهره فرود آمد و از سطح آن داده ارسال کرد.</p>
      </article>
      <article class="card">
        <div class="icon">📡</div>
        <h3>ماژلان — ۱۹۹۰</h3>
        <p>فضاپیمای ناسا با استفاده از رادار، نقشه‌ای گسترده از سطح زهره تهیه کرد؛ سطحی که ابرهای ضخیم آن را می‌پوشانند.</p>
      </article>
    </div>
  </section>

  <section id="facts">
    <div class="section-head">
      <span class="eyebrow">06 / DID YOU KNOW?</span>
      <h2>حقایق شگفت‌انگیز</h2>
    </div>
    <div class="fact-list">
      <div class="fact">✨ <b>روز طولانی:</b> چرخش نجومی زهره از سال آن طولانی‌تر است.</div>
      <div class="fact">🌅 <b>جهت طلوع:</b> زهره در جهت مخالف بیشتر سیاره‌ها می‌چرخد؛ بنابراین طلوع خورشید روی آن جهت متفاوتی دارد.</div>
      <div class="fact">☁️ <b>پوشش ابری:</b> ابرهای ضخیم باعث می‌شوند مشاهده مستقیم سطح با نور مرئی دشوار باشد.</div>
      <div class="fact">🌋 <b>آتشفشان‌ها:</b> ساختارهای آتشفشانی فراوانی روی زهره دیده شده‌اند و شواهدی از فعالیت زمین‌شناختی وجود دارد.</div>
    </div>
  </section>

  <section id="quiz">
    <div class="section-head">
      <span class="eyebrow">07 / KNOWLEDGE TEST</span>
      <h2>آزمون فضانوردی 🚀</h2>
      <p>به پنج سؤال پاسخ بده و نتیجه مأموریتت را ببین!</p>
    </div>
    <div class="quiz-box">
      <p class="small" id="counter"></p>
      <div id="question"><h3>در حال آماده‌سازی آزمون...</h3></div>
      <div id="options"></div>
      <p id="feedback" aria-live="polite"></p>
      <button class="btn primary" id="next" style="display:none">سؤال بعدی ←</button>
      <p id="result" aria-live="polite"></p>
      <button class="btn" id="restart" style="display:none">شروع دوباره ↻</button>
    </div>
  </section>

  <section id="sources">
    <div class="section-head">
      <span class="eyebrow">08 / REFERENCES</span>
      <h2>منابع و مراجع علمی</h2>
      <p>منابع پیشنهادی برای مطالعه و بررسی اطلاعات پژوهش.</p>
    </div>
    <div class="grid">
      <article class="card">
        <h3>📄 مقاله اول: بررسی جامع زهره</h3>
        <p>
          Taylor, F. W., Svedhem, H., & Head, J. W. (2018).<br>
          <i>Venus: The Atmosphere, Climate, Surface, Interior and Near-Space Environment of an Earth-Like Planet.</i><br>
          Space Science Reviews, 214, Article 35.
        </p>
        <p><a href="https://doi.org/10.1007/s11214-018-0467-8" target="_blank" rel="noopener">مشاهده صفحه مقاله و DOI ↗</a></p>
        <p><a href="https://scholar.google.com/scholar?q=Venus+Atmosphere+Climate+Surface+Interior+Taylor+Svedhem+Head+2018" target="_blank" rel="noopener">جست‌وجوی مقاله در Google Scholar ↗</a></p>
      </article>

      <article class="card">
        <h3>🔎 جست‌وجوی مقالات تکمیلی</h3>
        <p>برای پیدا کردن مقاله‌های معتبر درباره جو زهره، اثر گلخانه‌ای، سطح و مأموریت‌های فضایی.</p>
        <p><a href="https://scholar.google.com/scholar?q=Venus+atmosphere+surface+planetary+science+review" target="_blank" rel="noopener">مقالات علمی زهره در Google Scholar ↗</a></p>
        <p><a href="https://science.nasa.gov/venus/" target="_blank" rel="noopener">NASA Science — Venus ↗</a></p>
      </article>

      <article class="card">
        <h3>🛰️ منابع سازمان‌های فضایی</h3>
        <p>اطلاعات تکمیلی درباره پژوهش‌ها و مأموریت‌های علمی مرتبط با زهره.</p>
        <p><a href="https://www.esa.int/Science_Exploration/Space_Science/Venus_Express" target="_blank" rel="noopener">آژانس فضایی اروپا — Venus Express ↗</a></p>
        <p><a href="https://solarsystem.nasa.gov/planets/venus/overview/" target="_blank" rel="noopener">NASA Solar System Exploration ↗</a></p>
      </article>
    </div>

    <div class="highlight" style="margin-top:18px">
      <strong>روش پژوهش</strong>
      <p>
        این پروژه با روش مطالعه کتابخانه‌ای و مرور منابع علمی
        مرتبط با سیاره زهره تنظیم شده است. پیوندهای Google Scholar
        برای جست‌وجو و بررسی مقاله‌های مرتبط ارائه شده‌اند.
        پیش از تحویل، مقاله‌هایی را که واقعاً مطالعه شده‌اند
        به فهرست نهایی منابع اضافه کنید.
      </p>
    </div>
  </section>
</main>

<footer>
  <strong>AMIR SG</strong>
  <p>پروژه پژوهشی سیاره زهره | کاوش، یادگیری و کشف جهان</p>
  <p>طراحی و تنظیم: امیرحسین</p>
  <a href="#home">↑ بازگشت به ابتدای صفحه</a>
</footer>

<script>
"use strict";

const questions = [
  {
    q:"۱. کدام سیاره داغ‌ترین سیاره منظومه شمسی است؟",
    a:["عطارد","زهره","مریخ","زمین"],
    correct:1,
    why:"جو ضخیم و اثر گلخانه‌ای شدید باعث دمای بسیار زیاد زهره می‌شود."
  },
  {
    q:"۲. گاز اصلی جو زهره چیست؟",
    a:["اکسیژن","نیتروژن","دی‌اکسید کربن","هیدروژن"],
    correct:2,
    why:"بخش عمده جو زهره از دی‌اکسید کربن تشکیل شده است."
  },
  {
    q:"۳. کدام فضاپیما نخستین فرود موفق روی زهره را انجام داد؟",
    a:["مارینر ۲","ونرا ۷","ماژلان","وویجر ۱"],
    correct:1,
    why:"ونرا ۷ در سال ۱۹۷۰ با موفقیت روی زهره فرود آمد."
  },
  {
    q:"۴. زهره چند قمر طبیعی شناخته‌شده دارد؟",
    a:["یک","دو","چهار","هیچ‌کدام"],
    correct:3,
    why:"زهره قمر طبیعی شناخته‌شده‌ای ندارد."
  },
  {
    q:"۵. چرا زهره از عطارد داغ‌تر است؟",
    a:["چون قمر ندارد","به دلیل اثر گلخانه‌ای شدید","چون از همه سیاره‌ها بزرگ‌تر است","چون اقیانوس دارد"],
    correct:1,
    why:"جو ضخیم زهره گرما را به‌شدت در نزدیکی سطح نگه می‌دارد."
  }
];

let index = 0;
let score = 0;
let answered = false;

const questionEl = document.getElementById("question");
const optionsEl = document.getElementById("options");
const feedbackEl = document.getElementById("feedback");
const counterEl = document.getElementById("counter");
const nextBtn = document.getElementById("next");
const resultEl = document.getElementById("result");
const restartBtn = document.getElementById("restart");

function showQuestion() {
  answered = false;
  const item = questions[index];

  counterEl.textContent =
    "سؤال " + (index + 1) + " از " + questions.length;

  questionEl.replaceChildren();
  const heading = document.createElement("h3");
  heading.textContent = item.q;
  questionEl.appendChild(heading);

  optionsEl.replaceChildren();
  feedbackEl.textContent = "";
  resultEl.textContent = "";
  nextBtn.style.display = "none";
  restartBtn.style.display = "none";

  item.a.forEach((answer, i) => {
    const button = document.createElement("button");
    button.className = "option";
    button.textContent = answer;
    button.addEventListener("click", () => chooseAnswer(i));
    optionsEl.appendChild(button);
  });
}

function chooseAnswer(choice) {
  if (answered) return;
  answered = true;

  const item = questions[index];
  const buttons = optionsEl.querySelectorAll("button");

  buttons.forEach(button => {
    button.disabled = true;
  });

  if (choice === item.correct) {
    score++;
    feedbackEl.textContent = "✅ آفرین! پاسخ درست بود.";
  } else {
    feedbackEl.textContent =
      "📚 پاسخ درست: " + item.a[item.correct];
  }

  const explanation = document.createElement("p");
  explanation.className = "muted";
  explanation.textContent = item.why;
  optionsEl.appendChild(explanation);

  nextBtn.textContent =
    index === questions.length - 1
      ? "مشاهده نتیجه"
      : "سؤال بعدی ←";

  nextBtn.style.display = "inline-block";
}

nextBtn.addEventListener("click", () => {
  if (!answered) return;

  index++;

  if (index < questions.length) {
    showQuestion();
  } else {
    counterEl.textContent = "مأموریت به پایان رسید";
    questionEl.replaceChildren();

    const heading = document.createElement("h3");
    heading.textContent = "پایان مأموریت فضایی! 🌌";
    questionEl.appendChild(heading);

    optionsEl.replaceChildren();
    feedbackEl.textContent = "";
    nextBtn.style.display = "none";

    resultEl.textContent =
      "نتیجه: " + score + " از " + questions.length;

    const detail = document.createElement("p");
    detail.className = "muted";
    detail.textContent =
      score === questions.length
        ? "فوق‌العاده! همه پاسخ‌ها درست بود."
        : "عالی بود! می‌توانی دوباره امتحان کنی و نتیجه‌ات را بهتر بشناسی.";

    resultEl.appendChild(detail);
    restartBtn.style.display = "inline-block";
  }
});

restartBtn.addEventListener("click", () => {
  index = 0;
  score = 0;
  showQuestion();
});

window.addEventListener("scroll", () => {
  const pageHeight =
    document.documentElement.scrollHeight -
    document.documentElement.clientHeight;

  const percentage = pageHeight > 0
    ? window.scrollY / pageHeight * 100
    : 0;

  document.getElementById("progress").style.width =
    percentage + "%";
});

showQuestion();
</script>
</body>
</html>
