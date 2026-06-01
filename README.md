<!DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Marble Studios | Wrapping, PPF e Detailing Premium em Portugal</title>
<meta name="description" content="Especialistas em wrapping automóvel, PPF, proteção cerâmica e detailing premium em Portugal."/>
<link rel="preconnect" href="[fonts.googleapis.com](https://fonts.googleapis.com)"/>
<link rel="preconnect" href="[fonts.gstatic.com](https://fonts.gstatic.com)" crossorigin/>
<link href="[fonts.googleapis.com](https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;500;600&family=Cormorant+Garamond:ital@1&display=swap)" rel="stylesheet"/>
<style>
:root{
  --bg:#0a0a0a;--bg2:#0f0f0f;--bg3:#141414;
  --copper:#c8843a;--copper-l:#e8b87a;--copper-p:#f5e6d0;
  --white:#fff;--gray:#a89880;--gray-d:#3a3530;
  --glass:rgba(200,132,58,.06);--gb:rgba(200,132,58,.18);
  --ease:cubic-bezier(.16,1,.3,1);
}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--white);font-family:'Inter',sans-serif;overflow-x:hidden}
::-webkit-scrollbar{width:4px}
::-webkit-scrollbar-track{background:var(--bg)}
::-webkit-scrollbar-thumb{background:var(--copper);border-radius:2px}
/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:999;padding:1.2rem 5%;display:flex;align-items:center;justify-content:space-between;transition:.4s ease}
nav.scrolled{background:rgba(10,10,10,.95);backdrop-filter:blur(20px);border-bottom:1px solid var(--gb)}
.logo{display:flex;align-items:center;gap:.6rem;text-decoration:none}
.logo-box{background:linear-gradient(135deg,#6b2a1a,#3d1a0d,#8b3a1e);padding:.3rem .7rem;border:1px solid rgba(200,132,58,.4)}
.logo-box span{font-family:'Bebas Neue',sans-serif;font-size:1.4rem;color:var(--copper-p);letter-spacing:.1em}
.logo-right{display:flex;flex-direction:column;justify-content:center;padding-left:.2rem}
.logo-studios{font-family:'Inter',sans-serif;font-size:.8rem;color:var(--copper);letter-spacing:.45em;font-weight:400;position:relative;padding:4px 0}
.logo-studios::before,.logo-studios::after{content:'';position:absolute;left:0;right:0;height:1px;background:var(--copper)}
.logo-studios::before{top:0}.logo-studios::after{bottom:0}
.nav-links{display:flex;align-items:center;gap:2.5rem;list-style:none}
.nav-links a{color:var(--gray);text-decoration:none;font-size:.75rem;letter-spacing:.2em;text-transform:uppercase;transition:color .3s}
.nav-links a:hover{color:var(--copper-l)}
.nav-cta{padding:.55rem 1.3rem;border:1px solid var(--copper);color:var(--copper);text-decoration:none;font-size:.72rem;letter-spacing:.18em;text-transform:uppercase;font-weight:500;transition:all .3s}
.nav-cta:hover{background:var(--copper);color:var(--bg);box-shadow:0 0 20px rgba(200,132,58,.4)}
.hamburger{display:none;flex-direction:column;gap:5px;cursor:pointer;background:none;border:none;padding:4px}
.hamburger span{display:block;width:24px;height:1px;background:var(--copper);transition:.3s}
.mob-menu{display:none;position:fixed;inset:0;background:rgba(10,10,10,.98);z-index:998;flex-direction:column;align-items:center;justify-content:center;gap:2.5rem}
.mob-menu.open{display:flex}
.mob-menu a{font-family:'Bebas Neue',sans-serif;font-size:3rem;color:var(--white);text-decoration:none;letter-spacing:.1em;transition:color .3s}
.mob-menu a:hover{color:var(--copper)}
.mob-close{position:absolute;top:1.5rem;right:5%;font-size:2rem;color:var(--copper);cursor:pointer;background:none;border:none;color:var(--copper)}
/* HERO */
#hero{min-height:100vh;display:flex;align-items:center;padding:0 5%;position:relative;overflow:hidden}
.hero-bg{position:absolute;inset:0;z-index:0;
  background:
    radial-gradient(ellipse 70% 60% at 75% 50%,rgba(139,58,30,.2) 0%,transparent 60%),
    radial-gradient(ellipse 40% 40% at 15% 75%,rgba(200,132,58,.07) 0%,transparent 50%),
    radial-gradient(ellipse 50% 40% at 80% 15%,rgba(100,40,10,.15) 0%,transparent 55%),
    var(--bg);
  animation:heroPulse 8s ease-in-out infinite alternate}
@keyframes heroPulse{0%{filter:brightness(1)}100%{filter:brightness(1.1)}}
.hero-orb{position:absolute;border-radius:50%;filter:blur(80px);pointer-events:none;z-index:1}
.orb1{width:600px;height:600px;background:rgba(200,132,58,.07);top:-15%;right:5%;animation:orbf 12s ease-in-out infinite}
.orb2{width:350px;height:350px;background:rgba(139,58,30,.1);bottom:5%;right:25%;animation:orbf 14s ease-in-out infinite reverse}
.orb3{width:250px;height:250px;background:rgba(200,132,58,.05);top:30%;right:0;animation:orbf 10s ease-in-out infinite 3s}
@keyframes orbf{0%,100%{transform:translateY(0) scale(1)}50%{transform:translateY(-40px) scale(1.06)}}
.hero-content{position:relative;z-index:2;max-width:680px}
.hero-eyebrow{font-size:.68rem;letter-spacing:.45em;color:var(--copper);text-transform:uppercase;margin-bottom:1.5rem;display:flex;align-items:center;gap:1rem;opacity:0;animation:fadeUp .8s var(--ease) .2s forwards}
.hero-eyebrow::before{content:'';width:40px;height:1px;background:var(--copper)}
h1{font-family:'Bebas Neue',sans-serif;font-size:clamp(4.5rem,11vw,9rem);line-height:.92;letter-spacing:.02em;margin-bottom:1.5rem;opacity:0;animation:fadeUp .8s var(--ease) .4s forwards}
h1 .copper{background:linear-gradient(90deg,var(--copper),var(--copper-l));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.hero-sub{font-size:.93rem;color:var(--gray);line-height:1.75;max-width:460px;margin-bottom:2.5rem;letter-spacing:.04em;opacity:0;animation:fadeUp .8s var(--ease) .6s forwards}
.hero-btns{display:flex;gap:1rem;flex-wrap:wrap;opacity:0;animation:fadeUp .8s var(--ease) .8s forwards}
.btn-p{padding:.9rem 2rem;background:linear-gradient(135deg,var(--copper),var(--copper-l));color:var(--bg);text-decoration:none;font-size:.78rem;letter-spacing:.2em;text-transform:uppercase;font-weight:600;transition:all .3s;display:inline-block}
.btn-p:hover{box-shadow:0 0 30px rgba(200,132,58,.5);transform:translateY(-2px)}
.btn-s{padding:.9rem 2rem;border:1px solid rgba(200,132,58,.45);color:var(--white);text-decoration:none;font-size:.78rem;letter-spacing:.2em;text-transform:uppercase;transition:all .3s;display:inline-block}
.btn-s:hover{border-color:var(--copper);color:var(--copper);background:rgba(200,132,58,.05)}
.scroll-ind{position:absolute;bottom:2.5rem;left:50%;transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;gap:.5rem;z-index:2;opacity:0;animation:fadeIn 1s ease 1.5s forwards}
.scroll-ind span{font-size:.58rem;letter-spacing:.35em;color:var(--gray);text-transform:uppercase}
.scroll-line{width:1px;height:50px;background:linear-gradient(to bottom,var(--copper),transparent);animation:spulse 2s ease-in-out infinite}
@keyframes spulse{0%,100%{opacity:.3;transform:scaleY(1)}50%{opacity:1;transform:scaleY(1.2)}}
/* ANIMATIONS */
@keyframes fadeUp{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:translateY(0)}}
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
.reveal{opacity:0;transform:translateY(30px);transition:opacity .7s var(--ease),transform .7s var(--ease)}
.reveal.visible{opacity:1;transform:translateY(0)}
/* SECTIONS COMMON */
section{padding:7rem 5%;position:relative;overflow:hidden}
.sec-label{display:flex;align-items:center;gap:1rem;font-size:.68rem;letter-spacing:.42em;color:var(--copper);text-transform:uppercase;margin-bottom:2.5rem}
.sec-label::before{content:'';width:30px;height:1px;background:var(--copper)}
.sec-num{position:absolute;font-family:'Bebas Neue',sans-serif;font-size:clamp(8rem,18vw,16rem);color:rgba(200,132,58,.035);top:-1rem;left:3%;line-height:1;pointer-events:none;user-select:none}
/* SOBRE */
#sobre{background:var(--bg2)}
.sobre-grid{display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:center;position:relative;z-index:1}
.sobre-h{font-family:'Bebas Neue',sans-serif;font-size:clamp(2.5rem,5vw,4rem);line-height:1.05;letter-spacing:.02em;margin-bottom:1.5rem}
.sobre-h span{color:var(--copper)}
.sobre-p{color:var(--gray);line-height:1.85;font-size:.93rem;margin-bottom:2rem}
.divider{width:60px;height:1px;background:linear-gradient(90deg,var(--copper),transparent);margin-bottom:2rem}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem}
.stat-n{font-family:'Bebas Neue',sans-serif;font-size:3rem;background:linear-gradient(135deg,var(--copper),var(--copper-l));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;display:block}
.stat-l{font-size:.68rem;color:var(--gray);letter-spacing:.2em;text-transform:uppercase;margin-top:.3rem}
.sobre-card{background:var(--glass);border:1px solid var(--gb);padding:3rem;position:relative}
.sobre-card::before{content:'';position:absolute;top:0;left:0;width:3px;height:100%;background:linear-gradient(to bottom,var(--copper),transparent)}
.sobre-card-accent{position:absolute;bottom:-1px;right:-1px;width:50px;height:50px;border-bottom:2px solid var(--copper);border-right:2px solid var(--copper)}
.sobre-card h3{font-family:'Bebas Neue',sans-serif;font-size:1.8rem;letter-spacing:.1em;margin-bottom:1rem}
.sobre-card p{color:var(--gray);line-height:1.8;font-size:.9rem}
/* SERVIÇOS */
#servicos{background:var(--bg)}
.sec-h{font-family:'Bebas Neue',sans-serif;font-size:clamp(2.5rem,5vw,4rem);letter-spacing:.02em;margin-bottom:3rem;position:relative;z-index:1}
.srv-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;position:relative;z-index:1;background:rgba(200,132,58,.08)}
.srv-card{background:var(--bg3);padding:2.5rem 2rem;transition:all .4s var(--ease);position:relative;overflow:hidden;cursor:default}
.srv-card::after{content:'';position:absolute;inset:0;background:linear-gradient(135deg,rgba(200,132,58,.05),transparent);opacity:0;transition:.4s}
.srv-card:hover{transform:translateY(-4px);box-shadow:0 15px 50px rgba(200,132,58,.15)}
.srv-card:hover::after{opacity:1}
.srv-icon{width:44px;height:44px;color:var(--copper);margin-bottom:1.5rem}
.srv-icon svg{width:100%;height:100%}
.srv-t{font-family:'Bebas Neue',sans-serif;font-size:1.35rem;letter-spacing:.08em;margin-bottom:.8rem}
.srv-d{color:var(--gray);font-size:.84rem;line-height:1.7}
.srv-arr{position:absolute;bottom:1.5rem;right:1.5rem;color:var(--copper);font-size:1.1rem;opacity:0;transition:opacity .3s,transform .3s}
.srv-card:hover .srv-arr{opacity:1;transform:translateX(4px)}
/* GALERIA */
#projetos{background:var(--bg2)}
.gallery-grid{display:grid;grid-template-columns:repeat(12,1fr);grid-auto-rows:180px;gap:4px;position:relative;z-index:1}
.gi{position:relative;overflow:hidden;cursor:pointer}
.gi:nth-child(1){grid-column:1/6;grid-row:1/3}
.gi:nth-child(2){grid-column:6/9;grid-row:1/2}
.gi:nth-child(3){grid-column:9/13;grid-row:1/2}
.gi:nth-child(4){grid-column:6/10;grid-row:2/3}
.gi:nth-child(5){grid-column:10/13;grid-row:2/3}
.gi:nth-child(6){grid-column:1/5;grid-row:3/4}
.gi:nth-child(7){grid-column:5/9;grid-row:3/4}
.gi:nth-child(8){grid-column:9/13;grid-row:3/4}
.gi-bg{width:100%;height:100%;transition:transform .6s var(--ease)}
.gi:hover .gi-bg{transform:scale(1.06)}
.gb1{background:linear-gradient(135deg,#1a0e08,#2d1a0e,#160b05)}
.gb2{background:linear-gradient(135deg,#0c0c0c,#1a1205,#0f0a05)}
.gb3{background:linear-gradient(135deg,#100808,#1e0e0e,#0d0606)}
.gb4{background:linear-gradient(135deg,#080e12,#101820,#080f0c)}
.gb5{background:linear-gradient(135deg,#0f0f0d,#1a1005,#0e0e0c)}
.gb6{background:linear-gradient(135deg,#120808,#200f06,#100707)}
.gb7{background:linear-gradient(135deg,#090e09,#101b10,#090d09)}
.gb8{background:linear-gradient(135deg,#0d0a12,#18102a,#0d0a12)}
.gi-ov{position:absolute;inset:0;background:linear-gradient(to top,rgba(0,0,0,.8) 0%,transparent 60%)}
.gi-hover{position:absolute;inset:0;background:rgba(200,132,58,.1);opacity:0;transition:.4s;display:flex;align-items:center;justify-content:center}
.gi:hover .gi-hover{opacity:1}
.gi-plus{width:36px;height:36px;border:1px solid var(--copper);display:flex;align-items:center;justify-content:center;color:var(--copper);font-size:1.2rem}
.gi-info{position:absolute;bottom:1rem;left:1rem;right:1rem}
.gi-tag{font-size:.62rem;letter-spacing:.3em;color:var(--copper);text-transform:uppercase}
.gi-name{font-family:'Bebas Neue',sans-serif;font-size:1.1rem;letter-spacing:.06em}
/* Decorative car shapes in gallery */
.gi-shape{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);opacity:.08;pointer-events:none}
.gallery-cta{text-align:center;margin-top:2.5rem;position:relative;z-index:1}
/* BEFORE AFTER */
.ba-wrap{margin-top:3rem;position:relative;z-index:1}
.ba-lbl{font-size:.68rem;letter-spacing:.3em;color:var(--copper);text-transform:uppercase;margin-bottom:1rem}
.ba-cont{position:relative;width:100%;height:280px;overflow:hidden;cursor:ew-resize;border:1px solid var(--gb)}
.ba-side{position:absolute;inset:0;display:flex;align-items:center;justify-content:center}
.ba-before-side{background:linear-gradient(135deg,#1a1a1a,#2a2525);z-index:1}
.ba-after-side{background:linear-gradient(135deg,#2a1408,#3d1e08,#2a1408);z-index:2;clip-path:inset(0 50% 0 0);transition:clip-path .05s linear}
.ba-badge{position:absolute;font-family:'Bebas Neue',sans-serif;font-size:1.4rem;letter-spacing:.1em;padding:.4rem 1.2rem;top:1rem}
.ba-before-side .ba-badge{right:1rem;background:rgba(0,0,0,.5);color:var(--gray)}
.ba-after-side .ba-badge{left:1rem;background:rgba(200,132,58,.25);color:var(--copper-l)}
.ba-handle{position:absolute;top:0;bottom:0;left:50%;transform:translateX(-50%);width:2px;background:var(--copper);z-index:3;pointer-events:none}
.ba-handle-circle{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);width:34px;height:34px;border-radius:50%;background:var(--copper);border:2px solid var(--white);display:flex;align-items:center;justify-content:center;color:var(--bg);font-size:.8rem;font-weight:700}
.ba-car-before,.ba-car-after{opacity:.18}
.ba-car-svg{width:200px;height:80px}
/* TESTEMUNHOS */
#testemunhos{background:var(--bg)}
.test-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;position:relative;z-index:1}
.test-card{background:var(--glass);border:1px solid var(--gb);padding:2rem;position:relative;transition:all .4s var(--ease)}
.test-card::before{content:'';position:absolute;top:0;left:0;width:3px;height:100%;background:linear-gradient(to bottom,var(--copper),transparent)}
.test-card:hover{border-color:var(--copper);box-shadow:0 10px 40px rgba(200,132,58,.1);transform:translateY(-3px)}
.test-stars{color:var(--copper);font-size:.9rem;margin-bottom:1.2rem}
.test-q{font-family:'Cormorant Garamond',serif;font-style:italic;font-size:1.05rem;line-height:1.75;color:var(--copper-p);margin-bottom:1.5rem}
.test-author{font-size:.75rem;letter-spacing:.15em;text-transform:uppercase;color:var(--gray)}
.test-author span{color:var(--copper)}
.test-quote-mark{position:absolute;top:1.5rem;right:1.5rem;font-family:'Bebas Neue',sans-serif;font-size:4rem;line-height:1;color:rgba(200,132,58,.08)}
/* CTA */
#cta{background:linear-gradient(135deg,#0f0805,#1a0e06,#120a05);border-top:1px solid var(--gb);border-bottom:1px solid var(--gb);text-align:center;padding:6rem 5%}
.cta-h{font-family:'Bebas Neue',sans-serif;font-size:clamp(2.5rem,6vw,5rem);letter-spacing:.03em;margin-bottom:1rem;position:relative;z-index:1}
.cta-sub{color:var(--gray);font-size:.93rem;margin-bottom:2.5rem;position:relative;z-index:1}
.cta-btns{display:flex;gap:1rem;justify-content:center;flex-wrap:wrap;position:relative;z-index:1}
.btn-wa{padding:.85rem 2rem;background:#25D366;color:#fff;text-decoration:none;font-size:.78rem;letter-spacing:.18em;text-transform:uppercase;font-weight:600;display:flex;align-items:center;gap:.6rem;transition:all .3s}
.btn-wa:hover{background:#1da851;box-shadow:0 0 20px rgba(37,211,102,.3)}
.btn-ig{padding:.85rem 2rem;background:linear-gradient(135deg,#833ab4,#fd1d1d,#fcb045);color:#fff;text-decoration:none;font-size:.78rem;letter-spacing:.18em;text-transform:uppercase;font-weight:600;display:flex;align-items:center;gap:.6rem;transition:all .3s}
.btn-ig:hover{opacity:.85;box-shadow:0 0 20px rgba(200,132,58,.3)}
.btn-orcamento{padding:.85rem 2rem;background:linear-gradient(135deg,var(--copper),var(--copper-l));color:var(--bg);text-decoration:none;font-size:.78rem;letter-spacing:.18em;text-transform:uppercase;font-weight:600;display:flex;align-items:center;gap:.6rem;transition:all .3s}
.btn-orcamento:hover{box-shadow:0 0 25px rgba(200,132,58,.5);transform:translateY(-2px)}
.cta-pulse{position:absolute;top:50%;left:50%;transform:translate
