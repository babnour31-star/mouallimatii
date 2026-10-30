
<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<meta name="color-scheme" content="light only">
<title>Mouallimatii</title>
<meta name="description" content="Mouallimatii : apprendre la langue arabe pas à pas, en petits groupes de femmes adultes. Lecture, Coran, grammaire et méthodes de langue.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700&family=Instrument+Serif:ital@0;1&family=Figtree:wght@400;500;600;700&display=swap">
<style>
html,body{margin:0}
img{max-width:100%}
[hidden]{display:none!important}
:root{padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
</style>
<style>
/* Layout : une feuille de papier déchirée posée sur un fond bordeaux (comme la fiche « حروف الجر »),
   titre éditorial + orbite de cartes (Mindly), dunes lumineuses (Naqa), cartes bordeaux à bulles (tarifs).
   Design volontairement à thème unique : la palette de la fiche, quel que soit le mode clair/sombre. */
:root{
  color-scheme:light;
  --wine:#7A2A2E; --wine-m:#5E1F22; --wine-d:#3E1415; --wine-x:#260C0D;
  --paper:#F0EEE9; --paper2:#E4E0D8; --card:#F8F6F2; --ink:#2E1A1A; --muted:#806868;
  --on-wine:#F6EEEC; --rose:#C98C8C; --line:rgba(122,42,46,.22); --shadow:rgba(62,20,21,.22);
  --f-display:"Instrument Serif","Times New Roman",Georgia,serif;
  --f-body:"Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;
  --f-callig:"Amiri","Traditional Arabic","Arabic Typesetting",serif;
  --f-ar:"Amiri","Traditional Arabic","Arabic Typesetting",serif;
}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{color:var(--ink);font-family:var(--f-body);font-size:16px;line-height:1.6;overflow-x:hidden;
  background:linear-gradient(180deg,var(--wine) 0%,var(--wine-d) 55%,var(--wine-x) 100%) fixed var(--wine-d);
  padding-left:max(clamp(16px,3vw,40px),env(safe-area-inset-left,0px));padding-right:max(clamp(16px,3vw,40px),env(safe-area-inset-right,0px));padding-block:clamp(18px,3vw,40px)}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);z-index:30;background:var(--wine)}
h1,h2,h3{font-family:var(--f-display);font-weight:400;margin:0;text-wrap:balance;letter-spacing:-.01em}
a{color:inherit}
[lang="ar"]{font-family:var(--f-ar);font-weight:600}
.brand,.logo .ar,.ar-t,.watermark,.core .disc b,.badge-rot b,.pr .ar,.pg .ic,.doc .top .ar,.fm .orb span,.orb span,.why::before,footer .ar,.chip i,.chip b,.side .ic{font-weight:700!important}
:focus-visible{outline:2px solid var(--wine);outline-offset:3px}

