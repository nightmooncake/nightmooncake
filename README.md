<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="dark">
<meta name="description" content="Edson — Software Developer. Persona 5 inspired README profile content.">
<title>Glauedson / README.md</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Inter:wght@400;500;600;700;900&display=swap" rel="stylesheet">
<script>document.documentElement.classList.add('js');</script>
<style>
/* ================= TOKENS ================= */
:root{
  --red:#e60012;
  --red-bright:#ff1f2e;
  --red-deep:#a3000c;
  --ink:#0d1117;
  --ink-2:#11161d;
  --card:#161b22;
  --line:#2b323b;
  --white:#ffffff;
  --gray:#c9d1d9;
  --gray-2:#8b949e;
  --orange:#d29922;
  --font-display:'Anton','Arial Narrow',Impact,sans-serif;
  --font-body:'Inter',-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,Helvetica,Arial,sans-serif;
}
*,*::before,*::after{box-sizing:border-box;}
html{-webkit-text-size-adjust:100%;}
@media (prefers-reduced-motion: no-preference){html{scroll-behavior:smooth;}}
body{
  margin:0;
  background:var(--ink);
  color:var(--gray);
  font-family:var(--font-body);
  font-size:16px;
  line-height:1.65;
  overflow-x:hidden;
  -webkit-font-smoothing:antialiased;
}
body::before{
  content:"";
  position:fixed;inset:0;z-index:0;pointer-events:none;
  background-image:
    repeating-linear-gradient(135deg,rgba(255,255,255,.022) 0 2px,transparent 2px 10px),
    radial-gradient(820px 460px at 88% -12%,rgba(230,0,18,.20),transparent 62%),
    radial-gradient(680px 460px at -12% 108%,rgba(230,0,18,.13),transparent 62%);
}
img{max-width:100%;display:block;}
a{color:inherit;}
p{margin:0 0 1em;}
p:last-child{margin-bottom:0;}
/* ================= SCROLL PROGRESS ================= */
.scroll-progress{
  position:fixed;top:0;left:0;right:0;height:3px;z-index:60;
  background:rgba(255,255,255,.06);
}
.scroll-progress__bar{
  height:100%;width:0;
  background:linear-gradient(90deg,var(--red-deep),var(--red) 40%,var(--red-bright));
  box-shadow:0 0 14px rgba(230,0,18,.9);
  transition:width .1s linear;
}
/* ================= SHELL ================= */
.readme{
  position:relative;z-index:1;
  width:100%;max-width:900px;
  margin:0 auto;
  padding:16px 16px 56px;
  display:flex;flex-direction:column;
  gap:clamp(22px,3.4vw,36px);
}
.readme > *{min-width:0;}
/* ================= BREADCRUMB ================= */
.readme__head{
  display:flex;align-items:center;justify-content:space-between;gap:12px;
  font-size:.82rem;color:var(--gray-2);letter-spacing:.01em;
  padding-top:6px;
}
.readme__head .path{min-width:0;}
.readme__head .path b{color:var(--white);font-weight:600;}
.readme__head .sep{opacity:.5;margin:0 4px;}
.icon-btn{
  flex:none;width:30px;height:30px;border-radius:6px;
  border:1px solid var(--line);background:var(--card);
  display:grid;place-items:center;cursor:pointer;color:var(--gray-2);
  transition:background .18s,color .18s,border-color .18s;
}
.icon-btn:hover{background:#1f2630;color:var(--white);border-color:var(--red);}
.icon-btn svg{width:15px;height:15px;}
/* ================= BANNER ================= */
.banner{
  position:relative;overflow:hidden;border-radius:12px;
  background:linear-gradient(112deg,var(--red) 0%,var(--red) 55%,var(--red-deep) 100%);
  min-height:clamp(168px,30vw,258px);
  display:flex;align-items:center;
  padding:clamp(18px,4vw,38px);
  box-shadow:0 24px 50px -24px rgba(230,0,18,.85),inset 0 0 0 1px rgba(255,255,255,.10);
  isolation:isolate;
}
.banner::before{
  content:"";position:absolute;inset:0;z-index:0;pointer-events:none;
  background-image:repeating-linear-gradient(115deg,rgba(0,0,0,.16) 0 3px,transparent 3px 16px);
  opacity:.55;
}
.banner::after{
  content:"";position:absolute;z-index:0;pointer-events:none;
  width:70%;height:170%;top:-35%;left:-12%;
  background:linear-gradient(100deg,rgba(255,255,255,.14),rgba(255,255,255,0) 62%);
  transform:skewX(-14deg);
}
.banner__art{
  position:absolute;right:-2%;bottom:-6%;z-index:1;
  height:118%;width:auto;max-width:none;
  pointer-events:none;
  filter:drop-shadow(-8px 8px 0 rgba(0,0,0,.55));
}
.banner__content{position:relative;z-index:2;}
.banner__title{
  margin:0;font-family:var(--font-display);
  font-size:clamp(2.5rem,11vw,5.4rem);
  line-height:.88;letter-spacing:.015em;
  color:var(--white);
  transform:skewX(-7deg);
  -webkit-text-stroke:.055em var(--ink);
  text-shadow:.035em .055em 0 var(--ink), .075em .115em 0 rgba(0,0,0,.45);
}
.banner__sub{
  margin:.55rem 0 0;
  font-family:var(--font-display);
  font-size:clamp(.85rem,3vw,1.3rem);
  letter-spacing:.34em;text-transform:uppercase;
  color:var(--white);
  transform:skewX(-7deg);
  text-shadow:.06em .08em 0 var(--ink);
}
.banner__logo{
  position:absolute;top:clamp(10px,2.4vw,18px);right:clamp(10px,2.4vw,18px);z-index:3;
  display:flex;align-items:center;gap:6px;
  background:var(--ink);color:var(--white);
  padding:5px 11px 6px;
  transform:skewX(-12deg) rotate(-3deg);
  box-shadow:3px 3px 0 rgba(0,0,0,.55);
  border:2px solid var(--white);
}
.banner__logo span{
  transform:skewX(12deg) rotate(3deg);
  font-family:var(--font-display);font-size:.72rem;letter-spacing:.16em;
}
.banner__logo span em{color:var(--red-bright);font-style:normal;}
/* ================= STAT BADGES ================= */
.stats{
  display:flex;flex-wrap:wrap;gap:12px;justify-content:center;
}
.stat{
  display:flex;align-items:center;gap:9px;
  background:var(--red);color:var(--white);
  padding:8px 16px 9px;
  font-size:.72rem;font-weight:700;letter-spacing:.14em;text-transform:uppercase;
  transform:skewX(-12deg);
  box-shadow:4px 4px 0 #000;
  border:1px solid rgba(0,0,0,.35);
}
.stat > *{transform:skewX(12deg);}
.stat svg{width:14px;height:14px;flex:none;}
.stat b{font-family:var(--font-display);font-size:1rem;letter-spacing:.03em;font-weight:400;}
/* ================= SECTION BADGE (P5 CALLING CARD) ================= */
.p5-badge{
  display:inline-block;
  background:var(--red);color:var(--white);
  padding:.5rem 1.3rem .55rem;
  transform:skewX(-12deg) rotate(-2deg);
  box-shadow:6px 6px 0 #000;
  clip-path:polygon(0 10%,3% 0,97% 5%,100% 0,99% 86%,96% 100%,5% 95%,0 100%);
  max-width:100%;
}
.p5-badge span{
  display:block;transform:skewX(12deg) rotate(2deg);
  font-family:var(--font-display);
  font-size:clamp(.85rem,2.7vw,1.15rem);
  letter-spacing:.08em;text-transform:uppercase;white-space:nowrap;
}
/* ================= WHO AM I ================= */
.who{
  display:grid;gap:clamp(18px,3.4vw,32px);
  grid-template-columns:minmax(0,1fr);
  align-items:center;
}
@media (min-width:720px){
  .who{grid-template-columns:clamp(150px,24%,212px) minmax(0,1fr);}
}
.who__visual{display:flex;justify-content:center;}
.who__visual svg{
  width:min(100%,212px);height:auto;margin-bottom:6px;
  filter:drop-shadow(0 16px 30px rgba(230,0,18,.42));
}
.who__title{
  position:relative;display:inline-block;margin:0 0 16px;
  font-family:var(--font-display);
  font-size:clamp(1.55rem,5vw,2.3rem);
  letter-spacing:.02em;color:var(--white);line-height:1.05;
}
.who__title::after{
  content:"";position:absolute;left:0;right:-10px;bottom:-8px;height:4px;
  background:linear-gradient(90deg,var(--red),transparent);
  transform:skewX(-24deg);
}
.who__text{font-size:clamp(.9rem,2.4vw,.97rem);color:var(--gray);}
/* ================= SOCIAL CTA ================= */
.social{text-align:center;display:flex;flex-direction:column;gap:16px;}
.social__hint{
  margin:0;color:var(--white);font-size:.95rem;font-weight:500;letter-spacing:.01em;
}
.social__btns{display:flex;flex-wrap:wrap;gap:12px;justify-content:center;}
.btn-social{
  display:inline-flex;align-items:center;gap:9px;
  background:var(--red);color:var(--white);text-decoration:none;
  padding:10px 18px 11px;
  font-size:.72rem;font-weight:700;letter-spacing:.14em;text-transform:uppercase;
  transform:skewX(-12deg);
  box-shadow:4px 4px 0 #000;
  border:1px solid rgba(0,0,0,.35);
  transition:transform .18s ease,box-shadow .18s ease,background .18s ease;
}
.btn-social > *{transform:skewX(12deg);}
.btn-social:hover,.btn-social:focus-visible{
  background:var(--red-bright);
  transform:skewX(-12deg) translate(-2px,-2px);
  box-shadow:7px 7px 0 #000;
  outline:none;
}
.btn-social svg{width:15px;height:15px;flex:none;}
/* ================= CAUTION ================= */
.caution{
  position:relative;
  display:grid;gap:18px;
  grid-template-columns:minmax(0,1fr);
  background:linear-gradient(180deg,rgba(230,0,18,.09),rgba(230,0,18,.02));
  border:2px solid var(--red);
  border-radius:6px;
  padding:clamp(18px,3.2vw,28px);
}
@media (min-width:640px){
  .caution{grid-template-columns:minmax(0,1fr) auto;align-items:center;}
}
.caution::before,.caution::after{
  content:"";position:absolute;width:22px;height:22px;pointer-events:none;
}
.caution::before{top:-2px;left:-2px;border-top:5px solid var(--white);border-left:5px solid var(--white);}
.caution::after{bottom:-2px;right:-2px;border-bottom:5px solid var(--white);border-right:5px solid var(--white);}
.caution__label{
  display:inline-flex;align-items:center;gap:8px;
  color:var(--orange);font-weight:700;font-size:.74rem;
  letter-spacing:.18em;text-transform:uppercase;margin-bottom:14px;
}
.caution__label svg{width:15px;height:15px;}
.caution__q{
  margin:0 0 10px;
  font-family:var(--font-display);
  font-size:clamp(1.05rem,3.5vw,1.5rem);
  letter-spacing:.01em;line-height:1.28;color:var(--white);
}
.caution__sub{margin:0;color:var(--gray-2);font-size:.88rem;}
.caution__art{display:flex;justify-content:center;}
.caution__art svg{
  width:clamp(66px,16vw,104px);height:auto;
  filter:drop-shadow(0 10px 20px rgba(0,0,0,.7));
}
/* ================= CONTRIBUTIONS CHART ================= */
.contrib{display:flex;flex-direction:column;gap:14px;}
.chart-card{
  position:relative;overflow:hidden;
  background:#05080c;
  border:1px solid var(--line);
  border-radius:8px;
  padding:14px 14px 8px;
}
.chart-card__cap{
  font-size:.66rem;letter-spacing:.18em;text-transform:uppercase;
  color:var(--gray-2);margin-bottom:8px;
}
.chart{width:100%;height:clamp(132px,26vw,214px);display:block;}
.chart__grid line{stroke:rgba(255,255,255,.07);}
.chart__line{
  stroke:var(--red-bright);stroke-width:3;fill:none;
  stroke-linejoin:round;stroke-linecap:round;
  filter:drop-shadow(0 0 8px rgba(230,0,18,.85));
}
.chart__area{opacity:.9;}
.chart__dot{fill:var(--white);stroke:var(--red);stroke-width:3;}
html.js .chart__line{stroke-dasharray:1;stroke-dashoffset:1;}
html.js .chart__area{opacity:0;}
html.js .chart__dot{opacity:0;}
html.js .chart.is-drawn .chart__line{stroke-dashoffset:0;transition:stroke-dashoffset 1.8s ease .1s;}
html.js .chart.is-drawn .chart__area{opacity:1;transition:opacity 1.1s ease .7s;}
html.js .chart.is-drawn .chart__dot{opacity:1;transition:opacity .45s ease 1.7s;}
/* ================= BOTTOM: TECH + PROJECT/STATS ================= */
.bottom{
  display:grid;gap:clamp(18px,3.2vw,26px);
  grid-template-columns:minmax(0,1fr);
}
@media (min-width:880px){
  .bottom{grid-template-columns:minmax(0,1.02fr) minmax(0,1fr);align-items:start;}
}
.tech-col{display:flex;flex-direction:column;gap:16px;}
.tech{
  display:grid;gap:10px;
  grid-template-columns:repeat(auto-fill,minmax(56px,1fr));
}
.tech__item{
  position:relative;aspect-ratio:1/1;
  display:grid;place-items:center;
  background:var(--card);
  border:1px solid var(--line);
  border-radius:10px;
  transition:transform .18s ease,border-color .18s ease,box-shadow .18s ease;
}
.tech__item:hover{
  transform:translateY(-3px);
  border-color:var(--red);
  box-shadow:0 10px 20px -12px rgba(230,0,18,.95);
}
.tech__item img{width:54%;height:54%;object-fit:contain;}
.tech__item--fallback::after{
  content:attr(data-label);
  font-family:var(--font-display);
  font-size:.68rem;letter-spacing:.04em;
  color:var(--red-bright);
}
.right-col{display:flex;flex-direction:column;gap:12px;}
.project{
  position:relative;
  background:var(--red);color:var(--white);
  border:2px solid var(--ink);
  border-radius:8px;
  padding:15px 16px 17px;
  box-shadow:7px 7px 0 rgba(0,0,0,.85);
}
.project__head{
  display:flex;align-items:center;gap:8px;margin-bottom:8px;
}
.project__head svg{width:15px;height:15px;flex:none;}
.project__name{
  margin:0;font-family:var(--font-display);
  font-size:clamp(.92rem,2.8vw,1.1rem);
  letter-spacing:.04em;line-height:1.2;
}
.project__desc{margin:0;font-size:.8rem;line-height:1.5;color:rgba(255,255,255,.92);}
.project__meta{
  display:inline-flex;align-items:center;gap:7px;margin-top:11px;
  font-size:.66rem;letter-spacing:.14em;text-transform:uppercase;font-weight:700;
}
.project__meta i{
  width:10px;height:10px;border-radius:50%;
  background:#f1e05a;box-shadow:0 0 0 2px rgba(0,0,0,.35);
}
.stat-boxes{
  display:grid;gap:10px;
  grid-template-columns:repeat(3,minmax(0,1fr));
}
.stat-box{
  background:#0b0f14;
  border:1px solid rgba(230,0,18,.55);
  border-radius:8px;
  padding:13px 6px 12px;
  text-align:center;
  transition:border-color .18s ease,transform .18s ease;
}
.stat-box:hover{border-color:var(--red-bright);transform:translateY(-2px);}
.stat-box__num{
  font-family:var(--font-display);
  font-size:clamp(1.35rem,5.2vw,1.85rem);
  line-height:1;color:var(--white);
}
.stat-box__label{
  margin-top:7px;font-size:.56rem;letter-spacing:.12em;text-transform:uppercase;
  color:var(--red-bright);font-weight:700;line-height:1.35;
}
.stat-box__date{
  margin-top:6px;font-size:.53rem;line-height:1.35;color:var(--gray-2);
}
/* ================= FOOTER ================= */
.readme__foot{
  display:flex;flex-wrap:wrap;gap:8px;align-items:center;justify-content:space-between;
  border-top:1px solid var(--line);
  padding-top:16px;
  font-size:.72rem;color:var(--gray-2);letter-spacing:.04em;
}
.readme__foot b{color:var(--red-bright);font-weight:700;}
/* ================= REVEAL ================= */
html.js .reveal{
  opacity:0;transform:translateY(22px);
  transition:opacity .7s cubic-bezier(.2,.7,.3,1),transform .7s cubic-bezier(.2,.7,.3,1);
}
html.js .reveal.is-in{opacity:1;transform:none;}
@media (prefers-reduced-motion: reduce){
  html.js .reveal{opacity:1;transform:none;transition:none;}
  html.js .chart__line{stroke-dasharray:none;stroke-dashoffset:0;}
  html.js .chart__area,html.js .chart__dot{opacity:1;}
}
/* ================= SMALL SCREENS ================= */
@media (max-width:420px){
  .readme{padding:14px 12px 48px;}
  .stat-boxes{grid-template-columns:repeat(3,minmax(0,1fr));gap:8px;}
  .stat-box{padding:10px 6px 9px;}
  .stat-box__num{font-size:1.15rem;}
  .stat-box__label{font-size:.57rem;letter-spacing:.04em;}
  .stat-box__date{font-size:.55rem;}
  .p5-badge span{white-space:normal;}
  .tech{grid-template-columns:repeat(auto-fill,minmax(48px,1fr));gap:8px;}
}
</style>
</head>
<body>
<div class="scroll-progress" aria-hidden="true"><div class="scroll-progress__bar" id="progressBar"></div></div>
<main class="readme">
  <!-- ============ BREADCRUMB ============ -->
  <header class="readme__head">
    <div class="path">
      <span><b>Glauedson</b><span class="sep">/</span>README.md</span>
    </div>
    <button class="icon-btn" type="button" aria-label="Edit README">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
        <path d="M12 20h9"/><path d="M16.5 3.5a2.12 2.12 0 0 1 3 3L7 19l-4 1 1-4Z"/>
      </svg>
    </button>
  </header>
  <!-- ============ BANNER ============ -->
  <section class="banner reveal" aria-label="Profile banner">
    <svg class="banner__art" viewBox="0 0 420 300" aria-hidden="true">
      <polygon points="238,300 268,26 420,60 420,300" fill="#0d1117" opacity=".92"/>
      <polygon points="300,300 330,0 420,0 420,300" fill="#7d0009" opacity=".95"/>
      <g transform="translate(196,44)">
        <path d="M52 0 L96 14 L124 54 L118 128 L134 246 L64 262 L22 244 L16 126 L-14 68 L22 34 Z"
              fill="#0d1117" stroke="#000" stroke-width="6"/>
        <path d="M30 34 L60 8 L98 28 L78 66 L46 72 Z" fill="#e60012" stroke="#0d1117" stroke-width="5" stroke-linejoin="round"/>
        <ellipse cx="58" cy="86" rx="34" ry="24" fill="#ffffff" stroke="#0d1117" stroke-width="5"/>
        <path d="M36 82 q11 -8 20 1 q-12 5 -20 -1 z" fill="#0d1117"/>
        <path d="M64 79 q9 -5 16 2 q-10 4 -16 -2 z" fill="#0d1117"/>
        <path d="M22 150 L96 140 L104 178 L30 190 Z" fill="#e60012" opacity=".9"/>
      </g>
    </svg>
    <div class="banner__content">
      <h1 class="banner__title">EDSON</h1>
      <p class="banner__sub">Developer</p>
    </div>
    <div class="banner__logo"><span><em>P5</em> DEV</span></div>
  </section>
  <!-- ============ STAT BADGES ============ -->
  <section class="stats reveal" aria-label="Repository stats">
    <div class="stat">
      <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="m12 2 3.1 6.3 6.9 1-5 4.9 1.2 6.8L12 17.8 5.8 21l1.2-6.8-5-4.9 6.9-1Z"/></svg>
      <span>Stars</span><b data-count="29">0</b>
    </div>
    <div class="stat">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="6" cy="6" r="2.4"/><circle cx="18" cy="6" r="2.4"/><circle cx="12" cy="18" r="2.4"/><path d="M8 7.2 10.4 15M16 7.2 13.6 15"/></svg>
      <span>Forks</span><b data-count="4">0</b>
    </div>
    <div class="stat">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="9" cy="8" r="3.2"/><path d="M2.6 20a6.6 6.6 0 0 1 12.8 0"/><path d="M17 14.4a3 3 0 1 0 0-6"/><path d="M18.4 20a5.6 5.6 0 0 0-2.2-4.4"/></svg>
      <span>Followers</span><b data-count="32">0</b>
    </div>
  </section>
  <!-- ============ WHO AM I ============ -->
  <section class="who reveal" aria-label="Who am I">
    <div class="who__visual">
      <svg viewBox="0 0 240 240" role="img" aria-label="Phantom thief mask and top hat illustration">
        <defs>
          <linearGradient id="maskRed" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0" stop-color="#ff2a37"/>
            <stop offset="1" stop-color="#8f0009"/>
          </linearGradient>
        </defs>
        <polygon points="16,216 44,40 216,22 196,210" fill="url(#maskRed)"/>
        <polygon points="44,40 216,22 196,210 152,218" fill="#0d1117" opacity=".28"/>
        <g transform="rotate(-10 120 96)">
          <rect x="78" y="54" width="86" height="64" rx="3" fill="#e60012" stroke="#0d1117" stroke-width="6"/>
          <rect x="74" y="110" width="94" height="16" rx="2" fill="#0d1117"/>
          <ellipse cx="121" cy="129" rx="60" ry="13" fill="#e60012" stroke="#0d1117" stroke-width="6"/>
          <rect x="90" y="66" width="9" height="42" fill="#ffffff" opacity=".55"/>
        </g>
        <ellipse cx="114" cy="180" rx="56" ry="40" fill="#ffffff" stroke="#0d1117" stroke-width="6"/>
        <path d="M84 172 q13 -9 24 1 q-14 6 -24 -1 z" fill="#0d1117"/>
        <path d="M122 168 q11 -6 19 3 q-12 5 -19 -3 z" fill="#0d1117"/>
        <path d="M60 170 l-24 -13 5 19 -21 2 28 15 z" fill="#e60012" stroke="#0d1117" stroke-width="4" stroke-linejoin="round"/>
      </svg>
    </div>
    <div class="who__text">
      <h2 class="who__title">Who Am I?</h2>
      <p>I am a graduated Software Developer with a degree in Systems Analysis and Development, currently working as a freelancer while actively seeking an opportunity in the technology field. My professional journey is driven by continuous learning, practical experience, and a strong commitment to delivering complete and functional systems for real-world needs.</p>
      <p>Over time, I have developed solid experience across the web development ecosystem, with a strong passion for Front-End Development, where logic meets creativity and visual design. Alongside web technologies, I have expanded my skills into mobile development, focusing on building modern applications using Android Studio and React Native.</p>
      <p>At the moment, I am working as a freelancer, developing complete systems for companies in my city, from planning and interface design to implementation and delivery. This hands-on experience has strengthened my problem-solving skills, technical versatility, and ability to understand business needs, while constantly pushing me to grow as a developer and professional.</p>
    </div>
  </section>
  <!-- ============ SOCIAL CTA ============ -->
  <section class="social reveal" aria-label="Social links">
    <p class="social__hint">You can Click here</p>
    <div class="social__btns">
      <a class="btn-social" href="#" aria-label="Pinterest">
        <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12.02 2C6.9 2 3.6 5.24 3.6 9.36c0 2.02 1.1 3.9 2.86 4.5.27.13.41.07.47-.18.05-.2.31-1.24.43-1.72a.4.4 0 0 0-.1-.39c-.42-.51-.76-1.44-.76-2.32 0-2.24 1.7-4.41 4.6-4.41 2.5 0 4.25 1.7 4.25 4.14 0 2.75-1.39 4.66-3.2 4.66-1 0-1.75-.83-1.5-1.84.29-1.2.85-2.5.85-3.37 0-.78-.42-1.43-1.28-1.43-1.02 0-1.84 1.06-1.84 2.47 0 .9.3 1.51.3 1.51s-1.03 4.37-1.22 5.15c-.2.8-.12 1.93-.06 2.66.04.42.5.52.71.2.29-.44 1.16-1.72 1.42-2.4.14-.37.7-2.74.7-2.74.35.66 1.36 1.24 2.44 1.24 3.2 0 5.38-2.92 5.38-6.83C18.2 4.85 15.5 2 12.02 2Z"/></svg>
        <span>Pinterest</span>
      </a>
      <a class="btn-social" href="#" aria-label="LinkedIn">
        <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M4.98 3.5a2.5 2.5 0 1 1 0 5 2.5 2.5 0 0 1 0-5ZM3 9h4v12H3V9Zm7 0h3.8v1.64h.05c.53-.95 1.83-1.95 3.76-1.95 4.02 0 4.76 2.5 4.76 5.76V21h-4v-5.6c0-1.34-.02-3.06-1.9-3.06-1.9 0-2.19 1.46-2.19 2.96V21h-4V9Z"/></svg>
        <span>LinkedIn</span>
      </a>
      <a class="btn-social" href="#" aria-label="Gmail">
        <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M2 6.2A2.2 2.2 0 0 1 4.2 4h.5l7.3 5.4L19.3 4h.5A2.2 2.2 0 0 1 22 6.2v11.6A2.2 2.2 0 0 1 19.8 20h-1.5V9.6l-6.3 4.6-6.3-4.6V20H4.2A2.2 2.2 0 0 1 2 17.8V6.2Z"/></svg>
        <span>Gmail</span>
      </a>
    </div>
  </section>
  <!-- ============ CAUTION ============ -->
  <section class="caution reveal" aria-label="Caution">
    <div>
      <div class="caution__label">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="12" cy="12" r="9.2"/><path d="M12 7.4v5.4"/><path d="M12 16.4h.01"/></svg>
        Caution
      </div>
      <p class="caution__q">Code is never finished, it only gets better.</p>
      <p class="caution__sub">What you see here is built with practice, curiosity, and persistence.</p>
    </div>
    <div class="caution__art">
      <svg viewBox="0 0 120 200" aria-hidden="true">
        <g transform="rotate(26 60 100)">
          <path d="M60 6 L75 38 L68 134 L52 134 L45 38 Z" fill="#e6edf3" stroke="#0d1117" stroke-width="5" stroke-linejoin="round"/>
          <rect x="34" y="132" width="52" height="12" rx="3" fill="#0d1117"/>
          <rect x="52" y="144" width="16" height="44" rx="6" fill="#0d1117"/>
          <rect x="52" y="152" width="16" height="5" fill="#e60012"/>
          <rect x="52" y="164" width="16" height="5" fill="#e60012"/>
          <circle cx="60" cy="192" r="7" fill="#e60012" stroke="#0d1117" stroke-width="4"/>
        </g>
      </svg>
    </div>
  </section>
  <!-- ============ CONTRIBUTIONS ============ -->
  <section class="contrib reveal" aria-label="My contributions">
    <div class="p5-badge"><span>My Contributions</span></div>
    <div class="chart-card">
      <div class="chart-card__cap">My Contributions</div>
      <svg class="chart" id="contribChart" viewBox="0 0 600 200" preserveAspectRatio="none" role="img" aria-label="Line chart of contribution activity">
        <defs>
          <linearGradient id="chartFill" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#e60012" stop-opacity=".55"/>
            <stop offset="100%" stop-color="#e60012" stop-opacity="0"/>
          </linearGradient>
        </defs>
        <g class="chart__grid">
          <line x1="0" y1="40" x2="600" y2="40" vector-effect="non-scaling-stroke"/>
          <line x1="0" y1="80" x2="600" y2="80" vector-effect="non-scaling-stroke"/>
          <line x1="0" y1="120" x2="600" y2="120" vector-effect="non-scaling-stroke"/>
          <line x1="0" y1="160" x2="600" y2="160" vector-effect="non-scaling-stroke"/>
        </g>
        <polygon class="chart__area" fill="url(#chartFill)"
          points="20,170 48,172 76,168 104,171 132,166 160,170 188,165 216,169 244,160 272,166 300,158 328,164 356,152 384,160 412,150 440,158 468,148 496,140 524,120 552,45 580,155 580,200 20,200"/>
        <polyline class="chart__line" pathLength="1" vector-effect="non-scaling-stroke"
          points="20,170 48,172 76,168 104,171 132,166 160,170 188,165 216,169 244,160 272,166 300,158 328,164 356,152 384,160 412,150 440,158 468,148 496,140 524,120 552,45 580,155"/>
        <circle class="chart__dot" cx="552" cy="45" r="6" vector-effect="non-scaling-stroke"/>
      </svg>
    </div>
  </section>
  <!-- ============ TECH STACK + PROJECT + STATS ============ -->
  <section class="bottom reveal" aria-label="Tech stack and activity stats">
    <div class="tech-col">
      <div class="p5-badge"><span>My Tech Stack</span></div>
      <div class="tech">
        <div class="tech__item" data-label="HTML"><img src="https://cdn.simpleicons.org/html5/E34F26" alt="HTML5" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="CSS"><img src="https://cdn.simpleicons.org/css3/1572B6" alt="CSS3" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="JS"><img src="https://cdn.simpleicons.org/javascript/F7DF1E" alt="JavaScript" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="TS"><img src="https://cdn.simpleicons.org/typescript/3178C6" alt="TypeScript" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="C"><img src="https://cdn.simpleicons.org/c/A8B9CC" alt="C" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="React"><img src="https://cdn.simpleicons.org/react/61DAFB" alt="React" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Node"><img src="https://cdn.simpleicons.org/nodedotjs/5FA04E" alt="Node.js" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Express"><img src="https://cdn.simpleicons.org/express/FFFFFF" alt="Express" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Styled"><img src="https://cdn.simpleicons.org/styledcomponents/DB7093" alt="Styled Components" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Bootstrap"><img src="https://cdn.simpleicons.org/bootstrap/7952B3" alt="Bootstrap" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="VS Code"><img src="https://cdn.simpleicons.org/visualstudiocode/007ACC" alt="Visual Studio Code" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Git"><img src="https://cdn.simpleicons.org/git/F05032" alt="Git" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="GitHub"><img src="https://cdn.simpleicons.org/github/FFFFFF" alt="GitHub" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="MySQL"><img src="https://cdn.simpleicons.org/mysql/4479A1" alt="MySQL" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Firebase"><img src="https://cdn.simpleicons.org/firebase/FFCA28" alt="Firebase" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Android"><img src="https://cdn.simpleicons.org/android/3DDC84" alt="Android" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Java"><img src="https://cdn.simpleicons.org/java/ED8B00" alt="Java" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Expo"><img src="https://cdn.simpleicons.org/expo/FFFFFF" alt="Expo" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Figma"><img src="https://cdn.simpleicons.org/figma/F24E1E" alt="Figma" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
        <div class="tech__item" data-label="Python"><img src="https://cdn.simpleicons.org/python/3776AB" alt="Python" loading="lazy" onerror="this.parentNode.classList.add('tech__item--fallback');this.remove();"></div>
      </div>
    </div>
    <div class="right-col">
      <article class="project">
        <div class="project__head">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M4 19V5a2 2 0 0 1 2-2h11l3 3v13a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2Z"/><path d="M8 7h7M8 11h8M8 15h5"/></svg>
          <h3 class="project__name">Lembra-Plus-note-app</h3>
        </div>
        <p class="project__desc">A note-taking application for creating, editing and organizing memos — built with a fast, clean interface and local data persistence.</p>
        <div class="project__meta"><i></i> JavaScript</div>
      </article>
      <div class="stat-boxes">
        <div class="stat-box">
          <div class="stat-box__num" data-count="573">0</div>
          <div class="stat-box__label">Total<br>Contributions</div>
          <div class="stat-box__date">Sep 12, 2024 –<br>Mar 14, 2025</div>
        </div>
        <div class="stat-box">
          <div class="stat-box__num" data-count="2">0</div>
          <div class="stat-box__label">Current<br>Streak</div>
          <div class="stat-box__date">Mar 13 –<br>Mar 14</div>
        </div>
        <div class="stat-box">
          <div class="stat-box__num" data-count="42">0</div>
          <div class="stat-box__label">Longest<br>Streak</div>
          <div class="stat-box__date">Feb 1, 2025 –<br>Mar 14, 2025</div>
        </div>
      </div>
    </div>
  </section>
  <!-- ============ FOOTER ============ -->
  <footer class="readme__foot">
    <span><b>EDSON</b> · Software Developer</span>
    <span>Built with practice, curiosity &amp; persistence.</span>
  </footer>
</main>
<script>
(function () {
  'use strict';
  var reduce = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  var supportsIO = 'IntersectionObserver' in window;
  /* ---------- scroll progress ---------- */
  var bar = document.getElementById('progressBar');
  function onScroll() {
    if (!bar) return;
    var doc = document.documentElement;
    var max = doc.scrollHeight - doc.clientHeight;
    var top = window.pageYOffset || doc.scrollTop || 0;
    bar.style.width = (max > 0 ? (top / max) * 100 : 0).toFixed(2) + '%';
  }
  window.addEventListener('scroll', onScroll, { passive: true });
  window.addEventListener('resize', onScroll);
  window.addEventListener('load', onScroll);
  onScroll();
  /* ---------- reveal on scroll ---------- */
  var reveals = document.querySelectorAll('.reveal');
  if (!supportsIO || reduce) {
    for (var i = 0; i < reveals.length; i++) { reveals[i].classList.add('is-in'); }
  } else {
    var io = new IntersectionObserver(function (entries) {
      entries.forEach(function (entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('is-in');
          io.unobserve(entry.target);
        }
      });
    }, { threshold: 0.12, rootMargin: '0px 0px -8% 0px' });
    for (var j = 0; j < reveals.length; j++) { io.observe(reveals[j]); }
  }
  /* ---------- animated counters ---------- */
  function animateCount(el) {
    var target = parseInt(el.getAttribute('data-count'), 10) || 0;
    if (reduce) { el.textContent = String(target); return; }
    var duration = 1100;
    var start = null;
    function step(ts) {
      if (start === null) { start = ts; }
      var p = Math.min((ts - start) / duration, 1);
      var eased = 1 - Math.pow(1 - p, 3);
      el.textContent = String(Math.round(target * eased));
      if (p < 1) { window.requestAnimationFrame(step); }
    }
    window.requestAnimationFrame(step);
  }
  var counters = document.querySelectorAll('[data-count]');
  if (!supportsIO) {
    for (var k = 0; k < counters.length; k++) { animateCount(counters[k]); }
  } else {
    var ioCount = new IntersectionObserver(function (entries) {
      entries.forEach(function (entry) {
        if (entry.isIntersecting) {
          animateCount(entry.target);
          ioCount.unobserve(entry.target);
        }
      });
    }, { threshold: 0.5 });
    for (var m = 0; m < counters.length; m++) { ioCount.observe(counters[m]); }
  }
  /* ---------- chart draw-in ---------- */
  var chart = document.getElementById('contribChart');
  if (chart) {
    if (!supportsIO || reduce) {
      chart.classList.add('is-drawn');
    } else {
      var ioChart = new IntersectionObserver(function (entries) {
        entries.forEach(function (entry) {
          if (entry.isIntersecting) {
            entry.target.classList.add('is-drawn');
            ioChart.unobserve(entry.target);
          }
        });
      }, { threshold: 0.35 });
      ioChart.observe(chart);
    }
  }
})();
</script>
</body>
</html>
