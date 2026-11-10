
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080a10">
<title>AMIR CODE | آموزش برنامه‌نویسی با امیرعلی</title>
<style>
:root{
--bg:#080a10;
--panel:#111622;
--red:#ff3048;
--white:#f5f7fb;
--muted:#a6adbd;
--line:#272e3c;
--cyan:#36e6f5
}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{
margin:0;
background:radial-gradient(circle at 80% 0%,#25101b 0,transparent 36%),linear-gradient(145deg,#080a10,#0b101a 60%,#120910);
color:var(--white);
font-family:Tahoma,Arial,sans-serif;
min-height:100vh
}
a{color:inherit;text-decoration:none}
.wrap{max-width:1100px;margin:auto;padding:20px}
nav{
display:flex;justify-content:space-between;
align-items:center;gap:12px;padding:14px 0;
border-bottom:1px solid var(--line)
}
.brand{font-weight:900;letter-spacing:1px}
.brand span{color:var(--red)}
.navlinks{display:flex;gap:18px;color:var(--muted);font-size:14px}
.navlinks a:hover{color:#fff}
.hero{
display:grid;grid-template-columns:1.2fr .8fr;
gap:25px;align-items:center;padding:55px 0 35px
}
.eyebrow{color:var(--red);font-weight:bold;letter-spacing:2px;font-size:12px}
.hero h1{
font-size:clamp(34px,6vw,65px);
line-height:1.18;margin:12px 0
}
.hero h1 em{
font-style:normal;color:var(--red);
text-shadow:0 0 24px #ff304833
}
.hero p{color:var(--muted);line-height:2;max-width:620px}
.btns{display:flex;flex-wrap:wrap;gap:12px;margin-top:25px}
.btn{
display:inline-flex;align-items:center;justify-content:center;
border:1px solid var(--red);background:var(--red);color:white;
padding:13px 20px;border-radius:12px;font-weight:bold;
cursor:pointer;box-shadow:0 8px 25px #ff304826
}
.btn.secondary{background:transparent;border-color:var(--line);box-shadow:none}
.hero-card{
background:linear-gradient(145deg,#1a1f2c,#0e121b);
border:1px solid #34303c;border-radius:24px;padding:22px;
position:relative;overflow:hidden;box-shadow:0 20px 60px #0007
}
.hero-card:before{
content:"";position:absolute;width:180px;height:180px;
background:#ff30481c;filter:blur(30px);
border-radius:50%;top:-50px;left:-40px
}
.code-art{
position:relative;min-height:180px;display:flex;
align-items:center;justify-content:center;
font:700 clamp(30px,5vw,55px) monospace;
color:var(--cyan);text-shadow:0 0 25px #36e6f544
}
.code-art span{color:var(--red)}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.stat{
background:#0b0f17;border:1px solid var(--line);
border-radius:12px;padding:12px;text-align:center
}
.stat b{display:block;font-size:20px}
.stat small{color:var(--muted);font-size:11px}
section{padding:35px 0}
.section-head{
display:flex;justify-content:space-between;
align-items:end;gap:10px;margin-bottom:18px
}
.section-head h2{margin:0;font-size:25px}
.section-head p{color:var(--muted);margin:6px 0 0;font-size:13px}
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.card{
background:linear-gradient(145deg,#141a27,#0d1119);
border:1px solid var(--line);border-radius:18px;
padding:19px;transition:.2s
}
.card:hover{transform:translateY(-4px);border-color:#74303b}
.icon{font-size:30px;margin-bottom:12px}
.card h3{margin:0 0 8px}
.card p{color:var(--muted);font-size:13px;line-height:1.9;margin:0}
.tag{
display:inline-block;font-size:11px;color:#ff8794;
border:1px solid #5a2631;border-radius:20px;
padding:5px 9px;margin-top:12px
}
.channel{display:flex;align-items:center;gap:14px}
.channel .icon{margin:0;font-size:34px}
.channel .btn{margin-right:auto;padding:10px 14px;font-size:12px}
.lesson{
background:#101520;border:1px solid #3b2832;
border-radius:22px;padding:22px
}
.lesson pre{
direction:ltr;text-align:left;overflow:auto;
background:#080b12;border:1px solid #252d3a;
border-radius:13px;padding:16px;color:#b6f5fa;
font-size:14px;line-height:1.8
}
.lesson p{color:var(--muted);line-height:1.9}
footer{
border-top:1px solid var(--line);padding:24px 0;
color:var(--muted);font-size:12px;
display:flex;justify-content:space-between;
gap:12px;flex-wrap:wrap
}
.creator{color:#fff}
.creator b{color:var(--red)}
@media(max-width:760px){
.hero{grid-template-columns:1fr;padding-top:35px}
.grid{grid-template-columns:1fr}
.navlinks{gap:10px;font-size:12px}
.wrap{padding:15px}
.hero-card{max-width:500px}
.channel{flex-wrap:wrap}
.channel .btn{margin-right:0}
}
</style>
</head>
<body>
<div class="wrap">

<nav>
<a class="brand" href="#">AMIR <span>CODE</span></a>
<div class="navlinks">
<a href="#courses">آموزش‌ها</a>
<a href="#channels">کانال‌ها</a>
<a href="#sample">نمونه کد</a>
</div>
</nav>

<header class="hero">
<div>
<div class="eyebrow">CODE • CREATE • LEVEL UP</div>
<h1>برنامه‌نویسی رو<br><em>با امیرعلی یاد بگیر!</em></h1>
<p>
به دنیای کدنویسی خوش اومدی!
اینجا از قدم‌های اول تا ساخت سایت و بازی،
با آموزش‌های ساده و پروژه‌محور همراهت هستم.
آماده‌ای ایده‌هات رو به واقعیت تبدیل کنی؟
</p>
<div class="btns">
<a class="btn" href="#courses">🚀 شروع یادگیری</a>
<a class="btn secondary" href="#channels">▶ دیدن کانال‌ها</a>
</div>
</div>

<div class="hero-card">
<div class="code-art">&lt;<span>AMIR</span> /&gt;</div>
<div class="stats">
<div class="stat"><b>HTML</b><small>ساخت صفحات وب</small></div>
<div class="stat"><b>CSS</b><small>طراحی زیبا</small></div>
<div class="stat"><b>JS</b><small>تعامل و بازی</small></div>
</div>
</div>
</header>

<section id="courses">
<div class="section-head">
<div>
<h2>مسیرهای یادگیری</h2>
<p>از پایه شروع کن و پروژه‌های واقعی بساز</p>
</div>
</div>

<div class="grid">
<div class="card">
<div class="icon">🌐</div>
<h3>طراحی سایت با HTML</h3>
<p>ساختار صفحات، عنوان‌ها، متن‌ها، لینک‌ها و اولین صفحه‌ی وب خودت.</p>
<span class="tag">سطح مبتدی</span>
</div>

<div class="card">
<div class="icon">🎨</div>
<h3>طراحی با CSS</h3>
<p>رنگ‌ها، فونت‌ها، کارت‌ها، چیدمان واکنش‌گرا و ظاهر حرفه‌ای برای سایت.</p>
<span class="tag">ظاهر سایت</span>
</div>

<div class="card">
<div class="icon">⚡</div>
<h3>JavaScript</h3>
<p>دکمه‌های تعاملی، امتیازدهی، سؤال‌های بازی و امکانات جذاب به صفحات اضافه کن.</p>
<span class="tag">کدنویسی پویا</span>
</div>

<div class="card">
<div class="icon">📱</div>
<h3>برنامه‌نویسی با گوشی</h3>
<p>آشنایی با ابزارهای اندرویدی مثل Acode و ساخت پروژه بدون نیاز به کامپیوتر.</p>
<span class="tag">Android</span>
</div>

<div class="card">
<div class="icon">🎮</div>
<h3>ساخت بازی ساده</h3>
<p>با HTML، CSS و JavaScript یک بازی کوچک بساز؛ قوانین، امتیاز و صفحه‌ی شروع.</p>
<span class="tag">پروژه عملی</span>
</div>

<div class="card">
<div class="icon">🧩</div>
<h3>پروژه‌های تمرینی</h3>
<p>تمرین‌های کوتاه برای تقویت مهارت و تبدیل ایده‌ها به پروژه‌های قابل اجرا.</p>
<span class="tag">تمرین و تجربه</span>
</div>
</div>
</section>

<section id="channels">
<div class="section-head">
<div>
<h2>ویدیوهای آموزشی من</h2>
<p>برای دیدن آموزش‌ها وارد کانال‌های رسمی شو</p>
</div>
</div>

<div class="grid">
<div class="card channel">
<div class="icon">▶️</div>
<div>
<h3>YouTube</h3>
<p>ویدیوها و آموزش‌های کانال یوتیوب</p>
</div>
<a class="btn"
href="https://youtube.com/@amirshotiamirali?si=D9UX_giAB6B5HLz4"
target="_blank" rel="noopener">رفتن به یوتیوب ↗</a>
</div>

<div class="card channel">
<div class="icon">📺</div>
<div>
<h3>Aparat</h3>
<p>ویدیوهای کوتاه آموزشی در آپارات</p>
</div>
<a class="btn"
href="https://www.aparat.com/AmirAliRajabiAhmedAbadi/short-videos"
target="_blank" rel="noopener">رفتن به آپارات ↗</a>
</div>

<div class="card">
<div class="icon">💡</div>
<h3>یادگیری با پروژه</h3>
<p>هر آموزش رو با یک تمرین کوچیک همراه کن؛ بهترین راه یادگیری، ساختن و امتحان کردنه.</p>
<span class="tag">قدم‌به‌قدم</span>
</div>
</div>
</section>

<section id="sample">
<div class="section-head">
<div>
<h2>اولین کد تو</h2>
<p>یک نمونه خیلی ساده HTML</p>
</div>
</div>

<div class="lesson">
<p>
این کد یک عنوان و پیام ساده در صفحه نمایش می‌دهد.
می‌تونی آن را در فایل <b>index.html</b> داخل Acode امتحان کنی.
</p>

<pre><code>&lt;!DOCTYPE html&gt;
&lt;html lang="fa" dir="rtl"&gt;
&lt;head&gt;
  &lt;meta charset="UTF-8"&gt;
  &lt;title&gt;اولین سایت من&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
  &lt;h1&gt;سلام! من برنامه‌نویسم 👨‍💻&lt;/h1&gt;
  &lt;p&gt;این اولین صفحه‌ی وب من است.&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;</code></pre>

<a class="btn secondary" href="#courses">برگشت به مسیر آموزش ↑</a>
</div>
</section>

<section id="about">
<div class="card">
<div class="eyebrow">CREATED BY</div>
<h2>آموزش برنامه‌نویسی با امیرعلی</h2>
<p style="color:var(--muted);line-height:1.9">
سازنده و ارائه‌دهنده‌ی آموزش‌های برنامه‌نویسی:
<b style="color:#fff">امیرعلی رجبی</b>
</p>
<div class="btns">
<a class="btn"
href="https://youtube.com/@amirshotiamirali?si=D9UX_giAB6B5HLz4"
target="_blank" rel="noopener">▶ YouTube</a>
<a class="btn secondary"
href="https://www.aparat.com/AmirAliRajabiAhmedAbadi/short-videos"
target="_blank" rel="noopener">📺 Aparat</a>
</div>
</div>
</section>

<footer>
<span>© 2026 AMIR CODE</span>
<span class="creator">سازنده: <b>امیرعلی رجبی</b></span>
</footer>

</div>
</body>
</html>