/* FEUILLE DÉCHIRÉE */
.sheet-shadow{filter:drop-shadow(0 18px 40px rgba(0,0,0,.35));max-width:1260px;margin:0 auto}
.sheet{position:relative;background:var(--paper);overflow-x:clip;
  -webkit-mask:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 14 120'%3E%3Cpath d='M14 0H6L9 8 3 15 8 24 2 33 7 41 4 52 10 60 3 70 8 79 1 88 6 97 3 108 9 114 6 120H14Z'/%3E%3C/svg%3E") left top/14px 120px repeat-y,
    url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 14 120'%3E%3Cpath d='M0 0H8L5 9 11 17 6 26 12 34 7 44 10 53 4 61 11 71 6 80 13 90 8 99 11 107 5 115 8 120H0Z'/%3E%3C/svg%3E") right top/14px 120px repeat-y,
    linear-gradient(#000 0 0) center/calc(100% - 26px) 100% no-repeat;
  mask:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 14 120'%3E%3Cpath d='M14 0H6L9 8 3 15 8 24 2 33 7 41 4 52 10 60 3 70 8 79 1 88 6 97 3 108 9 114 6 120H14Z'/%3E%3C/svg%3E") left top/14px 120px repeat-y,
    url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 14 120'%3E%3Cpath d='M0 0H8L5 9 11 17 6 26 12 34 7 44 10 53 4 61 11 71 6 80 13 90 8 99 11 107 5 115 8 120H0Z'/%3E%3C/svg%3E") right top/14px 120px repeat-y,
    linear-gradient(#000 0 0) center/calc(100% - 26px) 100% no-repeat;
  background-image:radial-gradient(50% 30% at 15% 10%,var(--card),transparent 70%),radial-gradient(40% 25% at 90% 45%,var(--paper2),transparent 70%),radial-gradient(50% 30% at 30% 85%,var(--card),transparent 70%)}
.watermark{position:absolute;pointer-events:none;font-family:var(--f-callig);color:var(--wine);opacity:.05;line-height:1;white-space:nowrap;z-index:0}
.wm1{font-size:clamp(14rem,34vw,30rem);top:60px;left:-6%;transform:rotate(-12deg);animation:drift 30s ease-in-out infinite}
.wm2{font-size:clamp(10rem,24vw,22rem);top:1700px;right:-4%;transform:rotate(10deg);animation:drift 36s ease-in-out infinite reverse}
.wrap{position:relative;z-index:1;max-width:1080px;margin:0 auto;padding-left:max(clamp(32px,6vw,80px),env(safe-area-inset-left,0px));padding-right:max(clamp(32px,6vw,80px),env(safe-area-inset-right,0px))}
.eyebrow{font-size:.74rem;text-transform:uppercase;letter-spacing:.16em;color:var(--muted);font-weight:600}
.btn{display:inline-flex;align-items:center;gap:.55em;border:0;border-radius:999px;padding:.85em 1.4em;font:600 .95rem var(--f-body);cursor:pointer;text-decoration:none;transition:transform .25s,box-shadow .25s}
.btn-wine{background:var(--wine);color:var(--on-wine);box-shadow:0 8px 22px var(--shadow),inset 0 -3px 0 rgba(0,0,0,.18)}
.btn-wine:hover{transform:translateY(-2px);box-shadow:0 14px 30px var(--shadow),inset 0 -3px 0 rgba(0,0,0,.18)}
.btn-ghost{background:var(--card);color:var(--ink);border:1px solid var(--line)}
.btn-ghost:hover{transform:translateY(-2px)}
.btn-light{background:var(--paper);color:var(--wine)}
.btn-light:hover{transform:translateY(-2px)}

/* NAV */
header{position:sticky;top:env(safe-area-inset-top,0px);z-index:20;padding-block:22px;background:color-mix(in srgb,var(--paper) 82%,transparent);backdrop-filter:blur(10px);-webkit-backdrop-filter:blur(10px)}
.nav{display:grid;grid-template-columns:1fr auto 1fr;align-items:center;gap:16px}
.pill{display:flex;gap:4px;background:var(--card);border:1px solid var(--line);border-radius:999px;padding:4px;width:max-content}
.pill a{padding:.45em 1em;border-radius:999px;text-decoration:none;font-size:.88rem;color:var(--muted);transition:background .2s,color .2s}
.pill a:hover{background:var(--wine);color:var(--on-wine)}
.pill.right{justify-self:end}
.logo{display:flex;flex-direction:column;align-items:center;text-decoration:none;line-height:1}
.logo .ar{font-family:var(--f-callig);font-size:2rem;color:var(--wine)}
.logo .fr{font-size:.62rem;letter-spacing:.3em;text-transform:uppercase;color:var(--muted);margin-top:2px}

/* HERO */
.hero{position:relative;padding-top:34px;text-align:center}
.brand{display:inline-block;position:relative;font-family:var(--f-callig);font-size:clamp(2.6rem,6vw,4rem);color:var(--wine);line-height:1.2;animation:fade 1s both}
.brand::after{content:"";position:absolute;left:-6%;right:-6%;bottom:.08em;height:3px;background:var(--wine);transform-origin:right;animation:underline 1.1s .5s cubic-bezier(.7,0,.2,1) both}
.hero h1{font-size:clamp(2.6rem,7vw,5.6rem);line-height:.98;margin-top:10px}
.hero h1 .l{display:block;overflow:hidden;padding-bottom:.08em}
.hero h1 .l span{display:inline-block;animation:rise 1s .2s cubic-bezier(.2,.8,.2,1) both}
.hero h1 .l:nth-child(2) span{animation-delay:.35s}
.hero h1 em{color:var(--wine)}
.hero p.lead{max-width:34rem;margin:28px auto 0;color:var(--muted);font-size:1.05rem;animation:fade 1s .5s both}
.hero .cta{display:flex;gap:14px;justify-content:center;flex-wrap:wrap;margin-top:34px;animation:fade 1s .65s both}
.stage{position:relative;height:440px;margin-top:6px}
.orbit-wrap{position:absolute;left:50%;top:44%;width:0;height:0;perspective:1100px}
.ring{position:absolute;transform-style:preserve-3d;animation:orbit 28s linear infinite}
.chip{position:absolute;left:-80px;top:-31px;width:160px;height:62px;border-radius:18px;background:var(--wine-m);color:var(--on-wine);
  display:flex;align-items:center;gap:10px;padding:0 12px;box-shadow:inset 0 3px 8px rgba(0,0,0,.35),0 10px 24px var(--shadow);backface-visibility:hidden}
.chip i{width:30px;height:30px;flex:none;border-radius:9px;display:grid;place-items:center;font-style:normal;font-family:var(--f-ar);font-size:1.25rem;background:var(--paper);color:var(--wine)}
.chip b{display:block;font-family:var(--f-ar);font-weight:700;font-size:1.05rem;line-height:1.1}
.chip small{display:block;color:var(--rose);font-size:.7rem;line-height:1.2}
.core{position:absolute;left:50%;top:44%;width:196px;height:196px;transform:translate(-50%,-50%);display:grid;place-items:center}
.core .disc{width:150px;height:150px;border-radius:50%;background:radial-gradient(circle at 35% 30%,var(--wine),var(--wine-d));
  box-shadow:0 20px 50px var(--shadow),inset 0 0 0 8px rgba(255,255,255,.06),inset 0 -10px 20px rgba(0,0,0,.3);display:grid;place-items:center;text-align:center;color:var(--on-wine)}
.core .disc b{font-family:var(--f-callig);font-weight:400;font-size:4rem;line-height:1}
.core .disc small{display:block;font-size:.66rem;letter-spacing:.2em;text-transform:uppercase;color:var(--rose)}
.core svg{position:absolute;inset:0;animation:spin 30s linear infinite reverse}
.side{position:absolute;width:220px;text-align:left;background:var(--card);border:1px solid var(--line);border-radius:22px;padding:24px;box-shadow:0 14px 34px var(--shadow);animation:bob 6s ease-in-out infinite;z-index:3}
.side h3{font-size:1.35rem;line-height:1.1;margin:.45em 0 .3em}
.side p{margin:0;font-size:.82rem;color:var(--muted);line-height:1.4}
.side.a{left:5%;top:4%}
.side.b{right:5%;top:4%;animation-delay:-3s}
.side .ic{width:36px;height:36px;border-radius:10px;background:var(--wine);display:grid;place-items:center;color:var(--on-wine);font-family:var(--f-ar);font-size:1.2rem}
.stat{position:absolute;left:6%;bottom:120px;text-align:left;font-size:.82rem;color:var(--muted);z-index:3}
.stat b{display:block;font-family:var(--f-display);font-weight:400;font-size:2.1rem;color:var(--wine);line-height:1}
.badge-rot{position:absolute;right:6%;bottom:110px;width:98px;height:98px;z-index:3}
.badge-rot svg{animation:spin 18s linear infinite}
.badge-rot b{position:absolute;inset:0;display:grid;place-items:center;font-family:var(--f-callig);font-size:1.8rem;color:var(--wine)}
.dunes{position:absolute;left:0;right:0;bottom:0;width:100%;height:210px;z-index:1;pointer-events:none}
.d1{fill:var(--paper2)} .d2{fill:var(--rose);opacity:.35} .d3{fill:var(--wine);opacity:.85}
.trail{fill:none;stroke:var(--wine);stroke-width:1.6;stroke-dasharray:6 8;animation:dash 3s linear infinite;opacity:.7}
.spark{fill:var(--wine);filter:drop-shadow(0 0 5px var(--rose))}

/* SECTIONS */
section{padding-block:clamp(80px,10vw,130px);position:relative}
.head{display:flex;justify-content:space-between;align-items:end;gap:28px 48px;flex-wrap:wrap;margin-bottom:56px}
.head h2{font-size:clamp(2.2rem,4.6vw,3.6rem);line-height:1}
.head h2 em{color:var(--wine)}
.head .ar-t{display:block;font-family:var(--f-callig);color:var(--wine);font-size:1.6rem;line-height:1.2;margin-bottom:4px}
.head p{max-width:30rem;color:var(--muted);margin:0}
.rule{height:3px;background:var(--wine);border-radius:3px;max-width:340px;margin:0 auto;opacity:.85}

/* SUPPORTS */
.toolbar{display:flex;gap:18px;flex-wrap:wrap;align-items:center;justify-content:space-between;margin-bottom:40px}
.tabs{display:flex;gap:6px;flex-wrap:wrap}
.tab{border:1px solid var(--line);background:var(--card);color:var(--muted);border-radius:999px;padding:.5em 1.05em;font:500 .9rem var(--f-body);cursor:pointer;transition:all .2s}
.tab span{font-family:var(--f-ar);margin-left:.35em}
.tab[aria-pressed="true"]{background:var(--wine);color:var(--on-wine);border-color:var(--wine)}
.search{position:relative;flex:1;max-width:360px;min-width:220px;display:block}
.search input{width:100%;border:1px solid var(--line);background:var(--card);color:var(--ink);border-radius:14px;padding:.8em 1em .8em 2.6em;font:inherit;font-size:.93rem}
.search svg{position:absolute;left:12px;top:50%;transform:translateY(-50%);color:var(--muted)}
.sr{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:32px}
.doc{background:var(--card);border:1px solid var(--line);border-radius:20px;overflow:hidden;display:flex;flex-direction:column;min-width:0;transition:transform .3s,box-shadow .3s}
.doc:hover{transform:translateY(-5px);box-shadow:0 18px 36px var(--shadow)}
.doc .top{background:var(--wine-m);color:var(--on-wine);padding:44px 24px 22px;box-shadow:inset 0 3px 10px rgba(0,0,0,.35);position:relative}
.doc .top .ar{font-family:var(--f-callig);font-size:2rem;line-height:1.2;display:block;text-align:right}
.doc .top .lvl{position:absolute;left:20px;top:18px;font-size:.68rem;font-weight:700;letter-spacing:.06em;text-transform:uppercase;padding:.25em .6em;border-radius:6px;background:var(--paper);color:var(--wine)}
.doc .body{padding:24px 26px 26px;display:flex;flex-direction:column;gap:12px;flex:1}
.doc .cat{font-size:.74rem;color:var(--muted);letter-spacing:.08em;text-transform:uppercase;font-weight:600}
.doc h3{font-size:1.4rem;line-height:1.1}
.doc p{margin:0;font-size:.87rem;color:var(--muted);flex:1}
.doc .foot{display:flex;justify-content:space-between;align-items:center;border-top:1px dashed var(--line);padding-top:16px;margin-top:8px;font-size:.8rem;color:var(--muted)}
.doc .foot a{font-weight:600;color:var(--wine);text-decoration:none}
.doc .foot a:hover{text-decoration:underline}
.empty{grid-column:1/-1;text-align:center;color:var(--muted);padding:40px;border:1px dashed var(--line);border-radius:18px}

/* MOT DU JOUR */
.word{display:grid;grid-template-columns:auto 1fr auto;gap:48px;align-items:center;background:var(--card);border:1px solid var(--line);border-radius:28px;padding:clamp(28px,5vw,56px)}
.word .frame{width:130px;height:130px;border-radius:50%;background:var(--wine);display:grid;place-items:center;position:relative;box-shadow:inset 0 -8px 18px rgba(0,0,0,.3)}
.word .frame::before{content:"";position:absolute;inset:8px;border-radius:50%;border:1px dashed var(--rose);animation:spin 20s linear infinite}
.word .frame b{font-family:var(--f-callig);font-size:3.6rem;font-weight:400;color:var(--on-wine);line-height:1}
.word .w-ar{font-family:var(--f-ar);font-size:2.6rem;line-height:1.2;color:var(--wine);font-weight:700}
.word .tr{font-size:.85rem;color:var(--muted);font-style:italic}
.word .fr{font-family:var(--f-display);font-size:1.6rem;margin:.3em 0 .6em}
.word .ex{font-family:var(--f-ar);font-size:1.25rem;margin:0}
.word .exfr{color:var(--muted);font-size:.9rem;margin:0}
.swap{animation:fade .6s both}

/* TARIFS */
.prices{display:grid;grid-template-columns:repeat(3,1fr);gap:32px}
.price{position:relative;border-radius:30px;padding:40px 34px 34px;background:var(--wine-m);color:var(--on-wine);
  box-shadow:inset 0 4px 14px rgba(0,0,0,.4),0 22px 44px var(--shadow);display:flex;flex-direction:column;gap:18px;min-width:0;transition:transform .35s}
.price:hover{transform:translateY(-6px)}
.price.feat{background:linear-gradient(160deg,var(--wine),var(--wine-d))}
.price .eyebrow{color:var(--rose)}
.orb{width:96px;height:96px;border-radius:50%;margin:4px auto 6px;
  background:radial-gradient(circle at 30% 25%,rgba(255,255,255,.95),rgba(255,255,255,0) 32%),radial-gradient(circle at 70% 78%,rgba(201,140,140,.9),transparent 55%),radial-gradient(circle,rgba(240,238,233,.15),rgba(240,238,233,.35));
  border:1px solid rgba(255,255,255,.35);box-shadow:inset -8px -10px 20px rgba(0,0,0,.18),0 14px 30px rgba(0,0,0,.3);display:grid;place-items:center;animation:float 5s ease-in-out infinite}
.orb span{font-family:var(--f-callig);font-size:2.4rem;color:var(--on-wine);line-height:1}
.price:nth-child(2) .orb{animation-delay:-1.6s}.price:nth-child(3) .orb{animation-delay:-3.2s}
.price .tag{position:absolute;top:22px;right:22px;font-size:.68rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;background:var(--paper);color:var(--wine);padding:.3em .7em;border-radius:999px}
.price h3{font-size:1.8rem;line-height:1}
.amount{font-family:var(--f-display);font-size:3rem;line-height:1;font-variant-numeric:tabular-nums}
.amount small{font-family:var(--f-body);font-size:.85rem;color:var(--rose)}
.price ul{list-style:none;margin:6px 0 10px;padding:0;display:grid;gap:12px;font-size:.9rem;flex:1}
.price li{display:flex;gap:10px}
.price li::before{content:"✦";color:var(--rose);font-size:.8rem;margin-top:.15em}
.switch{display:inline-flex;background:var(--card);border:1px solid var(--line);border-radius:999px;padding:4px}
.switch button{border:0;background:transparent;color:var(--muted);padding:.5em 1.1em;border-radius:999px;font:600 .88rem var(--f-body);cursor:pointer}
.switch button[aria-pressed="true"]{background:var(--wine);color:var(--on-wine)}

/* PARCOURS */
.path{position:relative}
.path svg.road{position:absolute;inset:0;width:100%;height:100%;z-index:0}
.road .bed{fill:none;stroke:var(--paper2);stroke-width:26;stroke-linecap:round}
.road .ln{fill:none;stroke:var(--wine);stroke-width:2;stroke-dasharray:4 10;animation:dash 2.4s linear infinite}
.steps{position:relative;z-index:1;display:grid;grid-template-columns:repeat(4,1fr);gap:28px}
.step{background:var(--card);border:1px solid var(--line);border-radius:22px;padding:30px 28px;min-width:0}
.step:nth-child(even){margin-top:70px}
.step .n{margin-bottom:18px!important;width:44px;height:44px;border-radius:50%;display:grid;place-items:center;background:var(--wine);color:var(--on-wine);font-family:var(--f-display);font-size:1.4rem;margin-bottom:12px;box-shadow:0 0 0 6px rgba(122,42,46,.15)}
.step h3{font-size:1.45rem;line-height:1.1;margin-bottom:6px}
.step p{margin:0;color:var(--muted);font-size:.9rem}

/* CONTACT */
.contact{display:grid;grid-template-columns:1fr 1.1fr;gap:36px;align-items:start}
.card-c{background:var(--card);border:1px solid var(--line);border-radius:26px;padding:clamp(28px,4vw,48px);min-width:0}
.card-c.dark{background:var(--wine-m);color:var(--on-wine);border:0;box-shadow:inset 0 4px 14px rgba(0,0,0,.4)}
.card-c.dark .eyebrow,.card-c.dark p{color:var(--rose)}
.card-c h2{font-size:clamp(2rem,4vw,3rem);line-height:1}
.copyline{display:flex;gap:12px;align-items:center;flex-wrap:wrap;background:rgba(0,0,0,.18);border-radius:14px;padding:14px 16px;margin-top:16px;font-weight:600}
.copyline span{flex:1;min-width:0;overflow-wrap:anywhere;user-select:all}
.copyline button{border:0;background:var(--paper);color:var(--wine);border-radius:8px;padding:.4em .8em;font:600 .8rem var(--f-body);cursor:pointer}
form{display:grid;gap:20px}
label{font-size:.82rem;font-weight:600;color:var(--muted);display:grid;gap:6px}
input,select,textarea{border:1px solid var(--line);background:var(--paper);color:var(--ink);border-radius:12px;padding:.75em .9em;font:inherit;font-size:.95rem;width:100%}
.row2{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.note{font-size:.88rem;color:var(--wine);min-height:1.4em;margin:0}

footer{max-width:1260px;margin:0 auto;padding:28px 6px 10px;color:var(--rose);font-size:.85rem;display:flex;justify-content:space-between;gap:16px;flex-wrap:wrap}
footer .ar{font-family:var(--f-callig);color:var(--on-wine);font-size:1.3rem}


/* PRÉSENTATION */
.welcome{display:grid;grid-template-columns:1fr 1.25fr;gap:clamp(32px,6vw,80px);align-items:start}
.welcome h2{font-size:clamp(2.4rem,5vw,4rem);line-height:1}
.welcome h2 em{color:var(--wine)}
.prose{display:grid;gap:18px;font-size:1.06rem;max-width:36rem;min-width:0}
.prose p{margin:0}
.prose strong{color:var(--wine);font-weight:600}
.callout{font-family:var(--f-display);font-style:italic;font-size:clamp(1.5rem,2.6vw,2rem);line-height:1.2;color:var(--wine);border-left:3px solid var(--wine);padding:6px 0 6px 22px;margin:8px 0 0}
.principles{display:grid;grid-template-columns:repeat(3,1fr);gap:32px;margin-top:56px}
.pr{background:var(--card);border:1px solid var(--line);border-radius:26px;padding:36px 30px;text-align:center;min-width:0;transition:transform .3s}
.pr:hover{transform:translateY(-5px)}
.pr .ar{display:block;font-family:var(--f-callig);color:var(--wine);font-size:2.6rem;line-height:1.3}
.pr h3{font-size:1.7rem;margin:6px 0 10px}
.pr p{margin:0;color:var(--muted);font-size:.95rem}
.band{margin-top:56px;background:var(--wine-m);color:var(--on-wine);border-radius:28px;padding:clamp(30px,5vw,56px);box-shadow:inset 0 4px 14px rgba(0,0,0,.4);display:grid;grid-template-columns:auto 1fr;gap:36px;align-items:center}
.band .big{font-family:var(--f-display);font-size:clamp(3.5rem,8vw,6rem);line-height:.9}
.band .big small{display:block;font-family:var(--f-body);font-size:.8rem;letter-spacing:.14em;text-transform:uppercase;color:var(--rose);margin-top:10px}
.band p{margin:0;font-size:1.05rem;max-width:40rem}
.pedago{display:grid;grid-template-columns:repeat(6,1fr);gap:28px}
.pg{grid-column:span 2;background:var(--card);border:1px solid var(--line);border-radius:24px;padding:28px 30px 34px;min-width:0}
.pg:nth-child(4){grid-column:2/span 2}
.pg .ic{width:52px;height:52px;border-radius:16px;background:var(--wine);color:var(--on-wine);display:grid;place-items:center;font-family:var(--f-callig);font-size:1.6rem;margin-bottom:20px;box-shadow:inset 0 -4px 8px rgba(0,0,0,.25)}
.pg h3{font-size:1.5rem;line-height:1.1;margin-bottom:10px}
.pg p{margin:0;color:var(--muted);font-size:.93rem}
.why{position:relative;overflow:hidden;background:linear-gradient(150deg,var(--wine),var(--wine-d));color:var(--on-wine);border-radius:32px;padding:clamp(40px,7vw,90px);text-align:center;box-shadow:0 30px 60px var(--shadow)}
.why::before{content:"لماذا";position:absolute;font-family:var(--f-callig);font-size:16rem;opacity:.06;left:-2%;top:-30%;line-height:1;pointer-events:none}
.why .ar-t{color:var(--rose)!important}
.why h2{font-size:clamp(2.2rem,5vw,3.8rem);line-height:1;margin-bottom:26px}
.why p{max-width:40rem;margin:0 auto 16px;font-size:1.05rem;color:var(--on-wine)}
.why p.amb{font-family:var(--f-display);font-style:italic;font-size:clamp(1.4rem,2.4vw,1.9rem);line-height:1.25;margin-top:28px;color:var(--on-wine)}

.pg{position:relative;overflow:hidden}
.pg .ill{width:92px;height:92px;margin:0 0 16px -4px;position:relative;display:grid;place-items:center}
.pg .ill::before{content:"";position:absolute;inset:18% 10% 6%;border-radius:50%;background:radial-gradient(circle,rgba(122,42,46,.14),transparent 70%);filter:blur(6px);animation:shadowp 5s ease-in-out infinite}
.pg .ill img{position:relative;width:100%;height:100%;object-fit:contain;filter:drop-shadow(0 14px 18px rgba(62,20,21,.22));animation:float3d 5s ease-in-out infinite;transition:transform .5s cubic-bezier(.2,.8,.2,1)}
.pg:nth-child(2) .ill img,.pg:nth-child(2) .ill::before{animation-delay:-1s}
.pg:nth-child(3) .ill img,.pg:nth-child(3) .ill::before{animation-delay:-2s}
.pg:nth-child(4) .ill img,.pg:nth-child(4) .ill::before{animation-delay:-3s}
.pg:nth-child(5) .ill img,.pg:nth-child(5) .ill::before{animation-delay:-4s}
.pg:hover .ill img{transform:scale(1.1) rotate(-6deg)}
.pg::after{content:"";position:absolute;right:-60px;top:-60px;width:180px;height:180px;border-radius:50%;background:radial-gradient(circle,rgba(201,140,140,.18),transparent 70%);pointer-events:none}
@keyframes float3d{0%,100%{translate:0 0;rotate:-3deg}50%{translate:0 -10px;rotate:3deg}}
@keyframes shadowp{0%,100%{transform:scale(1);opacity:1}50%{transform:scale(.85);opacity:.6}}

/* FORMATIONS */
.forms{display:grid;grid-template-columns:repeat(3,1fr);gap:32px}
.fm{position:relative;border-radius:30px;padding:40px 32px 32px;background:var(--wine-m);color:var(--on-wine);box-shadow:inset 0 4px 14px rgba(0,0,0,.4),0 22px 44px var(--shadow);display:flex;flex-direction:column;gap:14px;min-width:0;transition:transform .35s}
.fm:hover{transform:translateY(-6px)}
.fm:nth-child(3n+2){background:linear-gradient(160deg,var(--wine),var(--wine-d))}
.fm .orb{width:78px;height:78px;margin:0 0 6px}
.fm .orb span{font-size:2.1rem}
.fm .eyebrow{color:var(--rose)}
.fm h3{font-size:1.85rem;line-height:1.05}
.fm .ar{font-family:var(--f-ar);font-size:1.3rem;color:var(--rose);line-height:1.3}
.fm .tl{font-family:var(--f-display);font-style:italic;font-size:1.2rem;line-height:1.25}
.fm .desc{margin:0;font-size:.9rem;color:rgba(246,238,236,.82)}
.fm h4{margin:8px 0 0;font-size:.72rem;letter-spacing:.14em;text-transform:uppercase;color:var(--rose);font-weight:600}
.fm ul{list-style:none;margin:0;padding:0;display:grid;gap:10px;font-size:.9rem}
.fm li{display:flex;gap:10px}
.fm li::before{content:"✦";color:var(--rose);font-size:.75rem;margin-top:.2em}
.fm .gift{align-self:flex-start;font-size:.75rem;font-weight:600;background:var(--paper);color:var(--wine);border-radius:999px;padding:.35em .9em}
.fm .btn{margin-top:auto;align-self:flex-start}
.fm .sp{flex:1}

/* CONTACT */
.join{background:var(--card);border:1px solid var(--line);border-radius:32px;padding:clamp(36px,6vw,72px);display:grid;grid-template-columns:1.2fr 1fr;gap:clamp(32px,5vw,64px);align-items:center}
.join h2{font-size:clamp(2.4rem,5vw,4rem);line-height:1}
.join h2 em{color:var(--wine)}
.join .callout{margin-top:22px}
.socials{display:grid;gap:18px;min-width:0}
.soc{display:flex;align-items:center;gap:16px;background:var(--wine-m);color:var(--on-wine);border-radius:22px;padding:20px 22px;box-shadow:inset 0 3px 10px rgba(0,0,0,.35);text-decoration:none;transition:transform .3s;min-width:0}
.soc:hover{transform:translateX(-6px)}
.soc .ic{width:48px;height:48px;flex:none;border-radius:14px;background:var(--paper);color:var(--wine);display:grid;place-items:center}
.soc b{display:block;font-size:1.05rem}
.soc small{color:var(--rose);font-size:.85rem}
.soc .go{margin-left:auto;font-size:1.3rem}
@media (max-width:920px){
  .welcome,.join{grid-template-columns:1fr}
  .principles,.forms{grid-template-columns:1fr 1fr}
  .pedago{grid-template-columns:1fr 1fr}.pg,.pg:nth-child(4){grid-column:auto}
  .band{grid-template-columns:1fr}
}
@media (max-width:640px){
  .principles,.forms,.pedago{grid-template-columns:1fr;gap:24px}
}

/* EXEMPLES, GALERIE, ESPACE PROF */
.exb{position:absolute;right:20px;top:20px;font-size:.62rem;letter-spacing:.1em;text-transform:uppercase;color:var(--rose)}
.doc .top.img{min-height:120px;background-size:cover;background-position:center}
.doc .top.img::before{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(38,12,13,.1),rgba(38,12,13,.75))}
.doc .top.img > *{position:relative}
.editing .doc,.ph{position:relative}
.gallery{columns:3 240px;column-gap:28px}
.ph{break-inside:avoid;margin:0 0 28px;border-radius:18px;overflow:hidden;background:var(--card);border:1px solid var(--line);cursor:zoom-in;transition:transform .3s}
.ph:hover{transform:translateY(-4px)}
.ph img{display:block;width:100%;height:auto}
.ph figcaption{padding:14px 18px;font-size:.85rem;color:var(--muted)}
.gal-empty{border:2px dashed var(--line);border-radius:22px;padding:44px 20px;text-align:center;color:var(--muted)}
.gal-empty b{display:block;font-family:var(--f-callig);color:var(--wine);font-size:2.4rem;font-weight:400;line-height:1.2}
.lightbox{position:fixed;inset:0;z-index:60;background:rgba(38,12,13,.9);display:grid;place-items:center;padding:24px;cursor:zoom-out}
.lightbox img{max-height:84vh;border-radius:14px;box-shadow:0 20px 60px rgba(0,0,0,.5)}
.lightbox p{color:var(--on-wine);text-align:center;margin:12px 0 0}
@keyframes slidein{from{transform:translateX(100%)}to{transform:none}}

.reveal.in{animation:rise .9s cubic-bezier(.2,.8,.2,1) both}
@keyframes rise{from{transform:translateY(40px);opacity:.15}to{transform:none;opacity:1}}
@keyframes fade{from{opacity:.1;transform:translateY(12px)}to{opacity:1;transform:none}}
@keyframes underline{from{transform:scaleX(0)}to{transform:scaleX(1)}}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes orbit{from{transform:rotateX(-12deg) rotateY(0)}to{transform:rotateX(-12deg) rotateY(360deg)}}
@keyframes bob{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
@keyframes float{0%,100%{transform:translateY(0) scale(1)}50%{transform:translateY(-8px) scale(1.03)}}
@keyframes dash{to{stroke-dashoffset:-56}}
@keyframes drift{0%,100%{translate:0 0}50%{translate:30px -20px}}

@media (max-width:920px){
  .prices{grid-template-columns:1fr;max-width:460px;margin:0 auto}
  .steps{grid-template-columns:1fr 1fr}.step:nth-child(even){margin-top:0}
  .path svg.road{display:none}
  .contact{grid-template-columns:1fr}
  .side,.stat,.badge-rot{display:none}
}
@media (max-width:640px){
  .wrap{padding-left:max(30px,env(safe-area-inset-left,0px));padding-right:max(30px,env(safe-area-inset-right,0px))}
  .grid,.prices,.steps{gap:24px}
  .word{gap:24px}
  .nav{grid-template-columns:auto 1fr auto}
  .pill.left{display:none}.pill.right a:not(.keep){display:none}
  .stage{height:330px}
  .orbit-wrap{transform:scale(.66)}
  .core{transform:translate(-50%,-50%) scale(.78)}
  .word{grid-template-columns:1fr;text-align:center;justify-items:center}
  .steps{grid-template-columns:1fr}
  .row2{grid-template-columns:1fr}
  section{padding-block:72px}
}

/* ===== SYSTÈME D'ANIMATION =====
   Durées : micro 200ms · survol 260ms · apparition 650ms · sections 750ms
   Courbe : cubic-bezier(.16,1,.3,1) · Fade-up 24px · Survol cartes 4px · Scale 0.96 → 1 */
:root{--ease:cubic-bezier(.16,1,.3,1);--t-micro:200ms;--t-hover:260ms;--t-in:650ms;--t-sec:750ms;--rise:24px;--lift:-4px;--stagger:80ms}
@keyframes fadeup{from{opacity:0;transform:translateY(var(--rise))}to{opacity:1;transform:none}}
@keyframes fadein{from{opacity:0}to{opacity:1}}
@keyframes scalein{from{opacity:0;transform:scale(.96)}to{opacity:1;transform:none}}
@keyframes drawline{from{transform:scaleX(0)}to{transform:scaleX(1)}}

/* Hero : séquence d'entrée */
.brand{animation:fadeup var(--t-in) var(--ease) 0s backwards}
.brand::after{animation:drawline var(--t-sec) var(--ease) .35s backwards}
.hero h1 .l span{animation:fadeup var(--t-sec) var(--ease) .12s backwards}
.hero h1 .l:nth-child(2) span{animation-delay:.22s}
.hero p.lead{animation:fadeup var(--t-in) var(--ease) .38s backwards}
.hero .cta{animation:fadeup var(--t-in) var(--ease) .5s backwards}
.stage{animation:scalein 900ms var(--ease) .6s backwards}
.dunes{animation:fadein var(--t-sec) ease-out .8s backwards}
.side{animation:bob 7s ease-in-out infinite}
@keyframes bob{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}
.hero.offscreen *,.hero.offscreen *::before,.hero.offscreen *::after{animation-play-state:paused!important}
.watermark{animation:none!important;will-change:translate}

/* Apparition au défilement (le contenu n'est masqué que s'il est sous l'écran au chargement) */
.reveal.pre{opacity:0}
.reveal.in{animation:fadeup var(--t-in) var(--ease) calc(var(--i,0) * var(--stagger)) backwards}
.reveal.pop{animation:fadeup 450ms var(--ease) calc(var(--i,0) * 45ms) backwards}
.why.reveal.in,.band.reveal.in,.join.reveal.in{animation-name:scalein;animation-duration:var(--t-sec)}

/* Survol : cartes */
.doc,.pr,.pg,.ph,.fm,.side,.soc,.word{transition:transform var(--t-hover) var(--ease),box-shadow var(--t-hover) var(--ease),border-color var(--t-hover) var(--ease)}
.doc:hover,.pr:hover,.pg:hover,.ph:hover{transform:translateY(var(--lift));box-shadow:0 18px 40px var(--shadow);border-color:rgba(122,42,46,.35)}
.fm:hover{transform:translateY(var(--lift));box-shadow:inset 0 4px 14px rgba(0,0,0,.4),0 26px 50px var(--shadow)}
.soc:hover{transform:translateX(-4px)}
.doc .cover-zoom{transition:transform 600ms var(--ease)}
.pg .ill img{transition:transform var(--t-hover) var(--ease)}
.pg:hover .ill img{transform:scale(1.06)}
.pg .ill::before{animation:none!important}
.fm .orb,.price .orb{animation:none!important;transition:transform var(--t-hover) var(--ease)}
.fm:hover .orb{transform:scale(1.06)}
.ph img{transition:transform 600ms var(--ease)}
.ph:hover img{transform:scale(1.03)}

/* Boutons et liens */
.btn{transition:transform var(--t-micro) var(--ease),box-shadow var(--t-hover) var(--ease),background-color var(--t-hover) var(--ease),color var(--t-hover) var(--ease),border-color var(--t-hover) var(--ease)}
.btn:active{transform:translateY(0) scale(.98);transition-duration:120ms}
.btn-ghost:hover{border-color:var(--wine);color:var(--wine)}
.btn-light:hover{box-shadow:0 10px 24px rgba(0,0,0,.25)}
.arr{display:inline-block;transition:transform var(--t-hover) var(--ease)}
.btn:hover .arr,.soc:hover .go{transform:translateX(-4px)}
.soc .go{display:inline-block;transition:transform var(--t-hover) var(--ease)}
.btn:disabled{opacity:.55;cursor:not-allowed;transform:none!important}
.doc .foot a,.ulink{text-decoration:none!important;background:linear-gradient(currentColor,currentColor) 0 100%/0 1px no-repeat;transition:background-size var(--t-hover) var(--ease)}
.doc .foot a:hover,.ulink:hover{background-size:100% 1px}
.tab{transition:background-color var(--t-hover) var(--ease),color var(--t-hover) var(--ease),border-color var(--t-hover) var(--ease),transform var(--t-micro) var(--ease)}
.tab:hover{border-color:var(--wine);color:var(--wine)}
.tab[aria-pressed="true"]:hover{color:var(--on-wine)}
.tab:active{transform:scale(.97)}
.pill a{transition:background-color var(--t-hover) var(--ease),color var(--t-hover) var(--ease)}

/* Navigation : état au défilement + menu mobile */
header{transition:background-color var(--t-sec) var(--ease),box-shadow var(--t-sec) var(--ease)}
header.scrolled{background:color-mix(in srgb,var(--paper) 94%,transparent);box-shadow:0 10px 30px rgba(62,20,21,.08)}
.burger{display:none;justify-self:end;width:44px;height:44px;border-radius:50%;border:1px solid var(--line);background:var(--card);cursor:pointer;position:relative}
.burger span{position:absolute;left:13px;right:13px;height:2px;border-radius:2px;background:var(--wine);transition:transform var(--t-hover) var(--ease),opacity var(--t-micro)}
.burger span:nth-child(1){top:16px}.burger span:nth-child(2){top:21px}.burger span:nth-child(3){top:26px}
.burger[aria-expanded="true"] span:nth-child(1){transform:translateY(5px) rotate(45deg)}
.burger[aria-expanded="true"] span:nth-child(2){opacity:0}
.burger[aria-expanded="true"] span:nth-child(3){transform:translateY(-5px) rotate(-45deg)}
.mnav{display:none}
@media (max-width:640px){
  .nav{grid-template-columns:1fr auto}
  .logo{align-items:flex-start;justify-self:start}
  .pill.left,.pill.right{display:none}
  .burger{display:block}
  .mnav{display:grid;gap:4px;position:absolute;left:max(22px,env(safe-area-inset-left,0px));right:max(22px,env(safe-area-inset-right,0px));top:calc(100% + 4px);background:var(--card);border:1px solid var(--line);border-radius:20px;padding:8px;box-shadow:0 20px 40px var(--shadow);
    opacity:0;transform:translateY(-8px) scale(.98);transform-origin:top right;pointer-events:none;visibility:hidden;transition:opacity var(--t-hover) var(--ease),transform var(--t-hover) var(--ease),visibility 0s linear var(--t-hover)}
  .mnav.open{opacity:1;transform:none;pointer-events:auto;visibility:visible;transition-delay:0s}
  .mnav a{display:flex;align-items:center;justify-content:space-between;min-height:48px;padding:0 16px;border-radius:14px;text-decoration:none;font-weight:500}
  .mnav a:hover,.mnav a:focus-visible{background:var(--paper2)}
  .mnav a.cta-m{background:var(--wine);color:var(--on-wine);margin-top:4px}
}

/* Panneaux */
.lightbox{animation:fadein 300ms ease-out}
.lightbox figure{animation:scalein 450ms var(--ease)}

/* Cartes latérales du hero : masquées tant qu'elles toucheraient l'orbite */
@media (max-width:1180px){ .side,.stat,.badge-rot{display:none} }


/* Cartes qui glissent sur la vague */
.chip.wchip{left:0;top:0;transform-origin:0 0;will-change:transform,opacity;z-index:2;backface-visibility:visible;opacity:0;transition:none}
.chip.wchip{width:auto;min-width:0;height:auto;min-height:56px;padding:8px 16px 8px 10px;white-space:nowrap}
.chip.wchip b,.chip.wchip small{white-space:nowrap}
.chip.wchip.swap b,.chip.wchip.swap small{animation:fadein 400ms ease-out}
@media (max-width:640px){ .core{top:34%} }

/* Arabe : naskh calligraphique (Amiri), titres agrandis, espace constant autour */
[lang="ar"]{font-family:var(--f-ar)!important;font-weight:700}
.brand{font-size:clamp(3.4rem,7.5vw,5.4rem)!important;line-height:1.45!important;padding:0 .1em .28em;margin-bottom:6px}
.brand::after{bottom:0!important}
.hero h1{margin-top:22px!important}
.logo .ar{font-size:2.3rem;line-height:1.5}
.logo .fr{margin-top:2px}
.ar-t,.head .ar-t{display:block!important;font-size:clamp(2.1rem,3.4vw,2.8rem)!important;line-height:1.5!important;margin:0 0 14px!important}
.why .ar-t{margin-bottom:18px!important}
.lock-card .ar-t,.drawer .ar-t{font-size:1.9rem!important;margin-bottom:6px!important}
.pr .ar{font-size:3.1rem;line-height:1.5;margin-bottom:10px}
.pr h3{margin-top:0}
.doc .top{padding-top:52px}
.doc .top .ar{font-size:2.5rem;line-height:1.5}
.fm .ar{font-size:1.85rem;line-height:1.5;margin:2px 0 8px}
.fm h3{margin-bottom:2px}
.side .ic,.chip i{line-height:1}
.chip b{font-size:1.2rem;line-height:1.35}
.gal-empty b{font-size:2.9rem;line-height:1.5;margin-bottom:8px}
footer .ar{font-size:1.8rem;line-height:1.5}
.core .disc b{font-size:3.4rem;line-height:1.3}
@media (prefers-reduced-motion:reduce){*,*::before,*::after{animation:none!important;transition:none!important}html{scroll-behavior:auto}}
</style>
</head>
<body>
<div class="sheet-shadow"><div class="sheet">
  <div class="watermark wm1" aria-hidden="true" lang="ar">معلّمتي</div>
  <div class="watermark wm2" aria-hidden="true" lang="ar">اقرأ</div>

<header>
  <div class="wrap nav">
    <nav class="pill left" aria-label="Présentation">
      <a href="#apropos">À propos</a><a href="#pedagogie">Pédagogie</a>
    </nav>
    <a class="logo" href="#top" aria-label="Mouallimatii, accueil"><span class="ar" lang="ar">مُعَلِّمَتِي</span><span class="fr">Mouallimatii</span></a>
    <nav class="pill right" aria-label="Formations">
      <a href="#supports">Supports</a><a href="#formations">Formations</a><a class="keep" href="#contact">Nous contacter</a>
    </nav>
    <button class="burger" id="burger" type="button" aria-label="Ouvrir le menu" aria-expanded="false" aria-controls="mnav"><span></span><span></span><span></span></button>
  </div>
  <nav class="mnav" id="mnav" aria-label="Menu">
    <a href="#apropos">À propos <span aria-hidden="true">←</span></a>
    <a href="#pedagogie">Pédagogie <span aria-hidden="true">←</span></a>
    <a href="#supports">Supports de cours <span aria-hidden="true">←</span></a>
    <a href="#formations">Formations <span aria-hidden="true">←</span></a>
    <a class="cta-m" href="#contact">Nous contacter <span aria-hidden="true">←</span></a>
  </nav>
</header>

<main id="top">
  <section class="hero" style="padding-block:34px 0">
    <div class="wrap">
      <span class="brand" lang="ar">مُعَلِّمَتِي</span>
      <h1><span class="l"><span>Apprenez la langue arabe,</span></span><span class="l"><span><em>pas à pas, avec méthode et sérénité.</em></span></span></h1>
      <p class="lead">Un espace dédié à l'enseignement de la langue arabe aux femmes adultes, de la découverte de l'alphabet jusqu'à la grammaire et l'expression écrite.</p>
      <div class="cta">
        <a class="btn btn-wine" href="#formations">Découvrir les formations <span class="arr" aria-hidden="true">←</span></a>
        <a class="btn btn-ghost" href="#bienvenue">Qui sommes-nous ?</a>
      </div>
    </div>

    <div class="stage" id="stage">
      <div class="side a" data-depth="18">
        <div class="ic" lang="ar">ن</div>
        <h3>Des petits groupes de 3 à 5 élèves.</h3>
        <p>Un accompagnement attentif, chacune à son rythme.</p>
      </div>
      <div class="side b" data-depth="-14">
        <div class="ic" lang="ar">ق</div>
        <h3>De l'alphabet à la grammaire.</h3>
        <p>9 formations, de la première lettre au texte sans voyelles.</p>
      </div>
      <div class="core" aria-hidden="true">
        <svg viewBox="0 0 196 196"><defs><path id="c1" d="M98 98 m-88 0 a88 88 0 1 1 176 0 a88 88 0 1 1 -176 0"/></defs>
          <text style="fill:var(--wine);font:600 10.5px var(--f-body);letter-spacing:3.4px"><textPath href="#c1">LECTURE · CORAN · GRAMMAIRE · ÉCRITURE ·</textPath></text></svg>
        <div class="disc"><div><b lang="ar">أ ب</b><small>alif · ba</small></div></div>
      </div>

      <svg class="dunes" viewBox="0 0 1440 210" preserveAspectRatio="none" aria-hidden="true">
        <path class="d1" d="M0 120 C220 60 420 70 640 110 S1080 40 1440 90 V210 H0Z"/>
        <path class="d2" d="M0 160 C260 110 520 120 760 150 S1180 100 1440 140 V210 H0Z"/>
        <path id="ridge" class="trail" d="M0 150 C200 120 380 100 560 128 S920 170 1100 120 1340 70 1440 80"/>
        <path class="d3" d="M0 192 C300 165 600 178 900 186 S1300 162 1440 176 V210 H0Z"/>
        <circle class="spark" r="4"><animateMotion dur="9s" repeatCount="indefinite"><mpath href="#ridge"/></animateMotion></circle>
        <circle class="spark" r="3"><animateMotion dur="9s" begin="-3s" repeatCount="indefinite"><mpath href="#ridge"/></animateMotion></circle>
        <circle class="spark" r="3.5"><animateMotion dur="9s" begin="-6s" repeatCount="indefinite"><mpath href="#ridge"/></animateMotion></circle>
      </svg>
    </div>
  </section>

  
  <section id="bienvenue">
    <div class="wrap welcome">
      <div class="reveal"><span class="ar-t" lang="ar" style="display:block;font-family:var(--f-callig);color:var(--wine);font-size:1.6rem;line-height:1.2;margin-bottom:6px">أهلاً وسهلاً</span><h2>Bienvenue chez <em>Mouallimatii</em></h2></div>
      <div class="prose reveal">
        <p>Bienvenue chez <strong>Mouallimatii</strong>, un espace d'apprentissage dédié à la transmission et à l'enseignement de la langue arabe.</p>
        <p>Que vous soyez débutante ou que vous souhaitiez approfondir vos connaissances, nous vous accompagnons à chaque étape : de la découverte de l'alphabet jusqu'à la maîtrise de la lecture, de la grammaire et de l'expression écrite.</p>
        <p>Notre objectif est de vous proposer un enseignement progressif, structuré et accessible, dans un cadre bienveillant qui favorise la compréhension, la pratique et la progression.</p>
        <p class="callout">Chaque apprentissage commence par une première étape. Faisons-la ensemble !</p>
      </div>
    </div>
  </section>

  <section id="apropos" style="padding-top:0">
    <div class="wrap">
      <div class="head reveal">
        <div><span class="ar-t" lang="ar">من نحن</span><h2>À propos <em>de Mouallimatii</em></h2></div>
        <p>Un espace consacré à l'enseignement de la langue arabe aux femmes adultes, fondé sur trois principes.</p>
      </div>
      <div class="principles">
        <div class="pr reveal"><span class="ar" lang="ar">الدقّة</span><h3>Rigueur</h3><p>Des programmes définis et des notions travaillées avec précision.</p></div>
        <div class="pr reveal"><span class="ar" lang="ar">التعليم</span><h3>Pédagogie</h3><p>Des explications claires, illustrées par des exemples concrets.</p></div>
        <div class="pr reveal"><span class="ar" lang="ar">التدرّج</span><h3>Progression</h3><p>Avancer pas à pas, vers une vraie autonomie dans la langue.</p></div>
      </div>
      <div class="band reveal">
        <div class="big">3 à 5<small>élèves par groupe</small></div>
        <p>Nous accordons une importance particulière à la compréhension. Il ne s'agit pas de mémoriser des règles, mais de les comprendre, de les appliquer et de développer peu à peu une véritable autonomie. Les cours se font en petits groupes pour que chacune soit suivie avec attention et évolue à son rythme.</p>
      </div>
    </div>
  </section>

  <section id="pedagogie" style="padding-top:0">
    <div class="wrap">
      <div class="head reveal">
        <div><span class="ar-t" lang="ar">منهجنا</span><h2>Notre <em>pédagogie</em></h2></div>
        <p>Un apprentissage efficace repose avant tout sur une bonne compréhension des notions. C'est pourquoi nous privilégions :</p>
      </div>
      <div class="pedago">
        <div class="pg reveal"><div class="ill"><img src="data:image/webp;base64,UklGRnAoAABXRUJQVlA4WAoAAAAQAAAA+AAA7QAAQUxQSAMMAAANoG5te5TmSt4EgoCI2mnP539c37jbOqEggeTNWhUsKubdw5+IkEXbSt1aVhNvRNJrfcAGc/LN/jf7cMbPBMccoVdAKsH7yWqLBLLjpytCqWSWCN5L5a5E12X3UURaDxNJniaJgt63QV1q7LKzpltE0JVOD5Og4rCpNPYCqERBh13ddosMkpIBGaleD0Ndloe636ocOsOtw451irbFsUUyyDlE+TJLuj3MlLV159oThBK8yy6IPorq/WpTam1IuMBBxvkvj6qtuj3MuUFLKgglRacoYsfqsC11bZCAXLbIQ6v3px522ULTLZovp2FTlcVqW6PXL0IwmS2WiV3tzZkrFxbJSTZPkzjQbz82xxY9nqL50zJh5arGa/ZMpZJ8qkSzfd3U6O00Wfz6KD5y1l19xQ2z5yV7+772NRVEi18zu+3nrntBqPwpl8Wrr6mC+e/Tem/dzSal+VNmPE0lJk9LW+AthY6P8elpqmC2EIW98YzsaSoxWaaHur8GU0oFkzyz6955BFRH9CrHR7nS4xBAclGcWHiU429Zcei20gioov3XTetTjqbAsaiU8yexej1aTwY5W8jCjmuW2nnyBHKa6mpU61JyWNXWn3imG5ck4taFH08OqyacAIznFM3jYm3Qi3kp0LgxnWQa6tL4UXjIF3alR/UfEYDWi2eZvcyqAzLq4hDIkovkxHVkP2GidGnutR17APyFNkaQSp4isPboRrYsz5JyZ/D+zKkglGC2YRIcl+dsjANaHtRimQrOsNm+NWOTQKOgHa8AcVnHSWYxq0oXgwuU4GdsjJ+0PGMsyP/4NRaMmeJriSMLtm6DCO7K8PKQCM56hqUjU4CBhHM2xjMt3/998oXqmFwPemwJza5MovsyvDwk0GtepiZMIzet69sYz7d8b7TZatueohsfSNVWWsn7Mrxg4zrdqTYsTvnRQmvQnbEx9lv+TLOsvumRNgOahoVwb4YXdKzbc0TAnOOf2BjPtHzv0BYNjjSYUqsY7tbwwj93nznf8r3o3GjP248S7xhe+Ke/xIgP8j7SLz3Diz8+iA7gLtJLWu29kmMMRMCNQTd6WPaX9LBH30Cm2YM4FMcWR29oq7yTQL78men1yA0aIn5c2gI9ZAV7fknt27f1iCNE+ZxtrY9A03i2mInN161xbrTXXsKV9pbn0pxvdroxjvERep6KyeOyORH5KaOyNAzMdmcDway2OC7SIFuKnfUYgrj87YGtVpjErNqV1tkRueGBnGd1zfwVwodfplIgTBTTpUZT7kqtLXZgqFEALK3PsNM0FWq5FLVmqu+Uui3ROaNvj4ahtUKAx04CWDDLeW1YfNYN2dny/eZeiM61VgSc+w08liFzjInzjudYvv/YVuamGc4DYb1nGuNDthrwEJrturhtRihpjH+3HHCRPi9FuVrf1tHcccc9vJ0IVN7Ba27qaG4qrWLpbxfljqN554K7DbSUS/C2U3rX0fyw6cwyNzt4OtNxNA+b/Wq9u52nubczSiV5Gk9Yubo+ZCBjpSv0/har+TK5PmQAQZ4cau9vLwsm2Qky+La5KmQAaiorQ8Omo0Ww2VbN9ZZUiDJVF0jFNrOEV9uriRMwmT+yV03DBCvi579yrMre/rFr4NlxcaBi+Qnypzw9KY2H/WqtcYx4ts805yhK8pM4Uf34smndLTZweH9JzdNAr97LBi+F+QpL085pVb9v6wsiyEV2rCnaKy8mz79Hm8vEqCBWjSFJgg7yl4Vcf9u0FxxC1iBJAWQ8n7O/Vw1e4rJYIVVKk8qU3g2+Fcg8KTslNF1UM1UXGi/QBw1dIVw+2r+vsI2IKgZq9Xa0PsN8xmx0n9n1rvUpyncX24hMqVXiocNdbCNCRAAvnUe3jcijVe5hGxEAICIZ4YJ2Hb7ZhLYeyBlzF0mMJI+95EKJkbyxR/bzG5n77/xJpcwRTolk8yrpC/8ZyE0CEMlO9r9nSscYJ5DyAkiPZJ3Q6jZQQwLnzDnirrnGipBTLChzBtwhcxTXdNYKwSmuiXZfR9FgQZlAksCbQN8on9xDMfwBMkvKwuAw2IfGA8mwDxorJJDMC+smjDjJsA92JMaBvCg8KJrNVrZuAzlYNSJPZEQAmmtaBEFgzeE+VUBxTWy3ZRoNcRQnsCbqQxvLYY7i9P37UAUpkOcoPtRf9JBEQ811FFLKgeY6kqUHBgB0Sg+DUAAipQe/fe7r4aKcMUckJdkaAgy1TJNIOVB8IJFy4MHQSDlQfKCRkmTYBxEBaK7pHOOc5pqIAP8kagYxmTUHwj5kgwAVElhzeAnZNQ2JZxjoLU1jzYHe0jTWJNtqJWmmRByMfhgaaw6EtEms+f83pI1UQ9qMOcaG+sfTmAhXjciGtJOh4sN/5AZaoYJW02igHfhnaByJlIP/8BDFlFa3gRIUGmgHPy2QRA1h2IdI2IdARsPH0lClkGJBGeQsKWsKBeXBfzmRwpqDXxFBECgoD31FhJkE+rylB78xQEAypI2mYaEEgikZaysdppJgSoZmXcTzSFAsKLfFmi2ygD5odxirTZXNA6A3MWb2lcwUGeG6Wi/qolZZBAQbaLFZvbLH+QSI4zWQePOtiF8W3oh39Q4vWK9/HFIPxLt8hxc8rn/6II77HV6uEckquTj+soiAKEH54lhNf58HBCO7eNy82uVjLGgSGC+O2y3L8wg4tYkxW729i0U+CYBxsgTlCwSorxsxmydKSeC0ehRivf72ZidxOs865JTwukbcvK72TThdfpBHEsjgdaWH8hx3m0N1ZJM4W84joNRO6dBoXW5W+zZ6+n0RARHVrvYNT+TFZq/5/Pd5QEm6HnlTbOyDf8WoMTgdOGZ1R4xSwBhnnBb/+CuJUfNUcC6VBMYcp4PXdcQoF3AukodcMUQh4OyIZYz7m9dVxKivryUySB5eEqhtlCneH7HWcQHAOOM0ed1gvXkvrXMNQsCMm71kYHpPF60RokhwoQT4rsjdaESg0cY5e/j5XrkgVGliGus6L3vXIIQBl8ksEVKJTpcjJfXeVAn19iOEsjzopvuaJxAEgG2LoJIoSGbJmS7nOV63YssAi587HvDT3YSacHfUBnXZfbelM12OM+6v3V43ZOt0UYuemgycIxpmy13Z1qXudrnz4807jwMdwWtGfTps0WpzKup2uc/Hmz8eBzqOKWpQF0Srret2ufPjLVACGON+eBzomCds1+lyn463RcYhlOCPx4GOmvST8cbj+ZQFN1AxfPnqmxeOt6axVj48p4JzoSS4+6yKbTvg1TfHP97M4X3nGIqQc5Hk08ChOI03fnfUTZLAnYlpDvX+yJv39xIZRNNZaEw0uz/0sN3+bR7VPboxWmZ2JxUDdW3BoEySbNmZa+5mtsFm9SancJ/iueuoGFiud1pCW7Xq8SUVnLF7ETBQ73Qk71c1cYyhqQ+tlPVury2EndSVLcc+12BdaDWDO9fM0CJnqJvi53tnJ0JfsFZKjHiVxePmjT0pD2ilPfTwNNcw1hOskzRPoLvK8jHm1z+qbKzS4s1gBcYcdmTLqgljBVwkeTaR47tNu/m6j4fVueu5pq9TbQ9lqTur7HKeAB/ZTGurt5XIwEt4jEOrdbnrrrIsOt3mylDCdTwMhL9AODTaOocnO1mN3Zl2JEXuZHK1yytxuPNV9lhsS+s+gRLkLSdah6bavtbTFDxoVevcpjfT9ovyWXwrsRrb4269tdlZDr67zSdQAotmT895cKPlc/O6KsXj2PJ3BCW0ukn+eI7FLRRSvf7+ZpNlz6zu46JDoaNlPoGrQnGdgWr274XMI8F9bUl3aMrVVj7NlWD8Sgood40+gU6uddm0n/N0Ubv5to8eZuEVllTHUBdHbvcdMQySp7vjOUoZ/3vB1DTvLakX9Ek07e5ngfbYngRvmRCwswWP62+vdRCfltQs/sgMXn/qWhd7bSCO00gCJ+EZG1hvVkVZahZNl4uT+vTJbHJG4mgblNOEiUhwToiHe6078kTNkuU8OZs91e3LmEGoFqm4XQ/zmhZhbLlZlSxSnxx0qXtahZqElyPXHl9Sj8X6pD6dDaCSjh4ZSQA/0t9S2+moT2dCty4fQ11fqk9nv8jwukTdif3X82EAVlA4IEYcAAAwdACdASr5AO4APkkgjUUioaETOS3EKASEsrd3RTEOXIDnfjsmH5tnT9huvUy/dn8X5BD1/+69d24F/oXpN/mHoy2NJ63VVN+QfV/6v+48jmJf8v/G/83zl/6/ir8gv8v1Bfyf+n/6LgsbY/6f1FPeb6l/l/77+8v9y+Mr7rzq/hv7b/tPRX/0H5c/2n2jv+Z5C/pn+Q9wj+Zf2b/X/5D8vPkw/5P896af0L/N/9P/N/Ap/Mv6//xf752zvR2NHDwnGjJ+qhqxo+C2dQ12QXwOI+zulSN9y/CgauaHzObXGXGETtrz9IKCHwAfFqi7U3gyRz4J9l6c0PHYSNDV1aQ4kZ8G/O8m65qj8ITtdwfFoOqbTJPEJdeYpyLGOHAyTtVlCkZkQF5RquWKKzqFBQA7ix0TTlftCSHbd7grOMIy21ncj+VrHmZXXHP8udhspv8FkP2+sIUnopNWhuOX3JYy/WCxrSNO9MlpqhuCB6LxLHs4JUcMywtLx2qY6aM43We/nVEF0b/KpeIVBgTh41YCcx2cK5psQs5mliVc2AUVfNVnlzSWKv8j48eqG9Ar0dkZqd3E16FgPEA+JvneFOXWPFA11bL4bFfffx5wB1v75eSFTypu+JmMwLJ6VgWq7NLdJ0GEtJAA1HijY9POIXnAwpCrT9eUXbeOEVDPkqVnDTNy1ZmnAViFEs/HVVSw0/lCz5ZBlYaNJhTbm/SMEaW8yhcP+fdu+k5eJWXF6wtWa4QASEPpNk4JOugqJfLubwLsgepMj/JaF0rbWE4OQPclwNVnn7vceVqUR4emmx8AuDXyYCBhp8Y4S35pLpyrCCOx1RdRdfL5CD+fZGA6c8CI5UNIpxtji9SVuDUHQBg1ZWomI/rZ3dbKVYQbgClta/xNmlaho72bqgW06pEeaqrf0RkVvxJfX3Hw1c8mCMmdUn8eKKm04Bh0/ClapEy5mfBpciCPBuM0HUNKmQVb9dkSNcIsSWTwsCOopmObe4IN0dNiNmJyaycXCx8246vZnpeNxfLcZ5TIVmf1T0eEO0vEcMG94Nwbui3BHo91aJZDNyzXZ3IIIGDmX3nvyJsz7AndXFmf9KNB6L5KxPtbXl+FPM4rNWgniRG4r0kbpRKgsvDG39v6qpIC0PeO6CHb2I0fGh5emkZ1RYB07ig1sv3fqKpAbrmy+daNiTjqVdTqTnwzKWgfyl9iqtUFQ843OVGrkQPCgc+XVjMiU7yOXOBQuGZsKPVre1uX4AD+6mSAEji0lwvRFy/ziHjl4HaXDfAH8qUbcwePfuikLpc5r06L3dmzom/Etf65nz3x2RS4Vw16qmvzuHNWYYcyAybi6gPHKPDVGcxAChOrfdNePtLu5R0+7UBSm7+czWseRZhQzFcmlBQlvhGWvmZ0K7Wdd94CYNAKoIbAqQ2KnkU5vV8EvwvYeTyBgcuoqV+7Nutt73wad+3iHz41bZudnh5YwYmhmTlOj9yUZebi6KliYunrGybcWUbGiwaazti6UPiCxNmidM6vcAccY320HMTEN5TngFx6uVcAAABQhaQEuT7h92GM8eHeA2Yv+4QtSUMhYsnLeWYvIIkxP4cG8QMkp+CVpKL3I6K+t6jGJj53fLIjC8yIPJunnS651/GrfcRkN9L67Rn6kVKw9VmCWj+oVI8T49K/23+6uLv7nwJXtwDN971vmMuWlz1nLsRIbgn11wFctx2UKl3ivHFTeP29Gx+19GE6NaN36QEKsOruRvby7UcVkNFDRYZ2UrbpixoWy+P7E1YyTh2YlP9l7FHoT2lOE/uxDHCSFnKYF8HHinp4ewZ3yOgrxEEoFauuHhq/aBr97Nm4WHRNMRZWUOxZggkaI6HiFm0S5/U1GhcQtnGWWw5+eEs3Sk99DOvw9cvGlJNsBiPK9ILmPNgKtOnov8dzj3cqxAoNKfPFM9rBzKNReIDpuUhEWoHueR75oYZhF3WeHrx2LlEgEL8yahqBl+HR7KYEYrNwALJAlpFQVSqWfdOWkoYqcbP/F+o79qOdTqbnPE71DfDamg2EVMIoZJpq7GzZQHhtbQ8bwon+UcriFpj2XwM7K3WAab29bkV2Yi1km3N4AbCXShOGEKSRENlQg/Emdx+BJqeOHd7fFfG8iTkCzRDCu9fZu8aN0rctRmWkHzwYiMUIvTf3loxblbGyVhmPi+nzPejcOvmim74I33RRPNfYqpN3CFOVkczDsXORIXxupQeM3L2//ZvBGcG/y3cjtw+yrvvnv6RADjyrli5u2ZKCuayoqNwNigwqt8gQqqymuzxkLpQNE3WMqvg/M75mra/fntFhOws8fYeUTUDsX07rEUUv0KXvle7A97D+5bddIAf89CnH+/hGf4zpyzgQKLllI2MrC9KQUjneUv/5wo/OwFmJUDuo3UL373ww+0zpKzwjCpbLFGUO1B8fSjV3WEj9XwQxIb0wFkoFwx/u8q2qrdHle57AyfbZ4B/jvuz8eaA3ZkkiXBeblM96um2EjrZfzbaL9vG5NIANVmATLSc/Jv0eBRoiQEKTbdnTLPCS6/HLuwDEY4sYJxGamyzo+7JZPiR10dmMtvSFZ3zp7bjCB2uIP+n99RY/PNXmupCJORgkJP8DRZ9gJwBT+kM3WLmmy7FVifERj3BR7lZO4OxzCmDyaQ2ztmUq1zHnVrEUv4ViWUIcFoGmcTtn6Ju4twnSrxM7guNq27UH2AJrbuVJvJNLKZugR5fgztMsVI+mUWG7j5MfMR6CmEs/PWjs2JMEvvAO4Iig8hyDgEjne/y2ojqXg0rkEtqJEtskSAwKOfctO41YxQ7V2QOpeNIRZkk8KhlaE8X7nOduwT6Wikf7bb9hdCU+woIBOHn0XgF5kLPehtRT1DUMoGot6i0soYQrjMaDXNTPm5xq55+Z1V/AoNI9urxSrXDbiJPEk1SkvfQwgAZFVcC641tv6AaXD8VdhDM9TMJ79zjm3jVpj/mAmqkM/7FC4dVijK5ipTA5n2zQigylw3XLO2uvsYSkY4qXE+yrxuA8J6exJ+QM2CvXiLiZPX5I9X1N/vy5AqjV9jCvm5j4f6M9pn1+H5gQHSu+DvXr2VHT3i31jF0NyLa5U2QGp/QBrHxfLC10Or7I4jfafArUhA9lc+muVYFn3YEN5uc87tH3rzxc590wOFcxvVnwGq51d5Lzx37VX564QWFN2tit4N85bAIhFuE0mSAA5uy6zaKvAoM3mCJ3EiI5gBga+GxoyBlEa+wTADGpKi6P8ja0leLXsVA/4viLQa4cPrYgtTpslNSckE1gMNfhwMOYvfiCmqXTzuxKndH1BYI+R9blZ/JJVFaUdJLsvo5WCcK3+O4C7/2Qyt1m2O3ux9LBxAhx3AAOzkNEPyr6ZW4ACuX9iD19w4nqBUDjZnRSsqtfcW0w3Vpb/6uFOA8OliaG+Aav2JOGiUDtEeGboc6IWMtffvFXfZoIiPcg/xzB776Hs856r/p0KDcbJxwNwzRp7VcZTBzH19g37SavTPRM0l1eM1gJjeAN+ZlzwcmzDwhyPxmAfg8gcfro/7vAUAU8R/r2F8d6XzujODIjLNFd4utTF968S7x9fwyDnUjPggwvh9q2LdXZKMXjXaPOf8fn/ToxjPZwwkvcttHht7ufIGn440IN3CeS+mv9VTi3v9Pi+rYJQP+t62UkBVQX0Lf+sCWMha4XOvY+bxlzkwOLsJvbTOWw76YUSgeZxZTBwdLEvHRjmsof+6YedlBFgBnRuk3l7pIa5+0kF5LE6EEXd6dM8iGQweeRGlps+y92Mbu53LQ0zmPZ7DVI1wR/yvhWRXBURnK6u4CX/WHfkAg8vyPJJhzCTFJMXBlLndEEiGjAiQkKXChlh0nb+T0uJ1Zd2Sh9WGtTAEbJ33HvLBzxGtr/LRydZNgZvnOvtYxo2QHC9rtzkQ6p2JyZWV8SKWLIHLOVt1YP+vOGkek88UPvaHIC/IWoP48S1Grk6CMW4KXC7eWzDdPIbYGlczYIzaZZDp9/HKeYeHm8xg/BVYgqPWtts5E3RRg/7YLS1Ntl/NyimvdbOBD7zwNgnV17w9tiiP1kGsgCescW72BxGAphtNilx8W3/08p7Jvh4vIPpdIQjJgNUlI0ZEuWCwX/6uSMm5cqKJnA9KRbP3nYm48chUp7StizjzEcipoAKht82T2NlqJGv1v6XWofkGPR0jZsIMj/aD+4WM3jgwRWJ0VxnbAO6Xx12pHhlUWYNuFq6B52UL5K7J/x3/4clFIkPJGm1/pLQNiq8hp6RqSlBo4I9QJkcDMYnbFj7XPBL7CG6oCMV1cCMA6mupeokCllqMINJHWrlRVhh5rh+gBrav7+lL7+1rVNvozLdxDEq7QF6EyFNxPhXDwhJtmolpFPE8h3v9+14QQsdp6vtHBAsbi8PgQBxzyutD9MZdOb6brKpqJhKHTMoTBd/8gRdcY12ju9yaEp96qNwSq4SXf6R9dJtIqZ5rkGBhDeb608mYyjr9JkEyeh+ueeos3jUKkRke5rGD2EfyJblT1mxVmcKl4t4e8407j9aRR9XJ7SQQP+tpQ4OrtwLGNEglz71N7B8d3sO/U8Kv3oIBmWC//TwACeM/YIynINsPRTrX1Bd8ufU/8s9FTmQg+JI2xQ9bWdlsfmF/73q3+tI0BFoNR1R+tJCe9rHzyeqq8NpqRonqlLfg7LIORJIv2YmX0sI7xmZqZUYs43RCUuJypZjoVzWkPWB2AQWgj9vq5NBIZfmd7dqG1x9zxvA0ZCjF1356j9xWr1/40Kz9wkFUtphJlNx9qBgdyuOItW4VlAwFXkZsonmyg+QFfFn4Gh6DLvK7nUV59OgJsaDkcwL/+lGXRPJgPkLnNKFPSQqRIX3/3+fqp4Com7w/Ju/iCjKpcdStZkpPyc2+/+LbxSy83hM4PrkBxV3g/UJbnjBXX1arwI4vhXNFy6Xw8lbby1T57iuNlT9yo3PLwKjghJht9CTCSsEKVQVfT64XY7mmRFbaIJexoBB9Jq1nmWiLXeWDOTwvi6cfGALb1iNJJ+S2m5fSUqr621JE95XP961LujY77tmXeBppkuN3HEiOTsADI++HWwhd7Xeq9e2//ung+fiqKcuOSF/WkPzMppbvSvefEXkaSVfzFd2kpVIAcnif5g/XkfMRaj72pY6zolGv7YdylDQyZ62z+yWFVKAlN/Pobeh1FPJeQBqcmAd4PYarPVVe1/xoDHuqkbGKpHJLts9+og53I9K8vWymqYH4ZXiubf/G01Z6QxloO3Dbx/TM+z4FfgxNr7yOWKsTSy+mfHdQZNe6lDB/y1T9r+HXeXGu7P2QSkosdc7rCIM1ki5HdT4EgpkDa/p7ntGTm3vl/jegOdTaqv4n/aXUMp34DxmRVqJu0oGpjO+OtLI4vKmxLdrB2dNqVs6eTMMz00qp9RsGm5hDDD/xfmZlZDjls9Wx8J3dgP0LRO4oMMOfUSDTcpdCzy9cN47KBEpaHGNH3cyHka9NV3Myd6VHQW7ZrmQvAG02Os/vOEfZHfTgx9/JlaW8YceM++XdM1Hav63RrUnd1oxkETkEuYJbresVlakMkptFm0hMaAKsaecnly58fCK3YSkrMqaALqdsoVm2Pa1Te8YwrLmfUjiv5HKt6D18kVgjtRIKcasu/DlvsPZb9P9CBWNcDHMxPdyZvxvbLHpBqTy0KlC75hRHTGfxiVVL9kLa0NYKYMvxbCaewJdr5DEzGOyWevBIMghG0hIheB5cdBMIC+zsQjNaiKLDC7cPS+z+ASIuuDLAKUJGn2auoyFtzDNczWpWQ4zXzwLBQPJjPnzNH0a7DAXd+jL92khX1reBPsIC6KUni7HXyGmFSqUGdeqpZY3NOBak7iUK5MVzzKQzO560tD6KNZeViTrVJrzXutt7P5vvDh0DxNY4/diBf9trHdjqceR4zcwncQ0lnlFEzlYyRVi3VqTRqeaA4jiofpD1VgyRbYIydddB4/Z+GAateDrZ/Vg64HPrvACBym+bttRkvBWXiDe7NN+Cm8JNXWMNoW0NbGaGEmD6Nfs+QOklKBnCPRxKfUvpl+7R6eyb2Hc4s5t+O2WyWZEN61OJ6SxKxHoVei3kbHCB2z3UvIMInHXKOBuOU97sKBJ5wE3KqQaKxqGArLZvmtILDkm1rH0q/u1r5kG9whU3RgxqF3gMaJ0tCL3Yp3eBGUPwEwudyKTSzJzfKCGfe8WPjDIkef9YmPhZR50yfX5eE/Vgy50TCJ54k6zDhmgbdIoYVD+0spX9yIeV4ZsCoRg8/4CQgdYxihBcKPvDjNaPIufkAnD8w/Lcdk9q9g7kfUMQL3UDyORA4uJ9/CwYIXNER2e8+k5ZdGKaZa2X8HqMLh8tMcYZlTqSdiih++DZsSGSVwfNM3sL/8HRMihDjECGKn+yrJi6zKyLJFXyTyDd+aRnq7LugdscZLp1eDvNpF+OFzp5b7vzodL40dCBX+OuIC7I6GFCHpYZQ2+9fINrbpa/rhnn2fX9lI4/c/LY2wB6XK6WF7fLEz+u36HvSSuCTU+nu8/WzzK6X4JCpQ7hqdCyONZTLPiIzlC+NZ4lmQ/XE5ecGtczTO/OAb0Px9D2lHmabU8ngTzP/KRwxy3RQzCu30Y+R2QGRUg3NzyyA+TLGLY8+SCFqK5nodtUabZTaYUETLKUzspaFCl57z257XVb5Bxcmb9uzT3b8p7fTRRkGkF6xVjI0NdmLhoEP74yO/T21F/bSaLw+ovPtk97O7zpYFH7K7tkP9FUACScOTy4xoezSKdm/L/kudX+6XAtUczpUHML24D1HI3TWnxIRY9+d6Q26aShNh/2vH2RjswJhy80xFezJKftoJjA93UEizayRqqiPp/4BLSHE0R8rpIcWGwUCX2zuZm4gZbPS/SkRk+mYniP6RlnhmDdGNN0tpATRcbDjm4WwQutNjZHSfroHVcPzleJQj3ftoK95gkSIbnlKm1+9TyzUD4jbr2OuY4P9PXkKIZfqvJ2+z8fBeQ+qMS8ksx1VyZ1jc+l5zJcZpQT+GeNl/vJrnlPH0cm6m9ov6jJhytJF5VNN/kCs2HxsV1pXjxcS4AB+5/bBoe3WnEcxMUb8waW+F8jgkPCFm0jnUOEeZttBiwdHSxKmxB1++zUfVWfgepDNyirRsodIx1QCh4kIojAtIizymBZGhfAy7CrnEaJRVO9NgUQatfxuAlm3Npms3J7Jcql9yY/a/gVxqjtvfA0bx/Xf/CuM3wtRMeH7t8yV0JtOM8BNeWfbMXJevyrTSCbZ0QahJBgGN1pbincPUMUSWHgidoeJZzt8m2Nge7nQFcnO8Z+Bozn52EckcvMp5FCXXfn6T7C/PF8gYMARltYq10QEYpEZocWF1vsVywYH88BHK9Cx/pteHCsmtsPRWABP8XsANssXo5CEngDvt/BCjVhv6tId6LubsBJjkq7LPDxajVjHGovJwIigHPJhI4Dmf4k4AQ0fYHjoEFP6h5yBVVoKqShGhQlbS1+qr/BbTv4/sfq34zMps+AJOX4lxsyrLqFnCWRvR4omh1fhp+jDc8SnjfD4T+RHgCR3g1rEL/d0PLBwlR4iiWDzqqp64xSfIf7Jk5YpYNZR+BlIHACEcWgirHA9ztJRBGj6IAQcSOnOk1WHmp4kO/O9bLxUf0JCoJYGrLC6haN7qrERnDfYuvgqFxTNonjFgx9o87SWdtFJtMGSdOpQOByptyOJjHlRghbGLomaCyF1Xbj4cFAzpIztdZjaiLqECBuYDhlj1Ke/kFVmym5IjVSm2rR4z1Tt5x7JByUCskhWrkrs92bjOWJKedB5oYDIJ9MAj71/wokNprgJe9JYAUjOi797LScA3Dhei1h46yanrkLIUHMdJBN2/PGiYGUaYyCuTnrvKcjNu83nGLuNsZVkUGASxRALFMHCW8JZzuF3pmIEW7Pg3pj5LUvdTkxpnEnWoXO8py+r9EKk3p9W59VUKVG90dDyCotcm/m14y0mXhTaiVUPXVyNpuRa1UfBBr1cKiCNhutLPAOttG1c88MKbK1TwfkAWb0snK+FCfRXJhhwGjxe5FLPeL9is/HnPQ8Ao60pYkLf9z5NzORX3kjFqp0cePy3kJ++1sziOFYLIgPOGCDTv3X7JFWbdV/XHkeIr9i835NepJhQfQMvmq0OIctBkKUxXNUnqjILHY2xyPGx77uaiodmjlrFxqgETNRFrvcl+QPCHOh+11EA6tzsWIRM2bpmGCjb3nNeGO8HFFnseEjoy6wTb9jQ5+XPjj3BBvQ1ccqK6GQqOINgt8AhvjhOs/d0eW+p8dMFJ2nXP9/WcMDvK0ku8BM44BBun1+++Mjs02i6wUtUcvZTtQ8fzwECfpx5xVbG/kqD3eiRpP5DFjfGGKd/z1MmFxIPGJ7oGz+wIwPkLrxvJGDRBjA6om9XeqNci4tBFkcJ7tdG5/fnJ0dM6gy52+LHlzfp4psA5rAW2nnhWhlXxwht8IItjtWL0lq8GdiEdFB/kL7CpnqmdmDGuOzTZJz9DmNhZJWkZsJ6SegFkxyAKc2sskwmlgaWkkL7iKyd/k/gRFnAUIo1P8DFckgRXw1dztdXPHDbSXW5dSb2aa81z+uKdG1vs38FDhiCDSfKaRNg0qKG9W1Svg7oMOA+Y8S22myBiSa4qVMqceRlADqazbD/me8J8iL4EEPWKHfd5Hd+vqyovWKH64roHDiBX1ilkUGapS62DgdRMAN9zOFcsKh5DmM63ejbI8+KBpzoAAADHiTwH2TTrkRLQYxHVfwEZiYhEav5fX13ar4cQDWMP7fCL9bvy/SqRyhraECqj88wI/YcifkAgmuJoLNqap7yC81EcJOsGmB++fwYd+SB+N6l9xXmcwRf2UXVV/ZyFvNe35BBn9jRd3wH0HjpdnNryPhguEUi4kJwnZatuTzj/GUnfeI0HhxB547NwZ35qfhgVA/jVadSZO45uDRp0MTEtNlFWb5h+s6lxDLhjUL/CqsKM3tR6yVhRcXU/x91NxjatRMpnUT13lvPuWymltpp7NS+Wj4R8qI0ZPtS6coGlIH3n8+8fxbzyt6zJIcWmN/gn7zwqA2/ssRdIBMx4v6CyqPcseXfPstiz2kIc2Sl/DoNTVhzIiQf20+qVNZG2R8fRsdL8gPCBisj9AUqh4m4H+9xXshd8o9IYG6LvXKjNcq6n3d7KeQlYwOgt9eurwLLEt+TTF+pb1OHeAbiqsuiLhXJ28fV2OsbnRnXnXoSefyHYuF6KbP4vYijt4gvtzJLhnNpZsvRqfVyEx9GEaFMzlm11McnJOypVrZBUc0l05R3Chcor3EgzW4ySm6Qd/euM/jO4NVHW17hAJB4FD8C44wY19efcbGn1UKy/9VqjIHDd8Nq2b9vo8uY7viD0eB0Mex0cAAAAAMdkCzENWVqVG7+69cq1iVl0cwZ389Oxi2QmrGZlqH8/I0JLbrn97pYzy/57eN4QOW2O6CVAM26dWlivlTnQYLAtptmrHEx9aMQS5WfX6PRCkIILawGC/eIukc+MiBNRv51vg/BleFbKaSRo38rz3mEdJTsKLbHe083viPjMSz/SUeY7LGfvjF90tZVW2ngYtAMHgKLLnPhT16s9J2N1nGxPZKImYiAAexTlnOzksCVx9ZG7OzSvMAAAAA==" alt="" width="130" height="130"></div><h3>Des petits groupes</h3><p>De 3 à 5 élèves pour favoriser les échanges et le suivi.</p></div>
        <div class="pg reveal"><div class="ill"><img src="data:image/webp;base64,UklGRt4oAABXRUJQVlA4WAoAAAAQAAAA7QAA6AAAQUxQSNEKAAAN8Ghte9Patm1JQkJgcLZr6LWNeP9X1WPt1QEnbISkX6VUwHY1qr9GLCUiYMG2EjZKtC4SSce1+ADj5Jv89+SkLqQHiyKwQFwoczJKbKUqA4HMs9cJVMdNUQUxiemPhZTR5eO37SWAKRosF1TxJCGH37fh+5OlkwnZGxePFsnht0KH76Il3yhCmJwuycdaQ+gu+ml8OEGrv3NRljpwZTx/cgdofwchSG0gbIccJcp0x9dAqtIE7eD5wByh0+N8kpW7oBVMTPJTdaXLM6nOOmz0kJ8NId0iJlpD0HJSNXSXkWV1qcAFx64ktMN/4oW6+ntaLGF9qOF2pSMOh766vxsocZTQrxiWMqLNt2NJ4gpLrn1MXjN1LqubfzqrLNxzfLN/BeOS0zu7gTEGjsno7kRZNs6aL+Xgsi/O7jqgmzxNpNW3c7kvwX09G2XAa6g5XWQRvasbKEu4Mckouz8xmUnWfEFz/O1D37RMfhqngt36nqBKBV/P9rTZKvAZV789Z+zObqBCaBCZvNZZ9/aaA3Wsb3UMH46yVEb0rv/Kl097/v2XrfYXjgxfl9y4O7sBjObMfGEcOFtWpj0EwbnbqoR/Unf+4r6uvVj1vrpYXyWwdJxoDe6ubnBWacGrpifvTs59SeUSepc2fUSOBgO7PvhaOGdIHN3fDeAoc86zWecRzgg5TQ+F9pVtlRGSfaEb6LeE+sOBPnp7MQAwxtABhOJ8NL4CGucQsmymo3NRWU8BDTGVBWzcL6MZ3e61j2N1usjc4eOIzREl86zceFjw4Y8fI/vn7wof39p45rb+CaZsMJ2ncKiBEHSK6cBDwY6QKInJAy4MhGD6mbm9YuoHTTAlLGKOZcm57cQKnGDGE5lwoyOClgNWjGbk82KPZrxhKmp1XHUc7SRoF/Phj7cRGA7r7r2CdjFl6XQeGyPYqQbEvKe5OJ+MJ9alBplFhDHnUAsDZCdf4hym3Jl8IhlOIR4f4xy2Wq3ly0QgFwjgsT8BSl38aZfzGKvCwwAlqEMlx8iRjE/ycqfBl7RXcpQw7GKz+qR8OerNB1lO0yahJ9QX9m+HwcssZdiFov0hq+0fp7xJYSQJXLbvp/x1ljD8SI/SefQ2FfjBOH9SsSJP85hhCON8aXBQzWyPIozzZ7ZPRpJhCOO8me1X0TNKbF/Xe+ndu5ovBlEgGQSqXUEmk5QFkkHsebXhy1nCEGPUnZneI+SK2GTP+My3KCNU25WZP6URcg5en9Jld4jmo04RwECUvRSX0Yy32EEMRJlTLQcCO4vEqypTk5gz7CwSrwSeVZxz3ICNZx/bQzpNo0ACG0L0YWPHk4ThZpH41Xi1aZz4KDp4PXLiLwRDzSvmF1ud6iwTwRRKQOtGMHIOXt8Ey4yTYJJmV2YTzoJJmlLJgUAOxvmIWpGDcR6iVtxgnJeoFTcY5yVqRQ3GeYda45epCKVQoov3er5Mo2DCuGq3b/xiyME4H/1iuJE++sVwI31ENrjBOB9NkmDCODC7UzYRDDEY5x/jLHLJQgnjCKiTHuTYkD7vUwJ6d8o/ScwYXpKoMfwkUYuX+0liFi/3k8QsXu4niVm83NPGmMXL/WyMmEXiKbAJpkUCelfmE44bsPHSfR9OYGNqIgQLJrAhuizjXAYT2IBetxYPowdsPFs8vEwjzICNnx5e1ICNzx7eAG4TZE61zDhqOzT4vPdTCLcJclc378Jqm6BQnmL8KXivfTz+bSjc9uBrgRmy8TMFE9kg+Fy7l0c4l1vit0WD52Qo99TEbDuzkE71oxn9ry6O+18pweT/g4q83FyCWkT7XQXBLNLlXL3vdDiL6XO02tTBLJgcJdVBAQlo4qG1ry9FSIWM5sEVUr8XIRXyEm9W4axiyWRsg4pb03l+2vRdOEIouri1/2Vp4WxiSiUzjmuT9dn2vzUQok2mpPisCuQHiQaLVlX/1ehW9d8M1ard7hJO4DpYzs1qWwUzienb6MaLewTxDT5WZxvMlE4mPd6Kku6L52B7q53upbsYYwCAsM0p95uyhp6ewiwBYZtzkVTrQkE/W3hUGN/q+Ydc/Vrofj4MxreaPI/rP9Y19FONsUCe5uJyUNBTM4RP2nXjuyBmQlg8fyZFcdHQgyy0kevM7j+KCpCR5fU7cizJ6vftBR4vC+s0fZpErReZerAsxENS6fQpOf5a6F5koSy8qYweaodRSpzD3g5ruVAe2hJ/F0ojvPeWiMYtfhrs348G1ZZ9ei7BsnxIysq5wLV0rZCDUuVRp+NxHLSWjjiwGqg+FqfybEZvGXtkS4x5ytjyCFTtj3U8yIeSBamlI460eftSVxdgEKWDPIkofSw6x3QoWdfmlYrIlDk5Trs1D2yJ61AyoBpelogsjSCO6KN30cWwJRhlrgwlYC1ewhml1PWyDxqgl6tifWUoScbbvB73uAP08vbXj/LqULqDFxaO3v1agKD3D6XQcMAWazO6eyiFiOMcAKW+7OsQ48dhfJjbU1WDL49L4zfL8/FTVq8LBZ48Cm8RXIj2/JdWpMmPR5kqTCNNXjw9bLGMNJ0PNfiw52iFpEMzlrzqfzk0z2RtcLS6nOOCGOf6LiIGgKJ9aapjnYxj0jvBrAUcnSPbI13krPfgTc7PJ8DROaLY0oM8W9APhZUPE+xVS5okw3nCfHhJ2j1GpSNgNLjD9rpzJIlo/1G5xZM74JJdR64qj5YcixuWtCfvDWuQGUrKOgfl7nQ+A4/iuGtJe/Su2YBKjSr3pXWgzrVIIzoe3rakPZjjsZDsWjW7U1kqIExmWZ5Gzrvt/XkeI+C/du3rL4cmqlLHA8lolCXRHT7MAFjUrmkL5pOyZbE5ftZkecIZvfdX44tF/e2DDVWlL0pXFelEVbx+Di87Vd8bhO5L43Rtat1glvSzxv9nLO03VYTmWrBBxDwWLczivRfiRW7Ut1ODpKUId6WuusEGmQr5mJncA/y2tEf4Rr+ZthokDhpFWJEuNCOM+s278Z7K5jtph7YatA5URZIuCP1WDiZBDFxfNkH9jQnqlnZoqUEgrFGEX+B53FoKreAK/tc0jpiPhgUBtVu3tUNLDdI2ZPmGzjTKSW0JBdvG/6WYj4SHszhx9vS+PrtGO3TVIKXfExBf9pVIGbTwv9Mw/bHwpnCkO7c1qQYWt7RDSw1+39Mc/1gZTkG18H/+9mPKqTcKolLdWZwQli1aFhQGceff/mxZ6ZJRsfjni1Z+6AcCarc5lJ1ZnNAokwyRNQU2ak1B8eyF723P1zqrjCMtBbFSYtCZ2wilFJX1Iq1eYGI6vlS9KsLaMjhuS9ukGiI5bM3iCHlOr24TbPo1KyoeNd4r0lEQlOK3BTT0aEDpqjQsbrxXpK0g0AvKTtNDm76B6R7FaylCAa7xXjWJUgy319nYqx6bOzCda29eQO/kJeKTMlYwNJeLvyQb1X7H8Csem5LPx+JqWMQ6GsmIkXt4bUXo0FyMyqLp3BZ1pVqaHNoeG1Xnby9p1Lm2hceibJx9Hvfw2j85VBcZa6VO+7JJHY+NzNPhdCjctbWbbfxDQN3i4XuC3X4cre28CH3HYzMY6L1JY6N01b22g20fwcNvNd/Pv5dOtmYsGnVMJHb8/b2m2lxbuwlNIxLd5GFcqO2mJIMWwCRdjw3U21WhuLiydrOtOXqe2DCBruR274G+nDRvxs91yIf7+cX+c2CBhPV05D+OJwEAVlA4IOYdAABwcACdASruAOkAPkkgjkUioiETKI4sKASEsrdwYDQyWeYa9ekyMvnHybkVW5fh/6Dy/ujfOF/vPWj5iXmS/8Xri81/7resH6evIA683eu/8ja77XzZL9nxjIk3gP6K9Cv/F/ifHv4gf6nqHYsfjr4EtlP+7/mfYF9nvoH/A/w/sZ/Teb39d/mvYA/0fFAfcv+h7AX8382DS39Y/tb8Dv82/xZmHiF06AiSfEh7TpiDVW7nGJDg7qAnLGyoTZtWkuf3lB/k2nGmeTCKaIi8eAO5llh7vGfOLAa5CCvIfvh706o3B4FO+7RgiYYPnNixSFsDhQ0emLt2ZbCCNwOTcJG/hHBA3+KCxl+T+FZtNAqmqlruTpm3y1ZrUxvWNMjVuEjHAprFqb+7c5jNgg3VbM8bxRQckd+2ifSGZnahoAyW1ZuMOWi0ucaEMKBo5KbO6vfHqCPC+aVneeXF10RZfRCaTMcVAzoePmSU/dj3iJi/Uk16J9a5UIuflT57Br6q7h+UCMcq0IPlpFOjZHs30xRJaUoaXjO6AbQQUrczy4iTUeeP8HZ9cLzFXmoeJG/c2Pv+uqtbUCakMTDqlNF6LUSLmYmy1oW+vmMwAiTONmBbBQpfx0OHPKCJW5YxnDHyxMUPMiV4DyyvG1l0q1LlzxQGzhQMB6KE0aYtzq1RnKCrxuJgamn2w+3f0l+1AZM2T5oe9eUrCenrtQ5u7xQcW6acovkW5xP3bm/aPzPqc/mQSRNvYpGSWKOFMLLOo2flYMMaKsqPt+RztCt6ofxV4SEXqZ7U7GuiUcLcMyljXbJD7g+3+iOcrMSHZX7BcsjEnAQUmQ4qcBQU3rZsJ56A9qrDAVO4xLJa+Ugw2AKPutXf2mMrQQuVR4XSjl5yCG2qc0VOUyRDmVCkjRv4JXBHZLo9qssxMpRsSKUev+4EQbEpEAQMlqKjWxuXkcqy2+eb60M0KBeBUfVgDwbLBqw0bKHvAKVcm1uPzrsFBqWPEVuqcfYhhwzOo32bsuy60+qEC7B3+1zWWKvVU3TKz9Ff0ufjXlExh555BKt26GzGOv4wT4xj3cw2blF7bI+j82nWFGIb+lO9FOjR7yiSefwLKPrj8o6klA7mKlpUCtdCmENRIrfXb0iM8Ec1QBtR9NDokTx1fTENRD2pb/sHeer6kPZRLKF4RKvOv1g7SUvC7HP8Sc8N1YP1OfF3MSHNAAD+5D4EP1rFRkpj1qyX2UlTORC9qDeM/syurN0/WpcY7m6tqzrXx9pj0L4P/1Q/7O/OnUH8SmEbxNNRu+tmCiEYuuuMhhTR8sLluzvDuyauXKWahcbjExxpnkLsx3dFpuMgLbQ1d524EdV+3S/8Iev/BVyGlA7OwdYKwlTiN2FxgVnzVt9IGleOn48LA97WE9so078htrFKi+L6IPsC3RkEVOOV32YIpzbCMPs9ra6Pzl2mOXC+PQnNMlaDvYfxFzcjfWulJb45gKrPrYCeZJeDQG31pBcPFWTRHqffHoeS6hh10iv9FjfTw3dBqE4STxMpnZH/pNdkcmcngtLXohM6YXJNZjoo+lpynY++zVyOkHiN8gPOf5yBMPeicJXJnTdOsU4iNL1lGkgb7MQisn82Trq8VAloFXG0WccWwG0m2Cmn/oqdLSvZqTgtSLQA4WYCiq6QIgu4PPvChsVCLtNiL0q0EqOB4i4X6seE+NZNrfx7JJmz6VBDn94BT8h/WsPbdvCUI7ZjmnZ3UmS/ciE86NSPa/ZRA6x2aYrZ9c6tsE4HhMxY8ZNhfhh6Wq4E6x+5LDyyVSUwBfyQza8wgXzQVnZSoSBSp+uHqJmzZzqM7WZPg24+eMpX//jYx16typHeVTDdxEG0Fg278mkjbg8nnBmIGv8wOi45BhfDXe/62LgThlwv+WsSWF8vU0poWkjVxNL67W4qEjaxSg3bdBZl0/taFy5hyRHTjhYnGTZmEyOz3O5PnwlLv/d9jYAKBwBQRD6lsU0tCZB5NjMGvbiNX6QSKzcnRf+NDJ5w89k7FD7U7jgHrZqVZSIqqFNpFz5Yka/VuCOckVaIZrF5AHzfn42oWGTABvqs6ypEMQZsO+p7EhHArsnp8LXTHV1ceeLD2O8htjgq3vXrf03HKFMoPu20nPYuUIjmMo7++aBAfLSe1x8ACDldV7aGliHx2ZSOIMXmAisgeKTbvMrny7V/jOpgrR9btDfp6GgVSoTa6zCwMmn3BEOphTAB/8SSIpkOlZWgjTU8tjw9P8TixNDGCMJN9+O7JThklYgrYAttXdgJhXWA0g7h+kCUK8vDJ6RWusflecndaOPx8UQ/s6R+OP8fZzx5FepJ6HiBTge1FQKQjOI+DVEPnUoNEMjvgoKZCzTibGpNOKR/Gcp8yV/GAptD4EnR7phKHN9T2DFhkc2bbrv9RXB+xavXtjq+IX5A6tYGhjS8k4d2WY7gwmcue/nlN+0gMMAZO1gP7PIAKejxyBmgCQw1v6oF65hHIak0DZ2lbW7XPVW8FFQWxtVPrykfN6aeFe6z7wFmEuG9L6L8DfAmyXVi5nf+uHFUDV3OYn8z3OXcZH9tEzEX509dnW0DHjjrO6CDtOfIC1wqlKXYN2OyZ0pWTTprOfX6FUIzchAGnRnWlxQ9Yx7PCKctBBFE1o3ML/3+e5LImVAR2F3wO9JeO/Kdj1OQ3GPho76IJLsUn91z8HycFbkptXVfroXynIHgw1vWee1U4fGxj6xr6qcp3P9GlE7F4W2MQLRoqpgk0QnY9nJ8dFUCOKyFzM4hGOqPoaxxUeGY/vtRY1FkNtyM55C+XsRb4LqT9eptw91WFGEMbwFAcSoZ3QCktVfWFmipqW+zjghKnHHshyneU+qDfRI6fq6BccEnmngMAreEsOyxcR35lsv95B1FFysWJ1kzfi87lyOmYIXOLEI8heJNsbomgO+mdnbCF48I43+hHIT7ZIzq/WsT5tRWI4q2/VrivG1aSkZZLok6wZ9YgCk9+qaRJkZs19orBAr3WM530QQ8iTDaTHFzxOejbXQk/uiB3bbvK4CeNGSUbssgsN4O/1HKMJW/DMXbgSETJfyDhj95WDFUaxdMXJiQTjX52NlCg+kt/6YX7khmvQcVQWD4b7WfGmrcYfbeGeNSrF29vB75qR4mIRYX7Bnui2kRy6CEGoI+fIkpwGQ3BHpJyGg9RxIx2KNQBF7u/tDIrvhlASHzpi/zLw3Yu2HLEldM04qfMo0F1rPLdki7/P5c23X01iHtT0Hp3KnH/xjW1o34KYkRqOnoypcUMBmPeZQ3G7vObaQhR31ondGnAt07E1Jm2zFqLj7UxPwRqNmz5a/OczJDjo+d1IhNrbH9s+qnGso8OGmLp6KcPiykOgCXC8Wv+vmjCedo2WkkMTOCcGOxWpJvjGGeKMJsqcnlEAKzCQaqvAjo1L8xG+SZLNct7i7FXs4cVXlxn1wlcuUoNOusRpONfW9kGcUcDxeeK0Mnt02K+/gXBRAEomnihmfRN5pRLe7S3IFSCe/eMZ9PRrHJBydgjFAnLV7wD4LOExoOEhIvl6iDjvN75UvnqgSQpjFir2O+dZMmkUkwC24susn8F+oyCFzT8i3UQDXIskqG4JfYXH+nLxhM2LU/ImV4FDDZYx2Pl8tBkEDDuLdINPesnYeaOVOhoF0Fzs2y333XqICN73NqfD0HVXsJR2Yg9txKPiosptuiHWvffU9ysilQyI+ioECLOSaatCjr6Hzd+FohW9Bw83NAV5jzyi3DFkyJCLnbd9PHjJFHKGivPjkOOF19qJGMq8rwqiZswuiY9G9LAED0XT2HfWHuxmtdzuT5GEgHO+HU5pOfip8THAJhdCn/RqOgIOM7Unu7WzNNo4KtdntWjbUXEtsDtWxSD0iVPqa1dgYdyszGd3TJ5xmk5qg9UgMECD1ObSiMWu79PoPab8DoYH6M0c8TgQHutm5QDbVjfutc5mYmJayPUbLsJrkxM5omop5MWArkG0MrN94JpMxEW0evRUX4MzGKtk/KdRSMBvMeA1Gg9+RAwXaghX7MLAO6MAjDwY6tilJxn7gOc1Er9++cgb1dFI0Zp1nCXfedrj9ukpLrOM2YlvZg9e/bm7y+oSAyLIBLN+wxBICdYQW4PXPZ9cXpKvsL7Iu2fln6H7hzEqBF2TZabeuyf2NJkMcUt1S/nOUDu0cKYTZiu9VazS57E5Nen/y+3td9jX8Tv6Iy55GtUAHLUBZPOVHGqlxbV9VthSMUZjxbeSXtPVDuU/iZnRQ8u0ahGgswSDzF2LLl4sXN4dgbjDZoKWv8EuvMg01zitSspucTkEM338CxTSCd/ZW4izrnnWTUUEpuYep6ImqualEWmeDWEM2v1bP+QNh0GsobjSDdycpPKa612jQbO/Dn33klaaJVTLsPnv/rlNWizID6Tr/PO3MG6GkBPqAAn7/szgxkLOVVRK/gFSyharylsECT0d9VB5FF9uXAbSEPZm73DEFsnSrlQFPw8EVhcB4TBNhN/XjbeGVpTCQ3Qe+3HiIwf1/b08aq7BJjjD6ZoD5/c1y2dVCDj/xwXpwSHJ+0mFI1Ux9B7cVzpExDSdz46+3Oob0biucVhLEBOhgH4galdXck/NXOvIzCdAwrWVYFnhBUgXzN9NM5vth2C5bdcTvfut+Pf9tvE0YsJCS3vWRAss1rL0q5bRF4yRNu2qI864OG9HuW9Xn+o+IWn2X3cJc9Hzi9ISqE1KKlJKq0k54Gqh/cbknxrpJ/d3Mz+5++zm0XAePB86G/EU9I9TOlVxMJBCZmcs7hca62m5vIUkiGUgLb24QXaVNOq7mF6o9Yoo2fY6+W/fxUo+T5ICYEM89e82DafZWYn6xzeyl5sBhkhRGKOztYiq2s8ytXONsyxnJrbKswXfMvsQlBqzMajAptyueeHuHbPeUcyMupjnOE4wuhCyyaeU7Squ7fQ6AbYFHHjfLKjzvNxbL9VAqisaRP12WLi0Gab1GwnfE11xAKGp5BWTWSPE2U76DINe+SXBukVqdej6/FUlU+AwOQoAg2ZHZkhP+A/o1q/n6XMhutT+ULtpNBlDaianDLbnRqxzKT5thnL/ySpVt0kV+XnmrJ7hEZA9SklMyLIjS9+PhmaC4qMi8/w8a9Q57lcpqsyQ7b4MKJhl+4inpTDPWqAuv8hyvDOxVq/BMz5+1GoN8okGMgKUDpILRWcXytOV+KRbGofqbeCH+sxCgalWmDjPzqjdD5aZfBFxCOb0z1BINtswohNxZ9VQyl7uYi6DPsj2Wlr8GgqE7expy6yDPZozUYnDolwOjc1B3VYmsYqoq13s+GrPTOv6JhzZ8Kf1eDDA9urPPqBqmow992ncI2FwcJft5xOoSjWyrfVf42ixnJz7hi05IPM1E3cscxdAfM25c1Mw/MN42TTej4/vF3IwJ5OC9EJk3EtQdaX95bH7oD8Fsc6pbMWMd5LdZVkL/d2fElgUgWisQUMu4swMGuPdC/2oFcM9tiT++YPK/SD9MzqLTouWOXJo7XHLDNKmiKaGla4R9yu4jRIVSnCBvlUptR7oSXTQ6PVLshJrdA7io3+8KQpZYYnulLqtGOIb59vnnRdwwNglOGLrW8qWuuECwMv7sfgI1jrbUEV5HBAh40exbw2We6U/NX/uSBewnI8VyvV85c3vFXkMB9ojaCVrrgBNhj9AaEydNM2Cskg5q/iVO7UTyt+LzA3NyaStPWNT3rjyDoTj3VWwq+viJ4KEHlNFSYaVUKle1ULRjCsPuphdJuO11u7FG5gFuVjcO5iHd5LLMCyx4QWJ0H6QaRgqjPT0lXp0Ku9CLJBzMQOsXc0edUHEwQGXsnHFzLGGnMSnQwAQPvOtEYdVY9zklUT0TBB5f31nWGryih/+8cUaePhxXQ53+CTNhjQk1PQMsVZSU4FS272maZD0gLVe+3xcf5wVdUs50zPlbvKzlBN7CqjGxUPSvWmLVqkeQ1vEa/TAUFaB1oMDYd9huUYZ1KgBM6+72ZI6tMz6tjQdbIbV1s65WfxQX7Tv75DXtKLaXDloMfZjdeeep7KblovJE78SraFQVThTT21nOxpvueBvGJwaU5YljNg//+inB1cYraWOw7pPyxezCGRXmS/tfQxJcQfCagYKvhwXGH8GgliknHQdpk2neB1lTl+dQ3ZPJkBfuHC+U4kpzidqJqRLAudI2RPRUkDvPj7ZeyW2fTCsO93MIuIaDPvJZz2EG6jooBsW4u4ywwwOe41Y31g+BYSBzfXM4OBhmrsu6WxTRvWeuemZlre3UhG+RFuziJh44/xsMUfL8c1VPUcZ2aft7ksUQRMFun639yXSLrP1OFmSrwjEvY4TOO39S7R535Sofpd933zrvU6S/3f1MCRorpNB0NC/7k6UuUtXGx7/AJA3ODlLYV9oD6dCXmhro46Ou27M6zzw/PO1Uhi49ekgD79g7y72MMqhw3IKVZ/EmW66RU62Kfb6IHKL16r9cH79a8rYViAaSwx3bEkmJEKh+WubuNVJR2D6kpDK+IUNWFszo7AxhCPUVluAHhrpLBeNRPSao5xO04n/qfFcOWoVRFkMJzdglU0BKR5AV74eZdRlNPWZgzddLIKJAA1YHSfE6/8HV3HRxhD7Q0I1ncE4riVC017nokgkacpG8zZ7vW6gDwDH18UCfxHbQ8ppaxs/6VvA4nP8W8JUvfvoWzn7qcsR7suWTNuuyeEdBq8Km5tXIznII+cnqK9Df6uHX25oFeB9tSTwoQngKp4LS1dDs1+xNTKc95INXePO1FzHnX5arnKWbNvS4c6T8qGP+GDE98+7kKb++Kk8RPKvjSS9c3rlasGV+Uew6S6uxW6KyadKtgigIRDpHB/5aUJzPZ0wIqlxgvb+YbX5YH0Lk+et9BUaFfv05behnQkscrRL32h6SH6XdmobkKpXcgG4ZspNCbajWDaYxJY18KCaWLXemWjhw+rLBGNHMjvaOABeNBDLdKNXESB4xp74naaoLgcgMMfPu+I844MxzruQElEew6slupUNAkII7s58iAELt0EVFb6r685dv4sx92h9S61DF7/vQ9QMLKrLlTC0NRsXB5StNkVUBzAJ8aObEItFW5LrOKKdzuukq/qwp+3BRW8M/NKfj5oYW4iOc6MKE2r7x49pOUPX7FATDQbN2JhWjRVHsXnT7NMqPDIR70OeD/wRJ5ebv8gPhG2A+zU952puPAI8h3ysKXHAynpI1vn0vhNoVV+aV3g8HuCm1UXcFjspIuJ2b6VQhkXOQc2QXBhynHAkqSEQLh57A/w6k2hWJ6Xhp6s/CXLpCY4nduvWDWfznWz6iHAnLXtN07LlPgFm5w7VB7f+BwuUol6iR2MkfdGfvLXeCc/rzbD+V5okOeXVZtN8ZfK1lBK9ArhHYEvPJfoqEMpsIsM/s5J7FKmm+MoBLkvgYCVPTnwWYMWKgw74hPoruRNaJsmmOrYcOEb4rHRLZZwmpVBlF/E+ics2GoqnmgFt3Ua+ChCVsSaXs7/pDrmF41CHukGcTpge31zpRV0vgIT5pRUJ8BwIYAksCIUZd8r/bcj7QPpaATfTFv0DvjUeQBy5s5Y1AIf+qTuAw0OY2LQBHIwbkzuma6wirA6hGQ155Q2Dy5A7KII092R1pervPRtdSnZf2WHMG0oVMhHkEfCVFmW/PDgdknFxVcRXknbzAC8OHTY/1o40Cjng2oc8jQZObj15j97PZk7tNmx+bhea1gkkA48DiNjyTz/KEbatWF/BNC7zYXNzGU+e6TB0ZTvqKCnxJ7bDp8TA69IiC+BbeyBktcYGOpbUnIZihwTDW3KaCOnZTPA1AyCya9wy2Njt4GVm8ELcBJLxcdMUml3BSDQoaPmHBMy52S/muiDcZHioHtE+DFh9XXBhqz0KVIrCmhEsHaFUNgzZ9XvqTCATcQ/5CqSDZ7xmMT3PBAh/szR37z89ssJwsh4KD7u6rcAAeGJVGyHY6WovHKot613rl/EXzn7yHjQESdc+LM47Jm2daj2GmK5qqi589TelV705dR3em+hktd7181/Z5tFkUWBIaSyY7isKnnyH5Qcak3HK71lI+VXol+ZSnHVIe1rGndjcsnLTsYtrP+txAylYvVRFfgXdKY9tL3K6XukvcsFu3cnuMvdFmM3KYLQxcmfbDTShiswuQUAvBum95WODA3EOPssEhELL+oW1cdJEZxMSxyNF6Q40vMtvyowzrID9yI084O8gn4/Zs2RWkkrJRLaq97NbLb3aOenkIBMoT0gZ7OpM+4hn1eKO1FfJigzoF3DYmsgiZMl1T3rCJs5nM8LuHEeGc+MXxH/nKu0Q22Jz7zFFVu7/YdDsg7RHATH0JYG8HrK+/bbvI93NFY+f/P4B0YOuB/hNrfqJcvVDuFCNFZoXC3q6odXm3YeQC9GOcb5Tor8nWtPv8IDdGBVyroOUSrztEz0lvF3yWx5DUvnd1bMYzBTVTNrq59/M1XVf/IoHaUptMO0trbP+6W/8ZD1srXfdLrFEKw40JK5IQ0lCd/1cRD5ckEoSMCwA/893qfBspBRGiDq+ebQmWcESFVLiE/YXnRcvB/GW2wCL7X7lz0shrKmRqTMSD91IOkPCB723coBRKYdbFgtkpp+zz4228LYbebZxk4XZCPNdjPVJOUnycRgqf6km5/ThACMsjeLxQDeiAx3cNrzB1EyrX09tMrM7IRlvMe9WcMXqhvraiS8kmj36mxsMZlguGIAX0yeSAR6IpLVVfnVw5sYUabMFUJ/5h9VHzGluQ/mHGXpfbqmsp1HIdC96oVYHBfNaUgLPXdzlZCgALjxtYD6iTsnjS9WvwJhpL5mtl0SglGQuiBPx2fz+oT6uBQJJyhYfOFs8fUv7XdrH91VYKLNr6C8sb1a9tyuKUs/cmr3iftw0KEKfvlTWSAfxFCmQ63iBiva0RcGoHV2KydcyCSjof0aAQg4qd69QXzcoCU3ZwFgOKGEx0dtvIXBF5zchbJVS/j35rn4gFi3jzWq6UZXC2ZXOTrKr0aOrE2i2wRm8xsabj9EZJuSObfvxPKtC+cjLt0LhkEBkTm8CDifa+OWVb4FVidNR9+mUljQSU6+1ovRgdgCR60qlPAUfT7QmWPM2EdtnaQojyuKIqe8d1hENWz1SlVC4IJ4sqQtiaG40UZaLKJvCOCURxLmbBpbxsApRADL4dnL0b2b88drXvror67f1rrVv8Q1SRvd3mNvAD88VJHcNjCVfudyPH1Um6SZvNAfKWp8b4It5fatQMkwAcOr1bY/8lgBAmQFAuyjNJ7jYT7wEuQ+m+BhBhkcfztkIZrOtdwdkUdj9JRdUFFZtn9zyc7iBQluPBw/ZWt+2gcPvBumcwgYxzO42i0PwVPn0ECz/hoCldVz/BbfRNA0iaFngr64Bs8wu2RjvOrI/Z9vW1I40OsNSFrtGAbFzjWu+nwWhP9rFHAuzCMZw8FX1LVtO+wz7IgBhWDWlgT5FM7JUI9UsuIwGszBF88faC5xroRwddLhvmxy2LHHlAoiczyuvunIIBdgAXBBeFuIz9Jyt4RrsnHVL04x5bsu8fVFJJ+fD7FQL3iv35QKxQJbW1lKY0njok0PUHbLKFBGoXJ+mHAjXYDabZk6INBttvfmxQa4NB+TPW/K8roWfLv0JPKXv+jismPM9y4pQisEKO3Ohtc4K5Rxua+liBG06q1pVqTgJ7e9z1o2cx9uHS0YZ81URuNPPS5HGdFWqI7GGUte/y1Fke2lmP/fzFVSCckM8wWaNql3zD43daCYsvOsYVfyFUeMzaxBWhykasOHwthsxjHMZS48m1VRMzrounXDbEydNiHUnpIhyHuYaPzhUShZr137nhZQK7JtWGx9pwm9nRO+bUN1TYPrcqz5y7em8/QhcD9mzkM3sHaB4ZOipP8eUUklyKD5sZTtNCcW3lv3O/L/uknDNePHc0Fe5750T+uW9wYaJPeTW6hDCUvXaO7R0sm/HnzCazdF27WSeV55QHOjHg5gsi8DlLw+xJSC1W74EN6XSOMFOpOXLUXcuB4LwYq6gMkht3nvfDtowXeM9Y5AhoDkwjBO/MuucKrxjRjRMSp6ZNbxHPYOm8EvLhKh6Bvee1cL3gHppp2ANvvwAID+gMbgek+0lDoVFgO/NGVSlY6P1SRNbL7YXTQ9SvbkCJIZ7G1fx6lYKY0oPN8lhyQDyFXcXyFoD3GDDSTAAAAAAAA" alt="" width="130" height="130"></div><h3>Une progression structurée</h3><p>Chaque formation suit un programme défini.</p></div>
        <div class="pg reveal"><div class="ill"><img src="data:image/webp;base64,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" alt="" width="130" height="130"></div><h3>Une pédagogie accessible</h3><p>Les notions sont expliquées avec clarté et illustrées par des exemples.</p></div>
        <div class="pg reveal"><div class="ill"><img src="data:image/webp;base64,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" alt="" width="130" height="130"></div><h3>La mise en pratique</h3><p>Les connaissances sont appliquées régulièrement par des exercices et des lectures.</p></div>
        <div class="pg reveal"><div class="ill"><img src="data:image/webp;base64,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" alt="" width="130" height="130"></div><h3>Un accompagnement attentif</h3><p>Chaque élève est encouragée à progresser à son rythme.</p></div>
      </div>
    </div>
  </section>

  <section id="pourquoi" style="padding-top:0">
    <div class="wrap">
      <div class="why reveal">
        <span class="ar-t" lang="ar" style="display:block;font-family:var(--f-callig);font-size:1.7rem;line-height:1.2;margin-bottom:8px">لماذا معلّمتي؟</span>
        <h2>Pourquoi choisir <em>Mouallimatii</em> ?</h2>
        <p>Apprendre une langue demande du temps, de la régularité et une méthode adaptée.</p>
        <p>Nous souhaitons rendre cet apprentissage plus accessible : un enseignement organisé, des groupes restreints et des programmes adaptés aux différents niveaux.</p>
        <p class="amb">Notre ambition : vous aider à bâtir des connaissances solides et durables en langue arabe.</p>
      </div>
    </div>
  </section>

  <section id="supports">
    <div class="wrap">
      <div class="head reveal">
        <div><span class="ar-t" lang="ar">الدروس</span><h2>Supports <em>de cours</em></h2></div>
        <p>Les fiches qui accompagnent les formations, classées par thème et par niveau.</p>
      </div>
      <div class="toolbar">
        <div class="tabs" role="group" aria-label="Filtrer par thème" id="tabs"></div>
        <label class="search" for="q">
          <span class="sr">Rechercher une fiche</span>
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="7"/><path d="m20 20-4-4"/></svg>
          <input id="q" type="search" placeholder="Chercher : prépositions, tajwid, الفعل…">
        </label>
      </div>
      <div class="grid" id="docs"></div>
    </div>
  </section>

  <section id="galerie" style="padding-top:0">
    <div class="wrap">
      <div class="head reveal">
        <div><span class="ar-t" lang="ar">معرض الصور</span><h2>En images, <em>la classe</em></h2></div>
        <p>Fiches, tableaux, travaux d'élèves : un aperçu de ce qu'on fait en cours.</p>
      </div>
      <div id="gallery"></div>
    </div>
  </section>

  
  <section id="formations" style="padding-top:0">
    <div class="wrap">
      <div class="head reveal">
        <div><span class="ar-t" lang="ar">دوراتنا</span><h2>Nos <em>formations</em></h2></div>
        <p>De la première lettre à l'analyse grammaticale : choisissez la formation qui correspond à votre parcours.</p>
      </div>
      <div class="toolbar"><div class="tabs" role="group" aria-label="Filtrer les formations" id="ftabs"></div></div>
      <div class="forms" id="forms"></div>
    </div>
  </section>

  <section id="contact" style="padding-top:0;padding-bottom:clamp(90px,10vw,130px)">
    <div class="wrap">
      <div class="join reveal">
        <div>
          <span class="ar-t" lang="ar" style="display:block;font-family:var(--f-callig);color:var(--wine);font-size:1.6rem;line-height:1.2;margin-bottom:6px">انضمّي إلينا</span>
          <h2>Rejoignez <em>Mouallimatii</em> !</h2>
          <p style="color:var(--muted);margin:22px 0 0;max-width:32rem">Que vous souhaitiez apprendre à lire l'arabe, améliorer votre lecture du Coran ou approfondir vos connaissances grammaticales, vous trouverez une formation adaptée à votre parcours. Faites le premier pas et rejoignez notre communauté d'apprenantes.</p>
          <p class="callout">Il n'est jamais trop tard pour commencer à apprendre.</p>
        </div>
        <div class="socials">
          <a class="soc" href="https://www.instagram.com/mouallimatii/" target="_blank" rel="noopener">
            <span class="ic"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor"/></svg></span>
            <span><b>Instagram</b><small>@mouallimatii</small></span><span class="go" aria-hidden="true">←</span>
          </a>
          <a class="soc" href="https://t.me/Mouallimatii" target="_blank" rel="noopener">
            <span class="ic"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linejoin="round"><path d="M21 4 3 11l6 2 2 6 3-4 5 4z"/><path d="m9 13 8-6"/></svg></span>
            <span><b>Telegram</b><small>@Mouallimatii</small></span><span class="go" aria-hidden="true">←</span>
          </a>
        </div>
      </div>
    </div>
  </section>
</main>
</div></div>

<footer><span class="ar" lang="ar">مُعَلِّمَتِي</span><span>Mouallimatii · Apprendre, comprendre et progresser en langue arabe.</span></footer>

<div class="lightbox" id="lightbox" hidden><figure style="margin:0"><img id="lb-img" alt=""><p id="lb-cap"></p></figure></div>

<script type="application/json" id="state">{"supports":[
{"id":"ex1","ex":true,"cat":"Lecture","niv":"Débutant","ar":"الحروف الهجائية","titre":"L'alphabet","desc":"Les 28 lettres et leurs formes au début, au milieu et à la fin du mot.","lien":""},
{"id":"ex2","ex":true,"cat":"Lecture","niv":"Débutant","ar":"الحركات","titre":"Les voyelles courtes","desc":"Fatha, damma, kasra et soukoun pour lire sans hésiter.","lien":""},
{"id":"ex3","ex":true,"cat":"Tajwid","niv":"Intermédiaire","ar":"النون الساكنة","titre":"Le noun sakin et le tanwin","desc":"Les quatre règles : idhhar, idgham, iqlab et ikhfa.","lien":""},
{"id":"ex4","ex":true,"cat":"Grammaire","niv":"Débutant","ar":"حروف الجر","titre":"Les prépositions","desc":"من، إلى، عن، على، في… et le nom au cas indirect (مجرور).","lien":""},
{"id":"ex5","ex":true,"cat":"Grammaire","niv":"Débutant","ar":"الجملة الاسمية","titre":"La phrase nominale","desc":"Construire une phrase sans verbe avec المبتدأ et الخبر.","lien":""},
{"id":"ex6","ex":true,"cat":"Grammaire","niv":"Avancé","ar":"إنّ وأخواتها","titre":"Inna et ses sœurs","desc":"Les particules qui modifient la phrase nominale, avec exercices.","lien":""},
{"id":"ex7","ex":true,"cat":"Conjugaison","niv":"Débutant","ar":"الفعل الماضي","titre":"Le verbe au passé","desc":"Conjuguer كَتَبَ à toutes les personnes, tableau et exercices.","lien":""},
{"id":"ex8","ex":true,"cat":"Conjugaison","niv":"Intermédiaire","ar":"الفعل المضارع","titre":"Le verbe au présent","desc":"Les préfixes et suffixes du présent, avec 30 verbes courants.","lien":""}
],"gallery":[]}</script>

<script>
const STATE = JSON.parse(document.getElementById('state').textContent);
const SUPPORTS = STATE.supports;
const CAT_AR = {"Tout":"الكل","Lecture":"القراءة","Tajwid":"التجويد","Grammaire":"النحو","Conjugaison":"الصرف"};
const CHIPS = [["ن","القاعدة النورانية","An-Nouraaniyyah"],["أ","محو الأمية","Alphabétisation"],["م","دروس اللغة","Méthode de Médine"],["ع","العربية بين يديك","Bayna Yadayk"],["ت","التجويد","Tajwid"],["ق","طلاقة القراءة","Lecture fluide"],["إ","الإعراب","Analyse"],["ح","متون النحو","Mutun"]];

const $ = s => document.querySelector(s);
const esc = s => String(s).replace(/[&<>"]/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[c]));

// Cartes qui avancent sur la ligne de la vague, dans le sens du courant
const stageEl = $('#stage'), ridge = document.getElementById('ridge'), dunesEl = document.querySelector('.dunes');
const VB_W = 1440, VB_H = 210, GAP = 250, SPEED = 38; // px entre les cartes, px par seconde
const ridgeLen = ridge.getTotalLength();
let wave = [], waveLen = 0, labelNext = 0, lastT = null, travelled = 0;
function ridgePoint(frac){ // point de la ligne en coordonnées de la scène
  const sx = dunesEl.clientWidth / VB_W, sy = dunesEl.clientHeight / VB_H, top = stageEl.clientHeight - dunesEl.clientHeight;
  const p = ridge.getPointAtLength(Math.max(0, Math.min(1, frac)) * ridgeLen);
  return {x: p.x * sx, y: top + p.y * sy};
}
function buildWave(){
  wave.forEach(w=>w.el.remove()); wave = [];
  // longueur de la ligne à l'écran
  let len = 0, prev = ridgePoint(0);
  for(let k=1;k<=60;k++){ const q = ridgePoint(k/60); len += Math.hypot(q.x-prev.x, q.y-prev.y); prev = q; }
  waveLen = len;
  const n = Math.max(2, Math.round(len / GAP));
  labelNext = 0;
  for(let k=0;k<n;k++){
    const el = document.createElement('div'); el.className = 'chip wchip'; el.setAttribute('aria-hidden','true');
    stageEl.appendChild(el);
    const w = {el, offset: k * len / n}; setLabel(w); wave.push(w);
  }
}
function setLabel(w){
  const c = CHIPS[labelNext++ % CHIPS.length];
  w.el.innerHTML = `<i lang="ar">${esc(c[0])}</i><div><b lang="ar" dir="rtl">${esc(c[1])}</b><small>${esc(c[2])}</small></div>`;
}
function placeWave(now){
  if(lastT === null) lastT = now;
  const dt = Math.min(0.1, (now - lastT) / 1000); lastT = now;
  if(!document.querySelector('.hero.offscreen') && !reduceMotionW) travelled += dt * SPEED;
  const small = stageEl.clientWidth < 700, scale = small ? .72 : .9;
  wave.forEach(w=>{
    const prevD = w.d ?? -1;
    const d = (w.offset + travelled) % waveLen;
    if(prevD > d && prevD >= 0){ setLabel(w); w.el.classList.remove('swap'); void w.el.offsetWidth; w.el.classList.add('swap'); }
    w.d = d;
    const f = d / waveLen, p = ridgePoint(f), q = ridgePoint(f + 0.004);
    let ang = Math.atan2(q.y - p.y, q.x - p.x) * 180 / Math.PI;
    ang = Math.max(-14, Math.min(14, ang));
    const fade = Math.min(1, d / 70, (waveLen - d) / 70);
    w.el.style.opacity = fade.toFixed(3);
    w.el.style.transform = `translate(${p.x.toFixed(1)}px,${(p.y - 6).toFixed(1)}px) rotate(${ang.toFixed(2)}deg) scale(${scale}) translate(-50%,-100%)`;
  });
  if(!reduceMotionW) requestAnimationFrame(placeWave);
}
const reduceMotionW = matchMedia('(prefers-reduced-motion: reduce)').matches;
buildWave(); requestAnimationFrame(placeWave);
let rwT; addEventListener('resize', ()=>{ clearTimeout(rwT); rwT = setTimeout(()=>{ buildWave(); if(reduceMotionW) placeWave(performance.now()); }, 150); });

// Supports
const cats = ["Tout","Lecture","Tajwid","Grammaire","Conjugaison"];
let cat = "Tout";
$('#tabs').innerHTML = cats.map(c=>`<button type="button" class="tab" aria-pressed="${c===cat}" data-c="${esc(c)}">${esc(c)}<span lang="ar">${esc(CAT_AR[c]||'')}</span></button>`).join('');
function renderDocs(){
  const q = $('#q').value.trim().toLowerCase();
  const list = SUPPORTS.filter(s => (cat==="Tout"||s.cat===cat) && (!q || [s.titre,s.desc,s.cat,s.ar,s.niv].join(' ').toLowerCase().includes(q)));
  $('#docs').innerHTML = list.length ? list.map((s,i)=>{
    const href = s.file || s.lien;
    const kind = s.fileType ? (s.fileType.includes('pdf') ? 'PDF' : 'Image') : (s.lien ? 'Lien' : 'Fiche');
    const cover = s.cover ? ` img" style="background-image:url('${esc(s.cover)}')` : '';
    return `<article class="doc reveal" style="--i:${i%3}">
      <div class="top${cover}"><span class="lvl">${esc(s.niv)}</span><span class="ar" lang="ar" dir="rtl">${esc(s.ar||' ')}</span>${s.ex?'<span class="exb">exemple</span>':''}</div>
      <div class="body">
        <span class="cat">${esc(s.cat)}</span>
        <h3>${esc(s.titre)}</h3><p>${esc(s.desc||'')}</p>
        <div class="foot"><span>${kind}</span>${href ? `<a href="${esc(href)}" target="_blank" rel="noopener">Ouvrir la fiche →</a>` : '<span>Bientôt en ligne</span>'}</div>
      </div>
    </article>`}).join('') : `<div class="empty">Aucune fiche ne correspond à « ${esc(q)} ». Essayez un autre mot.</div>`;
}
function renderGallery(){
  const g = STATE.gallery;
  $('#gallery').innerHTML = g.length ? `<div class="gallery">${g.map(p=>`
    <figure class="ph reveal" data-src="${esc(p.url)}" data-cap="${esc(p.cap||'')}">
      <img src="${esc(p.url)}" alt="${esc(p.cap||'Image de la classe')}" loading="lazy">${p.cap?`<figcaption>${esc(p.cap)}</figcaption>`:''}
    </figure>`).join('')}</div>`
    : `<div class="gal-empty"><b lang="ar">قريباً</b>Les premières images arrivent bientôt. La professeure les ajoute depuis son Espace prof.</div>`;
}
renderGallery();
$('#gallery').addEventListener('click', e=>{
  const f = e.target.closest('.ph'); if(!f) return;
  $('#lb-img').src = f.dataset.src; $('#lb-img').alt = f.dataset.cap; $('#lb-cap').textContent = f.dataset.cap;
  $('#lightbox').hidden = false;
});
$('#lightbox').addEventListener('click', ()=>{ $('#lightbox').hidden = true; });
$('#tabs').addEventListener('click', e=>{
  const b = e.target.closest('.tab'); if(!b) return;
  cat = b.dataset.c;
  document.querySelectorAll('#tabs .tab').forEach(t=>t.setAttribute('aria-pressed', t===b));
  renderDocs();
});
$('#q').addEventListener('input', renderDocs);
renderDocs();

// Formations
const FORMATIONS = [
  {n:"١", cat:"Lecture & Coran", t:"Alphabétisation arabe", ar:"محو الأمية", tl:"Apprendre à lire et à écrire l'arabe simultanément.", d:"Pour découvrir les bases de la langue arabe ou reprendre son apprentissage depuis le début.", p:["Acquisition des bases de la lecture","Écriture des lettres sous toutes leurs formes","Reconnaissance et distinction des lettres","Écritures spécifiques du Mushaf"]},
  {n:"٢", cat:"Lecture & Coran", t:"An-Nouraaniyyah", ar:"القاعدة النورانية", tl:"Apprendre à lire le Coran correctement.", d:"Une méthode pour acquérir pas à pas les fondamentaux de la lecture coranique.", p:["Maîtrise des bases de la lecture","Familiarisation avec l'écriture du Mushaf","Principales règles du tajwid","Précision et fluidité de la lecture"], gift:"Correction du Juz' Amma offerte"},
  {n:"٣", cat:"Lecture & Coran", t:"Fluidification de la lecture", ar:"طلاقة القراءة", tl:"Gagner en aisance et améliorer sa lecture.", d:"Consolider ses acquis grâce à un travail progressif sur les textes.", p:["Règles de fluidification","Règles d'orthographe","Notions fondamentales de linguistique","Pratique sur différents textes"]},
  {n:"٤", cat:"Méthodes de langue", t:"Méthode de Médine, tome 1", ar:"دروس اللغة العربية ١", tl:"Découvrir les fondements de la grammaire arabe.", d:"Poser les premières bases grammaticales avec une méthode progressive et structurée.", p:["Initiation aux bases de la grammaire","Lecture et compréhension des structures","Construction des phrases","Expression écrite"]},
  {n:"٥", cat:"Grammaire", t:"Grammaire simplifiée", ar:"النحو الميسّر", tl:"Comprendre la grammaire de manière logique et accessible.", d:"Démystifier les règles et mieux comprendre le fonctionnement de la langue.", p:["Principales règles grammaticales","Exemples du Coran et du langage courant","Structure des phrases","Initiation à l'analyse syntaxique"]},
  {n:"٦", cat:"Grammaire", t:"Les Mutun de la grammaire", ar:"متون النحو", tl:"Approfondir la grammaire et maîtriser l'analyse.", d:"Une approche traditionnelle des règles fondamentales de la grammaire arabe.", p:["Règles fondamentales","Analyse syntaxique (al-i'rab)","Lecture de textes sans voyelles","Correction des erreurs courantes"]},
  {n:"٧", cat:"Méthodes de langue", t:"Al Arabiyya Bayna Yadayk, tome 1", ar:"العربية بين يديك ١", tl:"Progresser grâce à une méthode immersive.", d:"Un apprentissage structuré de la compréhension et de la pratique de la langue.", p:["Grammaire appliquée","Lecture et compréhension","Structure syntaxique","Expression écrite"]},
  {n:"٨", cat:"Méthodes de langue", t:"Al Arabiyya Bayna Yadayk, tome 2", ar:"العربية بين يديك ٢", tl:"Aller plus loin dans la maîtrise de la langue.", d:"La suite du premier tome, pour des compétences linguistiques plus avancées.", p:["Grammaire appliquée approfondie","Structures syntaxiques complexes","Lecture et compréhension","Perfectionnement de l'écrit"]},
  {n:"٩", cat:"Méthodes de langue", t:"Méthode de Médine, tome 2", ar:"دروس اللغة العربية ٢", tl:"Consolider et approfondir les notions grammaticales.", d:"La suite du premier tome, avec des notions grammaticales plus complexes.", p:["Fondamentaux grammaticaux avancés","Analyse des structures syntaxiques","Développement de la lecture","Perfectionnement de l'écrit"]},
];
const FCATS = ["Toutes","Lecture & Coran","Grammaire","Méthodes de langue"];
let fcat = "Toutes";
$('#ftabs').innerHTML = FCATS.map(c=>`<button type="button" class="tab" aria-pressed="${c===fcat}" data-c="${esc(c)}">${esc(c)}</button>`).join('');
function renderForms(){
  $('#forms').innerHTML = FORMATIONS.filter(f=>fcat==="Toutes"||f.cat===fcat).map((f,i)=>`
    <article class="fm reveal" style="--i:${i%3}">
      <div class="orb"><span lang="ar">${f.n}</span></div>
      <p class="eyebrow" style="margin:0">${esc(f.cat)}</p>
      <h3>${esc(f.t)}</h3>
      <div class="ar" lang="ar" dir="rtl">${esc(f.ar)}</div>
      <div class="tl">${esc(f.tl)}</div>
      <p class="desc">${esc(f.d)}</p>
      <h4>Au programme</h4>
      <ul>${f.p.map(x=>`<li>${esc(x)}</li>`).join('')}</ul>
      ${f.gift?`<span class="gift">✦ ${esc(f.gift)}</span>`:''}
      <span class="sp"></span>
      <a class="btn btn-light" href="#contact">S'inscrire</a>
    </article>`).join('');
}
$('#ftabs').addEventListener('click', e=>{
  const b = e.target.closest('.tab'); if(!b) return;
  fcat = b.dataset.c;
  document.querySelectorAll('#ftabs .tab').forEach(t=>t.setAttribute('aria-pressed', t===b));
  renderForms();
});
renderForms();

// ===== Apparitions au défilement (fade-up + cascade) =====
const reduceMotion = matchMedia('(prefers-reduced-motion: reduce)').matches;
const revealIO = (!reduceMotion && 'IntersectionObserver' in window) ? new IntersectionObserver(es=>es.forEach(en=>{
  if(!en.isIntersecting) return;
  const el = en.target; el.classList.remove('pre'); el.classList.add('in'); revealIO.unobserve(el);
}),{threshold:.12, rootMargin:'0px 0px -6% 0px'}) : null;
function armReveal(nodes, popVisible){
  nodes.forEach(el=>{
    if(!revealIO){ return; }
    const r = el.getBoundingClientRect();
    if(r.top < innerHeight*0.94){ if(popVisible){ el.classList.remove('pop'); void el.offsetWidth; el.classList.add('pop'); } }
    else { el.classList.add('pre'); revealIO.observe(el); }
  });
}
// index de cascade dans chaque grille
document.querySelectorAll('.principles,.pedago,.socials').forEach(g=>[...g.children].forEach((c,i)=>c.style.setProperty('--i',i)));
armReveal(document.querySelectorAll('.reveal'), false);
// les grilles filtrées réapparaissent en cascade
const _renderDocs = renderDocs; renderDocs = function(){ _renderDocs(); armReveal($('#docs').querySelectorAll('.reveal'), true); };
const _renderForms = renderForms; renderForms = function(){ _renderForms(); armReveal($('#forms').querySelectorAll('.reveal'), true); };
const _renderGallery = renderGallery; renderGallery = function(){ _renderGallery(); armReveal($('#gallery').querySelectorAll('.reveal'), true); };

// ===== Navigation : état au défilement + menu mobile =====
const header = document.querySelector('header'), burger = $('#burger'), mnav = $('#mnav');
function setMenu(open){ burger.setAttribute('aria-expanded', open); burger.setAttribute('aria-label', open ? 'Fermer le menu' : 'Ouvrir le menu'); mnav.classList.toggle('open', open); }
burger.addEventListener('click', ()=>setMenu(burger.getAttribute('aria-expanded') !== 'true'));
mnav.addEventListener('click', e=>{ if(e.target.closest('a')) setMenu(false); });
addEventListener('keydown', e=>{ if(e.key === 'Escape') setMenu(false); });
document.addEventListener('click', e=>{ if(!e.target.closest('header')) setMenu(false); });

// ===== Défilement : barre de navigation + parallaxe léger (ordinateur uniquement) =====
const wms = [...document.querySelectorAll('.watermark')];
const ills = [...document.querySelectorAll('.pg .ill')];
const orbitWrap = document.querySelector('.orbit-wrap');
const desktop = matchMedia('(min-width: 921px)');
let ticking = false;
function onScroll(){
  const y = scrollY;
  header.classList.toggle('scrolled', y > 12);
  if(!reduceMotion && desktop.matches){
    if(wms[0]) wms[0].style.translate = `0 ${(y*0.12).toFixed(1)}px`;
    if(wms[1]) wms[1].style.translate = `0 ${(-y*0.06).toFixed(1)}px`;
    if(orbitWrap) orbitWrap.style.translate = `0 ${Math.min(y*0.06, 30).toFixed(1)}px`;
    ills.forEach(el=>{
      const r = el.getBoundingClientRect();
      if(r.bottom < 0 || r.top > innerHeight) return;
      const d = (r.top + r.height/2 - innerHeight/2) / innerHeight; // -0.5 … 0.5
      el.style.translate = `0 ${(d*-16).toFixed(1)}px`;
    });
  }
  ticking = false;
}
addEventListener('scroll', ()=>{ if(!ticking){ ticking = true; requestAnimationFrame(onScroll); } }, {passive:true});
onScroll();

// ===== Pause des animations du hero quand il n'est plus visible =====
const heroEl = document.querySelector('.hero'), dunesSvg = document.querySelector('.dunes');
if('IntersectionObserver' in window){
  new IntersectionObserver(([en])=>{
    heroEl.classList.toggle('offscreen', !en.isIntersecting);
    try{ en.isIntersecting ? dunesSvg.unpauseAnimations() : dunesSvg.pauseAnimations(); }catch(e){}
  }).observe(heroEl);
}

</script>
</body>
</html>
