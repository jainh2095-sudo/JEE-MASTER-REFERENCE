<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>JEE Master Reference — Math & Science Complete</title>
<link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=JetBrains+Mono:wght@300;400;500;600;700&family=Syne:wght@400;600;700;800&family=Playfair+Display:ital,wght@0,700;0,800;1,700&family=Crimson+Pro:ital,wght@0,300;0,400;1,300&family=DM+Sans:wght@300;400;500&family=IBM+Plex+Mono:wght@400;600&family=Outfit:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;height:auto;overflow-y:auto;}
body{background:#06080f;color:#e8e0d0;font-family:'EB Garamond',serif;overflow-x:hidden;min-height:100vh;overflow-y:auto;}
:root{
  --bg:#06080f;--p1:#0d1018;--p2:#11151e;--p3:#161c28;
  --b1:#1e2535;--b2:#252d3d;--b3:#2e3850;
  --gold:#e8c060;--gold2:#c89030;--gold3:#f8d888;
  --teal:#40d0c0;--rose:#f06080;--violet:#a080f0;
  --sky:#60b8f0;--green:#50d890;--orange:#f08040;
  --text:#e8e0d0;--t2:#8090a8;--t3:#404e66;
  --sidebar-w:310px;
}
::-webkit-scrollbar{width:4px;height:4px;}
::-webkit-scrollbar-track{background:transparent;}
::-webkit-scrollbar-thumb{background:#1e2a3a;border-radius:4px;}

/*══ HERO ══*/
#hero{min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;position:relative;overflow:hidden;padding:60px 20px 48px;background:#06080f;}
#hero::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse 100% 70% at 50% 0%,rgba(232,192,96,.09) 0%,transparent 55%),radial-gradient(ellipse 70% 50% at 15% 80%,rgba(64,208,192,.06) 0%,transparent 50%),radial-gradient(ellipse 60% 80% at 85% 50%,rgba(160,128,240,.05) 0%,transparent 50%);pointer-events:none;}
.hero-grid{position:absolute;inset:0;pointer-events:none;background-image:linear-gradient(rgba(232,192,96,.025) 1px,transparent 1px),linear-gradient(90deg,rgba(232,192,96,.025) 1px,transparent 1px);background-size:64px 64px;animation:gB 10s ease-in-out infinite alternate;}
@keyframes gB{from{opacity:.3;background-size:64px 64px}to{opacity:1;background-size:66px 66px}}
.hero-orb{position:absolute;border-radius:50%;pointer-events:none;}
.hero-orb:nth-child(2){width:600px;height:600px;top:50%;left:50%;transform:translate(-50%,-50%);background:radial-gradient(circle,rgba(232,192,96,.04) 0%,transparent 65%);animation:oP 6s ease-in-out infinite alternate;}
.hero-orb:nth-child(3){width:400px;height:400px;top:25%;left:15%;background:radial-gradient(circle,rgba(64,208,192,.05) 0%,transparent 65%);animation:oP 8s ease-in-out infinite alternate;animation-delay:-3s;}
.hero-orb:nth-child(4){width:320px;height:320px;top:55%;right:10%;background:radial-gradient(circle,rgba(160,128,240,.05) 0%,transparent 65%);animation:oP 7s ease-in-out infinite alternate;animation-delay:-1s;}
@keyframes oP{from{transform:scale(1) translate(0,0)}to{transform:scale(1.15) translate(5px,-5px)}}
.hero-ring{position:absolute;border-radius:50%;border:1px solid rgba(232,192,96,.06);top:50%;left:50%;animation:sR linear infinite;}
.hero-ring:nth-child(5){width:520px;height:520px;animation-duration:50s;transform:translate(-50%,-50%);}
.hero-ring:nth-child(6){width:770px;height:770px;animation-duration:75s;animation-direction:reverse;border-color:rgba(64,208,192,.05);transform:translate(-50%,-50%);}
.hero-ring:nth-child(7){width:1050px;height:1050px;animation-duration:110s;border-color:rgba(160,128,240,.04);transform:translate(-50%,-50%);}
@keyframes sR{from{transform:translate(-50%,-50%) rotate(0)}to{transform:translate(-50%,-50%) rotate(360deg)}}
.hero-content{position:relative;z-index:2;max-width:820px;}
.hero-eyebrow{display:inline-flex;align-items:center;gap:10px;font-family:'JetBrains Mono',monospace;font-size:.6rem;letter-spacing:.28em;text-transform:uppercase;color:var(--gold);border:1px solid rgba(232,192,96,.22);padding:7px 22px;border-radius:2px;margin-bottom:30px;background:rgba(232,192,96,.04);animation:fSD .8s .05s both;}
.hero-eyebrow::before,.hero-eyebrow::after{content:'';width:18px;height:1px;background:currentColor;opacity:.5;}
@keyframes fSD{from{opacity:0;transform:translateY(-10px)}to{opacity:1;transform:none}}
#hero h1{font-family:'Syne',sans-serif;font-weight:800;font-size:clamp(2.6rem,9vw,6rem);line-height:.93;letter-spacing:-3px;margin-bottom:18px;animation:hTI .9s .15s both;}
@keyframes hTI{from{opacity:0;transform:translateY(18px) scale(.97)}to{opacity:1;transform:none}}
.h1-line1{display:block;color:#e8e0d0;}
.h1-line2{display:block;background:linear-gradient(120deg,#e8c060 0%,#f08040 35%,#f06080 65%,#a080f0 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;background-size:200%;animation:gS 5s ease-in-out infinite alternate;}
@keyframes gS{from{background-position:0%}to{background-position:100%}}
.h1-line3{display:block;color:var(--t2);font-style:italic;font-size:.55em;letter-spacing:-1px;margin-top:4px;}
.hero-sub{font-family:'Crimson Pro',serif;font-style:italic;font-size:1.08rem;color:var(--t2);line-height:1.8;margin-bottom:42px;animation:fU .9s .3s both;}
@keyframes fU{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:none}}
.hero-modules{display:grid;grid-template-columns:repeat(auto-fit,minmax(138px,1fr));gap:11px;max-width:800px;margin:0 auto 38px;animation:fU .9s .45s both;}
.hmod{background:rgba(255,255,255,.02);border:1px solid rgba(255,255,255,.06);border-radius:12px;padding:18px 10px 16px;cursor:pointer;transition:transform .22s cubic-bezier(.4,0,.2,1),box-shadow .22s,border-color .22s;display:flex;flex-direction:column;align-items:center;gap:7px;position:relative;overflow:hidden;}
.hmod::before{content:'';position:absolute;inset:0;border-radius:12px;background:radial-gradient(circle at 50% 0%,var(--mc,#e8c060),transparent 65%);opacity:0;transition:opacity .25s;}
.hmod:hover{transform:translateY(-6px);box-shadow:0 20px 50px rgba(0,0,0,.55),0 0 0 1px var(--mc,#e8c060);border-color:var(--mc,#e8c060);}
.hmod:hover::before{opacity:.09;}
.hmod:active{transform:translateY(-2px) scale(.97);}
.hmod-icon{font-size:1.75rem;position:relative;z-index:1;}
.hmod-title{font-family:'JetBrains Mono',monospace;font-size:.58rem;letter-spacing:.1em;text-transform:uppercase;color:var(--t2);text-align:center;line-height:1.5;position:relative;z-index:1;}
.hmod-tag{font-family:'JetBrains Mono',monospace;font-size:.51rem;color:var(--mc,#e8c060);border:1px solid currentColor;padding:2px 7px;border-radius:2px;background:rgba(0,0,0,.35);position:relative;z-index:1;}
.hero-hint{font-family:'JetBrains Mono',monospace;font-size:.55rem;color:var(--t3);letter-spacing:.22em;animation:bnc 2.5s ease-in-out infinite;}
@keyframes bnc{0%,100%{transform:translateY(0)}50%{transform:translateY(6px)}}

/*══ TOP NAV ══*/
#topnav{position:sticky;top:0;z-index:500;background:rgba(6,8,15,.96);border-bottom:1px solid rgba(255,255,255,.05);backdrop-filter:blur(24px);-webkit-backdrop-filter:blur(24px);display:flex;align-items:stretch;overflow-x:auto;scrollbar-width:none;box-shadow:0 1px 40px rgba(0,0,0,.7);}
#topnav::-webkit-scrollbar{display:none;}
.nav-brand{font-family:'Syne',sans-serif;font-size:.78rem;font-weight:800;color:var(--gold);letter-spacing:.06em;padding:0 14px 0 10px;border-right:1px solid rgba(255,255,255,.05);margin-right:2px;white-space:nowrap;flex-shrink:0;cursor:pointer;display:flex;align-items:center;gap:6px;transition:opacity .2s;}
.nav-brand:hover{opacity:.7;}
.nav-brand-dot{width:5px;height:5px;border-radius:50%;background:var(--gold);box-shadow:0 0 8px var(--gold);animation:dP 2s ease-in-out infinite;}
@keyframes dP{0%,100%{opacity:1}50%{opacity:.4}}
.ntab{display:flex;align-items:center;gap:5px;padding:0 12px;font-family:'JetBrains Mono',monospace;font-size:.58rem;letter-spacing:.12em;text-transform:uppercase;color:var(--t3);cursor:pointer;white-space:nowrap;border-bottom:2px solid transparent;transition:color .2s,border-color .2s;position:relative;flex-shrink:0;min-height:42px;}
.ntab:hover{color:var(--t2);}
.ntab.active{color:var(--tc,#e8c060);border-bottom-color:var(--tc,#e8c060);}
.ntab-icon{font-size:.78rem;}

/*══ PAGE SECTIONS ══*/
.psec{display:none;}
.psec.active{display:block;animation:secIn .38s cubic-bezier(.4,0,.2,1) both;}
@keyframes secIn{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
#sec-conic{display:none;height:calc(100vh - 43px);overflow:hidden;}
#sec-conic.active{display:block;}

/*══ CONTENT WRAP ══*/
.cwrap{max-width:1200px;margin:0 auto;padding:26px 16px 70px;}

/*══ SECTION HERO BANNERS ══*/
.shero{padding:30px 0 22px;text-align:center;border-bottom:1px solid var(--b1);margin-bottom:28px;position:relative;overflow:hidden;}
.shero::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse 80% 100% at 50% 0%,var(--sc,rgba(232,192,96,.07)) 0%,transparent 70%);pointer-events:none;}
.shero-badge{font-family:'JetBrains Mono',monospace;font-size:.54rem;letter-spacing:.25em;text-transform:uppercase;color:var(--gold);margin-bottom:7px;display:block;position:relative;z-index:1;}
.shero h2{font-family:'Syne',sans-serif;font-weight:800;font-size:clamp(1.55rem,4vw,2.7rem);line-height:1.05;position:relative;z-index:1;margin-bottom:6px;}
.shero p{font-family:'Crimson Pro',serif;font-style:italic;font-size:.93rem;color:var(--t2);position:relative;z-index:1;}
.snav{display:flex;gap:5px;flex-wrap:wrap;justify-content:center;margin:12px 0 0;position:relative;z-index:1;}
.snav a{font-family:'JetBrains Mono',monospace;font-size:.54rem;letter-spacing:.1em;text-transform:uppercase;color:var(--t3);border:1px solid var(--b2);padding:4px 10px;border-radius:2px;text-decoration:none;background:rgba(255,255,255,.015);transition:all .18s;}
.snav a:hover{color:var(--gold);border-color:var(--gold2);background:rgba(232,192,96,.04);}

/*══ TRIG SECTION STYLES ══*/
.trig-wrap{--bg:#06080f;--card:#13161f;--border:#1e2535;--gold:#e8b84b;--blue:#4b9fe8;--pink:#e84b7a;--green:#4be8a0;--purple:#b84be8;--orange:#e8a04b;--text:#e8e8f0;--muted:#7878a0;--fbg:#0d0d18;}
.trig-wrap .sec{padding:50px 0;border-top:1px solid var(--border);}
.trig-wrap .wrap{max-width:100%;padding:0;}
.trig-wrap .sh{display:flex;align-items:baseline;gap:16px;margin-bottom:38px;}
.trig-wrap .sn{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--gold);letter-spacing:2px;opacity:.7;}
.trig-wrap h2{font-family:'Syne',sans-serif;font-size:1.95rem;font-weight:700;color:#fff;letter-spacing:-.5px;}
.trig-wrap h3{font-family:'Syne',sans-serif;font-size:1.18rem;color:var(--gold);margin:26px 0 13px;padding-bottom:6px;border-bottom:1px solid rgba(232,184,75,.14);}
.trig-wrap h4{font-family:'JetBrains Mono',monospace;font-size:.79rem;letter-spacing:1.5px;text-transform:uppercase;color:var(--blue);margin:18px 0 8px;}
.trig-wrap .fg{display:grid;grid-template-columns:repeat(auto-fill,minmax(275px,1fr));gap:2px;background:var(--border);border:1px solid var(--border);border-radius:6px;overflow:hidden;margin:13px 0;}
.trig-wrap .fb{background:var(--fbg);padding:15px 17px 12px;cursor:pointer;transition:background .18s,transform .15s;position:relative;border-left:2px solid transparent;}
.trig-wrap .fb:hover{background:#131325;transform:translateX(3px);border-left-color:var(--gold);}
.trig-wrap .fl{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:7px;display:flex;justify-content:space-between;align-items:center;}
.trig-wrap .ph{font-size:8px;color:var(--gold);opacity:0;transition:opacity .18s;background:rgba(232,184,75,.1);padding:2px 7px;border-radius:2px;border:1px solid rgba(232,184,75,.25);}
.trig-wrap .fb:hover .ph{opacity:1;}
.trig-wrap .fm{font-family:'JetBrains Mono',monospace;font-size:.88rem;color:#fff;line-height:1.65;}
.trig-wrap .fm .v{color:var(--gold);}.trig-wrap .fm .e{color:var(--muted);}.trig-wrap .fm .o{color:var(--pink);}.trig-wrap .fm .n{color:var(--blue);}.trig-wrap .fm .f{color:var(--green);}
.trig-wrap .flist{display:grid;grid-template-columns:repeat(auto-fill,minmax(225px,1fr));gap:2px;background:var(--border);border:1px solid var(--border);border-radius:6px;overflow:hidden;margin:11px 0;}
.trig-wrap .fi{background:var(--fbg);padding:10px 13px;font-family:'JetBrains Mono',monospace;font-size:.84rem;color:var(--text);transition:background .18s,transform .15s;cursor:pointer;display:flex;align-items:center;justify-content:space-between;border-left:2px solid transparent;}
.trig-wrap .fi:hover{background:#131325;transform:translateX(3px);border-left-color:var(--blue);}
.trig-wrap .lhs{color:var(--green);}.trig-wrap .rhs{color:#fff;}.trig-wrap .sep{color:var(--muted);margin:0 6px;}
.trig-wrap .fph{font-size:8px;color:var(--gold);opacity:0;transition:opacity .18s;background:rgba(232,184,75,.1);padding:2px 6px;border-radius:2px;border:1px solid rgba(232,184,75,.25);white-space:nowrap;margin-left:6px;flex-shrink:0;}
.trig-wrap .fi:hover .fph{opacity:1;}
.trig-wrap .atbl{width:100%;border-collapse:collapse;font-family:'JetBrains Mono',monospace;font-size:.81rem;margin:13px 0;}
.trig-wrap .atbl th{background:rgba(232,184,75,.08);color:var(--gold);font-size:9px;letter-spacing:1.5px;text-transform:uppercase;padding:10px 11px;text-align:center;border-bottom:1px solid var(--border);}
.trig-wrap .atbl td{padding:8px 11px;text-align:center;border-bottom:1px solid rgba(30,37,53,.6);background:var(--fbg);transition:background .12s;}
.trig-wrap .atbl tr:hover td{background:#0f1022;}
.trig-wrap .atbl td:first-child{color:var(--blue);font-weight:600;}
.trig-wrap .dtbl{width:100%;border-collapse:collapse;font-size:.85rem;margin:13px 0;}
.trig-wrap .dtbl th{background:rgba(75,159,232,.08);color:var(--blue);padding:10px 12px;text-align:left;font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:1px;text-transform:uppercase;border-bottom:1px solid var(--border);}
.trig-wrap .dtbl td{padding:9px 12px;border-bottom:1px solid rgba(30,37,53,.6);background:var(--fbg);font-family:'JetBrains Mono',monospace;font-size:.81rem;transition:background .12s;}
.trig-wrap .dtbl td:first-child{color:var(--green);}
.trig-wrap .dtbl tr:hover td{background:#0f1022;}
.trig-wrap .rb{border-left:2px solid var(--gold);background:rgba(232,184,75,.04);padding:11px 16px;margin:11px 0;border-radius:0 4px 4px 0;font-family:'JetBrains Mono',monospace;font-size:.82rem;line-height:1.9;}
.trig-wrap .rb.b{border-color:var(--blue);background:rgba(75,159,232,.04);}
.trig-wrap .rb.r{border-color:var(--pink);background:rgba(232,75,122,.04);}
.trig-wrap .rb.g{border-color:var(--green);background:rgba(75,232,160,.04);}
.trig-wrap .nb{background:rgba(75,232,160,.04);border:1px solid rgba(75,232,160,.17);border-radius:4px;padding:11px 15px;margin:13px 0;font-family:'JetBrains Mono',monospace;font-size:.79rem;color:var(--green);line-height:1.8;}
.trig-wrap .nb strong{display:block;margin-bottom:4px;letter-spacing:1px;}
.trig-wrap .gg{background:var(--card);border:1px solid var(--border);border-radius:6px;overflow:hidden;margin:22px 0;}
.trig-wrap .gc{padding:11px 14px;background:rgba(255,255,255,.015);border-bottom:1px solid var(--border);display:flex;flex-wrap:wrap;gap:6px;align-items:center;}
.trig-wrap canvas{display:block;width:100%;background:#06080f;}
.trig-wrap .ft{font-family:'JetBrains Mono',monospace;font-size:10px;padding:5px 11px;border:1px solid var(--border);border-radius:2px;background:transparent;cursor:pointer;transition:all .18s;}
.trig-wrap .ft.on{opacity:1;}.trig-wrap .ft:not(.on){opacity:.3;}
.trig-wrap .ft:hover{background:rgba(255,255,255,.04);}
.trig-wrap .g{color:var(--gold);}.trig-wrap .bl{color:var(--blue);}.trig-wrap .pk{color:var(--pink);}.trig-wrap .gr{color:var(--green);}

/*══ PROOF MODAL ══*/
#proof-overlay{position:fixed;inset:0;z-index:9999;background:rgba(3,4,10,.92);backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);display:flex;align-items:center;justify-content:center;padding:16px;opacity:0;pointer-events:none;transition:opacity .25s cubic-bezier(.4,0,.2,1);}
#proof-overlay.show{opacity:1;pointer-events:all;}
#proof-box{background:linear-gradient(135deg,#0f1220 0%,#0d1018 50%,#111526 100%);border:1px solid rgba(232,184,75,.15);border-radius:12px;max-width:680px;width:100%;max-height:88vh;overflow-y:auto;box-shadow:0 40px 100px rgba(0,0,0,.9),0 0 0 1px rgba(232,184,75,.06),inset 0 1px 0 rgba(232,184,75,.1);transform:translateY(24px) scale(.96);transition:transform .3s cubic-bezier(.16,1,.3,1);scrollbar-width:thin;scrollbar-color:#1e2535 transparent;}
#proof-overlay.show #proof-box{transform:translateY(0) scale(1);}
#proof-box::-webkit-scrollbar{width:3px;}
#proof-box::-webkit-scrollbar-thumb{background:#1e2535;border-radius:3px;}
#proof-hdr{padding:20px 24px 16px;border-bottom:1px solid rgba(232,184,75,.1);display:flex;align-items:flex-start;justify-content:space-between;gap:14px;position:sticky;top:0;background:linear-gradient(135deg,#0f1220,#0d1018);backdrop-filter:blur(12px);z-index:2;}
#proof-hdr::after{content:'';position:absolute;bottom:0;left:24px;right:24px;height:1px;background:linear-gradient(90deg,rgba(232,184,75,.4),transparent);}
#proof-tag{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2.5px;text-transform:uppercase;color:rgba(232,184,75,.7);margin-bottom:5px;display:block;}
#proof-title{font-family:'JetBrains Mono',monospace;font-size:.95rem;color:#fff;line-height:1.4;}
#proof-close{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);color:#8090a8;font-size:14px;width:32px;height:32px;border-radius:6px;cursor:pointer;display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:all .15s;font-family:sans-serif;}
#proof-close:hover{background:rgba(240,96,128,.15);border-color:rgba(240,96,128,.4);color:#f06080;}
#proof-body{padding:22px 24px 28px;}
.ps{margin-bottom:20px;}
.pst{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2px;text-transform:uppercase;color:#60b8f0;margin-bottom:10px;padding-bottom:5px;border-bottom:1px solid rgba(75,159,232,.12);}
.pstep{display:flex;gap:12px;align-items:flex-start;margin-bottom:6px;padding:10px 14px;background:rgba(255,255,255,.02);border-radius:4px;border-left:2px solid transparent;transition:border-color .18s,background .18s;}
.pstep:hover{border-left-color:#e8b84b;background:rgba(232,184,75,.04);}
.sn2{font-family:'JetBrains Mono',monospace;font-size:9px;color:#e8b84b;background:rgba(232,184,75,.12);min-width:22px;height:22px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px;font-weight:700;}
.st{font-family:'Crimson Pro',serif;font-size:.97rem;color:#e8e8f0;line-height:1.7;flex:1;}
.st .m{font-family:'JetBrains Mono',monospace;font-size:.82rem;color:#fff;background:rgba(255,255,255,.06);padding:2px 7px;border-radius:3px;display:inline-block;margin:1px 2px;border:1px solid rgba(255,255,255,.06);}
.st .h{color:#4be8a0;font-family:'JetBrains Mono',monospace;font-size:.82rem;}
.pnote{background:rgba(232,184,75,.05);border:1px solid rgba(232,184,75,.18);border-radius:4px;padding:10px 14px;margin-top:12px;font-family:'JetBrains Mono',monospace;font-size:.77rem;color:#e8b84b;line-height:1.75;}
.pnote::before{content:'💡  ';}
.pdiag{background:rgba(75,159,232,.04);border:1px solid rgba(75,159,232,.12);border-radius:4px;padding:12px 14px;margin-bottom:12px;font-family:'JetBrains Mono',monospace;font-size:.76rem;color:#60b8f0;line-height:1.9;white-space:pre;}

/*══ CALCULATOR ══*/
#calc-wrap{display:flex;justify-content:center;padding:24px 0 60px;}
#calc{background:linear-gradient(160deg,#0d1120 0%,#090c14 60%,#0d0f1e 100%);border:1px solid rgba(232,192,96,.18);border-radius:20px;width:min(440px,100%);box-shadow:0 40px 100px rgba(0,0,0,.8),0 0 0 1px rgba(232,192,96,.06),inset 0 1px 0 rgba(232,192,96,.12);overflow:hidden;position:relative;}
#calc::before{content:'';position:absolute;top:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent,rgba(232,192,96,.4),transparent);}
.calc-header{padding:11px 16px 7px;border-bottom:1px solid rgba(255,255,255,.04);display:flex;align-items:center;justify-content:space-between;}
.calc-header-title{font-family:'JetBrains Mono',monospace;font-size:.57rem;letter-spacing:.2em;text-transform:uppercase;color:rgba(232,192,96,.5);}
.calc-mode-btns{display:flex;gap:4px;}
.calc-mode-btn{font-family:'JetBrains Mono',monospace;font-size:.54rem;padding:3px 8px;border-radius:3px;cursor:pointer;border:1px solid rgba(255,255,255,.07);background:rgba(255,255,255,.03);color:var(--t3);transition:all .14s;letter-spacing:.06em;}
.calc-mode-btn.active{background:rgba(232,192,96,.12);color:var(--gold);border-color:rgba(232,192,96,.3);}
#calc-display{padding:14px 16px 10px;background:linear-gradient(180deg,rgba(0,0,0,.4) 0%,rgba(0,0,0,.2) 100%);border-bottom:1px solid rgba(255,255,255,.04);min-height:88px;display:flex;flex-direction:column;justify-content:flex-end;align-items:flex-end;position:relative;overflow:hidden;}
#calc-display::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at 50% 0%,rgba(64,208,192,.03) 0%,transparent 60%);}
#calc-history{font-family:'JetBrains Mono',monospace;font-size:.7rem;color:rgba(128,144,168,.45);min-height:17px;text-align:right;margin-bottom:3px;position:relative;z-index:1;word-break:break-all;}
#calc-expr{font-family:'JetBrains Mono',monospace;font-size:1rem;color:var(--t2);min-height:20px;text-align:right;position:relative;z-index:1;word-break:break-all;}
#calc-result{font-family:'JetBrains Mono',monospace;font-size:2.1rem;font-weight:600;letter-spacing:-1px;background:linear-gradient(120deg,#e8c060,#f8d888);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;text-align:right;min-height:42px;line-height:1.15;position:relative;z-index:1;word-break:break-all;transition:transform .1s;}
#calc-result.flash{animation:rF .22s ease;}
@keyframes rF{0%,100%{transform:scale(1)}50%{transform:scale(1.04);filter:brightness(1.3)}}
.calc-btns{display:grid;grid-template-columns:repeat(5,1fr);gap:1px;background:rgba(255,255,255,.025);padding:1px;}
.cb{background:#09020f;border:none;font-family:'JetBrains Mono',monospace;font-size:.78rem;font-weight:500;padding:0;height:50px;cursor:pointer;display:flex;align-items:center;justify-content:center;color:var(--t2);position:relative;overflow:hidden;transition:color .12s,background .12s;user-select:none;-webkit-user-select:none;}
.cb:hover{background:#0f1422;color:#fff;}
.cb:active{background:#141824;}
.cb.num{color:#c0c8d8;background:#0a0c18;}
.cb.num:hover{color:#fff;background:#0f1828;}
.cb.op{color:var(--teal);}
.cb.op:hover{color:#fff;background:rgba(64,208,192,.14);}
.cb.fn{color:var(--gold);font-size:.7rem;}
.cb.fn:hover{color:#fff;background:rgba(232,192,96,.1);}
.cb.eq{background:linear-gradient(135deg,#c89030,#e8c060);color:#000;font-size:1.05rem;font-weight:700;}
.cb.eq:hover{background:linear-gradient(135deg,#e8c060,#f8d888);box-shadow:0 0 20px rgba(232,192,96,.3);}
.cb.clr{color:var(--rose);}
.cb.clr:hover{color:#fff;background:rgba(240,96,128,.14);}
.cb.wide{grid-column:span 2;}
.cb.mem{color:var(--violet);font-size:.66rem;}
.cb.mem:hover{color:#fff;background:rgba(160,128,240,.1);}
.cb .cb-ripple{position:absolute;border-radius:50%;background:rgba(255,255,255,.13);transform:scale(0);animation:cbR .38s ease-out forwards;pointer-events:none;}
@keyframes cbR{to{transform:scale(4);opacity:0;}}
.calc-status{display:flex;justify-content:space-between;align-items:center;padding:5px 11px;border-top:1px solid rgba(255,255,255,.03);}
.calc-status span{font-family:'JetBrains Mono',monospace;font-size:.54rem;color:var(--t3);letter-spacing:.08em;}
.calc-status .mem-ind{color:var(--violet);}
.calc-status .angle-ind{color:#60b8f0;}

/*══ CURSOR ══*/
body{cursor:none !important;}
canvas,input,select,button,textarea,.cb,a,.ntab,.hmod,.nav-brand,.trig-wrap .fb,.trig-wrap .fi,.io-fb,.ch-fb,.rd-fb,.snav a,.dsm-preset{cursor:pointer !important;}
#cur-dot{position:fixed;z-index:999999;pointer-events:none;width:10px;height:10px;border-radius:50%;background:radial-gradient(circle,#e8c060,#f08040);box-shadow:0 0 10px #e8c060,0 0 20px rgba(232,192,96,.3);transform:translate(-50%,-50%);top:-20px;left:-20px;transition:width .12s,height .12s,box-shadow .12s;}
#cur-ring{position:fixed;z-index:999998;pointer-events:none;width:28px;height:28px;border-radius:50%;border:1.5px solid rgba(232,192,96,.4);box-shadow:0 0 8px rgba(232,192,96,.12);transform:translate(-50%,-50%);top:-40px;left:-40px;transition:width .18s,height .18s,border-color .2s,opacity .2s;}
</style>
<!-- Coord Geometry Styles -->
<style>
  /* Coord Geometry scoped variables */
  #sec-coord { --text-mid:#a8b0c0; --text-dim:#606878; --gold-light:#e8c97a; --gold-dim:rgba(201,168,76,0.35); --surface:#0d0f18; --formula-bg:rgba(10,12,20,0.9); --border:#1e2535; --teal:#4ecdc4; --rose:#e8677a; --violet:#a78bfa; --sky:#60a5fa; --green:#6ee7b7; }
  /* ── LAYOUT ── */
  #sec-coord main { max-width: 1200px; margin: 0 auto; padding: 2rem 1.5rem 4rem; }

  /* ── SECTION ── */
  #sec-coord .section {
    margin-bottom: 3.5rem;
    animation: fadeUp 0.4s ease both;
  }
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  #sec-coord .section-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 1.8rem;
    padding-bottom: 0.7rem;
    border-bottom: 1px solid var(--border);
  }
  #sec-coord .section-num {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.7rem;
    color: var(--gold);
    background: rgba(201,168,76,0.08);
    border: 1px solid var(--gold-dim);
    padding: 0.2rem 0.5rem;
    border-radius: 3px;
  }
  #sec-coord .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.65rem;
    font-weight: 700;
    color: var(--text);
  }

  /* ── GRID ── */
  #sec-coord .grid { display: grid; gap: 1.2rem; }
  #sec-coord .grid-2 { grid-template-columns: repeat(auto-fit, minmax(340px, 1fr)); }
  #sec-coord .grid-3 { grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); }

  /* ── CARD ── */
  #sec-coord .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 1.4rem 1.5rem;
    position: relative;
    overflow: hidden;
    transition: border-color 0.2s, box-shadow 0.2s;
  }
  #sec-coord .card:hover {
    border-color: var(--gold-dim);
    box-shadow: 0 0 24px rgba(201,168,76,0.06);
  }
  #sec-coord .card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--gold-dim), transparent);
    opacity: 0.6;
  }
  #sec-coord .card.teal::before  { background: linear-gradient(90deg, var(--teal), transparent); }
  #sec-coord .card.rose::before  { background: linear-gradient(90deg, var(--rose), transparent); }
  #sec-coord .card.violet::before{ background: linear-gradient(90deg, var(--violet), transparent); }
  #sec-coord .card.sky::before   { background: linear-gradient(90deg, var(--sky), transparent); }
  #sec-coord .card.green::before { background: linear-gradient(90deg, var(--green), transparent); }

  #sec-coord .card h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--gold-light);
    margin-bottom: 0.8rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }
  #sec-coord .card h3 .icon { font-size: 1.1rem; }
  #sec-coord .card p { color: var(--text-mid); font-size: 0.95rem; margin-bottom: 0.5rem; }
  #sec-coord .card p:last-child { margin-bottom: 0; }

  /* ── FORMULA BOX ── */
  #sec-coord .formula {
    background: var(--formula-bg);
    border: 1px solid rgba(201,168,76,0.2);
    border-radius: 5px;
    padding: 0.5rem 0.9rem;
    margin: 0.5rem 0;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.88rem;
    color: var(--sky);
    display: block;
    overflow-x: auto;
    white-space: nowrap;
  }
  #sec-coord .formula.gold { color: var(--gold-light); }
  #sec-coord .formula.green { color: var(--green); }
  #sec-coord .formula.rose { color: #f4a7b3; }
  #sec-coord .formula.violet { color: var(--violet); }
  #sec-coord .formula.teal { color: var(--teal); }

  /* ── SVG DIAGRAM ── */
  #sec-coord .diagram-wrap {
    margin: 1rem 0 0.5rem;
    background: #080a0e;
    border: 1px solid var(--border);
    border-radius: 6px;
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  #sec-coord .diagram-wrap svg {
    max-width: 100%;
    height: auto;
    display: block;
  }
  #sec-coord .diagram-cap {
    font-size: 0.78rem;
    color: var(--text-dim);
    text-align: center;
    font-style: italic;
    margin-top: 0.3rem;
    font-family: 'JetBrains Mono', monospace;
  }

  /* proof / note */
  #sec-coord .note {
    background: rgba(201,168,76,0.04);
    border-left: 2px solid var(--gold-dim);
    padding: 0.5rem 0.9rem;
    margin-top: 0.7rem;
    font-size: 0.88rem;
    color: var(--text-mid);
    border-radius: 0 4px 4px 0;
  }
  #sec-coord .note strong { color: var(--gold); }

  #sec-coord .tag {
    display: inline-block;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.6rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    padding: 0.15rem 0.45rem;
    border-radius: 3px;
    margin-left: 0.4rem;
    vertical-align: middle;
  }
  #sec-coord .tag.adv { background: rgba(232,103,122,0.15); color: var(--rose); border: 1px solid rgba(232,103,122,0.3); }
  #sec-coord .tag.imp { background: rgba(201,168,76,0.12); color: var(--gold); border: 1px solid var(--gold-dim); }

  #sec-coord ul.props {
    list-style: none;
    padding: 0;
    margin-top: 0.5rem;
  }
  #sec-coord ul.props li {
    padding: 0.25rem 0 0.25rem 1.2rem;
    position: relative;
    font-size: 0.93rem;
    color: var(--text-mid);
    border-bottom: 1px solid rgba(42,47,62,0.5);
  }
  #sec-coord ul.props li:last-child { border-bottom: none; }
  #sec-coord ul.props li::before {
    content: '▸';
    position: absolute;
    left: 0;
    color: var(--gold-dim);
    font-size: 0.7rem;
    top: 0.45rem;
  }

  /* toc table */
  #sec-coord .toc-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 0.6rem;
    margin-bottom: 2.5rem;
  }
  #sec-coord .toc-item {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 5px;
    padding: 0.55rem 0.8rem;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.72rem;
    color: var(--text-mid);
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    transition: all 0.2s;
  }
  #sec-coord .toc-item:hover { border-color: var(--gold-dim); color: var(--gold); background: rgba(201,168,76,0.04); }
  #sec-coord .toc-item .num { color: var(--gold-dim); min-width: 1.5rem; }

  #sec-coord hr.divider {
    border: none;
    border-top: 1px solid var(--border);
    margin: 0.8rem 0 1rem;
  }

  /* responsive */
  @media (max-width: 600px) {
    #sec-coord header { padding: 2rem 1rem 1.5rem; }
    #sec-coord .section-title { font-size: 1.3rem; }
    #sec-coord .card { padding: 1rem; }
  }

</style>
<!-- Constants Styles -->
<style>

  
  /* Constants section scoped variables */
  #sec-const { --cyan:#22d3ee; --amber:#fbbf24; --orange:#fb923c; --green:#4ade80; --violet:#c084fc; --red:#fb7185; --blue:#60a5fa; --muted:#6b7280; --soft:#9ca3af; --s2:#0d1018; --border2:#1e2535; }
  #sec-const .page { max-width: 980px; margin: 0 auto; }

  /* HEADER */
  #sec-const .header {
    text-align: center;
    padding: 30px 0 36px;
    position: relative;
  }
  #sec-const .header-line {
    display: flex;
    align-items: center;
    gap: 16px;
    justify-content: center;
    margin-bottom: 12px;
  }
  #sec-const .header-line .dot {
    width: 8px; height: 8px; border-radius: 50%;
    background: var(--cyan);
    box-shadow: 0 0 12px var(--cyan);
    animation: pulse 2s infinite;
  }
  @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:0.4} }
  #sec-const .header h1 {
    font-family: 'Syne', sans-serif;
    font-size: clamp(1.9rem, 5vw, 3rem);
    font-weight: 800;
    letter-spacing: -1px;
    line-height: 1.1;
  }
  #sec-const .h1-line1 { color: var(--cyan); }
  #sec-const .h1-line2 {
    background: linear-gradient(90deg, var(--amber), var(--orange));
    -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
  }
  #sec-const .header .sub {
    margin-top: 10px;
    font-size: 0.78rem;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--muted);
  }
  #sec-const .pills {
    margin-top: 14px;
    display: flex; justify-content: center; flex-wrap: wrap; gap: 8px;
  }
  #sec-const .pill {
    padding: 3px 12px; border-radius: 20px;
    font-size: 0.68rem; letter-spacing: 1.5px; text-transform: uppercase; font-weight: 600;
  }
  #sec-const .p-cyan  { background: rgba(34,211,238,0.1);  color: var(--cyan);   border: 1px solid rgba(34,211,238,0.2); }
  #sec-const .p-amber { background: rgba(251,191,36,0.1);  color: var(--amber);  border: 1px solid rgba(251,191,36,0.2); }
  #sec-const .p-green { background: rgba(74,222,128,0.08); color: var(--green);  border: 1px solid rgba(74,222,128,0.18); }
  #sec-const .p-vio   { background: rgba(192,132,252,0.08);color: var(--violet); border: 1px solid rgba(192,132,252,0.18); }
  #sec-const .p-red   { background: rgba(251,113,133,0.08);color: var(--red);    border: 1px solid rgba(251,113,133,0.18); }

  /* SECTION */
  #sec-const .sec { margin-bottom: 28px; }
  #sec-const .sec-head {
    display: flex; align-items: center; gap: 10px;
    margin-bottom: 14px;
  }
  #sec-const .sec-icon {
    width: 30px; height: 30px; border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 0.85rem; flex-shrink: 0;
  }
  #sec-const .sec-label {
    font-family: 'Syne', sans-serif;
    font-size: 1.05rem; font-weight: 700;
  }
  #sec-const .sec-rule { flex:1; height:1px; background: var(--border2); }

  /* GRID LAYOUTS */
  #sec-const .g2 { display:grid; grid-template-columns:1fr 1fr; gap:16px; }
  #sec-const .g3 { display:grid; grid-template-columns:1fr 1fr 1fr; gap:16px; }
  @media(max-width:700px) { #sec-const .g2, #sec-const .g3 { grid-template-columns:1fr; } }
  @media(min-width:701px) and (max-width:860px) { #sec-const .g3 { grid-template-columns:1fr 1fr; } }

  /* CARD */
  #sec-const .card {
    background: var(--s2);
    border: 1px solid var(--border);
    border-radius: 14px;
    overflow: hidden;
  }
  #sec-const .card-header {
    padding: 9px 14px;
    font-size: 0.68rem; letter-spacing: 2px; text-transform: uppercase;
    font-weight: 600; color: var(--muted);
    background: rgba(255,255,255,0.02);
    border-bottom: 1px solid var(--border);
  }

  /* CONSTANT ROWS */
  #sec-const .const-row {
    display: flex; justify-content: space-between; align-items: center;
    padding: 9px 14px;
    border-bottom: 1px solid rgba(26,37,64,0.7);
    gap: 8px;
  }
  #sec-const .const-row:last-child { border-bottom: none; }
  #sec-const .const-row:hover { background: rgba(255,255,255,0.02); }
  #sec-const .const-name { font-size: 0.8rem; color: var(--soft); flex:1.2; }
  #sec-const .const-sym  { font-family: 'IBM Plex Mono', monospace; font-size: 0.78rem; color: var(--amber); flex:0.8; text-align:center; }
  #sec-const .const-val  { font-family: 'IBM Plex Mono', monospace; font-size: 0.78rem; font-weight:600; flex:1.5; text-align:right; }
  #sec-const .cv-cyan   { color: var(--cyan); }
  #sec-const .cv-green  { color: var(--green); }
  #sec-const .cv-vio    { color: var(--violet); }
  #sec-const .cv-red    { color: var(--red); }
  #sec-const .cv-orange { color: var(--orange); }
  #sec-const .cv-blue   { color: var(--blue); }

  /* LOG TABLE */
  #sec-const table { width:100%; border-collapse:collapse; font-family:'IBM Plex Mono',monospace; font-size:0.82rem; }
  #sec-const thead th {
    padding: 9px 12px; text-align:center;
    font-family:'Outfit',sans-serif; font-size:0.68rem;
    letter-spacing:2px; text-transform:uppercase; font-weight:600;
    color: var(--muted); border-bottom:1px solid var(--border);
    background: rgba(255,255,255,0.02);
  }
  #sec-const tbody td { padding: 8px 12px; text-align:center; border-bottom:1px solid rgba(26,37,64,0.6); }
  #sec-const tbody tr:last-child td { border-bottom:none; }
  #sec-const tbody tr:hover { background:rgba(255,255,255,0.02); }
  #sec-const .t-n   { color: var(--blue);   font-weight:600; }
  #sec-const .t-log { color: var(--amber);  }
  #sec-const .t-ln  { color: var(--green);  }
  #sec-const .t-der { color: var(--violet); font-size:0.72rem; }
  #sec-const .hl    { background: rgba(251,191,36,0.04) !important; }

  /* MOLAR MASS GRID */
  #sec-const .mol-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(120px,1fr));
    gap: 1px; background: var(--border);
    border-radius: 14px; overflow: hidden;
  }
  #sec-const .mol-cell {
    background: var(--s2);
    padding: 12px 10px; text-align:center;
    transition: background 0.15s;
  }
  #sec-const .mol-cell:hover { background: rgba(255,255,255,0.03); }
  #sec-const .mol-formula { font-family:'IBM Plex Mono',monospace; font-size:0.82rem; font-weight:600; color: var(--cyan); }
  #sec-const .mol-name    { font-size:0.67rem; color:var(--muted); margin-top:3px; }
  #sec-const .mol-mass    { font-family:'IBM Plex Mono',monospace; font-size:1rem; font-weight:600; color:var(--amber); margin-top:5px; }
  #sec-const .mol-unit    { font-size:0.6rem; color:var(--muted); }

  /* INDUCTIVE / MESOMERIC */
  #sec-const .effect-card {
    background: var(--s2);
    border: 1px solid var(--border);
    border-radius: 14px;
    overflow: hidden;
  }
  #sec-const .effect-header {
    padding: 10px 16px;
    font-size: 0.68rem; letter-spacing:2px; text-transform:uppercase;
    font-weight:600; border-bottom:1px solid var(--border);
    background: rgba(255,255,255,0.02);
  }
  #sec-const .effect-body { padding: 14px 16px; }

  #sec-const .effect-row {
    display: flex; align-items: center; gap: 0;
    margin-bottom: 10px;
    flex-wrap: wrap;
  }
  #sec-const .effect-label {
    font-size:0.72rem; letter-spacing:1px; text-transform:uppercase;
    font-weight:600; color:var(--muted); width:40px; flex-shrink:0;
  }
  #sec-const .chain {
    display:flex; align-items:center; flex-wrap:wrap; gap:0; flex:1;
  }
  #sec-const .grp {
    font-family:'IBM Plex Mono',monospace;
    font-size:0.75rem; font-weight:600;
    padding: 3px 9px; border-radius:6px;
    white-space: nowrap;
  }
  #sec-const .arrow {
    font-size:0.7rem; color:var(--muted); padding: 0 4px;
    flex-shrink:0;
  }
  /* -I groups: red shades */
  #sec-const .gi { background:rgba(251,113,133,0.12); color:var(--red); border:1px solid rgba(251,113,133,0.2); }
  /* +I groups: green shades */
  #sec-const .gp { background:rgba(74,222,128,0.1); color:var(--green); border:1px solid rgba(74,222,128,0.18); }
  /* -M groups: orange */
  #sec-const .gm { background:rgba(251,146,60,0.12); color:var(--orange); border:1px solid rgba(251,146,60,0.2); }
  /* +M groups: violet */
  #sec-const .gv { background:rgba(192,132,252,0.1); color:var(--violet); border:1px solid rgba(192,132,252,0.2); }

  #sec-const .effect-note {
    margin-top:8px; padding:8px 12px;
    background:rgba(255,255,255,0.02); border-radius:8px;
    border-left:3px solid var(--border2);
    font-size:0.75rem; color:var(--soft); line-height:1.6;
  }
  #sec-const .effect-note b { color:var(--amber); font-weight:600; }

  /* APPROX BOX */
  #sec-const .approx-grid {
    display:grid; grid-template-columns: repeat(auto-fill, minmax(140px,1fr));
    gap:1px; background:var(--border); border-radius:14px; overflow:hidden;
  }
  #sec-const .approx-cell {
    background:var(--s2); padding:12px 10px; text-align:center;
    transition:background 0.15s;
  }
  #sec-const .approx-cell:hover { background:rgba(255,255,255,0.03); }
  #sec-const .approx-expr { font-family:'IBM Plex Mono',monospace; font-size:0.9rem; font-weight:600; color:var(--violet); }
  #sec-const .approx-eq   { font-size:0.7rem; color:var(--muted); margin:3px 0; }
  #sec-const .approx-val  { font-family:'IBM Plex Mono',monospace; font-size:0.95rem; font-weight:600; color:var(--cyan); }

  /* FOOTER */
  #sec-const .footer {
    text-align:center; margin-top:40px; padding-top:20px;
    border-top:1px solid var(--border);
    color:var(--muted); font-size:0.72rem; letter-spacing:2px; text-transform:uppercase;
  }
  #sec-const .footer .badge {
    display:inline-block; margin-top:8px; padding:4px 18px;
    border-radius:20px; background:rgba(34,211,238,0.08);
    color:var(--cyan); font-size:0.68rem; border:1px solid rgba(34,211,238,0.15);
  }

  #sec-const sub { font-size:0.65em; }

</style>
<!-- Cheatsheet Styles -->
<style>

  

  /* Cheatsheet section variables */
  #sec-cheat { --blue:rgba(96,165,250,1); --lavender:rgba(167,139,250,1); --border2:#1e2535; }
  #sec-cheat .page {
    max-width: 960px;
    margin: 0 auto;
  }

  /* HEADER */
  #sec-cheat .header {
    text-align: center;
    margin-bottom: 40px;
    position: relative;
    padding: 36px 0 28px;
  }

  #sec-cheat .header::before {
    content: '';
    position: absolute;
    top: 0; left: 50%; transform: translateX(-50%);
    width: 60px; height: 3px;
    background: var(--gold);
    border-radius: 2px;
  }

  #sec-cheat .header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 5vw, 3.2rem);
    font-weight: 900;
    letter-spacing: -0.5px;
    background: linear-gradient(135deg, #f5c842 0%, #ff6b8a 50%, #a78bfa 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    line-height: 1.15;
  }

  #sec-cheat .header .sub {
    margin-top: 10px;
    font-size: 0.95rem;
    color: var(--muted);
    font-weight: 300;
    letter-spacing: 3px;
    text-transform: uppercase;
  }

  #sec-cheat .header .tag-row {
    margin-top: 16px;
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
  }

  #sec-cheat .tag {
    padding: 4px 14px;
    border-radius: 20px;
    font-size: 0.72rem;
    font-weight: 500;
    letter-spacing: 1px;
    text-transform: uppercase;
  }

  #sec-cheat .tag-gold { background: rgba(245,200,66,0.12); color: var(--gold); border: 1px solid rgba(245,200,66,0.25); }
  #sec-cheat .tag-teal { background: rgba(56,217,192,0.1); color: var(--teal); border: 1px solid rgba(56,217,192,0.2); }
  #sec-cheat .tag-rose { background: rgba(255,107,138,0.1); color: var(--rose); border: 1px solid rgba(255,107,138,0.2); }
  #sec-cheat .tag-lav { background: rgba(167,139,250,0.1); color: var(--lavender); border: 1px solid rgba(167,139,250,0.2); }

  /* SECTION */
  #sec-cheat .section {
    margin-bottom: 32px;
  }

  #sec-cheat .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.25rem;
    font-weight: 700;
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  #sec-cheat .section-title .icon {
    width: 32px; height: 32px;
    border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 0.9rem;
    flex-shrink: 0;
  }

  #sec-cheat .icon-gold { background: rgba(245,200,66,0.15); }
  #sec-cheat .icon-teal { background: rgba(56,217,192,0.12); }
  #sec-cheat .icon-rose { background: rgba(255,107,138,0.12); }
  #sec-cheat .icon-lav { background: rgba(167,139,250,0.12); }

  #sec-cheat .section-title .line {
    flex: 1;
    height: 1px;
    background: var(--border);
  }

  /* CARDS */
  #sec-cheat .card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 14px;
    overflow: hidden;
  }

  #sec-cheat table {
    width: 100%;
    border-collapse: collapse;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.82rem;
  }

  #sec-cheat thead tr {
    background: rgba(255,255,255,0.03);
  }

  #sec-cheat thead th {
    padding: 12px 14px;
    text-align: center;
    font-family: 'DM Sans', sans-serif;
    font-size: 0.7rem;
    letter-spacing: 2px;
    text-transform: uppercase;
    font-weight: 500;
    color: var(--muted);
    border-bottom: 1px solid var(--border);
  }

  #sec-cheat tbody tr {
    border-bottom: 1px solid rgba(30,45,74,0.6);
    transition: background 0.15s;
  }

  #sec-cheat tbody tr:last-child { border-bottom: none; }
  #sec-cheat tbody tr:hover { background: rgba(255,255,255,0.025); }

  #sec-cheat tbody td {
    padding: 10px 14px;
    text-align: center;
    vertical-align: middle;
  }

  #sec-cheat .n { color: var(--blue); font-weight: 600; font-size: 0.9rem; }
  #sec-cheat .sq { color: var(--gold); }
  #sec-cheat .cb { color: var(--rose); }
  #sec-cheat .sqr { color: var(--teal); }
  #sec-cheat .cbr { color: var(--lavender); }

  #sec-cheat .highlight-row { background: rgba(245,200,66,0.04) !important; }

  /* GRID LAYOUT */
  #sec-cheat .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }

  @media (max-width: 640px) {
    #sec-cheat .grid-2 { grid-template-columns: 1fr; }
  }

  /* FRACTIONS */
  #sec-cheat .frac-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(130px, 1fr));
    gap: 1px;
    background: var(--border);
    border-radius: 14px;
    overflow: hidden;
  }

  #sec-cheat .frac-cell {
    background: var(--card);
    padding: 14px 12px;
    text-align: center;
    transition: background 0.15s;
  }

  #sec-cheat .frac-cell:hover { background: rgba(255,255,255,0.04); }

  #sec-cheat .frac-top {
    font-family: 'JetBrains Mono', monospace;
    font-size: 1.1rem;
    font-weight: 600;
    color: var(--gold);
    display: block;
  }

  #sec-cheat .frac-denom {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.7rem;
    color: var(--muted);
    display: block;
    margin-top: 2px;
  }

  #sec-cheat .frac-decimal {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    color: var(--teal);
    display: block;
    margin-top: 6px;
  }

  #sec-cheat .frac-bar {
    width: 40px;
    height: 1px;
    background: var(--border);
    margin: 4px auto;
  }

  /* SURDS */
  #sec-cheat .surd-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
    gap: 1px;
    background: var(--border);
    border-radius: 14px;
    overflow: hidden;
  }

  #sec-cheat .surd-cell {
    background: var(--card);
    padding: 16px 12px;
    text-align: center;
  }

  #sec-cheat .surd-expr {
    font-family: 'JetBrains Mono', monospace;
    font-size: 1rem;
    font-weight: 600;
    color: var(--lavender);
  }

  #sec-cheat .surd-val {
    font-family: 'JetBrains Mono', monospace;
    font-size: 1rem;
    color: var(--teal);
    margin-top: 8px;
  }

  /* POWERS */
  #sec-cheat .pow-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
  }

  #sec-cheat .pow-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    overflow: hidden;
  }

  #sec-cheat .pow-header {
    padding: 10px 16px;
    font-family: 'DM Sans', sans-serif;
    font-size: 0.72rem;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--muted);
    border-bottom: 1px solid var(--border);
    background: rgba(255,255,255,0.02);
  }

  #sec-cheat .pow-row {
    display: flex;
    justify-content: space-between;
    padding: 8px 16px;
    border-bottom: 1px solid rgba(30,45,74,0.5);
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.82rem;
  }

  #sec-cheat .pow-row:last-child { border-bottom: none; }
  #sec-cheat .pow-exp { color: var(--muted); }
  #sec-cheat .pow-val-blue { color: var(--blue); font-weight: 600; }
  #sec-cheat .pow-val-rose { color: var(--rose); font-weight: 600; }

  /* FOOTER */
  #sec-cheat .footer {
    text-align: center;
    margin-top: 40px;
    padding-top: 24px;
    border-top: 1px solid var(--border);
    color: var(--muted);
    font-size: 0.75rem;
    letter-spacing: 1.5px;
    text-transform: uppercase;
  }

  #sec-cheat .badge {
    display: inline-block;
    margin-top: 8px;
    padding: 4px 16px;
    border-radius: 20px;
    background: rgba(245,200,66,0.08);
    color: var(--gold);
    font-size: 0.7rem;
    border: 1px solid rgba(245,200,66,0.15);
  }

  #sec-cheat sup { font-size: 0.65em; }

</style>
<!-- ConicLab Styles -->
<style>

#sec-conic, #sec-conic * {
  --bg:#080b10; --panel:#0d1018; --panel2:#11151e; --panel3:#161c28;
  --border:#1e2535; --border2:#252d3d; --border3:#2e3850;
  --gold:#f0c060; --gold2:#c89030; --gold3:#f8d888;
  --teal:#40d0c0; --rose:#f06080; --violet:#a080f0;
  --sky:#60b8f0; --green:#50d890; --orange:#f08040;
  --text:#e8e0d0; --text2:#8090a8; --text3:#404e66;
  --sidebar-w: 310px;
}

/* ConicLab shell overrides — scoped so body can scroll */
#conic-inner{-webkit-tap-highlight-color:transparent;}

/* ══ LAYOUT ══ */
#sec-conic #app{display:flex;height:100vh;position:relative;}
#sec-conic #canvas-wrap{position:absolute;inset:0;overflow:hidden;background:var(--bg);}
#sec-conic canvas{display:block;cursor:crosshair;}

/* ══ SIDEBAR OVERLAY ══ */
#sidebar{
  position:absolute; left:0; top:0; bottom:0; width:var(--sidebar-w);
  background:rgba(13,16,24,0.97); border-right:1px solid var(--border2);
  display:flex; flex-direction:column; z-index:50;
  transform:translateX(0); transition:transform 0.3s cubic-bezier(.4,0,.2,1);
  backdrop-filter:blur(16px); -webkit-backdrop-filter:blur(16px);
  box-shadow: 4px 0 32px rgba(0,0,0,0.6);
}
#sidebar.hidden{transform:translateX(calc(-100% - 4px));}

/* ══ TOGGLE TAB ══ */
#sidebar-toggle{
  position:absolute; top:50%; right:-36px; transform:translateY(-50%);
  width:36px; height:72px; background:rgba(13,16,24,0.95);
  border:1px solid var(--border2); border-left:none;
  border-radius:0 8px 8px 0; cursor:pointer; z-index:51;
  display:flex; align-items:center; justify-content:center;
  flex-direction:column; gap:3px;
  backdrop-filter:blur(8px); transition:background 0.2s, border-color 0.2s;
}
#sidebar-toggle:hover{background:rgba(240,192,96,0.1);border-color:var(--gold2);}
#sidebar-toggle span{width:14px;height:2px;background:var(--text2);border-radius:1px;transition:background 0.2s;}
#sidebar-toggle:hover span{background:var(--gold);}
#toggle-arrow{font-size:0.7rem;color:var(--text2);transition:transform 0.3s, color 0.2s;line-height:1;}
#sidebar.hidden #toggle-arrow{transform:scaleX(-1);}
#sidebar-toggle:hover #toggle-arrow{color:var(--gold);}

/* ══ HEADER ══ */
#hdr{padding:12px 14px 8px;border-bottom:1px solid var(--border);background:var(--panel2);flex-shrink:0;}
#hdr h1{font-family:'Syne',sans-serif;font-size:1rem;font-weight:800;color:var(--gold);letter-spacing:0.06em;}
#hdr p{font-size:0.58rem;color:var(--text3);margin-top:1px;letter-spacing:0.12em;}

/* ══ TABS ══ */
#tabs{display:flex;border-bottom:1px solid var(--border);flex-shrink:0;}
.tab{flex:1;padding:7px 0;font-size:0.6rem;letter-spacing:0.1em;text-transform:uppercase;text-align:center;cursor:pointer;color:var(--text3);border-bottom:2px solid transparent;transition:all .2s;}
.tab.active{color:var(--gold);border-bottom-color:var(--gold);background:rgba(240,192,96,0.04);}
.tab:hover:not(.active){color:var(--text2);}

/* ══ SCROLL BODY ══ */
#panel-body {flex:1;overflow-y:auto;padding:10px 10px 70px;scrollbar-width:thin;scrollbar-color:var(--border2) transparent;}
#panel-body::-webkit-scrollbar{width:3px;}
#panel-body::-webkit-scrollbar-thumb{background:var(--border2);border-radius:2px;}

/* ══ ADD ROW ══ */
.add-row{display:flex;gap:5px;margin-bottom:10px;}
.add-row select{flex:1;background:var(--panel2);border:1px solid var(--border2);color:var(--text);padding:6px 8px;border-radius:4px;cursor:pointer;font-family:'JetBrains Mono',monospace;font-size:0.66rem;}
.add-row select:focus{outline:none;border-color:var(--gold2);}
.btn-add{background:var(--gold2);color:#000;border:none;padding:6px 10px;border-radius:4px;font-weight:700;cursor:pointer;font-size:0.68rem;font-family:'JetBrains Mono',monospace;white-space:nowrap;transition:background .15s;}
.btn-add:hover{background:var(--gold);}

/* ══ CURVE ITEM ══ */
.ci{background:var(--panel2);border:1px solid var(--border);border-radius:6px;margin-bottom:7px;overflow:hidden;transition:border-color .2s;}
.ci:hover{border-color:var(--border2);}
.ci.sel{border-color:var(--gold2)!important;box-shadow:0 0 0 1px rgba(240,192,96,0.15);}
.ci-head{display:flex;align-items:center;gap:7px;padding:7px 9px;cursor:pointer;user-select:none;}
.ci-dot{width:9px;height:9px;border-radius:50%;flex-shrink:0;box-shadow:0 0 6px currentColor;}
.ci-name{flex:1;font-size:0.7rem;color:var(--text);overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
.ci-badge{font-size:0.54rem;letter-spacing:0.06em;text-transform:uppercase;padding:2px 4px;border-radius:2px;background:rgba(255,255,255,0.04);color:var(--text3);flex-shrink:0;}
.btn-del{background:none;border:none;color:var(--text3);cursor:pointer;font-size:0.8rem;padding:0 2px;line-height:1;flex-shrink:0;}
.btn-del:hover{color:var(--rose);}
.ci-body {padding:8px 10px 10px;border-top:1px solid var(--border);display:none;}
.ci.open .ci-body {display:block;}
.chev{font-size:0.55rem;color:var(--text3);transition:transform .2s;flex-shrink:0;}
.ci.open .chev{transform:rotate(180deg);}

/* ══ SECTION LABEL ══ */
.slbl{font-size:0.55rem;letter-spacing:0.15em;text-transform:uppercase;color:var(--text3);margin:8px 0 5px;padding-bottom:3px;border-bottom:1px solid var(--border);}

/* ══ PARAM ROW — UNIFIED WITH DIRECT INPUT ══ */
.prow{display:grid;grid-template-columns:58px 1fr 62px;align-items:center;gap:5px;margin-bottom:5px;}
.prow label{font-size:0.6rem;color:var(--text3);overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
.prow input[type=range]{width:100%;accent-color:var(--gold);height:3px;cursor:pointer;background:var(--border2);}
.prow .pval{font-family:'JetBrains Mono',monospace;font-size:0.65rem;color:var(--text);background:#07090e;border:1px solid var(--border2);padding:3px 5px;border-radius:3px;width:100%;text-align:right;}
.prow .pval:focus{outline:none;border-color:var(--gold2);color:var(--gold3);}

/* ══ EQN INPUT ══ */
.eqn-box{background:#06080d;border:1px solid var(--border2);border-radius:4px;padding:6px 8px;margin:5px 0;display:flex;flex-direction:column;gap:4px;}
.eqn-box label{font-size:0.56rem;color:var(--gold2);letter-spacing:0.1em;text-transform:uppercase;}
.eqn-input{font-family:'JetBrains Mono',monospace;font-size:0.7rem;color:var(--teal);background:transparent;border:none;outline:none;width:100%;caret-color:var(--teal);}
.eqn-input::placeholder{color:var(--text3);}
.eqn-apply{font-family:'JetBrains Mono',monospace;font-size:0.6rem;background:rgba(64,208,192,0.12);color:var(--teal);border:1px solid rgba(64,208,192,0.25);padding:3px 8px;border-radius:3px;cursor:pointer;margin-top:2px;width:fit-content;}
.eqn-apply:hover{background:rgba(64,208,192,0.22);}
.eqn-err{font-size:0.6rem;color:var(--rose);display:none;margin-top:2px;}

/* ══ SWATCH ══ */
.swatch-row{display:flex;gap:4px;flex-wrap:wrap;margin-bottom:6px;}
.sw{width:17px;height:17px;border-radius:3px;cursor:pointer;border:2px solid transparent;transition:border-color .12s;}
.sw.active{border-color:#fff!important;}

/* ══ CHECK ROW ══ */
.crow{display:flex;align-items:center;gap:5px;margin-bottom:4px;}
.crow label{font-size:0.62rem;color:var(--text2);cursor:pointer;}
.crow input[type=checkbox]{accent-color:var(--gold);cursor:pointer;}

/* ══ TAN ROW ══ */
.trow{display:flex;gap:5px;align-items:center;margin-bottom:4px;}
.trow label{font-size:0.6rem;color:var(--text3);width:50px;flex-shrink:0;}
.trow input{flex:1;background:#07090e;border:1px solid var(--border2);color:var(--text);padding:4px 6px;border-radius:3px;font-family:'JetBrains Mono',monospace;font-size:0.66rem;}
.trow input:focus{outline:none;border-color:var(--teal);}
.tbtn{font-family:'JetBrains Mono',monospace;font-size:0.6rem;padding:4px 8px;border-radius:3px;cursor:pointer;border:1px solid;transition:all .15s;white-space:nowrap;}
.tbtn.teal{background:rgba(64,208,192,0.1);color:var(--teal);border-color:rgba(64,208,192,0.25);}
.tbtn.teal:hover{background:rgba(64,208,192,0.2);}
.tbtn.rose{background:rgba(240,96,128,0.1);color:var(--rose);border-color:rgba(240,96,128,0.25);}
.tbtn.rose:hover{background:rgba(240,96,128,0.2);}

/* ══ CANVAS TOOLBAR (floating) ══ */
#ctoolbar{
  position:absolute;bottom:16px;left:50%;transform:translateX(-50%);
  display:flex;gap:6px;z-index:20;
  background:rgba(13,16,24,0.92);border:1px solid var(--border2);
  border-radius:40px;padding:6px 10px;
  backdrop-filter:blur(12px);box-shadow:0 4px 24px rgba(0,0,0,0.5);
  transition:left 0.3s, transform 0.3s;
}
#sidebar:not(.hidden) ~ #ctoolbar-anchor #ctoolbar{left:calc(50% + var(--sidebar-w)/2);}
.ctb{background:none;border:none;cursor:pointer;font-size:1rem;padding:4px 6px;border-radius:20px;transition:background .15s;color:var(--text2);font-family:'JetBrains Mono',monospace;font-size:0.7rem;display:flex;align-items:center;gap:4px;}
.ctb:hover{background:rgba(255,255,255,0.07);color:var(--text);}
.ctb.active{background:rgba(240,192,96,0.15);color:var(--gold);}
.ctb-sep{width:1px;height:20px;background:var(--border);align-self:center;}

/* ══ DRAW MODE INDICATOR ══ */
#draw-indicator{
  position:absolute;top:12px;left:50%;transform:translateX(-50%);
  background:rgba(240,192,96,0.12);border:1px solid rgba(240,192,96,0.3);
  color:var(--gold);font-size:0.62rem;letter-spacing:0.1em;
  padding:5px 14px;border-radius:20px;display:none;z-index:20;
  backdrop-filter:blur(8px);pointer-events:none;
}

/* ══ COORD DISPLAY ══ */
#coord-bar{
  position:absolute;top:12px;right:12px;
  background:rgba(13,16,24,0.85);border:1px solid var(--border2);
  padding:5px 10px;border-radius:5px;font-size:0.6rem;color:var(--text2);
  backdrop-filter:blur(8px);z-index:20;line-height:1.7;
  transition:right 0.3s;
}

/* ══ CANVAS ZOOM BTNS ══ */
#zoom-btns{position:absolute;right:12px;top:50%;transform:translateY(-50%);display:flex;flex-direction:column;gap:5px;z-index:20;}
.zbtn{width:30px;height:30px;background:rgba(13,16,24,0.88);border:1px solid var(--border2);color:var(--text2);border-radius:5px;cursor:pointer;font-size:0.85rem;display:flex;align-items:center;justify-content:center;transition:all .15s;backdrop-filter:blur(6px);}
.zbtn:hover{border-color:var(--gold2);color:var(--gold);}

/* ══ HELP / SETTINGS TABS ══ */
#tab-settings,#tab-help{overflow-y:auto;padding:12px;display:none;flex:1;}
.sg{margin-bottom:14px;}
.sg h4{font-size:0.58rem;letter-spacing:0.15em;text-transform:uppercase;color:var(--text3);margin-bottom:7px;}
.srow{display:flex;align-items:center;gap:8px;margin-bottom:5px;}
.srow label{font-size:0.63rem;color:var(--text2);flex:1;}
.srow input[type=range]{width:80px;accent-color:var(--gold);}
.srow span{font-size:0.63rem;color:var(--gold);width:28px;text-align:right;}
.srow input[type=checkbox]{accent-color:var(--gold);}

/* ══ EMPTY HINT ══ */
#empty-hint{text-align:center;padding:24px 8px;color:var(--text3);font-size:0.65rem;line-height:1.9;}
#empty-hint .ico{font-size:2rem;margin-bottom:8px;}

/* ══ STATUS ══ */
#statusbar{padding:6px 12px;border-top:1px solid var(--border);background:var(--panel2);font-size:0.58rem;color:var(--text3);display:flex;justify-content:space-between;flex-shrink:0;}

/* ══ TOOLTIP ══ */
#tip{position:absolute;background:rgba(13,16,24,0.96);border:1px solid var(--border2);padding:4px 8px;border-radius:4px;font-size:0.6rem;color:var(--text);pointer-events:none;display:none;z-index:99;backdrop-filter:blur(6px);}

/* ══ DRAW GHOST ══ */
#draw-ghost{position:absolute;top:8px;left:50%;transform:translateX(-50%);font-size:0.6rem;color:var(--gold);letter-spacing:0.08em;pointer-events:none;display:none;}

</style>
</head>
<body>

<section id="hero">
  <div class="hero-grid"></div>
  <div class="hero-orb"></div><div class="hero-orb"></div><div class="hero-orb"></div>
  <div class="hero-ring"></div><div class="hero-ring"></div><div class="hero-ring"></div>
  <div class="hero-content">
    <div class="hero-eyebrow">JEE Advanced &amp; Mains &nbsp;·&nbsp; Complete Reference</div>
    <h1>
      <span class="h1-line1">JEE</span>
      <span class="h1-line2">Master Reference</span>
      <span class="h1-line3">Mathematics &amp; Science</span>
    </h1>
    <p class="hero-sub">Every formula, proof, diagram &amp; interactive tool in one place —<br>
    Trigonometry · Coord Geometry · ConicLab · Constants · Periodic Table · Rotational Dynamics · Thermodynamics · Ionic Equilibrium</p>
    <div class="hero-modules">
      <div class="hmod" style="--mc:#e8c060" onclick="showSection('trig')"><div class="hmod-icon">∿</div><div class="hmod-title">Trigonometry</div><div class="hmod-tag">9 sections · proofs</div></div>
      <div class="hmod" style="--mc:#40d0c0" onclick="showSection('coord')"><div class="hmod-icon">⬡</div><div class="hmod-title">Coord Geometry</div><div class="hmod-tag">8 sections · SVGs</div></div>
      <div class="hmod" style="--mc:#a080f0" onclick="showSection('conic')"><div class="hmod-icon">🔭</div><div class="hmod-title">ConicLab</div><div class="hmod-tag">interactive grapher</div></div>
      <div class="hmod" style="--mc:#22d3ee" onclick="showSection('const')"><div class="hmod-icon">⚛</div><div class="hmod-title">Constants &amp; Logs</div><div class="hmod-tag">physics · chemistry</div></div>
      <div class="hmod" style="--mc:#f5c842" onclick="showSection('cheat')"><div class="hmod-icon">🔢</div><div class="hmod-title">Math Tables</div><div class="hmod-tag">squares · roots</div></div>
      <div class="hmod" style="--mc:#f08040" onclick="showSection('calc')"><div class="hmod-icon">🧮</div><div class="hmod-title">Calculator</div><div class="hmod-tag">scientific · full</div></div>
      <div class="hmod" style="--mc:#50e890" onclick="showSection('ptable')"><div class="hmod-icon">⚗️</div><div class="hmod-title">Periodic Table</div><div class="hmod-tag">interactive · JEE</div></div>
      <div class="hmod" style="--mc:#ff6b35" onclick="showSection('rotdyn')"><div class="hmod-icon">🌀</div><div class="hmod-title">Rotational Dynamics</div><div class="hmod-tag">JEE Advanced · animated</div></div>
      <div class="hmod" style="--mc:#e05aff" onclick="showSection('thermo')"><div class="hmod-icon">🔥</div><div class="hmod-title">Thermodynamics</div><div class="hmod-tag">Physical Chem · JEE</div></div>
      <div class="hmod" style="--mc:#22eea8" onclick="showSection('ionic')"><div class="hmod-icon">⚖️</div><div class="hmod-title">Ionic Equilibrium</div><div class="hmod-tag">pH · buffers · JEE</div></div>
    </div>
    <div class="hero-hint">▼ &nbsp; TAP A MODULE &nbsp; ▼</div>
  </div>
</section>

<div id="topnav">
  <div class="nav-brand" onclick="showSection('hero')"><span class="nav-brand-dot"></span>⬡ JEE</div>
  <div data-sec="trig" class="ntab active" id="nav-trig" style="--tc:#e8c060" onclick="showSection('trig')"><span class="ntab-icon">∿</span>Trig</div>
  <div data-sec="coord" class="ntab" id="nav-coord" style="--tc:#40d0c0" onclick="showSection('coord')"><span class="ntab-icon">📐</span>Coord</div>
  <div data-sec="conic" class="ntab" id="nav-conic" style="--tc:#a080f0" onclick="showSection('conic')"><span class="ntab-icon">🔭</span>ConicLab</div>
  <div data-sec="const" class="ntab" id="nav-const" style="--tc:#22d3ee" onclick="showSection('const')"><span class="ntab-icon">⚛</span>Constants</div>
  <div data-sec="cheat" class="ntab" id="nav-cheat" style="--tc:#f5c842" onclick="showSection('cheat')"><span class="ntab-icon">🔢</span>Tables</div>
  <div data-sec="calc" class="ntab" id="nav-calc" style="--tc:#f08040" onclick="showSection('calc')"><span class="ntab-icon">🧮</span>Calc</div>
  <div data-sec="desmos" class="ntab" id="nav-desmos" style="--tc:#50d890" onclick="showSection('desmos')"><span class="ntab-icon">📈</span>Desmos</div>
  <div data-sec="ptable" class="ntab" id="nav-ptable" style="--tc:#50e890" onclick="showSection('ptable')"><span class="ntab-icon">⚗️</span>Periodic Table</div>
  <div data-sec="rotdyn" class="ntab" id="nav-rotdyn" style="--tc:#ff6b35" onclick="showSection('rotdyn')"><span class="ntab-icon">🌀</span>Rot Dynamics</div>
  <div data-sec="thermo" class="ntab" id="nav-thermo" style="--tc:#e05aff" onclick="showSection('thermo')"><span class="ntab-icon">🔥</span>Thermo</div>
  <div data-sec="ionic" class="ntab" id="nav-ionic" style="--tc:#22eea8" onclick="showSection('ionic')"><span class="ntab-icon">⚖️</span>Ionic Eq</div>
</div>

<div id="proof-overlay">
  <div id="proof-box">
    <div id="proof-hdr">
      <div><span id="proof-tag">PROOF &amp; DERIVATION</span><div id="proof-title">—</div></div>
      <button id="proof-close">✕</button>
    </div>
    <div id="proof-body"></div>
  </div>
</div>
<div class="psec active" id="sec-trig"><div class="cwrap"><div class="shero" style="--sc:rgba(232,192,96,.08)"><span class="shero-badge">01 — JEE Advanced &amp; Mains</span><h2 style="color:#e8c060">Trigonometry</h2><p>All formulas with step-by-step proofs · click any card · interactive graphs</p><div class="snav"><a href="#s1">Basics</a><a href="#s2">Identities</a><a href="#s3">Compound</a><a href="#s4">Multiple</a><a href="#s5">Product</a><a href="#s6">Graphs</a><a href="#s7">Inverse</a><a href="#s8">Equations</a><a href="#s9">Results</a></div></div><div class="trig-wrap">

<!-- ═══ 01 BASICS ═══ -->
<section class="sec" id="s1"><div class="wrap">
  <div class="sh"><span class="sn">01 —</span><h2>Basic Definitions &amp; Ratios</h2></div>
  <h3>Six Trigonometric Ratios</h3>
  <div class="fg">
    <div class="fb" data-p="sin-def"><div class="fl">Sine<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sin</span>(θ) <span class="e">=</span> <span class="v">Opposite</span> <span class="o">/</span> <span class="v">Hypotenuse</span></div></div>
    <div class="fb" data-p="cos-def"><div class="fl">Cosine<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cos</span>(θ) <span class="e">=</span> <span class="v">Adjacent</span> <span class="o">/</span> <span class="v">Hypotenuse</span></div></div>
    <div class="fb" data-p="tan-def"><div class="fl">Tangent<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">tan</span>(θ) <span class="e">=</span> <span class="v">sin θ</span> <span class="o">/</span> <span class="v">cos θ</span></div></div>
    <div class="fb" data-p="cosec-def"><div class="fl">Cosecant<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cosec</span>(θ) <span class="e">=</span> <span class="n">1</span> <span class="o">/</span> <span class="f">sin</span>(θ)</div></div>
    <div class="fb" data-p="sec-def"><div class="fl">Secant<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sec</span>(θ) <span class="e">=</span> <span class="n">1</span> <span class="o">/</span> <span class="f">cos</span>(θ)</div></div>
    <div class="fb" data-p="cot-def"><div class="fl">Cotangent<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cot</span>(θ) <span class="e">=</span> <span class="f">cos</span>(θ) <span class="o">/</span> <span class="f">sin</span>(θ)</div></div>
  </div>
  <h3>Standard Angles Table</h3>
  <table class="atbl">
    <thead><tr><th>Angle</th><th>Radians</th><th>sin</th><th>cos</th><th>tan</th><th>cosec</th><th>sec</th><th>cot</th></tr></thead>
    <tbody>
      <tr><td>0°</td><td>0</td><td>0</td><td>1</td><td>0</td><td>∞</td><td>1</td><td>∞</td></tr>
      <tr><td>30°</td><td>π/6</td><td>1/2</td><td>√3/2</td><td>1/√3</td><td>2</td><td>2/√3</td><td>√3</td></tr>
      <tr><td>45°</td><td>π/4</td><td>1/√2</td><td>1/√2</td><td>1</td><td>√2</td><td>√2</td><td>1</td></tr>
      <tr><td>60°</td><td>π/3</td><td>√3/2</td><td>1/2</td><td>√3</td><td>2/√3</td><td>2</td><td>1/√3</td></tr>
      <tr><td>90°</td><td>π/2</td><td>1</td><td>0</td><td>∞</td><td>1</td><td>∞</td><td>0</td></tr>
      <tr><td>120°</td><td>2π/3</td><td>√3/2</td><td>−1/2</td><td>−√3</td><td>2/√3</td><td>−2</td><td>−1/√3</td></tr>
      <tr><td>135°</td><td>3π/4</td><td>1/√2</td><td>−1/√2</td><td>−1</td><td>√2</td><td>−√2</td><td>−1</td></tr>
      <tr><td>150°</td><td>5π/6</td><td>1/2</td><td>−√3/2</td><td>−1/√3</td><td>2</td><td>−2/√3</td><td>−√3</td></tr>
      <tr><td>180°</td><td>π</td><td>0</td><td>−1</td><td>0</td><td>∞</td><td>−1</td><td>∞</td></tr>
      <tr><td>270°</td><td>3π/2</td><td>−1</td><td>0</td><td>∞</td><td>−1</td><td>∞</td><td>0</td></tr>
      <tr><td>360°</td><td>2π</td><td>0</td><td>1</td><td>0</td><td>∞</td><td>1</td><td>∞</td></tr>
    </tbody>
  </table>
  <div class="nb"><strong>MEMORY TRICK — sin values 0°→90°</strong>sin = √0/2, √1/2, √2/2, √3/2, √4/2 &nbsp;=&nbsp; 0, 1/2, 1/√2, √3/2, 1<br>cos = reverse of sin &nbsp;|&nbsp; tan = sin/cos</div>
  <h3>ASTC Rule — Signs by Quadrant</h3>
  <div class="fg">
    <div class="fb" data-p="q1"><div class="fl">Q-I (0°–90°)<span class="ph">PROOF ▸</span></div><div class="fm gr">All ratios positive</div></div>
    <div class="fb" data-p="q2"><div class="fl">Q-II (90°–180°)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="g">sin, cosec</span> positive; rest negative</div></div>
    <div class="fb" data-p="q3"><div class="fl">Q-III (180°–270°)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="pk">tan, cot</span> positive; rest negative</div></div>
    <div class="fb" data-p="q4"><div class="fl">Q-IV (270°–360°)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="bl">cos, sec</span> positive; rest negative</div></div>
  </div>
</div></section>

<!-- ═══ 02 IDENTITIES ═══ -->
<section class="sec" id="s2"><div class="wrap">
  <div class="sh"><span class="sn">02 —</span><h2>Fundamental Identities</h2></div>
  <h3>Pythagorean Identities</h3>
  <div class="fg">
    <div class="fb" data-p="py1"><div class="fl">Primary<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sin²θ</span> <span class="o">+</span> <span class="f">cos²θ</span> <span class="e">=</span> <span class="n">1</span></div></div>
    <div class="fb" data-p="py2"><div class="fl">÷ cos²θ<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">1</span> <span class="o">+</span> <span class="f">tan²θ</span> <span class="e">=</span> <span class="f">sec²θ</span></div></div>
    <div class="fb" data-p="py3"><div class="fl">÷ sin²θ<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">1</span> <span class="o">+</span> <span class="f">cot²θ</span> <span class="e">=</span> <span class="f">cosec²θ</span></div></div>
  </div>
  <h3>Allied / Negative Angle Identities</h3>
  <h4>−θ (Odd / Even)</h4>
  <div class="flist">
    <div class="fi" data-p="n-sin"><span><span class="lhs">sin(−θ)</span><span class="sep">=</span><span class="rhs">−sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="n-cos"><span><span class="lhs">cos(−θ)</span><span class="sep">=</span><span class="rhs">+cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="n-tan"><span><span class="lhs">tan(−θ)</span><span class="sep">=</span><span class="rhs">−tan θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="n-cosec"><span><span class="lhs">cosec(−θ)</span><span class="sep">=</span><span class="rhs">−cosec θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="n-sec"><span><span class="lhs">sec(−θ)</span><span class="sep">=</span><span class="rhs">+sec θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="n-cot"><span><span class="lhs">cot(−θ)</span><span class="sep">=</span><span class="rhs">−cot θ</span></span><span class="fph">PROOF ▸</span></div>
  </div>
  <h4>90° − θ (Cofunction)</h4>
  <div class="flist">
    <div class="fi" data-p="c90m-sin"><span><span class="lhs">sin(90°−θ)</span><span class="sep">=</span><span class="rhs">cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90m-cos"><span><span class="lhs">cos(90°−θ)</span><span class="sep">=</span><span class="rhs">sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90m-tan"><span><span class="lhs">tan(90°−θ)</span><span class="sep">=</span><span class="rhs">cot θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90m-csc"><span><span class="lhs">cosec(90°−θ)</span><span class="sep">=</span><span class="rhs">sec θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90m-sec"><span><span class="lhs">sec(90°−θ)</span><span class="sep">=</span><span class="rhs">cosec θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90m-cot"><span><span class="lhs">cot(90°−θ)</span><span class="sep">=</span><span class="rhs">tan θ</span></span><span class="fph">PROOF ▸</span></div>
  </div>
  <h4>90°+θ, 180°±θ, 360°±θ</h4>
  <div class="flist">
    <div class="fi" data-p="a90p"><span><span class="lhs">sin(90°+θ)</span><span class="sep">=</span><span class="rhs">+cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="b90p"><span><span class="lhs">cos(90°+θ)</span><span class="sep">=</span><span class="rhs">−sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c90p"><span><span class="lhs">tan(90°+θ)</span><span class="sep">=</span><span class="rhs">−cot θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="a180m"><span><span class="lhs">sin(180°−θ)</span><span class="sep">=</span><span class="rhs">+sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="b180m"><span><span class="lhs">cos(180°−θ)</span><span class="sep">=</span><span class="rhs">−cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c180m"><span><span class="lhs">tan(180°−θ)</span><span class="sep">=</span><span class="rhs">−tan θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="a180p"><span><span class="lhs">sin(180°+θ)</span><span class="sep">=</span><span class="rhs">−sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="b180p"><span><span class="lhs">cos(180°+θ)</span><span class="sep">=</span><span class="rhs">−cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c180p"><span><span class="lhs">tan(180°+θ)</span><span class="sep">=</span><span class="rhs">+tan θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="a360m"><span><span class="lhs">sin(360°−θ)</span><span class="sep">=</span><span class="rhs">−sin θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="b360m"><span><span class="lhs">cos(360°−θ)</span><span class="sep">=</span><span class="rhs">+cos θ</span></span><span class="fph">PROOF ▸</span></div>
    <div class="fi" data-p="c360m"><span><span class="lhs">tan(360°−θ)</span><span class="sep">=</span><span class="rhs">−tan θ</span></span><span class="fph">PROOF ▸</span></div>
  </div>
</div></section>

<!-- ═══ 03 COMPOUND ═══ -->
<section class="sec" id="s3"><div class="wrap">
  <div class="sh"><span class="sn">03 —</span><h2>Compound Angle Formulas</h2></div>
  <h3>Addition &amp; Subtraction</h3>
  <div class="fg">
    <div class="fb" data-p="sin-add"><div class="fl">sin(A+B)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sinA cosB</span> <span class="o">+</span> <span class="f">cosA sinB</span></div></div>
    <div class="fb" data-p="sin-sub"><div class="fl">sin(A−B)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sinA cosB</span> <span class="o">−</span> <span class="f">cosA sinB</span></div></div>
    <div class="fb" data-p="cos-add"><div class="fl">cos(A+B)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cosA cosB</span> <span class="o">−</span> <span class="f">sinA sinB</span></div></div>
    <div class="fb" data-p="cos-sub"><div class="fl">cos(A−B)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cosA cosB</span> <span class="o">+</span> <span class="f">sinA sinB</span></div></div>
    <div class="fb" data-p="tan-add"><div class="fl">tan(A+B)<span class="ph">PROOF ▸</span></div><div class="fm">(<span class="f">tanA</span><span class="o">+</span><span class="f">tanB</span>) / (<span class="n">1</span><span class="o">−</span><span class="f">tanA tanB</span>)</div></div>
    <div class="fb" data-p="tan-sub"><div class="fl">tan(A−B)<span class="ph">PROOF ▸</span></div><div class="fm">(<span class="f">tanA</span><span class="o">−</span><span class="f">tanB</span>) / (<span class="n">1</span><span class="o">+</span><span class="f">tanA tanB</span>)</div></div>
    <div class="fb" data-p="cot-add"><div class="fl">cot(A+B)<span class="ph">PROOF ▸</span></div><div class="fm">(<span class="f">cotA cotB</span><span class="o">−1</span>) / (<span class="f">cotA</span><span class="o">+</span><span class="f">cotB</span>)</div></div>
    <div class="fb" data-p="cot-sub"><div class="fl">cot(A−B)<span class="ph">PROOF ▸</span></div><div class="fm">(<span class="f">cotA cotB</span><span class="o">+1</span>) / (<span class="f">cotB</span><span class="o">−</span><span class="f">cotA</span>)</div></div>
  </div>
  <h3>Sum-to-Product</h3>
  <div class="fg">
    <div class="fb" data-p="s2p-sp"><div class="fl">sinC + sinD<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">2</span> <span class="f">sin</span>((C+D)/2) <span class="f">cos</span>((C−D)/2)</div></div>
    <div class="fb" data-p="s2p-sm"><div class="fl">sinC − sinD<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">2</span> <span class="f">cos</span>((C+D)/2) <span class="f">sin</span>((C−D)/2)</div></div>
    <div class="fb" data-p="s2p-cp"><div class="fl">cosC + cosD<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">2</span> <span class="f">cos</span>((C+D)/2) <span class="f">cos</span>((C−D)/2)</div></div>
    <div class="fb" data-p="s2p-cm"><div class="fl">cosC − cosD<span class="ph">PROOF ▸</span></div><div class="fm"><span class="o">−</span><span class="n">2</span> <span class="f">sin</span>((C+D)/2) <span class="f">sin</span>((C−D)/2)</div></div>
  </div>
</div></section>

<!-- ═══ 04 MULTIPLE ANGLES ═══ -->
<section class="sec" id="s4"><div class="wrap">
  <div class="sh"><span class="sn">04 —</span><h2>Multiple &amp; Sub-Multiple Angles</h2></div>
  <h3>Double Angle</h3>
  <div class="fg">
    <div class="fb" data-p="sin2a"><div class="fl">sin 2A<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">2</span><span class="f">sinA cosA</span> <span class="e">=</span> <span class="n">2</span><span class="f">tanA</span>/(<span class="n">1+tan²A</span>)</div></div>
    <div class="fb" data-p="cos2a"><div class="fl">cos 2A (4 forms)<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cos²A−sin²A</span><br><span class="e">=</span> <span class="n">1−2sin²A</span> <span class="e">=</span> <span class="n">2cos²A−1</span><br><span class="e">=</span> (1−tan²A)/(1+tan²A)</div></div>
    <div class="fb" data-p="tan2a"><div class="fl">tan 2A<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">2</span><span class="f">tanA</span> / (<span class="n">1</span><span class="o">−</span><span class="f">tan²A</span>)</div></div>
    <div class="fb" data-p="sq-forms"><div class="fl">sin²A and cos²A<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sin²A</span> = (1−cos2A)/2<br><span class="f">cos²A</span> = (1+cos2A)/2</div></div>
  </div>
  <h3>Triple Angle</h3>
  <div class="fg">
    <div class="fb" data-p="sin3a"><div class="fl">sin 3A<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">3</span><span class="f">sinA</span> <span class="o">−</span> <span class="n">4</span><span class="f">sin³A</span></div></div>
    <div class="fb" data-p="cos3a"><div class="fl">cos 3A<span class="ph">PROOF ▸</span></div><div class="fm"><span class="n">4</span><span class="f">cos³A</span> <span class="o">−</span> <span class="n">3</span><span class="f">cosA</span></div></div>
    <div class="fb" data-p="tan3a"><div class="fl">tan 3A<span class="ph">PROOF ▸</span></div><div class="fm">(<span class="n">3</span><span class="f">tanA</span><span class="o">−</span><span class="f">tan³A</span>) / (<span class="n">1</span><span class="o">−</span><span class="n">3</span><span class="f">tan²A</span>)</div></div>
  </div>
  <h3>Half-Angle</h3>
  <div class="fg">
    <div class="fb" data-p="h-sin"><div class="fl">sin(θ/2)<span class="ph">PROOF ▸</span></div><div class="fm">±√((1<span class="o">−</span>cosθ)/2)</div></div>
    <div class="fb" data-p="h-cos"><div class="fl">cos(θ/2)<span class="ph">PROOF ▸</span></div><div class="fm">±√((1<span class="o">+</span>cosθ)/2)</div></div>
    <div class="fb" data-p="h-tan"><div class="fl">tan(θ/2) — 3 forms<span class="ph">PROOF ▸</span></div><div class="fm">±√((1−cosθ)/(1+cosθ))<br>= sinθ/(1+cosθ) = (1−cosθ)/sinθ</div></div>
  </div>
</div></section>

<!-- ═══ 05 PRODUCT ↔ SUM ═══ -->
<section class="sec" id="s5"><div class="wrap">
  <div class="sh"><span class="sn">05 —</span><h2>Product-to-Sum &amp; Key Forms</h2></div>
  <h3>Product-to-Sum</h3>
  <div class="fg">
    <div class="fb" data-p="p2s-sc"><div class="fl">2 sinA cosB<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sin</span>(A+B) <span class="o">+</span> <span class="f">sin</span>(A−B)</div></div>
    <div class="fb" data-p="p2s-cs"><div class="fl">2 cosA sinB<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">sin</span>(A+B) <span class="o">−</span> <span class="f">sin</span>(A−B)</div></div>
    <div class="fb" data-p="p2s-cc"><div class="fl">2 cosA cosB<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cos</span>(A−B) <span class="o">+</span> <span class="f">cos</span>(A+B)</div></div>
    <div class="fb" data-p="p2s-ss"><div class="fl">2 sinA sinB<span class="ph">PROOF ▸</span></div><div class="fm"><span class="f">cos</span>(A−B) <span class="o">−</span> <span class="f">cos</span>(A+B)</div></div>
  </div>
  <h3>a·sinθ + b·cosθ Form</h3>
  <div class="fg">
    <div class="fb" data-p="asinbcos"><div class="fl">Max/Min form<span class="ph">PROOF ▸</span></div><div class="fm">a·sinθ+b·cosθ = R·sin(θ+φ)<br>R = √(a²+b²), tanφ = b/a<br>Max = <span class="gr">+√(a²+b²)</span>, Min = <span class="pk">−√(a²+b²)</span></div></div>
  </div>
</div></section>

<!-- ═══ 06 GRAPHS ═══ -->
<section class="sec" id="s6"><div class="wrap">
  <div class="sh"><span class="sn">06 —</span><h2>Trigonometric Function Graphs</h2></div>
  <div class="gg">
    <div class="gc">
      <span style="font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--muted);margin-right:6px;letter-spacing:1px;">TOGGLE:</span>
      <button class="ft on" data-fn="sin" style="color:#e8b84b;border-color:rgba(232,184,75,.4);">sin x</button>
      <button class="ft on" data-fn="cos" style="color:#4b9fe8;border-color:rgba(75,159,232,.4);">cos x</button>
      <button class="ft" data-fn="tan" style="color:#e84b7a;border-color:rgba(232,75,122,.4);">tan x</button>
      <button class="ft" data-fn="csc" style="color:#4be8a0;border-color:rgba(75,232,160,.4);">cosec x</button>
      <button class="ft" data-fn="sec" style="color:#b84be8;border-color:rgba(184,75,232,.4);">sec x</button>
      <button class="ft" data-fn="cot" style="color:#e8a04b;border-color:rgba(232,160,75,.4);">cot x</button>
    </div>
    <canvas id="tc" height="380"></canvas>
  </div>
  <h3>Domain, Range &amp; Period</h3>
  <table class="dtbl">
    <thead><tr><th>Function</th><th>Domain</th><th>Range</th><th>Period</th></tr></thead>
    <tbody>
      <tr><td>sin x</td><td>ℝ</td><td>[−1, 1]</td><td>2π</td></tr>
      <tr><td>cos x</td><td>ℝ</td><td>[−1, 1]</td><td>2π</td></tr>
      <tr><td>tan x</td><td>ℝ − {(2n+1)π/2}</td><td>ℝ</td><td>π</td></tr>
      <tr><td>cosec x</td><td>ℝ − {nπ}</td><td>(−∞,−1] ∪ [1,+∞)</td><td>2π</td></tr>
      <tr><td>sec x</td><td>ℝ − {(2n+1)π/2}</td><td>(−∞,−1] ∪ [1,+∞)</td><td>2π</td></tr>
      <tr><td>cot x</td><td>ℝ − {nπ}</td><td>ℝ</td><td>π</td></tr>
    </tbody>
  </table>
</div></section>

<!-- ═══ 07 INVERSE TRIG ═══ -->
<section class="sec" id="s7"><div class="wrap">
  <div class="sh"><span class="sn">07 —</span><h2>Inverse Trigonometric Functions</h2></div>
  <h3>Domain &amp; Range</h3>
  <table class="dtbl">
    <thead><tr><th>Function</th><th>Domain</th><th>Range (Principal)</th></tr></thead>
    <tbody>
      <tr><td>sin⁻¹ x</td><td>[−1, 1]</td><td>[−π/2, π/2]</td></tr>
      <tr><td>cos⁻¹ x</td><td>[−1, 1]</td><td>[0, π]</td></tr>
      <tr><td>tan⁻¹ x</td><td>ℝ</td><td>(−π/2, π/2)</td></tr>
      <tr><td>cosec⁻¹ x</td><td>(−∞,−1] ∪ [1,+∞)</td><td>[−π/2,π/2]−{0}</td></tr>
      <tr><td>sec⁻¹ x</td><td>(−∞,−1] ∪ [1,+∞)</td><td>[0,π]−{π/2}</td></tr>
      <tr><td>cot⁻¹ x</td><td>ℝ</td><td>(0, π)</td></tr>
    </tbody>
  </table>
  <h3>Graphs of Inverse Trig Functions</h3>
  <div class="gg">
    <div class="gc">
      <span style="font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--muted);margin-right:6px;letter-spacing:1px;">TOGGLE:</span>
      <button class="ft itf-ind-btn on" data-iifn="asin"  style="color:#e8b84b;border-color:rgba(232,184,75,.4);">sin⁻¹ x</button>
      <button class="ft itf-ind-btn on" data-iifn="acos"  style="color:#4b9fe8;border-color:rgba(75,159,232,.4);">cos⁻¹ x</button>
      <button class="ft itf-ind-btn on" data-iifn="atan"  style="color:#e84b7a;border-color:rgba(232,75,122,.4);">tan⁻¹ x</button>
      <button class="ft itf-ind-btn"    data-iifn="acot"  style="color:#4be8a0;border-color:rgba(75,232,160,.4);">cot⁻¹ x</button>
      <button class="ft itf-ind-btn"    data-iifn="asec"  style="color:#b84be8;border-color:rgba(184,75,232,.4);">sec⁻¹ x</button>
      <button class="ft itf-ind-btn"    data-iifn="acsc"  style="color:#e8a04b;border-color:rgba(232,160,75,.4);">cosec⁻¹ x</button>
    </div>
    <canvas id="itf-ind-canvas" height="380"></canvas>
  </div>
  <div class="nb" style="margin-bottom:16px;"><strong>GRAPH NOTES:</strong>
    sin⁻¹x: S-curve on [−1,1], range [−π/2,π/2] · cos⁻¹x: decreasing on [−1,1], range [0,π] ·
    tan⁻¹x: horizontal asymptotes y=±π/2 · cot⁻¹x: decreasing, range (0,π) ·
    sec⁻¹x: defined for |x|≥1, range [0,π]−{π/2} · cosec⁻¹x: defined for |x|≥1, range [−π/2,π/2]−{0}
  </div>

  <h3>Key Properties</h3>
  <div class="fg">
    <div class="fb" data-p="iv-comp"><div class="fl">Complementary pairs<span class="ph">PROOF ▸</span></div><div class="fm">sin⁻¹x + cos⁻¹x = π/2<br>tan⁻¹x + cot⁻¹x = π/2<br>sec⁻¹x + cosec⁻¹x = π/2</div></div>
    <div class="fb" data-p="iv-neg"><div class="fl">Negative argument<span class="ph">PROOF ▸</span></div><div class="fm">sin⁻¹(−x) = −sin⁻¹x<br>cos⁻¹(−x) = π−cos⁻¹x<br>tan⁻¹(−x) = −tan⁻¹x</div></div>
    <div class="fb" data-p="iv-rec"><div class="fl">Reciprocal identities<span class="ph">PROOF ▸</span></div><div class="fm">sin⁻¹(1/x) = cosec⁻¹x, |x|≥1<br>cos⁻¹(1/x) = sec⁻¹x, |x|≥1<br>tan⁻¹(1/x) = cot⁻¹x, x&gt;0</div></div>
    <div class="fb" data-p="iv-tadd"><div class="fl">tan⁻¹x + tan⁻¹y<span class="ph">PROOF ▸</span></div><div class="fm">= tan⁻¹((x+y)/(1−xy)), xy&lt;1<br>= π+tan⁻¹((x+y)/(1−xy)), x,y&gt;0,xy&gt;1</div></div>
    <div class="fb" data-p="iv-2t"><div class="fl">2 tan⁻¹x<span class="ph">PROOF ▸</span></div><div class="fm">= sin⁻¹(2x/(1+x²))<br>= cos⁻¹((1−x²)/(1+x²))<br>= tan⁻¹(2x/(1−x²))</div></div>
  </div>
</div></section>

<!-- ═══ 08 EQUATIONS ═══ -->
<section class="sec" id="s8"><div class="wrap">
  <div class="sh"><span class="sn">08 —</span><h2>General Solutions of Trig Equations</h2></div>
  <div class="fg">
    <div class="fb" data-p="gs-sin"><div class="fl">sin θ = sin α<span class="ph">PROOF ▸</span></div><div class="fm">θ = <span class="v">nπ</span> + (−1)ⁿ α, n ∈ ℤ</div></div>
    <div class="fb" data-p="gs-cos"><div class="fl">cos θ = cos α<span class="ph">PROOF ▸</span></div><div class="fm">θ = <span class="n">2</span><span class="v">nπ</span> <span class="o">±</span> α, n ∈ ℤ</div></div>
    <div class="fb" data-p="gs-tan"><div class="fl">tan θ = tan α<span class="ph">PROOF ▸</span></div><div class="fm">θ = <span class="v">nπ</span> <span class="o">+</span> α, n ∈ ℤ</div></div>
    <div class="fb" data-p="gs-sin0"><div class="fl">sin θ = 0<span class="ph">PROOF ▸</span></div><div class="fm">θ = nπ</div></div>
    <div class="fb" data-p="gs-cos0"><div class="fl">cos θ = 0<span class="ph">PROOF ▸</span></div><div class="fm">θ = (2n+1)π/2</div></div>
    <div class="fb" data-p="gs-tan0"><div class="fl">tan θ = 0<span class="ph">PROOF ▸</span></div><div class="fm">θ = nπ</div></div>
    <div class="fb" data-p="gs-sq"><div class="fl">sin²θ = sin²α (and cos², tan²)<span class="ph">PROOF ▸</span></div><div class="fm">θ = nπ ± α</div></div>
  </div>
</div></section>

<!-- ═══ 09 KEY RESULTS ═══ -->
<section class="sec" id="s9"><div class="wrap">
  <div class="sh"><span class="sn">09 —</span><h2>Important Results &amp; Special Values</h2></div>
  <h3>Product Results</h3>
  <div class="fg">
    <div class="fb" data-p="pr-sin"><div class="fl">sin product<span class="ph">PROOF ▸</span></div><div class="fm">sinθ · sin(60°−θ) · sin(60°+θ) = (1/4) sin3θ</div></div>
    <div class="fb" data-p="pr-cos"><div class="fl">cos product<span class="ph">PROOF ▸</span></div><div class="fm">cosθ · cos(60°−θ) · cos(60°+θ) = (1/4) cos3θ</div></div>
    <div class="fb" data-p="pr-tan"><div class="fl">tan product<span class="ph">PROOF ▸</span></div><div class="fm">tanθ · tan(60°−θ) · tan(60°+θ) = tan3θ</div></div>
  </div>
  <h3>Special Angle Values</h3>
  <div class="rb b">sin18° = (√5−1)/4 = cos72° &nbsp;|&nbsp; cos36° = (√5+1)/4 = sin54°<br>sin15° = (√6−√2)/4 = cos75° &nbsp;|&nbsp; cos15° = (√6+√2)/4 = sin75°<br>tan15° = 2−√3 = cot75° &nbsp;|&nbsp; tan75° = 2+√3 = cot15°</div>
  <h3>Triangle Formulas</h3>
  <div class="fg">
    <div class="fb" data-p="sine-rule"><div class="fl">Sine Rule<span class="ph">PROOF ▸</span></div><div class="fm">a/sinA = b/sinB = c/sinC = 2R</div></div>
    <div class="fb" data-p="cos-rule"><div class="fl">Cosine Rule<span class="ph">PROOF ▸</span></div><div class="fm">cosA = (b²+c²−a²) / 2bc</div></div>
    <div class="fb" data-p="area"><div class="fl">Area of Triangle<span class="ph">PROOF ▸</span></div><div class="fm">Δ = ½ab sinC = √(s(s−a)(s−b)(s−c))</div></div>
  </div>
  <h3>Conditional Identities (A+B+C = π)</h3>
  <div class="fg">
    <div class="fb" data-p="ci-tan"><div class="fl">tan sum<span class="ph">PROOF ▸</span></div><div class="fm">tanA+tanB+tanC = tanA·tanB·tanC</div></div>
    <div class="fb" data-p="ci-half"><div class="fl">half-angle products<span class="ph">PROOF ▸</span></div><div class="fm">tan(A/2)tan(B/2)+tan(B/2)tan(C/2)+tan(C/2)tan(A/2) = 1</div></div>
  </div>
</div></section>

<!-- ═══ 10 ITF COMPOSITE GRAPHS ═══ -->
<section class="sec" id="s10"><div class="wrap">
  <div class="sh"><span class="sn">10 —</span><h2>ITF Composite Function Graphs</h2></div>
  <p style="font-family:'Crimson Pro',serif;font-style:italic;color:var(--t2);margin-bottom:18px;font-size:.95rem;">
    These graphs show the behaviour of compositions like sin⁻¹(sin x), cos⁻¹(cos x), tan⁻¹(tan x) — critical for JEE. Notice how domain restrictions create the characteristic "zigzag" and "sawtooth" shapes.
  </p>
  <div class="gg">
    <div class="gc">
      <span style="font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--muted);margin-right:6px;letter-spacing:1px;">TOGGLE:</span>
      <button class="ft itf-btn on" data-ifn="asin_sin"  style="color:#e8b84b;border-color:rgba(232,184,75,.4);">sin⁻¹(sin x)</button>
      <button class="ft itf-btn"    data-ifn="acos_cos"  style="color:#e84b7a;border-color:rgba(232,75,122,.4);">cos⁻¹(cos x)</button>
      <button class="ft itf-btn"    data-ifn="atan_tan"  style="color:#b84be8;border-color:rgba(184,75,232,.4);">tan⁻¹(tan x)</button>
    </div>
    <canvas id="itfc" height="380"></canvas>
  </div>
  <h3>Key Behaviour Summary</h3>
  <table class="dtbl">
    <thead><tr><th>Function</th><th>Domain</th><th>Range</th><th>Nature</th></tr></thead>
    <tbody>
      <tr><td>sin⁻¹(sin x)</td><td>ℝ</td><td>[−π/2, π/2]</td><td>Periodic zigzag, period 2π</td></tr>
      <tr><td>cos⁻¹(cos x)</td><td>ℝ</td><td>[0, π]</td><td>Periodic zigzag, period 2π</td></tr>
      <tr><td>tan⁻¹(tan x)</td><td>ℝ − {(2n+1)π/2}</td><td>(−π/2, π/2)</td><td>Periodic sawtooth, period π</td></tr>
    </tbody>
  </table>
  <div class="nb" style="margin-top:14px;"><strong>JEE KEY:</strong> sin⁻¹(sin x) = x only when x ∈ [−π/2, π/2]. Outside this, the graph folds back. Similarly cos⁻¹(cos x) = x only for x ∈ [0, π]. The "identity" compositions f⁻¹(f(x)) give y = x on the principal branch; f(f⁻¹(x)) is always y = x on the full domain of f⁻¹.</div>
</div></section>



</div></div></div>
<div class="psec" id="sec-coord"><div class="cwrap"><div class="shero" style="--sc:rgba(64,208,192,.08)"><span class="shero-badge">02 — JEE Advanced &amp; Mains</span><h2 style="color:#40d0c0">Coordinate <em>Geometry</em></h2><p>Formulae · loci · proofs · 2D SVG diagrams · miscellaneous properties</p><div class="snav"><a href="#basics">Basics</a><a href="#straight">Lines</a><a href="#circles">Circles</a><a href="#parabola">Parabola</a><a href="#ellipse">Ellipse</a><a href="#hyperbola">Hyperbola</a><a href="#pair">Pair</a><a href="#misc">Misc</a></div></div>



<main>

<!-- ══════════════════ TOC ══════════════════ -->
<div class="toc-grid">
  <a href="#basics" class="toc-item"><span class="num">01</span>Coordinate Basics</a>
  <a href="#straight" class="toc-item"><span class="num">02</span>Straight Lines</a>
  <a href="#circles" class="toc-item"><span class="num">03</span>Circles</a>
  <a href="#parabola" class="toc-item"><span class="num">04</span>Parabola</a>
  <a href="#ellipse" class="toc-item"><span class="num">05</span>Ellipse</a>
  <a href="#hyperbola" class="toc-item"><span class="num">06</span>Hyperbola</a>
  <a href="#pair" class="toc-item"><span class="num">07</span>Pair of Lines</a>
  <a href="#misc" class="toc-item"><span class="num">08</span>Misc Properties</a>
</div>

<!-- ══════════════════ 1. BASICS ══════════════════ -->
<section class="section" id="basics">
  <div class="section-header">
    <span class="section-num">01</span>
    <h2 class="section-title">Coordinate Basics</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3><span class="icon">📐</span> Distance & Section Formulae</h3>
      <p><strong>Distance</strong> between P(x₁,y₁) and Q(x₂,y₂):</p>
      <code class="formula gold">PQ = √[(x₂−x₁)² + (y₂−y₁)²]</code>
      <p><strong>Section Formula</strong> — point dividing PQ in ratio m:n (internally):</p>
      <code class="formula">(mx₂+nx₁)/(m+n) , (my₂+ny₁)/(m+n)</code>
      <p>Externally (replace + with −):</p>
      <code class="formula rose">(mx₂−nx₁)/(m−n) , (my₂−ny₁)/(m−n)</code>
      <p><strong>Midpoint:</strong></p>
      <code class="formula green">((x₁+x₂)/2 , (y₁+y₂)/2)</code>

      <div class="diagram-wrap">
        <svg viewBox="0 0 280 160" width="280" height="160" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="140" x2="260" y2="140" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="20" y1="20" x2="20" y2="140" stroke="#2a2f3e" stroke-width="1"/>
          <!-- points -->
          <circle cx="60" cy="110" r="4" fill="#c9a84c"/>
          <circle cx="220" cy="40" r="4" fill="#c9a84c"/>
          <circle cx="140" cy="75" r="4" fill="#4ecdc4"/>
          <!-- line -->
          <line x1="60" y1="110" x2="220" y2="40" stroke="#c9a84c" stroke-width="1.2" stroke-dasharray="4,3"/>
          <!-- labels -->
          <text x="50" y="125" fill="#e8c97a" font-size="11" font-family="JetBrains Mono">P(x₁,y₁)</text>
          <text x="222" y="36" fill="#e8c97a" font-size="11" font-family="JetBrains Mono">Q(x₂,y₂)</text>
          <text x="143" y="72" fill="#4ecdc4" font-size="10" font-family="JetBrains Mono">M</text>
          <!-- m:n markers -->
          <text x="88" y="90" fill="#8a8578" font-size="9" font-family="JetBrains Mono">m</text>
          <text x="175" y="62" fill="#8a8578" font-size="9" font-family="JetBrains Mono">n</text>
          <!-- distance brace -->
          <path d="M60 115 Q140 130 220 115" fill="none" stroke="#7a6030" stroke-width="0.8"/>
          <text x="122" y="138" fill="#c9a84c" font-size="9" font-family="JetBrains Mono">PQ</text>
        </svg>
      </div>
      <p class="diagram-cap">Section formula — M divides PQ in ratio m:n internally</p>
    </div>

    <div class="card teal">
      <h3><span class="icon">△</span> Area of Triangle & Collinearity</h3>
      <p>Area of △ with vertices (x₁,y₁), (x₂,y₂), (x₃,y₃):</p>
      <code class="formula teal">Δ = ½|x₁(y₂−y₃) + x₂(y₃−y₁) + x₃(y₁−y₂)|</code>
      <p>Equivalent determinant form:</p>
      <code class="formula">Δ = ½ |det [[x₁,y₁,1],[x₂,y₂,1],[x₃,y₃,1]]|</code>
      <p><strong>Collinearity condition:</strong> Area = 0, i.e.:</p>
      <code class="formula rose">x₁(y₂−y₃)+x₂(y₃−y₁)+x₃(y₁−y₂) = 0</code>
      <div class="note">
        <strong>Centroid G</strong> = ((x₁+x₂+x₃)/3 , (y₁+y₂+y₃)/3)<br>
        <strong>Incentre</strong> = (ax₁+bx₂+cx₃)/(a+b+c), same for y; where a,b,c are opposite side lengths.
      </div>

      <div class="diagram-wrap">
        <svg viewBox="0 0 240 150" width="240" height="150" xmlns="http://www.w3.org/2000/svg">
          <!-- triangle -->
          <polygon points="40,130 200,130 120,25" fill="rgba(78,205,196,0.06)" stroke="#4ecdc4" stroke-width="1.2"/>
          <!-- vertices -->
          <circle cx="40" cy="130" r="3.5" fill="#4ecdc4"/>
          <circle cx="200" cy="130" r="3.5" fill="#4ecdc4"/>
          <circle cx="120" cy="25" r="3.5" fill="#4ecdc4"/>
          <!-- centroid -->
          <circle cx="120" cy="95" r="3" fill="#c9a84c"/>
          <!-- medians -->
          <line x1="40" y1="130" x2="160" y2="77.5" stroke="#c9a84c" stroke-width="0.7" stroke-dasharray="3,3" opacity="0.5"/>
          <line x1="200" y1="130" x2="80" y2="77.5" stroke="#c9a84c" stroke-width="0.7" stroke-dasharray="3,3" opacity="0.5"/>
          <line x1="120" y1="25" x2="120" y2="130" stroke="#c9a84c" stroke-width="0.7" stroke-dasharray="3,3" opacity="0.5"/>
          <!-- labels -->
          <text x="26" y="145" fill="#b8b0a0" font-size="10" font-family="JetBrains Mono">A</text>
          <text x="202" y="145" fill="#b8b0a0" font-size="10" font-family="JetBrains Mono">B</text>
          <text x="115" y="18" fill="#b8b0a0" font-size="10" font-family="JetBrains Mono">C</text>
          <text x="124" y="93" fill="#e8c97a" font-size="9" font-family="JetBrains Mono">G</text>
          <!-- side labels -->
          <text x="152" y="88" fill="#8a8578" font-size="8" font-family="JetBrains Mono">b</text>
          <text x="72" y="88" fill="#8a8578" font-size="8" font-family="JetBrains Mono">c</text>
          <text x="118" y="140" fill="#8a8578" font-size="8" font-family="JetBrains Mono">a</text>
        </svg>
      </div>
      <p class="diagram-cap">Centroid G (medians intersect at 2:1 from vertex)</p>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Locus Concept <span class="tag imp">IMP</span></h3>
      <p>Locus is the set of all points satisfying a geometric condition.</p>
      <p><strong>Steps to find locus:</strong></p>
      <ul class="props">
        <li>Let the moving point be P(h,k).</li>
        <li>Write the geometric condition in terms of h,k.</li>
        <li>Eliminate parameters to get relation in h,k.</li>
        <li>Replace h→x, k→y for the locus equation.</li>
      </ul>
    </div>
    <div class="card rose">
      <h3>Transformation of Axes</h3>
      <p>Shift origin to (h,k): replace x → x+h, y → y+k.</p>
      <p><strong>Rotation by θ:</strong></p>
      <code class="formula rose">x = X cosθ − Y sinθ</code>
      <code class="formula rose">y = X sinθ + Y cosθ</code>
      <p>Invariants: x²+y², discriminant of conic.</p>
    </div>
    <div class="card violet">
      <h3>Useful Identities</h3>
      <code class="formula violet">tan(A+B) = (tanA+tanB)/(1−tanA·tanB)</code>
      <code class="formula violet">sin²θ+cos²θ = 1</code>
      <p>Slope from angle: <code class="formula">m = tanθ</code></p>
      <p>Angle between two lines with slopes m₁,m₂:</p>
      <code class="formula teal">tanθ = |(m₁−m₂)/(1+m₁m₂)|</code>
    </div>
  </div>
</section>

<!-- ══════════════════ 2. STRAIGHT LINES ══════════════════ -->
<section class="section" id="straight">
  <div class="section-header">
    <span class="section-num">02</span>
    <h2 class="section-title">Straight Lines</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Forms of a Line</h3>
      <p>Slope–intercept: <code class="formula gold">y = mx + c</code></p>
      <p>Point–slope: <code class="formula">y−y₁ = m(x−x₁)</code></p>
      <p>Two-point: <code class="formula">(y−y₁)/(y₂−y₁) = (x−x₁)/(x₂−x₁)</code></p>
      <p>Intercept form: <code class="formula teal">x/a + y/b = 1</code></p>
      <p>Normal form: <code class="formula green">x·cosα + y·sinα = p</code> (p = ⊥ distance from O)</p>
      <p>General: <code class="formula rose">ax + by + c = 0</code></p>
      <p>Parametric: <code class="formula">x=x₁+r·cosθ, y=y₁+r·sinθ</code></p>
    </div>

    <div class="card teal">
      <h3>Distance Formulae</h3>
      <p><strong>⊥ Distance</strong> from point (x₁,y₁) to line ax+by+c=0:</p>
      <code class="formula gold">d = |ax₁+by₁+c| / √(a²+b²)</code>
      <p><strong>Distance between parallel lines</strong> ax+by+c₁=0, ax+by+c₂=0:</p>
      <code class="formula teal">d = |c₁−c₂| / √(a²+b²)</code>
      <p><strong>Foot of perpendicular</strong> from (x₁,y₁) to ax+by+c=0:</p>
      <code class="formula">(x−x₁)/a = (y−y₁)/b = −(ax₁+by₁+c)/(a²+b²)</code>
      <p><strong>Reflection</strong> of (x₁,y₁) about ax+by+c=0:</p>
      <code class="formula rose">(x−x₁)/a = (y−y₁)/b = −2(ax₁+by₁+c)/(a²+b²)</code>

      <div class="diagram-wrap">
        <svg viewBox="0 0 260 150" width="260" height="150" xmlns="http://www.w3.org/2000/svg">
          <!-- line ax+by+c=0 -->
          <line x1="20" y1="130" x2="240" y2="30" stroke="#4ecdc4" stroke-width="1.5"/>
          <text x="230" y="26" fill="#4ecdc4" font-size="10" font-family="JetBrains Mono">ℓ: ax+by+c=0</text>
          <!-- point P -->
          <circle cx="80" cy="40" r="4" fill="#c9a84c"/>
          <text x="55" y="36" fill="#e8c97a" font-size="10" font-family="JetBrains Mono">P(x₁,y₁)</text>
          <!-- foot -->
          <circle cx="116" cy="95" r="3.5" fill="#6ee7b7"/>
          <text x="120" y="108" fill="#6ee7b7" font-size="9" font-family="JetBrains Mono">F (foot)</text>
          <!-- perpendicular -->
          <line x1="80" y1="40" x2="116" y2="95" stroke="#c9a84c" stroke-width="1" stroke-dasharray="4,3"/>
          <!-- right angle mark -->
          <rect x="108" y="87" width="8" height="8" fill="none" stroke="#6ee7b7" stroke-width="0.8" transform="rotate(-25 112 91)"/>
          <!-- d label -->
          <text x="85" y="72" fill="#c9a84c" font-size="10" font-family="JetBrains Mono">d</text>
        </svg>
      </div>
      <p class="diagram-cap">Perpendicular distance from P to line ℓ</p>
    </div>
  </div>

  <div class="grid grid-2" style="margin-top:1.2rem">
    <div class="card rose">
      <h3>Angle Bisectors <span class="tag adv">ADV</span></h3>
      <p>Bisectors of the angle between lines a₁x+b₁y+c₁=0 and a₂x+b₂y+c₂=0:</p>
      <code class="formula gold">(a₁x+b₁y+c₁)/√(a₁²+b₁²) = ±(a₂x+b₂y+c₂)/√(a₂²+b₂²)</code>
      <p>To find which bisector is acute: use the condition</p>
      <code class="formula rose">a₁a₂+b₁b₂ &lt; 0  ⟹  '+' is acute bisector</code>
      <div class="note"><strong>Locus:</strong> Every point on a bisector is equidistant from both lines.</div>
    </div>
    <div class="card violet">
      <h3>Concurrent Lines & Family</h3>
      <p>Three lines aᵢx+bᵢy+cᵢ=0 are concurrent if:</p>
      <code class="formula violet">det [[a₁,b₁,c₁],[a₂,b₂,c₂],[a₃,b₃,c₃]] = 0</code>
      <p><strong>Family of lines</strong> through intersection of L₁=0 and L₂=0:</p>
      <code class="formula teal">L₁ + λL₂ = 0  (λ ∈ ℝ)</code>
      <div class="note"><strong>Any line through intersection of two given lines</strong> can be written without finding the actual point of intersection.</div>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Parallel & Perpendicular</h3>
      <p>L₁: y=m₁x+c₁, L₂: y=m₂x+c₂</p>
      <code class="formula">Parallel:  m₁ = m₂</code>
      <code class="formula rose">Perp:  m₁·m₂ = −1</code>
      <p>For ax+by+c=0:<br>
        Parallel line: <code class="formula">ax+by+k=0</code><br>
        Perpendicular: <code class="formula">bx−ay+k=0</code>
      </p>
    </div>
    <div class="card green">
      <h3>Homogenisation <span class="tag adv">ADV</span></h3>
      <p>Equation of lines joining origin to intersections of y=mx+c and S(x,y)=0:</p>
      <code class="formula green">S(x,y) − (y−mx)²/c² · [coefficient] = 0</code>
      <p>General: replace '1' by (lx+my+n)/n in S=0 after homogenising. Combined equation of pair gives angle between them.</p>
    </div>
    <div class="card">
      <h3>Special Loci on Lines</h3>
      <ul class="props">
        <li>Perpendicular bisector of AB: locus of equidistant points</li>
        <li>PA²+PB² = k: locus is a circle</li>
        <li>PA/PB = k ≠ 1: Apollonius circle</li>
        <li>Locus when sum of intercepts = const.: x/a+y/b=1, a+b=k</li>
      </ul>
    </div>
  </div>
</section>

<!-- ══════════════════ 3. CIRCLES ══════════════════ -->
<section class="section" id="circles">
  <div class="section-header">
    <span class="section-num">03</span>
    <h2 class="section-title">Circles</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Standard Forms</h3>
      <p>Centre (h,k), radius r:</p>
      <code class="formula gold">(x−h)² + (y−k)² = r²</code>
      <p>General form:</p>
      <code class="formula">x²+y²+2gx+2fy+c = 0</code>
      <p>Centre = (−g,−f), Radius = √(g²+f²−c)</p>
      <p>Diameter form — endpoints (x₁,y₁) & (x₂,y₂):</p>
      <code class="formula teal">(x−x₁)(x−x₂)+(y−y₁)(y−y₂) = 0</code>
      <div class="note"><strong>Condition for real circle:</strong> g²+f²−c ≥ 0</div>

      <div class="diagram-wrap">
        <svg viewBox="0 0 240 200" width="240" height="200" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="100" x2="220" y2="100" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="120" y1="10" x2="120" y2="190" stroke="#2a2f3e" stroke-width="1"/>
          <!-- circle -->
          <circle cx="120" cy="100" r="60" fill="rgba(201,168,76,0.05)" stroke="#c9a84c" stroke-width="1.5"/>
          <!-- centre -->
          <circle cx="120" cy="100" r="3" fill="#c9a84c"/>
          <text x="124" y="96" fill="#e8c97a" font-size="10" font-family="JetBrains Mono">C(h,k)</text>
          <!-- radius -->
          <line x1="120" y1="100" x2="166" y2="62" stroke="#4ecdc4" stroke-width="1.2" stroke-dasharray="4,3"/>
          <text x="138" y="76" fill="#4ecdc4" font-size="10" font-family="JetBrains Mono">r</text>
          <!-- point on circle -->
          <circle cx="166" cy="62" r="3" fill="#4ecdc4"/>
          <!-- tangent at that point (perpendicular to radius) -->
          <line x1="145" y1="36" x2="187" y2="88" stroke="#a78bfa" stroke-width="1" stroke-dasharray="3,3"/>
          <text x="156" y="32" fill="#a78bfa" font-size="9" font-family="JetBrains Mono">tangent</text>
          <!-- right angle -->
          <rect x="160" y="58" width="7" height="7" fill="none" stroke="#a78bfa" stroke-width="0.7" transform="rotate(-45 163 61)"/>
          <!-- g,f labels on axes -->
          <circle cx="120" cy="100" r="2" fill="#7a6030"/>
          <text x="35" y="97" fill="#8a8578" font-size="8" font-family="JetBrains Mono">O</text>
        </svg>
      </div>
      <p class="diagram-cap">Circle with centre C, radius r; tangent ⊥ radius at contact point</p>
    </div>

    <div class="card teal">
      <h3>Tangent & Normal</h3>
      <p>Tangent to x²+y²+2gx+2fy+c=0 at point (x₁,y₁):</p>
      <code class="formula gold">T ≡ xx₁+yy₁+g(x+x₁)+f(y+y₁)+c = 0</code>
      <p>Tangent from external point — length of tangent:</p>
      <code class="formula teal">L = √(x₁²+y₁²+2gx₁+2fy₁+c)</code>
      <p>Normal at (x₁,y₁) passes through centre, slope = −(x₁+g)/(y₁+f).</p>
      <p>Tangent with slope m to x²+y²=r²:</p>
      <code class="formula rose">y = mx ± r√(1+m²)</code>
      <p><strong>Condition of tangency:</strong> for line lx+my+n=0 to x²+y²=r²:</p>
      <code class="formula violet">r² (l²+m²) = n²</code>
      <p><strong>Chord of contact</strong> from (x₁,y₁) to x²+y²=r²:</p>
      <code class="formula green">xx₁+yy₁ = r²</code>
    </div>
  </div>

  <div class="grid grid-2" style="margin-top:1.2rem">
    <div class="card rose">
      <h3>Chord & Power of a Point <span class="tag adv">ADV</span></h3>
      <p>Equation of chord with midpoint (h,k) on S=0:</p>
      <code class="formula rose">T(h,k) = S(h,k)</code>
      <p>i.e., T = S₁ (shorthand)</p>
      <p><strong>Power of a point</strong> P w.r.t. S≡x²+y²+2gx+2fy+c=0:</p>
      <code class="formula gold">Power = S(P) = x₁²+y₁²+2gx₁+2fy₁+c</code>
      <ul class="props">
        <li>Power &lt; 0: P is inside the circle</li>
        <li>Power = 0: P lies on circle</li>
        <li>Power &gt; 0: P is outside; = (length of tangent)²</li>
      </ul>
    </div>

    <div class="card violet">
      <h3>Two Circles — Relations</h3>
      <p>Circles C₁(r₁), C₂(r₂), d = distance between centres.</p>
      <ul class="props">
        <li>External: d &gt; r₁+r₂ (4 common tangents)</li>
        <li>External touch: d = r₁+r₂ (3 common tangents)</li>
        <li>Intersecting: |r₁−r₂| &lt; d &lt; r₁+r₂ (2 CTs)</li>
        <li>Internal touch: d = |r₁−r₂| (1 CT)</li>
        <li>One inside other: d &lt; |r₁−r₂| (0 CTs)</li>
      </ul>
      <p><strong>Radical axis</strong> S₁−S₂ = 0 (locus of equal power points).</p>
      <code class="formula teal">S₁ − S₂ = 0</code>
      <p><strong>Radical centre:</strong> radical axes of three circles are concurrent.</p>

      <div class="diagram-wrap">
        <svg viewBox="0 0 260 130" width="260" height="130" xmlns="http://www.w3.org/2000/svg">
          <!-- two circles -->
          <circle cx="85" cy="65" r="45" fill="rgba(78,205,196,0.04)" stroke="#4ecdc4" stroke-width="1.2"/>
          <circle cx="185" cy="65" r="45" fill="rgba(167,139,250,0.04)" stroke="#a78bfa" stroke-width="1.2"/>
          <!-- centres -->
          <circle cx="85" cy="65" r="3" fill="#4ecdc4"/>
          <circle cx="185" cy="65" r="3" fill="#a78bfa"/>
          <!-- radical axis -->
          <line x1="135" y1="10" x2="135" y2="120" stroke="#c9a84c" stroke-width="1" stroke-dasharray="4,3"/>
          <text x="137" y="18" fill="#c9a84c" font-size="9" font-family="JetBrains Mono">Radical Axis</text>
          <!-- labels -->
          <text x="60" y="63" fill="#4ecdc4" font-size="10" font-family="JetBrains Mono">C₁,r₁</text>
          <text x="158" y="63" fill="#a78bfa" font-size="10" font-family="JetBrains Mono">C₂,r₂</text>
          <!-- d label -->
          <line x1="85" y1="65" x2="185" y2="65" stroke="#7a6030" stroke-width="0.8"/>
          <text x="128" y="80" fill="#8a8578" font-size="9" font-family="JetBrains Mono">d</text>
        </svg>
      </div>
      <p class="diagram-cap">Radical axis is ⊥ to line of centres (for equal-radius circles it's the perpendicular bisector)</p>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Orthogonal Circles <span class="tag adv">ADV</span></h3>
      <p>Two circles are orthogonal if they intersect at right angles.</p>
      <code class="formula sky">2g₁g₂ + 2f₁f₂ = c₁ + c₂</code>
      <p>Geometrically, tangent at intersection point of one circle passes through centre of other.</p>
    </div>
    <div class="card green">
      <h3>Family of Circles</h3>
      <p>Family through intersection of S₁=0 and S₂=0:</p>
      <code class="formula green">S₁ + λS₂ = 0</code>
      <p>Family through intersection of circle S=0 and line L=0:</p>
      <code class="formula">S + λL = 0</code>
    </div>
    <div class="card">
      <h3>Director Circle</h3>
      <p>Locus of point from which two tangents to circle x²+y²=r² are perpendicular:</p>
      <code class="formula gold">x² + y² = 2r²</code>
      <p>i.e., director circle has same centre, radius r√2.</p>
    </div>
  </div>
</section>

<!-- ══════════════════ 4. PARABOLA ══════════════════ -->
<section class="section" id="parabola">
  <div class="section-header">
    <span class="section-num">04</span>
    <h2 class="section-title">Parabola</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Standard Parabola y² = 4ax</h3>
      <div class="diagram-wrap">
        <svg viewBox="0 0 280 200" width="280" height="200" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="30" y1="100" x2="260" y2="100" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="100" y1="10" x2="100" y2="190" stroke="#2a2f3e" stroke-width="1"/>
          <!-- parabola y²=4ax, a=40 -->
          <path d="M100,100 Q130,60 190,30" fill="none" stroke="#c9a84c" stroke-width="2"/>
          <path d="M100,100 Q130,140 190,170" fill="none" stroke="#c9a84c" stroke-width="2"/>
          <!-- focus -->
          <circle cx="140" cy="100" r="3.5" fill="#4ecdc4"/>
          <text x="142" y="96" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">F(a,0)</text>
          <!-- vertex -->
          <circle cx="100" cy="100" r="3" fill="#c9a84c"/>
          <text x="82" y="97" fill="#e8c97a" font-size="9" font-family="JetBrains Mono">V</text>
          <!-- directrix -->
          <line x1="60" y1="10" x2="60" y2="190" stroke="#e8677a" stroke-width="1" stroke-dasharray="4,3"/>
          <text x="30" y="20" fill="#e8677a" font-size="9" font-family="JetBrains Mono">x=−a</text>
          <!-- latus rectum -->
          <line x1="140" y1="60" x2="140" y2="140" stroke="#a78bfa" stroke-width="1" stroke-dasharray="3,3"/>
          <text x="142" y="55" fill="#a78bfa" font-size="8" font-family="JetBrains Mono">LR=4a</text>
          <!-- axis -->
          <text x="252" y="97" fill="#8a8578" font-size="9" font-family="JetBrains Mono">x</text>
          <!-- focal chord -->
          <circle cx="182" cy="68" r="2.5" fill="#6ee7b7"/>
          <circle cx="182" cy="132" r="2.5" fill="#6ee7b7"/>
          <line x1="140" y1="100" x2="182" y2="68" stroke="#6ee7b7" stroke-width="0.8" stroke-dasharray="2,2"/>
          <line x1="140" y1="100" x2="182" y2="132" stroke="#6ee7b7" stroke-width="0.8" stroke-dasharray="2,2"/>
          <text x="90" y="188" fill="#8a8578" font-size="8" font-family="JetBrains Mono">y²=4ax</text>
          <!-- a label -->
          <text x="112" y="112" fill="#8a8578" font-size="8" font-family="JetBrains Mono">a</text>
        </svg>
      </div>
      <p class="diagram-cap">y²=4ax: vertex O, focus F(a,0), directrix x=−a, LR=4a</p>
      <hr class="divider">
      <p>Focus: <code class="formula">(a, 0)</code>&nbsp; Directrix: <code class="formula rose">x = −a</code></p>
      <p>Vertex: (0,0), Axis: x-axis, LR length: <code class="formula teal">4a</code></p>
      <p>Parametric point: <code class="formula">(at², 2at)</code></p>
      <p>Focal distance of point (x,y): <code class="formula gold">r = x + a</code></p>
    </div>

    <div class="card teal">
      <h3>All 4 Standard Parabolas</h3>
      <div class="diagram-wrap">
        <svg viewBox="0 0 260 200" width="260" height="200" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="100" x2="240" y2="100" stroke="#333" stroke-width="1"/>
          <line x1="130" y1="10" x2="130" y2="190" stroke="#333" stroke-width="1"/>
          <!-- y²=4ax rightward -->
          <path d="M130,100 Q145,75 180,50" fill="none" stroke="#c9a84c" stroke-width="1.5"/>
          <path d="M130,100 Q145,125 180,150" fill="none" stroke="#c9a84c" stroke-width="1.5"/>
          <text x="182" y="48" fill="#c9a84c" font-size="8" font-family="JetBrains Mono">y²=4ax</text>
          <!-- y²=−4ax leftward -->
          <path d="M130,100 Q115,75 80,50" fill="none" stroke="#e8677a" stroke-width="1.5"/>
          <path d="M130,100 Q115,125 80,150" fill="none" stroke="#e8677a" stroke-width="1.5"/>
          <text x="38" y="48" fill="#e8677a" font-size="8" font-family="JetBrains Mono">y²=−4ax</text>
          <!-- x²=4ay upward -->
          <path d="M130,100 Q105,85 80,50" fill="none" stroke="#4ecdc4" stroke-width="1.5"/>
          <path d="M130,100 Q155,85 180,50" fill="none" stroke="#4ecdc4" stroke-width="1.5"/>
          <text x="148" y="50" fill="#4ecdc4" font-size="8" font-family="JetBrains Mono">x²=4ay↑</text>
          <!-- x²=−4ay downward -->
          <path d="M130,100 Q105,115 80,150" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
          <path d="M130,100 Q155,115 180,150" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
          <text x="148" y="163" fill="#a78bfa" font-size="8" font-family="JetBrains Mono">x²=−4ay↓</text>
          <!-- vertex -->
          <circle cx="130" cy="100" r="3" fill="white"/>
          <text x="134" y="97" fill="#8a8578" font-size="8" font-family="JetBrains Mono">V</text>
        </svg>
      </div>
      <p class="diagram-cap">All four standard parabola orientations</p>
      <hr class="divider">
      <p>y²=4ax: opens right, focus (a,0)</p>
      <p>y²=−4ax: opens left, focus (−a,0)</p>
      <p>x²=4ay: opens up, focus (0,a)</p>
      <p>x²=−4ay: opens down, focus (0,−a)</p>
    </div>
  </div>

  <div class="grid grid-2" style="margin-top:1.2rem">
    <div class="card rose">
      <h3>Tangent, Normal — Parabola</h3>
      <p>Tangent at (at²,2at) on y²=4ax:</p>
      <code class="formula gold">ty = x + at²</code>
      <p>Tangent with slope m:</p>
      <code class="formula">y = mx + a/m  (condition: c = a/m)</code>
      <p>Normal at (at²,2at):</p>
      <code class="formula rose">y = −tx + 2at + at³</code>
      <p>Normal with slope m:</p>
      <code class="formula">y = mx − 2am − am³</code>
      <div class="note"><strong>Intersection of tangents</strong> at t₁ and t₂ ⟹ point (at₁t₂, a(t₁+t₂)). Condition: t₁t₂ = −1 for perpendicular tangents (director circle equivalent).</div>
    </div>

    <div class="card violet">
      <h3>Focal Chord & Properties <span class="tag adv">ADV</span></h3>
      <p>For a focal chord through parameter t₁ and t₂:</p>
      <code class="formula violet">t₁ · t₂ = −1</code>
      <p><strong>Semi-latus rectum</strong> = HM of focal radii r₁,r₂:</p>
      <code class="formula teal">1/r₁ + 1/r₂ = 1/a  ⟹  ℓ = 2a</code>
      <p><strong>Chord of contact</strong> from (h,k):</p>
      <code class="formula">ky = 2a(x+h)</code>
      <p><strong>Chord with midpoint (h,k):</strong></p>
      <code class="formula rose">ky − 2ax = k² − 4ah  (T=S₁)</code>
      <p><strong>Director circle / locus of ⊥ tangents:</strong></p>
      <code class="formula gold">x = −a  (the directrix!)</code>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Normal Chord <span class="tag adv">ADV</span></h3>
      <p>If normals at t₁ and t₂ meet on the parabola at t₃:</p>
      <code class="formula sky">t₁ + t₂ + t₃ = 0</code>
      <p>Also t₃ = −t₁−t₂ and t₁t₂ = 2 for normal chord subtending 90° at vertex.</p>
    </div>
    <div class="card green">
      <h3>Reflection Property</h3>
      <p>Any ray parallel to axis of parabola reflects off the curve through the focus.</p>
      <p>This makes parabola the basis of satellite dishes, headlights, and reflecting telescopes.</p>
      <div class="note"><strong>Locus:</strong> foot of perpendicular from focus to any tangent lies on the tangent at vertex.</div>
    </div>
    <div class="card">
      <h3>General Parabola</h3>
      <p>Form: (lx+my)² + ...  or  (ax+by+c)² = k(bx−ay+d)</p>
      <p>Axis ∥ to bx−ay=0, directrix along lx+my+c=0.</p>
      <code class="formula gold">(ax+by)² + 2gx + 2fy + c = 0</code>
      <p>represents a parabola when a²+b²≠0 and the ab terms make it a perfect square part.</p>
    </div>
  </div>
</section>

<!-- ══════════════════ 5. ELLIPSE ══════════════════ -->
<section class="section" id="ellipse">
  <div class="section-header">
    <span class="section-num">05</span>
    <h2 class="section-title">Ellipse</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Standard Ellipse x²/a² + y²/b² = 1 (a>b)</h3>
      <div class="diagram-wrap">
        <svg viewBox="0 0 280 200" width="280" height="200" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="100" x2="260" y2="100" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="140" y1="10" x2="140" y2="190" stroke="#2a2f3e" stroke-width="1"/>
          <!-- ellipse -->
          <ellipse cx="140" cy="100" rx="80" ry="50" fill="rgba(201,168,76,0.05)" stroke="#c9a84c" stroke-width="1.5"/>
          <!-- foci -->
          <circle cx="94" cy="100" r="3.5" fill="#e8677a"/>
          <circle cx="186" cy="100" r="3.5" fill="#e8677a"/>
          <text x="80" y="115" fill="#e8677a" font-size="9" font-family="JetBrains Mono">F₁(−c,0)</text>
          <text x="176" y="115" fill="#e8677a" font-size="9" font-family="JetBrains Mono">F₂(c,0)</text>
          <!-- vertices -->
          <circle cx="60" cy="100" r="3" fill="#4ecdc4"/>
          <circle cx="220" cy="100" r="3" fill="#4ecdc4"/>
          <circle cx="140" cy="50" r="3" fill="#4ecdc4"/>
          <circle cx="140" cy="150" r="3" fill="#4ecdc4"/>
          <text x="48" y="97" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">A'</text>
          <text x="222" y="97" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">A</text>
          <text x="142" y="46" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">B</text>
          <!-- semi axes labels -->
          <line x1="140" y1="100" x2="220" y2="100" stroke="#c9a84c" stroke-width="0.8" stroke-dasharray="2,2"/>
          <text x="175" y="95" fill="#e8c97a" font-size="9" font-family="JetBrains Mono">a</text>
          <line x1="140" y1="100" x2="140" y2="50" stroke="#6ee7b7" stroke-width="0.8" stroke-dasharray="2,2"/>
          <text x="143" y="78" fill="#6ee7b7" font-size="9" font-family="JetBrains Mono">b</text>
          <!-- directrices -->
          <line x1="26" y1="15" x2="26" y2="185" stroke="#a78bfa" stroke-width="0.8" stroke-dasharray="3,3" opacity="0.7"/>
          <line x1="254" y1="15" x2="254" y2="185" stroke="#a78bfa" stroke-width="0.8" stroke-dasharray="3,3" opacity="0.7"/>
          <text x="5" y="13" fill="#a78bfa" font-size="7" font-family="JetBrains Mono">x=−a/e</text>
          <text x="230" y="13" fill="#a78bfa" font-size="7" font-family="JetBrains Mono">x=a/e</text>
          <!-- focal radii to a point -->
          <circle cx="192" cy="65" r="2.5" fill="#6ee7b7"/>
          <line x1="94" y1="100" x2="192" y2="65" stroke="#6ee7b7" stroke-width="0.8" stroke-dasharray="2,2"/>
          <line x1="186" y1="100" x2="192" y2="65" stroke="#6ee7b7" stroke-width="0.8" stroke-dasharray="2,2"/>
          <text x="194" y="63" fill="#6ee7b7" font-size="8" font-family="JetBrains Mono">P</text>
        </svg>
      </div>
      <p class="diagram-cap">PF₁+PF₂ = 2a (defining property)</p>
      <hr class="divider">
      <code class="formula gold">c² = a² − b²,   e = c/a &lt; 1</code>
      <p>Foci: <code class="formula">(±c, 0)</code>&nbsp; Directrices: <code class="formula rose">x = ±a/e</code></p>
      <p>LR length: <code class="formula teal">2b²/a</code></p>
      <p>Parametric: <code class="formula">(a cosθ, b sinθ)</code></p>
      <p>Focal radii: <code class="formula">r₁=a+ex, r₂=a−ex</code></p>
    </div>

    <div class="card teal">
      <h3>Tangent & Normal — Ellipse</h3>
      <p>Tangent at (x₁,y₁):</p>
      <code class="formula gold">xx₁/a² + yy₁/b² = 1</code>
      <p>Tangent at parametric point (a cosθ, b sinθ):</p>
      <code class="formula">x·cosθ/a + y·sinθ/b = 1</code>
      <p>Tangent with slope m:</p>
      <code class="formula rose">y = mx ± √(a²m²+b²)</code>
      <p>Condition: <code class="formula">c² = a²m²+b²</code></p>
      <p>Normal at (x₁,y₁):</p>
      <code class="formula violet">a²x/x₁ − b²y/y₁ = a²−b²</code>
      <p>Normal at (a cosθ, b sinθ):</p>
      <code class="formula teal">ax/cosθ − by/sinθ = a²−b²</code>
      <p><strong>Chord of contact</strong> from external (h,k):</p>
      <code class="formula green">hx/a² + ky/b² = 1</code>
      <p><strong>Director circle</strong> (locus of ⊥ tangents):</p>
      <code class="formula gold">x² + y² = a² + b²</code>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card rose">
      <h3>Special Properties <span class="tag adv">ADV</span></h3>
      <ul class="props">
        <li>Sum of focal distances = 2a (constant)</li>
        <li>Focal chord: 1/SP + 1/SQ = 2a/b²</li>
        <li>For focal chord at angle θ: semi-LR = b²/a = a(1−e²)</li>
        <li>Tangent & normal bisect external & internal angles with focal radii</li>
        <li>Eccentric angle difference for conjugate diameters: π/2</li>
      </ul>
    </div>
    <div class="card sky">
      <h3>Auxiliary Circle & Conjugate</h3>
      <p>Auxiliary circle: <code class="formula sky">x² + y² = a²</code></p>
      <p>Conjugate ellipse: <code class="formula">x²/a²+y²/b²=−1</code> (imaginary but e &gt; 1).</p>
      <p>For x²/a²+y²/b²=1, conjugate diameters satisfy: <code class="formula">mm' = −b²/a²</code></p>
    </div>
    <div class="card green">
      <h3>Chord with Midpoint</h3>
      <p>Chord of x²/a²+y²/b²=1 with midpoint (h,k): T=S₁</p>
      <code class="formula green">hx/a² + ky/b² = h²/a² + k²/b²</code>
      <p>Slope of this chord:</p>
      <code class="formula">m = −b²h/(a²k)</code>
    </div>
  </div>
</section>

<!-- ══════════════════ 6. HYPERBOLA ══════════════════ -->
<section class="section" id="hyperbola">
  <div class="section-header">
    <span class="section-num">06</span>
    <h2 class="section-title">Hyperbola</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Standard Hyperbola x²/a² − y²/b² = 1</h3>
      <div class="diagram-wrap">
        <svg viewBox="0 0 280 200" width="280" height="200" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="100" x2="260" y2="100" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="140" y1="10" x2="140" y2="190" stroke="#2a2f3e" stroke-width="1"/>
          <!-- asymptotes -->
          <line x1="20" y1="165" x2="260" y2="35" stroke="#7a6030" stroke-width="1" stroke-dasharray="4,3"/>
          <line x1="20" y1="35" x2="260" y2="165" stroke="#7a6030" stroke-width="1" stroke-dasharray="4,3"/>
          <text x="235" y="33" fill="#7a6030" font-size="8" font-family="JetBrains Mono">y=bx/a</text>
          <text x="220" y="170" fill="#7a6030" font-size="8" font-family="JetBrains Mono">y=−bx/a</text>
          <!-- right branch -->
          <path d="M185,10 Q170,45 168,100 Q170,155 185,190" fill="none" stroke="#c9a84c" stroke-width="2"/>
          <!-- left branch -->
          <path d="M95,10 Q110,45 112,100 Q110,155 95,190" fill="none" stroke="#c9a84c" stroke-width="2"/>
          <!-- vertices -->
          <circle cx="168" cy="100" r="3" fill="#4ecdc4"/>
          <circle cx="112" cy="100" r="3" fill="#4ecdc4"/>
          <text x="170" y="97" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">A(a,0)</text>
          <text x="86" y="97" fill="#4ecdc4" font-size="9" font-family="JetBrains Mono">A'</text>
          <!-- foci -->
          <circle cx="194" cy="100" r="3.5" fill="#e8677a"/>
          <circle cx="86" cy="100" r="3.5" fill="#e8677a"/>
          <text x="195" y="114" fill="#e8677a" font-size="8" font-family="JetBrains Mono">S(c,0)</text>
          <!-- conjugate axis -->
          <line x1="140" y1="65" x2="140" y2="135" stroke="#a78bfa" stroke-width="1" stroke-dasharray="2,2"/>
          <text x="143" y="63" fill="#a78bfa" font-size="8" font-family="JetBrains Mono">b</text>
        </svg>
      </div>
      <p class="diagram-cap">Hyperbola: |PF₁−PF₂|=2a; asymptotes y=±(b/a)x</p>
      <hr class="divider">
      <code class="formula gold">c² = a²+b²,   e = c/a &gt; 1</code>
      <p>Foci: <code class="formula">(±c,0)</code>&nbsp; Vertices: <code class="formula">(±a,0)</code></p>
      <p>Directrices: <code class="formula rose">x = ±a/e</code>&nbsp; LR: <code class="formula teal">2b²/a</code></p>
      <p>Asymptotes: <code class="formula">y = ±(b/a)x</code></p>
      <p>Parametric: <code class="formula">(a secθ, b tanθ)</code> or <code class="formula">(a cosh t, b sinh t)</code></p>
    </div>

    <div class="card rose">
      <h3>Tangent & Normal — Hyperbola</h3>
      <p>Tangent at (x₁,y₁):</p>
      <code class="formula gold">xx₁/a² − yy₁/b² = 1</code>
      <p>Tangent with slope m:</p>
      <code class="formula rose">y = mx ± √(a²m²−b²)  [m² &gt; b²/a²]</code>
      <p>Normal at (x₁,y₁):</p>
      <code class="formula">a²x/x₁ + b²y/y₁ = a²+b²</code>
      <p><strong>Combined equation of asymptotes:</strong></p>
      <code class="formula teal">x²/a² − y²/b² = 0</code>
      <p><strong>Hyperbola − Asymptotes pair:</strong> difference = 1</p>
      <code class="formula violet">S(hyperbola) − S(asym. pair) = 1</code>
      <p><strong>Rectangular hyperbola:</strong> a=b ⟹ xy=c² (rotated 45°)</p>
      <code class="formula green">xy = c²; parametric: (ct, c/t)</code>
    </div>
  </div>

  <div class="grid grid-2" style="margin-top:1.2rem">
    <div class="card violet">
      <h3>Rectangular Hyperbola xy = c² <span class="tag adv">ADV</span></h3>
      <p>Tangent at (ct, c/t):</p>
      <code class="formula violet">x/t + yt = 2c</code>
      <p>Normal at (ct, c/t):</p>
      <code class="formula">xt³ − yt − ct⁴ + c = 0</code>
      <p>Chord with midpoint (h,k):</p>
      <code class="formula rose">kx + hy = 2hk</code>
      <p>If chord joins t₁,t₂: <code class="formula">t₁t₂ = −1</code> for normal chord.</p>
      <p>Intersection of normals at t₁,t₂,t₃,t₄ on xy=c²:</p>
      <code class="formula teal">t₁t₂t₃t₄ = 1</code>
    </div>
    <div class="card sky">
      <h3>Properties <span class="tag adv">ADV</span></h3>
      <ul class="props">
        <li>|PF₁−PF₂| = 2a (definition)</li>
        <li>Tangent bisects angle between focal radii externally</li>
        <li>Conjugate hyperbola: −x²/a²+y²/b²=1, same asymptotes</li>
        <li>e₁²+e₂² for conjugate pair: 1/e₁²+1/e₂²=1</li>
        <li>Director circle: x²+y²=a²−b² (real only if a&gt;b)</li>
        <li>For RH: eccentricity = √2, asymptotes ⊥ each other</li>
      </ul>
    </div>
  </div>
</section>

<!-- ══════════════════ 7. PAIR OF LINES ══════════════════ -->
<section class="section" id="pair">
  <div class="section-header">
    <span class="section-num">07</span>
    <h2 class="section-title">Pair of Straight Lines</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>General Second Degree Equation</h3>
      <p>ax²+2hxy+by²+2gx+2fy+c=0 represents a pair of lines if:</p>
      <code class="formula gold">Δ = abc + 2fgh − af² − bg² − ch² = 0</code>
      <p>i.e., <code class="formula">det [[a,h,g],[h,b,f],[g,f,c]] = 0</code></p>
      <p><strong>Homogeneous second degree:</strong> ax²+2hxy+by²=0</p>
      <p>Slopes m₁,m₂ satisfy:</p>
      <code class="formula teal">m₁+m₂ = −2h/b,   m₁m₂ = a/b</code>
      <p>Angle between lines:</p>
      <code class="formula rose">tanθ = 2√(h²−ab)/(a+b)</code>
      <p>Perpendicular if a+b=0; coincident if h²=ab.</p>
    </div>

    <div class="card rose">
      <h3>Angle Bisectors of ax²+2hxy+by²=0</h3>
      <code class="formula gold">(x²−y²)/(a−b) = xy/h</code>
      <div class="note">These bisectors are always perpendicular to each other.</div>
      <p>If ax²+2hxy+by²=0 represents lines L₁ and L₂, then:</p>
      <ul class="props">
        <li>Combined equation of lines ⊥ to L₁,L₂ through origin: bx²−2hxy+ay²=0</li>
        <li>Lines parallel at distance d: (a+b)²d² = 4(h²−ab)(g²−ac)</li>
      </ul>

      <div class="diagram-wrap">
        <svg viewBox="0 0 240 180" width="240" height="180" xmlns="http://www.w3.org/2000/svg">
          <!-- axes -->
          <line x1="20" y1="90" x2="220" y2="90" stroke="#2a2f3e" stroke-width="1"/>
          <line x1="120" y1="10" x2="120" y2="170" stroke="#2a2f3e" stroke-width="1"/>
          <!-- two lines through origin -->
          <line x1="20" y1="155" x2="220" y2="25" stroke="#c9a84c" stroke-width="1.5"/>
          <line x1="20" y1="30" x2="220" y2="150" stroke="#4ecdc4" stroke-width="1.5"/>
          <!-- bisectors (45° ish) -->
          <line x1="20" y1="90" x2="220" y2="90" stroke="#e8677a" stroke-width="1" stroke-dasharray="4,3" opacity="0.5"/>
          <line x1="120" y1="10" x2="120" y2="170" stroke="#e8677a" stroke-width="1" stroke-dasharray="4,3" opacity="0.5"/>
          <!-- angles -->
          <path d="M145,90 A25,25 0 0 0 133,68" fill="none" stroke="#a78bfa" stroke-width="1"/>
          <text x="148" y="80" fill="#a78bfa" font-size="8" font-family="JetBrains Mono">θ</text>
          <!-- origin -->
          <circle cx="120" cy="90" r="3" fill="white"/>
          <text x="106" y="106" fill="#8a8578" font-size="9" font-family="JetBrains Mono">O</text>
          <!-- labels -->
          <text x="200" y="22" fill="#c9a84c" font-size="8" font-family="JetBrains Mono">L₁</text>
          <text x="200" y="155" fill="#4ecdc4" font-size="8" font-family="JetBrains Mono">L₂</text>
          <text x="200" y="87" fill="#e8677a" font-size="8" font-family="JetBrains Mono">bisectors</text>
        </svg>
      </div>
      <p class="diagram-cap">Pair of lines through origin with their angle bisectors (⊥ each other)</p>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Condition — Conic Types</h3>
      <p>For ax²+2hxy+by²+2gx+2fy+c=0:</p>
      <ul class="props">
        <li>Δ≠0, h²=ab: parabola</li>
        <li>Δ≠0, h²&lt;ab: ellipse (a+b &gt; 0 real)</li>
        <li>Δ≠0, h²&gt;ab: hyperbola</li>
        <li>Δ≠0, h²&gt;ab, a+b=0: rectangular hyperbola</li>
        <li>Δ=0: degenerate (line pair, point, or ∅)</li>
      </ul>
    </div>
    <div class="card green">
      <h3>Distance Between Parallel Lines</h3>
      <p>From ax²+2hxy+by²+2gx+2fy+c=0 (when it's a parallel pair):</p>
      <code class="formula green">d = 2√(g²−ac) / √(a(a+b))</code>
      <p>or for y-direction:</p>
      <code class="formula">d = 2√(f²−bc) / √(b(a+b))</code>
    </div>
    <div class="card violet">
      <h3>Joint Equation — Lines through Two Points</h3>
      <p>Lines joining origin to intersection of S=0 and lx+my=1:</p>
      <code class="formula violet">S(x,y) − (lx+my)² · [terms] = 0</code>
      <p>This is the homogenisation method used to find the combined equation of OA and OB where A,B lie on the conic.</p>
    </div>
  </div>
</section>

<!-- ══════════════════ 8. MISC ══════════════════ -->
<section class="section" id="misc">
  <div class="section-header">
    <span class="section-num">08</span>
    <h2 class="section-title">Miscellaneous Properties</h2>
  </div>

  <div class="grid grid-2">
    <div class="card">
      <h3>Comparison of Conics</h3>
      <div style="overflow-x:auto">
        <table style="border-collapse:collapse;width:100%;font-family:'JetBrains Mono',monospace;font-size:0.75rem;color:var(--text-mid);">
          <tr style="background:var(--surface2);color:var(--gold)">
            <th style="padding:0.4rem 0.6rem;border:1px solid var(--border);text-align:left">Property</th>
            <th style="padding:0.4rem 0.6rem;border:1px solid var(--border)">Parabola</th>
            <th style="padding:0.4rem 0.6rem;border:1px solid var(--border)">Ellipse</th>
            <th style="padding:0.4rem 0.6rem;border:1px solid var(--border)">Hyperbola</th>
          </tr>
          <tr>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">e</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border);color:#4ecdc4">e = 1</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border);color:#6ee7b7">e &lt; 1</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border);color:#e8677a">e &gt; 1</td>
          </tr>
          <tr style="background:rgba(26,30,40,0.5)">
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">Foci</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">1</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">2</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">2</td>
          </tr>
          <tr>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">Asymptotes</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">0</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">0</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">2</td>
          </tr>
          <tr style="background:rgba(26,30,40,0.5)">
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">LR</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">4a</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">2b²/a</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">2b²/a</td>
          </tr>
          <tr>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">Director circle</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">Directrix</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">x²+y²=a²+b²</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">x²+y²=a²−b²</td>
          </tr>
          <tr style="background:rgba(26,30,40,0.5)">
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">Tangent slope</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">c=a/m</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">c²=a²m²+b²</td>
            <td style="padding:0.35rem 0.6rem;border:1px solid var(--border)">c²=a²m²−b²</td>
          </tr>
        </table>
      </div>
    </div>

    <div class="card violet">
      <h3>Important JEE Loci <span class="tag imp">IMP</span></h3>
      <ul class="props">
        <li><strong>Apollonius circle:</strong> PA/PB=k (k≠1) ⟹ circle</li>
        <li><strong>⊥ from focus to tangent</strong> of parabola ⟹ lies on tangent at vertex</li>
        <li><strong>Circumcircle of triangle formed by tangents</strong> to parabola ⟹ passes through focus</li>
        <li><strong>Orthocentre of triangle inscribed in RH</strong> xy=c² ⟹ also lies on xy=c²</li>
        <li><strong>Midpoint of focal chord</strong> of y²=4ax ⟹ parabola y²=2a(x−a)</li>
        <li><strong>Reflection of focus</strong> in any tangent to parabola ⟹ lies on directrix</li>
        <li><strong>Pole-Polar:</strong> polar of (h,k) w.r.t conic S: T(h,k)=0</li>
      </ul>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card sky">
      <h3>Pole & Polar</h3>
      <p>Polar of point P(h,k) with respect to conic S=0 is T(h,k)=0.</p>
      <p>For circle x²+y²=r²:</p>
      <code class="formula sky">hx + ky = r²</code>
      <p>For ellipse x²/a²+y²/b²=1:</p>
      <code class="formula">hx/a² + ky/b² = 1</code>
      <div class="note"><strong>Self-polar triangle:</strong> each vertex is pole of opposite side.</div>
    </div>
    <div class="card green">
      <h3>T = S₁ Rule <span class="tag imp">IMP</span></h3>
      <p>For any conic S=0, the chord with midpoint (h,k):</p>
      <code class="formula green">T(h,k) = S(h,k)</code>
      <p>Applies to all conics uniformly. T is obtained by replacing x²→xx₁, y²→yy₁, x→(x+x₁)/2, y→(y+y₁)/2.</p>
    </div>
    <div class="card rose">
      <h3>Common Tangent Tricks <span class="tag adv">ADV</span></h3>
      <p>Common internal tangents: found by finding transverse/internal centre of similitude.</p>
      <p>For y²=4ax and circle x²+y²=r²:</p>
      <p>Tangent y=mx+a/m must satisfy distance from centre = r:</p>
      <code class="formula rose">|a/m| / √(1+m²) = r</code>
      <p>Solve for m to get common tangents.</p>
    </div>
  </div>

  <div class="grid grid-2" style="margin-top:1.2rem">
    <div class="card">
      <h3>Key Proofs Synopsis <span class="tag adv">ADV</span></h3>
      <p><strong>1. Tangent perpendicular to radius (Circle):</strong> Differentiate x²+y²=r² implicitly to get dy/dx=−x/y; slope of radius =y/x; product=−1. ✓</p>
      <p><strong>2. Reflection property of parabola:</strong> Show normal bisects angle between focal radius and the axis-parallel direction using the slope identity tanα = 1/t at point (at²,2at).</p>
      <p><strong>3. Sum of focal distances = 2a (Ellipse):</strong> SP=a−ex₁, S'P=a+ex₁; sum = 2a. Follows directly from focus-directrix definition.</p>
      <p><strong>4. Asymptotes of hyperbola:</strong> Find limit as points recede to infinity on hyperbola; y/x → ±b/a. Combined equation x²/a²−y²/b²=0.</p>
    </div>
    <div class="card teal">
      <h3>Quick Recall — Eccentricity</h3>
      <div class="diagram-wrap">
        <svg viewBox="0 0 260 140" width="260" height="140" xmlns="http://www.w3.org/2000/svg">
          <!-- number line for e -->
          <line x1="20" y1="70" x2="240" y2="70" stroke="#4ecdc4" stroke-width="1.5"/>
          <!-- marks -->
          <line x1="20" y1="60" x2="20" y2="80" stroke="#4ecdc4" stroke-width="1.5"/>
          <line x1="100" y1="60" x2="100" y2="80" stroke="#c9a84c" stroke-width="1.5"/>
          <line x1="180" y1="60" x2="180" y2="80" stroke="#c9a84c" stroke-width="1.5"/>
          <line x1="240" y1="60" x2="240" y2="80" stroke="#4ecdc4" stroke-width="1.5"/>
          <!-- labels -->
          <text x="16" y="55" fill="#8a8578" font-size="10" font-family="JetBrains Mono">0</text>
          <text x="96" y="55" fill="#c9a84c" font-size="10" font-family="JetBrains Mono">1</text>
          <text x="175" y="55" fill="#c9a84c" font-size="10" font-family="JetBrains Mono">√2</text>
          <text x="234" y="55" fill="#8a8578" font-size="10" font-family="JetBrains Mono">∞</text>
          <!-- regions -->
          <text x="28" y="95" fill="#6ee7b7" font-size="9" font-family="JetBrains Mono">Circle(e=0)</text>
          <text x="22" y="108" fill="#6ee7b7" font-size="9" font-family="JetBrains Mono">Ellipse (0&lt;e&lt;1)</text>
          <text x="94" y="95" fill="#e8c97a" font-size="9" font-family="JetBrains Mono">Parabola(e=1)</text>
          <text x="145" y="108" fill="#e8677a" font-size="9" font-family="JetBrains Mono">Hyperbola(e&gt;1)</text>
          <text x="168" y="122" fill="#a78bfa" font-size="9" font-family="JetBrains Mono">RH(e=√2)</text>
          <!-- arrows -->
          <polygon points="236,70 228,65 228,75" fill="#4ecdc4"/>
        </svg>
      </div>
      <p class="diagram-cap">Eccentricity number line for conic classification</p>
      <code class="formula gold">e = c/a;  c²=a²−b² (ellipse), c²=a²+b² (hyperbola)</code>
    </div>
  </div>

  <div class="grid grid-3" style="margin-top:1.2rem">
    <div class="card">
      <h3>Shift / Translation of Conics</h3>
      <p>Shifting vertex/centre to (h,k): replace x→x−h, y→y−k.</p>
      <p>E.g., parabola with vertex (h,k) opening right:</p>
      <code class="formula">(y−k)² = 4a(x−h)</code>
      <p>Ellipse with centre (h,k):</p>
      <code class="formula">(x−h)²/a²+(y−k)²/b²=1</code>
    </div>
    <div class="card rose">
      <h3>Parametric — All Conics</h3>
      <ul class="props">
        <li>Circle x²+y²=r²: (r cosθ, r sinθ)</li>
        <li>Parabola y²=4ax: (at², 2at)</li>
        <li>Ellipse x²/a²+y²/b²=1: (a cosθ, b sinθ)</li>
        <li>Hyperbola x²/a²−y²/b²=1: (a secθ, b tanθ)</li>
        <li>RH xy=c²: (ct, c/t)</li>
      </ul>
    </div>
    <div class="card sky">
      <h3>Number of Normals <span class="tag adv">ADV</span></h3>
      <p>From an external point, max normals that can be drawn:</p>
      <ul class="props">
        <li>Circle: 1 normal (through centre)</li>
        <li>Parabola: 3 normals (cubic in t)</li>
        <li>Ellipse: 4 normals</li>
        <li>Hyperbola: 4 normals</li>
      </ul>
      <p>For parabola, 3 normals through (h,k) iff h &gt; 2a.</p>
    </div>
  </div>

  <!-- final important results -->
  <div class="card" style="margin-top:1.2rem;border-color:var(--gold-dim)">
    <h3>★ Most Important JEE Results (Quick Fire)</h3>
    <div class="grid grid-3">
      <div>
        <p style="font-family:'JetBrains Mono',monospace;font-size:0.8rem;color:var(--gold);margin-bottom:0.4rem">CIRCLES</p>
        <code class="formula gold" style="white-space:normal">Length of tangent = √S₁</code>
        <code class="formula" style="white-space:normal">Radical axis ⊥ line of centres</code>
        <code class="formula teal" style="white-space:normal">Orthogonal: 2g₁g₂+2f₁f₂=c₁+c₂</code>
      </div>
      <div>
        <p style="font-family:'JetBrains Mono',monospace;font-size:0.8rem;color:var(--teal);margin-bottom:0.4rem">PARABOLA</p>
        <code class="formula teal" style="white-space:normal">t₁t₂=−1 (focal chord)</code>
        <code class="formula" style="white-space:normal">Tangent: ty = x+at²</code>
        <code class="formula rose" style="white-space:normal">Normal: y=−tx+2at+at³</code>
      </div>
      <div>
        <p style="font-family:'JetBrains Mono',monospace;font-size:0.8rem;color:var(--rose);margin-bottom:0.4rem">ELLIPSE/HYPERBOLA</p>
        <code class="formula rose" style="white-space:normal">PF₁+PF₂=2a (ellipse)</code>
        <code class="formula" style="white-space:normal">|PF₁−PF₂|=2a (hyperbola)</code>
        <code class="formula violet" style="white-space:normal">Director circle: x²+y²=a²±b²</code>
      </div>
    </div>
  </div>
</section>

</main>

<footer style="text-align:center;padding:2rem;border-top:1px solid var(--border);font-family:'JetBrains Mono',monospace;font-size:0.7rem;color:var(--text-dim);">
  Coordinate Geometry · JEE Advanced & Mains Reference · All key formulae, loci &amp; properties
</footer></div></div>
<div class="psec" id="sec-conic"><div id="conic-inner">
    <div id="app">

<!-- ══ CANVAS ══ -->
<div id="canvas-wrap">
  <canvas id="cvs"></canvas>
  <div id="draw-indicator">✏ DRAW MODE — TAP TO PLOT POINTS</div>
  <div id="coord-bar">
    <div>x: <span id="cx-val">0.00</span>  y: <span id="cy-val">0.00</span></div>
    <div style="color:var(--text3);font-size:0.55rem" id="sel-info">no selection</div>
  </div>
  <div id="zoom-btns">
    <button class="zbtn" onclick="zoomIn()">＋</button>
    <button class="zbtn" onclick="zoomOut()">－</button>
    <button class="zbtn" onclick="resetView()" title="Reset">⌖</button>
  </div>
  <div id="tip"></div>
</div>

<!-- ══ SIDEBAR ══ -->
<div id="sidebar">
  <div id="sidebar-toggle" onclick="toggleSidebar()">
    <span></span><span></span><span></span>
    <div id="toggle-arrow">◀</div>
  </div>

  <div id="hdr">
    <h1>⬡ ConicLab</h1>
    <p>INTERACTIVE GEOMETRY ENGINE · JEE</p>
  </div>

  <div id="tabs">
    <div class="tab active" onclick="switchTab('curves')">Curves</div>
    <div class="tab" onclick="switchTab('settings')">Settings</div>
    <div class="tab" onclick="switchTab('help')">Help</div>
  </div>

  <!-- CURVES -->
  <div id="tab-curves" style="display:flex;flex-direction:column;flex:1;overflow:hidden;">
    <div style="padding:8px 10px 0;flex-shrink:0;">
      <div class="add-row">
        <select id="curve-type-sel">
          <optgroup label="── Lines ──">
            <option value="line">Line  y = mx + c</option>
            <option value="line_g">Line  ax + by + c = 0</option>
          </optgroup>
          <optgroup label="── Circles ──">
            <option value="circle">Circle</option>
          </optgroup>
          <optgroup label="── Parabolas ──">
            <option value="para_r">Parabola y²= 4ax  →</option>
            <option value="para_l">Parabola y²=−4ax  ←</option>
            <option value="para_u">Parabola x²= 4ay  ↑</option>
            <option value="para_d">Parabola x²=−4ay  ↓</option>
          </optgroup>
          <optgroup label="── Ellipses ──">
            <option value="ellipse">Ellipse  x²/a²+y²/b²=1</option>
          </optgroup>
          <optgroup label="── Hyperbolas ──">
            <option value="hyp">Hyperbola  x²/a²−y²/b²=1</option>
            <option value="hyp_c">Conj. Hyperbola</option>
            <option value="rhyp">Rect. Hyperbola  xy=c²</option>
          </optgroup>
          <optgroup label="── Special ──">
            <option value="pt">Point</option>
          </optgroup>
        </select>
        <button class="btn-add" onclick="addCurve()">＋ ADD</button>
      </div>
    </div>
    <div id="panel-body">
      <div id="curves-list">
        <div id="empty-hint"><div class="ico">📐</div>Add a curve above.<br>Sidebar auto-hides on tap canvas.<br>Unlimited curves, tangents & normals.</div>
      </div>
    </div>
  </div>

  <!-- SETTINGS -->
  <div id="tab-settings">
    <div class="sg">
      <h4>Grid</h4>
      <div class="srow"><label>Grid unit</label><input type="range" id="sg-grid" min="20" max="150" value="60" oninput="S.gridPx=+this.value;updateSpan('sgv-grid',this.value);redraw()"><span id="sgv-grid">60</span></div>
      <div class="srow"><label>Show grid</label><input type="checkbox" id="sg-sg" checked onchange="S.showGrid=this.checked;redraw()"></div>
      <div class="srow"><label>Axis labels</label><input type="checkbox" id="sg-al" checked onchange="S.axisLabels=this.checked;redraw()"></div>
    </div>
    <div class="sg">
      <h4>Curves</h4>
      <div class="srow"><label>Line width</label><input type="range" id="sg-lw" min="1" max="5" step="0.5" value="2" oninput="S.lw=+this.value;updateSpan('sgv-lw',this.value);redraw()"><span id="sgv-lw">2</span></div>
      <div class="srow"><label>Show foci</label><input type="checkbox" id="sg-foci" checked onchange="S.foci=this.checked;redraw()"></div>
      <div class="srow"><label>Show vertices</label><input type="checkbox" id="sg-verts" checked onchange="S.verts=this.checked;redraw()"></div>
      <div class="srow"><label>Asymptotes</label><input type="checkbox" id="sg-asym" checked onchange="S.asym=this.checked;redraw()"></div>
      <div class="srow"><label>Directrices</label><input type="checkbox" id="sg-dir" checked onchange="S.dir=this.checked;redraw()"></div>
      <div class="srow"><label>Curve labels</label><input type="checkbox" id="sg-lbl" checked onchange="S.curveLabels=this.checked;redraw()"></div>
    </div>
  </div>

  <!-- HELP -->
  <div id="tab-help">
    <div style="font-size:0.66rem;line-height:1.9;color:var(--text2);">
      <div style="color:var(--gold);font-weight:600;margin-bottom:6px;font-size:0.68rem;">NAVIGATION</div>
      📱 Tap ◀ tab → hide sidebar for full canvas<br>
      🖱 Scroll / pinch → zoom<br>
      🖱 Drag → pan<br>
      <br>
      <div style="color:var(--gold);font-weight:600;margin-bottom:6px;">DRAWING TOOLS</div>
      ✏ <b>Draw mode</b> (toolbar) → tap/click on canvas to drop points that form your curve<br>
      📐 <b>Two-point line</b> → click 2 points on canvas<br>
      ⭕ <b>Circle</b> → click centre then radius point<br>
      <br>
      <div style="color:var(--gold);font-weight:600;margin-bottom:6px;">DIRECT INPUT</div>
      Each curve has an <b>Equation</b> box where you can type the equation directly, e.g.:<br>
      <span style="color:var(--teal)">y = 2x + 3</span><br>
      <span style="color:var(--teal)">a=3 b=2 h=1 k=-1</span><br>
      Parameters have both <b>sliders</b> AND <b>typed input</b> — type any number, no limits.<br>
      <br>
      <div style="color:var(--gold);font-weight:600;margin-bottom:6px;">TANGENT & NORMAL</div>
      Enter parameter t (or angle θ) → Draw<br>
      <span style="color:var(--teal)">━━</span> Tangent &nbsp; <span style="color:var(--orange)">┄┄</span> Normal<br>
      <br>
      <div style="color:var(--gold);font-weight:600;margin-bottom:6px;">KEYBOARD</div>
      R = reset view &nbsp; G = grid &nbsp; H = hide sidebar<br>
      Del = remove selected curve
    </div>
  </div>

  <div id="statusbar">
    <span id="curve-count">0 curves</span>
    <span id="mode-display">PAN MODE</span>
  </div>
</div>

<!-- ══ FLOATING TOOLBAR ══ -->
<div id="ctoolbar">
  <button class="ctb active" id="tb-pan" onclick="setMode('pan')" title="Pan">🖐 Pan</button>
  <div class="ctb-sep"></div>
  <button class="ctb" id="tb-draw-line" onclick="setMode('draw_line')" title="Draw line by 2 points">📏 Line</button>
  <button class="ctb" id="tb-draw-circle" onclick="setMode('draw_circle')" title="Draw circle">⭕ Circle</button>
  <button class="ctb" id="tb-draw-point" onclick="setMode('draw_point')" title="Plot points">✦ Point</button>
  <div class="ctb-sep"></div>
  <button class="ctb" id="tb-clear" onclick="clearAll()" title="Clear all">🗑</button>
  <button class="ctb" id="tb-grid" onclick="toggleGrid()" title="Grid">⊞</button>
</div>

</div><!-- #app -->


  </div></div>
<div class="psec" id="sec-const"><div class="cwrap"><div class="shero" style="--sc:rgba(34,211,238,.08)"><span class="shero-badge">04 — Physics &amp; Chemistry</span><h2 style="color:#22d3ee">Constants · Logs · Molar Masses</h2><p>Physical constants · logarithm tables · inductive &amp; mesomeric effects</p></div><div class="page">

  <!-- HEADER -->
  <div class="header">
    <div class="header-line"><div class="dot"></div></div>
    <h1>
      <div class="h1-line1">Constants · Logs · Molar Masses</div>
      <div class="h1-line2">Inductive & Mesomeric Effects</div>
    </h1>
    <p class="sub">JEE Mains & Advanced · Complete Reference</p>
    <div class="pills">
      <span class="pill p-cyan">Physical Constants</span>
      <span class="pill p-amber">Log Values</span>
      <span class="pill p-green">Molar Masses</span>
      <span class="pill p-vio">Mesomeric Effects</span>
      <span class="pill p-red">Inductive Effects</span>
    </div>
  </div>


  <!-- PHYSICAL CONSTANTS -->
  <div class="sec">
    <div class="sec-head">
      <div class="sec-icon" style="background:rgba(34,211,238,0.1)">⚛️</div>
      <span class="sec-label" style="color:var(--cyan)">Physical Constants</span>
      <div class="sec-rule"></div>
    </div>
    <div class="g3">
      <!-- Fundamental -->
      <div class="card">
        <div class="card-header">Fundamental</div>
        <div class="const-row"><span class="const-name">Speed of light</span><span class="const-sym">c</span><span class="const-val cv-cyan">3×10⁸ m/s</span></div>
        <div class="const-row"><span class="const-name">Planck's constant</span><span class="const-sym">h</span><span class="const-val cv-amber">6.626×10⁻³⁴ J·s</span></div>
        <div class="const-row"><span class="const-name">Avogadro's no.</span><span class="const-sym">Nₐ</span><span class="const-val cv-green">6.022×10²³</span></div>
        <div class="const-row"><span class="const-name">Boltzmann const.</span><span class="const-sym">k</span><span class="const-val cv-vio">1.38×10⁻²³ J/K</span></div>
        <div class="const-row"><span class="const-name">Electron charge</span><span class="const-sym">e</span><span class="const-val cv-red">1.6×10⁻¹⁹ C</span></div>
        <div class="const-row"><span class="const-name">Electron mass</span><span class="const-sym">mₑ</span><span class="const-val cv-orange">9.1×10⁻³¹ kg</span></div>
        <div class="const-row"><span class="const-name">Proton mass</span><span class="const-sym">mₚ</span><span class="const-val cv-blue">1.67×10⁻²⁷ kg</span></div>
      </div>
      <!-- Electro & Thermal -->
      <div class="card">
        <div class="card-header">Electro &amp; Thermal</div>
        <div class="const-row"><span class="const-name">Coulomb const.</span><span class="const-sym">k</span><span class="const-val cv-cyan">9×10⁹ N·m²/C²</span></div>
        <div class="const-row"><span class="const-name">ε₀ (permittivity)</span><span class="const-sym">ε₀</span><span class="const-val cv-amber">8.85×10⁻¹² F/m</span></div>
        <div class="const-row"><span class="const-name">μ₀ (permeability)</span><span class="const-sym">μ₀</span><span class="const-val cv-green">4π×10⁻⁷ T·m/A</span></div>
        <div class="const-row"><span class="const-name">Faraday's const.</span><span class="const-sym">F</span><span class="const-val cv-vio">96500 C/mol</span></div>
        <div class="const-row"><span class="const-name">Gas constant R</span><span class="const-sym">R</span><span class="const-val cv-red">8.314 J/mol·K</span></div>
        <div class="const-row"><span class="const-name">R (alt)</span><span class="const-sym">R</span><span class="const-val cv-red">0.0821 L·atm/mol·K</span></div>
        <div class="const-row"><span class="const-name">Stefan-Boltzmann</span><span class="const-sym">σ</span><span class="const-val cv-orange">5.67×10⁻⁸ W/m²K⁴</span></div>
      </div>
      <!-- Atomic & Nuclear -->
      <div class="card">
        <div class="card-header">Atomic &amp; Nuclear</div>
        <div class="const-row"><span class="const-name">1 eV</span><span class="const-sym">—</span><span class="const-val cv-cyan">1.6×10⁻¹⁹ J</span></div>
        <div class="const-row"><span class="const-name">1 amu</span><span class="const-sym">—</span><span class="const-val cv-amber">1.66×10⁻²⁷ kg</span></div>
        <div class="const-row"><span class="const-name">Rydberg const.</span><span class="const-sym">R∞</span><span class="const-val cv-green">1.097×10⁷ m⁻¹</span></div>
        <div class="const-row"><span class="const-name">Bohr radius</span><span class="const-sym">a₀</span><span class="const-val cv-vio">0.529 Å</span></div>
        <div class="const-row"><span class="const-name">g (gravity)</span><span class="const-sym">g</span><span class="const-val cv-red">9.8 ≈ 10 m/s²</span></div>
        <div class="const-row"><span class="const-name">Speed of sound</span><span class="const-sym">—</span><span class="const-val cv-orange">340 m/s</span></div>
        <div class="const-row"><span class="const-name">Escape velocity</span><span class="const-sym">vₑ</span><span class="const-val cv-blue">11.2 km/s</span></div>
      </div>
    </div>
  </div>


  <!-- LOG & LN VALUES -->
  <div class="sec">
    <div class="sec-head">
      <div class="sec-icon" style="background:rgba(251,191,36,0.1)">📊</div>
      <span class="sec-label" style="color:var(--amber)">Logarithm Values</span>
      <div class="sec-rule"></div>
    </div>
    <div class="g2">
      <div class="card">
        <table>
          <thead><tr><th>n</th><th style="color:var(--amber)">log₁₀(n)</th><th style="color:var(--green)">ln(n)</th><th style="color:var(--violet)">Derived from</th></tr></thead>
          <tbody>
            <tr class="hl"><td class="t-n">2</td><td class="t-log">0.3010</td><td class="t-ln">0.6931</td><td class="t-der">memorize</td></tr>
            <tr><td class="t-n">3</td><td class="t-log">0.4771</td><td class="t-ln">1.0986</td><td class="t-der">memorize</td></tr>
            <tr><td class="t-n">4</td><td class="t-log">0.6021</td><td class="t-ln">1.3863</td><td class="t-der">2 × log2</td></tr>
            <tr><td class="t-n">5</td><td class="t-log">0.6990</td><td class="t-ln">1.6094</td><td class="t-der">1 − log2</td></tr>
            <tr><td class="t-n">6</td><td class="t-log">0.7782</td><td class="t-ln">1.7918</td><td class="t-der">log2 + log3</td></tr>
            <tr class="hl"><td class="t-n">7</td><td class="t-log">0.8451</td><td class="t-ln">1.9459</td><td class="t-der">memorize</td></tr>
            <tr><td class="t-n">8</td><td class="t-log">0.9031</td><td class="t-ln">2.0794</td><td class="t-der">3 × log2</td></tr>
            <tr><td class="t-n">9</td><td class="t-log">0.9542</td><td class="t-ln">2.1972</td><td class="t-der">2 × log3</td></tr>
            <tr><td class="t-n">10</td><td class="t-log">1.0000</td><td class="t-ln">2.3026</td><td class="t-der">definition</td></tr>
          </tbody>
        </table>
      </div>
      <div>
        <div class="card" style="margin-bottom:12px">
          <div class="card-header">Key Natural Log Values</div>
          <div class="const-row"><span class="const-name">ln 2</span><span class="const-sym">—</span><span class="const-val cv-green">0.6931</span></div>
          <div class="const-row"><span class="const-name">ln 3</span><span class="const-sym">—</span><span class="const-val cv-green">1.0986</span></div>
          <div class="const-row"><span class="const-name">ln 5</span><span class="const-sym">—</span><span class="const-val cv-green">1.6094</span></div>
          <div class="const-row"><span class="const-name">ln 10</span><span class="const-sym">—</span><span class="const-val cv-green">2.3026</span></div>
          <div class="const-row"><span class="const-name">ln e = 1</span><span class="const-sym">—</span><span class="const-val cv-green">1.0000</span></div>
        </div>
        <div class="approx-grid">
          <div class="approx-cell"><div class="approx-expr">π</div><div class="approx-eq">≈</div><div class="approx-val">3.1416</div></div>
          <div class="approx-cell"><div class="approx-expr">π²</div><div class="approx-eq">≈</div><div class="approx-val">9.87 ≈ 10</div></div>
          <div class="approx-cell"><div class="approx-expr">e</div><div class="approx-eq">=</div><div class="approx-val">2.7183</div></div>
          <div class="approx-cell"><div class="approx-expr">1/e</div><div class="approx-eq">≈</div><div class="approx-val">0.3679</div></div>
          <div class="approx-cell"><div class="approx-expr">log π</div><div class="approx-eq">≈</div><div class="approx-val">0.4971</div></div>
          <div class="approx-cell"><div class="approx-expr">log e</div><div class="approx-eq">≈</div><div class="approx-val">0.4343</div></div>
        </div>
      </div>
    </div>
  </div>


  <!-- MOLAR MASSES -->
  <div class="sec">
    <div class="sec-head">
      <div class="sec-icon" style="background:rgba(74,222,128,0.08)">🧪</div>
      <span class="sec-label" style="color:var(--green)">Important Molar Masses (g/mol)</span>
      <div class="sec-rule"></div>
    </div>
    <div class="mol-grid">
      <div class="mol-cell"><div class="mol-formula">H₂</div><div class="mol-name">Hydrogen</div><div class="mol-mass">2</div></div>
      <div class="mol-cell"><div class="mol-formula">O₂</div><div class="mol-name">Oxygen</div><div class="mol-mass">32</div></div>
      <div class="mol-cell"><div class="mol-formula">N₂</div><div class="mol-name">Nitrogen</div><div class="mol-mass">28</div></div>
      <div class="mol-cell"><div class="mol-formula">Cl₂</div><div class="mol-name">Chlorine</div><div class="mol-mass">71</div></div>
      <div class="mol-cell"><div class="mol-formula">F₂</div><div class="mol-name">Fluorine</div><div class="mol-mass">38</div></div>
      <div class="mol-cell"><div class="mol-formula">Br₂</div><div class="mol-name">Bromine</div><div class="mol-mass">160</div></div>
      <div class="mol-cell"><div class="mol-formula">H₂O</div><div class="mol-name">Water</div><div class="mol-mass">18</div></div>
      <div class="mol-cell"><div class="mol-formula">CO₂</div><div class="mol-name">Carbon dioxide</div><div class="mol-mass">44</div></div>
      <div class="mol-cell"><div class="mol-formula">SO₂</div><div class="mol-name">Sulphur dioxide</div><div class="mol-mass">64</div></div>
      <div class="mol-cell"><div class="mol-formula">SO₃</div><div class="mol-name">Sulphur trioxide</div><div class="mol-mass">80</div></div>
      <div class="mol-cell"><div class="mol-formula">NH₃</div><div class="mol-name">Ammonia</div><div class="mol-mass">17</div></div>
      <div class="mol-cell"><div class="mol-formula">HCl</div><div class="mol-name">Hydrochloric acid</div><div class="mol-mass">36.5</div></div>
      <div class="mol-cell"><div class="mol-formula">HNO₃</div><div class="mol-name">Nitric acid</div><div class="mol-mass">63</div></div>
      <div class="mol-cell"><div class="mol-formula">H₂SO₄</div><div class="mol-name">Sulphuric acid</div><div class="mol-mass">98</div></div>
      <div class="mol-cell"><div class="mol-formula">H₃PO₄</div><div class="mol-name">Phosphoric acid</div><div class="mol-mass">98</div></div>
      <div class="mol-cell"><div class="mol-formula">NaCl</div><div class="mol-name">Sodium chloride</div><div class="mol-mass">58.5</div></div>
      <div class="mol-cell"><div class="mol-formula">NaOH</div><div class="mol-name">Sodium hydroxide</div><div class="mol-mass">40</div></div>
      <div class="mol-cell"><div class="mol-formula">KOH</div><div class="mol-name">Pot. hydroxide</div><div class="mol-mass">56</div></div>
      <div class="mol-cell"><div class="mol-formula">Ca(OH)₂</div><div class="mol-name">Slaked lime</div><div class="mol-mass">74</div></div>
      <div class="mol-cell"><div class="mol-formula">CaCO₃</div><div class="mol-name">Calcium carbonate</div><div class="mol-mass">100</div></div>
      <div class="mol-cell"><div class="mol-formula">Na₂CO₃</div><div class="mol-name">Washing soda</div><div class="mol-mass">106</div></div>
      <div class="mol-cell"><div class="mol-formula">NaHCO₃</div><div class="mol-name">Baking soda</div><div class="mol-mass">84</div></div>
      <div class="mol-cell"><div class="mol-formula">MnO₂</div><div class="mol-name">Manganese dioxide</div><div class="mol-mass">87</div></div>
      <div class="mol-cell"><div class="mol-formula">KMnO₄</div><div class="mol-name">Potassium permanganate</div><div class="mol-mass">158</div></div>
      <div class="mol-cell"><div class="mol-formula">K₂Cr₂O₇</div><div class="mol-name">Pot. dichromate</div><div class="mol-mass">294</div></div>
      <div class="mol-cell"><div class="mol-formula">FeSO₄</div><div class="mol-name">Ferrous sulphate</div><div class="mol-mass">152</div></div>
      <div class="mol-cell"><div class="mol-formula">Fe₂O₃</div><div class="mol-name">Ferric oxide</div><div class="mol-mass">160</div></div>
      <div class="mol-cell"><div class="mol-formula">CH₄</div><div class="mol-name">Methane</div><div class="mol-mass">16</div></div>
      <div class="mol-cell"><div class="mol-formula">C₂H₅OH</div><div class="mol-name">Ethanol</div><div class="mol-mass">46</div></div>
      <div class="mol-cell"><div class="mol-formula">C₆H₁₂O₆</div><div class="mol-name">Glucose</div><div class="mol-mass">180</div></div>
    </div>
  </div>


  <!-- INDUCTIVE EFFECT -->
  <div class="sec">
    <div class="sec-head">
      <div class="sec-icon" style="background:rgba(251,113,133,0.1)">⚡</div>
      <span class="sec-label" style="color:var(--red)">Inductive Effect — Order</span>
      <div class="sec-rule"></div>
    </div>
    <div class="g2">
      <!-- -I Effect -->
      <div class="effect-card">
        <div class="effect-header" style="color:var(--red)">−I Effect (electron withdrawing) · Stronger → Weaker</div>
        <div class="effect-body">
          <div class="effect-row">
            <span class="effect-label" style="color:var(--red)">−I</span>
            <div class="chain">
              <span class="grp gi">NR₃⁺</span><span class="arrow">></span>
              <span class="grp gi">NO₂</span><span class="arrow">></span>
              <span class="grp gi">CN</span><span class="arrow">></span>
              <span class="grp gi">SO₃H</span><span class="arrow">></span>
              <span class="grp gi">CHO</span><span class="arrow">></span>
              <span class="grp gi">CO</span><span class="arrow">></span>
              <span class="grp gi">COOH</span><span class="arrow">></span>
              <span class="grp gi">COCl</span>
            </div>
          </div>
          <div class="effect-row" style="margin-top:6px">
            <span class="effect-label" style="color:var(--red)"></span>
            <div class="chain">
              <span class="grp gi">CONH₂</span><span class="arrow">></span>
              <span class="grp gi">F</span><span class="arrow">></span>
              <span class="grp gi">Cl</span><span class="arrow">></span>
              <span class="grp gi">Br</span><span class="arrow">></span>
              <span class="grp gi">I</span><span class="arrow">></span>
              <span class="grp gi">OR</span><span class="arrow">></span>
              <span class="grp gi">OH</span><span class="arrow">></span>
              <span class="grp gi">NR₂</span><span class="arrow">></span>
              <span class="grp gi">NH₂</span><span class="arrow">></span>
              <span class="grp gi">C₆H₅</span>
            </div>
          </div>
          <div class="effect-note">
            <b>Halogens order:</b> F > Cl > Br > I (by electronegativity)<br>
            <b>Remember:</b> More electronegative atom = stronger −I effect<br>
            <b>Acids:</b> More −I groups on alpha carbon → stronger acid
          </div>
        </div>
      </div>
      <!-- +I Effect -->
      <div class="effect-card">
        <div class="effect-header" style="color:var(--green)">+I Effect (electron donating) · Stronger → Weaker</div>
        <div class="effect-body">
          <div class="effect-row">
            <span class="effect-label" style="color:var(--green)">+I</span>
            <div class="chain">
              <span class="grp gp">C(CH₃)₃</span><span class="arrow">></span>
              <span class="grp gp">CH(CH₃)₂</span><span class="arrow">></span>
              <span class="grp gp">C₂H₅</span><span class="arrow">></span>
              <span class="grp gp">CH₃</span><span class="arrow">></span>
              <span class="grp gp">H</span>
            </div>
          </div>
          <div class="effect-row" style="margin-top:8px">
            <span class="effect-label"></span>
            <div class="chain">
              <span class="grp gp">tert</span><span class="arrow">></span>
              <span class="grp gp">sec</span><span class="arrow">></span>
              <span class="grp gp">primary</span><span class="arrow">></span>
              <span class="grp gp">methyl</span>
            </div>
          </div>
          <div class="effect-note">
            <b>Rule:</b> More alkyl groups = stronger +I (hyperconjugation + induction)<br>
            <b>Bases:</b> More +I groups on N → stronger base (in gas phase)<br>
            <b>Stability:</b> tert carbocation > sec > primary > methyl
          </div>
        </div>
      </div>
    </div>
  </div>


  <!-- MESOMERIC EFFECT -->
  <div class="sec">
    <div class="sec-head">
      <div class="sec-icon" style="background:rgba(192,132,252,0.1)">🔀</div>
      <span class="sec-label" style="color:var(--violet)">Mesomeric (Resonance) Effect — Order</span>
      <div class="sec-rule"></div>
    </div>
    <div class="g2">
      <!-- -M Effect -->
      <div class="effect-card">
        <div class="effect-header" style="color:var(--orange)">−M Effect (electron withdrawing via resonance) · Stronger → Weaker</div>
        <div class="effect-body">
          <div class="effect-row">
            <span class="effect-label" style="color:var(--orange)">−M</span>
            <div class="chain">
              <span class="grp gm">NO₂</span><span class="arrow">></span>
              <span class="grp gm">CN</span><span class="arrow">></span>
              <span class="grp gm">CHO</span><span class="arrow">></span>
              <span class="grp gm">COR</span><span class="arrow">></span>
              <span class="grp gm">COOH</span><span class="arrow">></span>
              <span class="grp gm">COOR</span><span class="arrow">></span>
              <span class="grp gm">CONH₂</span><span class="arrow">></span>
              <span class="grp gm">SO₃H</span>
            </div>
          </div>
          <div class="effect-note">
            <b>−M groups</b> contain π bonds adjacent to the ring → pull electron density <i>away</i> from the ring via resonance.<br>
            <b>Directing:</b> −M groups are <b>meta</b> directors in EAS reactions.
          </div>
        </div>
      </div>
      <!-- +M Effect -->
      <div class="effect-card">
        <div class="effect-header" style="color:var(--violet)">+M Effect (electron donating via resonance) · Stronger → Weaker</div>
        <div class="effect-body">
          <div class="effect-row">
            <span class="effect-label" style="color:var(--violet)">+M</span>
            <div class="chain">
              <span class="grp gv">O⁻</span><span class="arrow">></span>
              <span class="grp gv">NH₂</span><span class="arrow">></span>
              <span class="grp gv">NR₂</span><span class="arrow">></span>
              <span class="grp gv">NHCOR</span><span class="arrow">></span>
              <span class="grp gv">OH</span><span class="arrow">></span>
              <span class="grp gv">OR</span><span class="arrow">></span>
              <span class="grp gv">OCOR</span><span class="arrow">></span>
              <span class="grp gv">F</span>
            </div>
          </div>
          <div class="effect-row" style="margin-top:6px">
            <span class="effect-label"></span>
            <div class="chain">
              <span class="grp gv">Cl</span><span class="arrow">></span>
              <span class="grp gv">Br</span><span class="arrow">></span>
              <span class="grp gv">I</span><span class="arrow">></span>
              <span class="grp gv">C₆H₅</span><span class="arrow">></span>
              <span class="grp gv">CH=CH₂</span>
            </div>
          </div>
          <div class="effect-note">
            <b>+M groups</b> donate lone pair into the ring → increase electron density.<br>
            <b>Directing:</b> +M groups are <b>ortho/para</b> directors in EAS reactions.<br>
            <b>Halogens:</b> −I but +M → overall weak deactivators, o/p directors.
          </div>
        </div>
      </div>
    </div>
    <!-- Combined note -->
    <div style="margin-top:14px; padding:14px 18px; background:var(--s2); border:1px solid var(--border2); border-radius:12px; border-left:4px solid var(--violet);">
      <div style="font-family:'Syne',sans-serif; font-size:0.85rem; font-weight:700; color:var(--violet); margin-bottom:8px;">⚡ Combined Effect Rules</div>
      <div style="display:grid; grid-template-columns:1fr 1fr; gap:10px; font-size:0.78rem; color:var(--soft); line-height:1.7;">
        <div>• <b style="color:var(--amber)">Halogens:</b> −I > +M → net EWG, but o/p director<br>
             • <b style="color:var(--amber)">OH / NH₂:</b> +M >> −I → net EDG, strong o/p director<br>
             • <b style="color:var(--amber)">NO₂:</b> −I + −M → very strong EWG, meta director</div>
        <div>• <b style="color:var(--amber)">Acidity:</b> EWG increases acidity; EDG decreases it<br>
             • <b style="color:var(--amber)">Basicity:</b> EDG on N increases basicity; EWG decreases it<br>
             • <b style="color:var(--amber)">Stability:</b> More resonance structures = more stable</div>
      </div>
    </div>
  </div>


  <!-- FOOTER -->
  <div class="footer">
    JEE Mains &amp; Advanced · Chemistry &amp; Physics · Complete Reference
    <br><span class="badge">Read · Understand · Apply ⚗️</span>
  </div>

</div></div></div>
<div class="psec" id="sec-cheat"><div class="cwrap"><div class="shero" style="--sc:rgba(245,200,66,.08)"><span class="shero-badge">05 — Speed Reference</span><h2 style="color:#f5c842">Mathematics Quick Tables</h2><p>Squares · cubes · roots · fractions · powers — memorize all</p></div><div class="page">

  <!-- HEADER -->
  <div class="header">
    <h1>JEE Mathematics<br>Quick Reference</h1>
    <p class="sub">Squares · Cubes · Roots · Fractions · Powers</p>
    <div class="tag-row">
      <span class="tag tag-gold">Mains</span>
      <span class="tag tag-teal">Advanced</span>
      <span class="tag tag-rose">Speed Boost</span>
      <span class="tag tag-lav">Memorize All</span>
    </div>
  </div>


  <!-- SQUARES & SQUARE ROOTS 1–30 -->
  <div class="section">
    <div class="section-title">
      <div class="icon icon-gold">🟨</div>
      <span style="color:var(--gold)">Squares & Square Roots</span>
      <div class="line"></div>
      <span style="font-size:0.75rem; color:var(--muted); font-family:'DM Sans'; font-weight:400;">n = 1 to 30</span>
    </div>
    <div class="card">
      <table>
        <thead>
          <tr>
            <th>n</th><th style="color:var(--gold)">n²</th><th style="color:var(--teal)">√n</th>
            <th>n</th><th style="color:var(--gold)">n²</th><th style="color:var(--teal)">√n</th>
            <th>n</th><th style="color:var(--gold)">n²</th><th style="color:var(--teal)">√n</th>
          </tr>
        </thead>
        <tbody>
          <tr class="highlight-row"><td class="n">1</td><td class="sq">1</td><td class="sqr">1.000</td><td class="n">11</td><td class="sq">121</td><td class="sqr">3.317</td><td class="n">21</td><td class="sq">441</td><td class="sqr">4.583</td></tr>
          <tr><td class="n">2</td><td class="sq">4</td><td class="sqr">1.414</td><td class="n">12</td><td class="sq">144</td><td class="sqr">3.464</td><td class="n">22</td><td class="sq">484</td><td class="sqr">4.690</td></tr>
          <tr><td class="n">3</td><td class="sq">9</td><td class="sqr">1.732</td><td class="n">13</td><td class="sq">169</td><td class="sqr">3.606</td><td class="n">23</td><td class="sq">529</td><td class="sqr">4.796</td></tr>
          <tr><td class="n">4</td><td class="sq">16</td><td class="sqr">2.000</td><td class="n">14</td><td class="sq">196</td><td class="sqr">3.742</td><td class="n">24</td><td class="sq">576</td><td class="sqr">4.899</td></tr>
          <tr><td class="n">5</td><td class="sq">25</td><td class="sqr">2.236</td><td class="n">15</td><td class="sq">225</td><td class="sqr">3.873</td><td class="n">25</td><td class="sq">625</td><td class="sqr">5.000</td></tr>
          <tr><td class="n">6</td><td class="sq">36</td><td class="sqr">2.449</td><td class="n">16</td><td class="sq">256</td><td class="sqr">4.000</td><td class="n">26</td><td class="sq">676</td><td class="sqr">5.099</td></tr>
          <tr><td class="n">7</td><td class="sq">49</td><td class="sqr">2.646</td><td class="n">17</td><td class="sq">289</td><td class="sqr">4.123</td><td class="n">27</td><td class="sq">729</td><td class="sqr">5.196</td></tr>
          <tr><td class="n">8</td><td class="sq">64</td><td class="sqr">2.828</td><td class="n">18</td><td class="sq">324</td><td class="sqr">4.243</td><td class="n">28</td><td class="sq">784</td><td class="sqr">5.292</td></tr>
          <tr><td class="n">9</td><td class="sq">81</td><td class="sqr">3.000</td><td class="n">19</td><td class="sq">361</td><td class="sqr">4.359</td><td class="n">29</td><td class="sq">841</td><td class="sqr">5.385</td></tr>
          <tr><td class="n">10</td><td class="sq">100</td><td class="sqr">3.162</td><td class="n">20</td><td class="sq">400</td><td class="sqr">4.472</td><td class="n">30</td><td class="sq">900</td><td class="sqr">5.477</td></tr>
        </tbody>
      </table>
    </div>
  </div>


  <!-- CUBES & CUBE ROOTS 1–20 -->
  <div class="section">
    <div class="section-title">
      <div class="icon icon-rose">🟥</div>
      <span style="color:var(--rose)">Cubes & Cube Roots</span>
      <div class="line"></div>
      <span style="font-size:0.75rem; color:var(--muted); font-family:'DM Sans'; font-weight:400;">n = 1 to 20</span>
    </div>
    <div class="card">
      <table>
        <thead>
          <tr>
            <th>n</th><th style="color:var(--rose)">n³</th><th style="color:var(--lavender)">∛n</th>
            <th>n</th><th style="color:var(--rose)">n³</th><th style="color:var(--lavender)">∛n</th>
          </tr>
        </thead>
        <tbody>
          <tr class="highlight-row"><td class="n">1</td><td class="cb">1</td><td class="cbr">1.000</td><td class="n">11</td><td class="cb">1,331</td><td class="cbr">2.224</td></tr>
          <tr><td class="n">2</td><td class="cb">8</td><td class="cbr">1.260</td><td class="n">12</td><td class="cb">1,728</td><td class="cbr">2.289</td></tr>
          <tr><td class="n">3</td><td class="cb">27</td><td class="cbr">1.442</td><td class="n">13</td><td class="cb">2,197</td><td class="cbr">2.351</td></tr>
          <tr><td class="n">4</td><td class="cb">64</td><td class="cbr">1.587</td><td class="n">14</td><td class="cb">2,744</td><td class="cbr">2.410</td></tr>
          <tr><td class="n">5</td><td class="cb">125</td><td class="cbr">1.710</td><td class="n">15</td><td class="cb">3,375</td><td class="cbr">2.466</td></tr>
          <tr><td class="n">6</td><td class="cb">216</td><td class="cbr">1.817</td><td class="n">16</td><td class="cb">4,096</td><td class="cbr">2.520</td></tr>
          <tr><td class="n">7</td><td class="cb">343</td><td class="cbr">1.913</td><td class="n">17</td><td class="cb">4,913</td><td class="cbr">2.571</td></tr>
          <tr><td class="n">8</td><td class="cb">512</td><td class="cbr">2.000</td><td class="n">18</td><td class="cb">5,832</td><td class="cbr">2.621</td></tr>
          <tr><td class="n">9</td><td class="cb">729</td><td class="cbr">2.080</td><td class="n">19</td><td class="cb">6,859</td><td class="cbr">2.668</td></tr>
          <tr><td class="n">10</td><td class="cb">1,000</td><td class="cbr">2.154</td><td class="n">20</td><td class="cb">8,000</td><td class="cbr">2.714</td></tr>
        </tbody>
      </table>
    </div>
  </div>


  <!-- FRACTIONS -->
  <div class="section">
    <div class="section-title">
      <div class="icon icon-teal">🟩</div>
      <span style="color:var(--teal)">Important Fractions → Decimals</span>
      <div class="line"></div>
    </div>
    <div class="frac-grid">
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">2</span><span class="frac-decimal">0.5000</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">3</span><span class="frac-decimal">0.3333</span></div>
      <div class="frac-cell"><span class="frac-top">2</span><div class="frac-bar"></div><span class="frac-denom">3</span><span class="frac-decimal">0.6667</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">4</span><span class="frac-decimal">0.2500</span></div>
      <div class="frac-cell"><span class="frac-top">3</span><div class="frac-bar"></div><span class="frac-denom">4</span><span class="frac-decimal">0.7500</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">5</span><span class="frac-decimal">0.2000</span></div>
      <div class="frac-cell"><span class="frac-top">2</span><div class="frac-bar"></div><span class="frac-denom">5</span><span class="frac-decimal">0.4000</span></div>
      <div class="frac-cell"><span class="frac-top">3</span><div class="frac-bar"></div><span class="frac-denom">5</span><span class="frac-decimal">0.6000</span></div>
      <div class="frac-cell"><span class="frac-top">4</span><div class="frac-bar"></div><span class="frac-denom">5</span><span class="frac-decimal">0.8000</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">6</span><span class="frac-decimal">0.1667</span></div>
      <div class="frac-cell"><span class="frac-top">5</span><div class="frac-bar"></div><span class="frac-denom">6</span><span class="frac-decimal">0.8333</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">7</span><span class="frac-decimal">0.1429</span></div>
      <div class="frac-cell"><span class="frac-top">2</span><div class="frac-bar"></div><span class="frac-denom">7</span><span class="frac-decimal">0.2857</span></div>
      <div class="frac-cell"><span class="frac-top">3</span><div class="frac-bar"></div><span class="frac-denom">7</span><span class="frac-decimal">0.4286</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">8</span><span class="frac-decimal">0.1250</span></div>
      <div class="frac-cell"><span class="frac-top">3</span><div class="frac-bar"></div><span class="frac-denom">8</span><span class="frac-decimal">0.3750</span></div>
      <div class="frac-cell"><span class="frac-top">5</span><div class="frac-bar"></div><span class="frac-denom">8</span><span class="frac-decimal">0.6250</span></div>
      <div class="frac-cell"><span class="frac-top">7</span><div class="frac-bar"></div><span class="frac-denom">8</span><span class="frac-decimal">0.8750</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">9</span><span class="frac-decimal">0.1111</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">11</span><span class="frac-decimal">0.0909</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">12</span><span class="frac-decimal">0.0833</span></div>
      <div class="frac-cell"><span class="frac-top">1</span><div class="frac-bar"></div><span class="frac-denom">16</span><span class="frac-decimal">0.0625</span></div>
    </div>
  </div>


  <!-- SURDS / IMPORTANT ROOTS -->
  <div class="section">
    <div class="section-title">
      <div class="icon icon-lav">🟣</div>
      <span style="color:var(--lavender)">Important Surd Values</span>
      <div class="line"></div>
    </div>
    <div class="surd-grid">
      <div class="surd-cell"><div class="surd-expr">√2</div><div class="surd-val">1.4142</div></div>
      <div class="surd-cell"><div class="surd-expr">√3</div><div class="surd-val">1.7321</div></div>
      <div class="surd-cell"><div class="surd-expr">√5</div><div class="surd-val">2.2361</div></div>
      <div class="surd-cell"><div class="surd-expr">√6</div><div class="surd-val">2.4495</div></div>
      <div class="surd-cell"><div class="surd-expr">√7</div><div class="surd-val">2.6458</div></div>
      <div class="surd-cell"><div class="surd-expr">√10</div><div class="surd-val">3.1623</div></div>
      <div class="surd-cell"><div class="surd-expr">√11</div><div class="surd-val">3.3166</div></div>
      <div class="surd-cell"><div class="surd-expr">√13</div><div class="surd-val">3.6056</div></div>
      <div class="surd-cell"><div class="surd-expr">1/√2</div><div class="surd-val">0.7071</div></div>
      <div class="surd-cell"><div class="surd-expr">1/√3</div><div class="surd-val">0.5774</div></div>
      <div class="surd-cell"><div class="surd-expr">√2/2</div><div class="surd-val">0.7071</div></div>
      <div class="surd-cell"><div class="surd-expr">√3/2</div><div class="surd-val">0.8660</div></div>
      <div class="surd-cell"><div class="surd-expr">√3/3</div><div class="surd-val">0.5774</div></div>
      <div class="surd-cell"><div class="surd-expr">∛2</div><div class="surd-val">1.2599</div></div>
      <div class="surd-cell"><div class="surd-expr">∛3</div><div class="surd-val">1.4422</div></div>
      <div class="surd-cell"><div class="surd-expr">∛5</div><div class="surd-val">1.7100</div></div>
    </div>
  </div>


  <!-- POWERS OF 2 AND 3 -->
  <div class="section">
    <div class="section-title">
      <div class="icon icon-blue" style="background:rgba(96,165,250,0.12)">🔵</div>
      <span style="color:var(--blue)">Powers of 2 & 3</span>
      <div class="line"></div>
    </div>
    <div class="pow-grid">
      <div class="pow-card">
        <div class="pow-header">Powers of 2</div>
        <div class="pow-row"><span class="pow-exp">2¹</span><span class="pow-val-blue">2</span></div>
        <div class="pow-row"><span class="pow-exp">2²</span><span class="pow-val-blue">4</span></div>
        <div class="pow-row"><span class="pow-exp">2³</span><span class="pow-val-blue">8</span></div>
        <div class="pow-row"><span class="pow-exp">2⁴</span><span class="pow-val-blue">16</span></div>
        <div class="pow-row"><span class="pow-exp">2⁵</span><span class="pow-val-blue">32</span></div>
        <div class="pow-row"><span class="pow-exp">2⁶</span><span class="pow-val-blue">64</span></div>
        <div class="pow-row"><span class="pow-exp">2⁷</span><span class="pow-val-blue">128</span></div>
        <div class="pow-row"><span class="pow-exp">2⁸</span><span class="pow-val-blue">256</span></div>
        <div class="pow-row"><span class="pow-exp">2⁹</span><span class="pow-val-blue">512</span></div>
        <div class="pow-row"><span class="pow-exp">2¹⁰</span><span class="pow-val-blue">1,024</span></div>
        <div class="pow-row"><span class="pow-exp">2¹¹</span><span class="pow-val-blue">2,048</span></div>
        <div class="pow-row"><span class="pow-exp">2¹²</span><span class="pow-val-blue">4,096</span></div>
      </div>
      <div class="pow-card">
        <div class="pow-header">Powers of 3</div>
        <div class="pow-row"><span class="pow-exp">3¹</span><span class="pow-val-rose">3</span></div>
        <div class="pow-row"><span class="pow-exp">3²</span><span class="pow-val-rose">9</span></div>
        <div class="pow-row"><span class="pow-exp">3³</span><span class="pow-val-rose">27</span></div>
        <div class="pow-row"><span class="pow-exp">3⁴</span><span class="pow-val-rose">81</span></div>
        <div class="pow-row"><span class="pow-exp">3⁵</span><span class="pow-val-rose">243</span></div>
        <div class="pow-row"><span class="pow-exp">3⁶</span><span class="pow-val-rose">729</span></div>
        <div class="pow-row"><span class="pow-exp">3⁷</span><span class="pow-val-rose">2,187</span></div>
        <div class="pow-row"><span class="pow-exp">3⁸</span><span class="pow-val-rose">6,561</span></div>
        <div class="pow-row"><span class="pow-exp">3⁹</span><span class="pow-val-rose">19,683</span></div>
        <div class="pow-row"><span class="pow-exp">3¹⁰</span><span class="pow-val-rose">59,049</span></div>
        <div class="pow-row"><span class="pow-exp">3¹¹</span><span class="pow-val-rose">1,77,147</span></div>
        <div class="pow-row"><span class="pow-exp">3¹²</span><span class="pow-val-rose">5,31,441</span></div>
      </div>
    </div>
  </div>


  <!-- FOOTER -->
  <div class="footer">
    JEE Mains & Advanced · Speed Reference Sheet
    <br>
    <span class="badge">Memorize → Recognize → Win ⚡</span>
  </div>

</div></div></div>

<div class="psec" id="sec-calc">
  <div class="cwrap">
    <div class="shero" style="--sc:rgba(240,128,64,.08)">
      <span class="shero-badge">06 — Scientific Calculator</span>
      <h2 style="color:#f08040">Scientific Calculator</h2>
      <p>Full scientific functions · trigonometry · logarithms · memory · degree/radian</p>
    </div>
    <div id="calc-wrap">
      <div id="calc">
        <div class="calc-header">
          <div class="calc-header-title">⬡ SCI-CALC</div>
          <div class="calc-mode-btns">
            <button class="calc-mode-btn active" id="btn-deg" onclick="setAngleMode('deg')">DEG</button>
            <button class="calc-mode-btn" id="btn-rad" onclick="setAngleMode('rad')">RAD</button>
          </div>
        </div>
        <div id="calc-display">
          <div id="calc-history"></div>
          <div id="calc-expr"></div>
          <div id="calc-result">0</div>
        </div>
        <div class="calc-status">
          <span class="mem-ind" id="mem-ind"></span>
          <span class="angle-ind" id="angle-ind">DEG</span>
        </div>
        <div class="calc-btns" id="calc-btns">
          <button class="cb mem" data-action="mc">MC</button>
          <button class="cb mem" data-action="mr">MR</button>
          <button class="cb mem" data-action="ms">MS</button>
          <button class="cb mem" data-action="m+">M+</button>
          <button class="cb mem" data-action="m-">M−</button>
          <button class="cb fn" data-action="sin">sin</button>
          <button class="cb fn" data-action="cos">cos</button>
          <button class="cb fn" data-action="tan">tan</button>
          <button class="cb fn" data-action="asin">sin⁻¹</button>
          <button class="cb fn" data-action="acos">cos⁻¹</button>
          <button class="cb fn" data-action="atan">tan⁻¹</button>
          <button class="cb fn" data-action="log">log</button>
          <button class="cb fn" data-action="ln">ln</button>
          <button class="cb fn" data-action="sqrt">√</button>
          <button class="cb fn" data-action="cbrt">∛</button>
          <button class="cb fn" data-action="sq">x²</button>
          <button class="cb fn" data-action="cube">x³</button>
          <button class="cb fn" data-action="pow">xʸ</button>
          <button class="cb fn" data-action="pi">π</button>
          <button class="cb fn" data-action="e">e</button>
          <button class="cb clr" data-action="ac">AC</button>
          <button class="cb clr" data-action="del">⌫</button>
          <button class="cb fn" data-action="(">(</button>
          <button class="cb fn" data-action=")">)</button>
          <button class="cb fn" data-action="pct">%</button>
          <button class="cb fn" data-action="inv">1/x</button>
          <button class="cb fn" data-action="abs">|x|</button>
          <button class="cb fn" data-action="fact">n!</button>
          <button class="cb op" data-action="÷">÷</button>
          <button class="cb op" data-action="×">×</button>
          <button class="cb num" data-action="7">7</button>
          <button class="cb num" data-action="8">8</button>
          <button class="cb num" data-action="9">9</button>
          <button class="cb op" data-action="−">−</button>
          <button class="cb op" data-action="+">+</button>
          <button class="cb num" data-action="4">4</button>
          <button class="cb num" data-action="5">5</button>
          <button class="cb num" data-action="6">6</button>
          <button class="cb fn" data-action="ans">ANS</button>
          <button class="cb fn" data-action="+/-">±</button>
          <button class="cb num" data-action="1">1</button>
          <button class="cb num" data-action="2">2</button>
          <button class="cb num" data-action="3">3</button>
          <button class="cb num wide" data-action="0">0</button>
          <button class="cb num" data-action=".">.</button>
          <button class="cb eq" data-action="=">=</button>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ═══ DESMOS MODULE ═══ -->
<style>
.dsm-panel{background:var(--p2);border:1px solid var(--b2);border-radius:10px;overflow:hidden;margin-bottom:12px;}
.dsm-panel-hdr{display:flex;align-items:center;gap:10px;padding:9px 14px;border-bottom:1px solid var(--b1);background:rgba(80,216,144,.03);}
.dsm-panel-hdr-label{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:#50d890;opacity:.8;}
.dsm-panel-#sec-desmos{padding:10px 12px;display:flex;flex-wrap:wrap;gap:6px;}
.dsm-preset{font-family:'JetBrains Mono',monospace;font-size:.62rem;padding:5px 11px;border:1px solid var(--b2);border-radius:3px;background:rgba(255,255,255,.02);cursor:pointer;transition:all .15s;letter-spacing:.05em;color:var(--t2);}
.dsm-preset:hover{background:rgba(255,255,255,.06);transform:translateY(-1px);box-shadow:0 4px 14px rgba(0,0,0,.4);}
.dsm-preset:active{transform:translateY(0);}
.dsm-group-label{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2px;text-transform:uppercase;color:var(--t3);display:block;width:100%;margin:4px 0 2px;}
.dsm-toolbar{display:flex;align-items:center;gap:8px;padding:8px 12px;background:rgba(255,255,255,.015);border-top:1px solid var(--b1);}
.dsm-toolbar-btn{font-family:'JetBrains Mono',monospace;font-size:.58rem;padding:4px 10px;border:1px solid var(--b2);border-radius:3px;background:transparent;color:var(--t3);cursor:pointer;transition:all .15s;letter-spacing:.06em;}
.dsm-toolbar-btn:hover{color:#fff;border-color:var(--t3);}
.dsm-toolbar-btn.danger{border-color:rgba(240,96,128,.3);color:#f06080;}
.dsm-toolbar-btn.danger:hover{background:rgba(240,96,128,.1);}
@keyframes spin{to{transform:rotate(360deg);}}
</style>
<div class="psec" id="sec-desmos">
  <div class="cwrap">
    <div class="shero" style="--sc:rgba(80,216,144,.08)">
      <span class="shero-badge">07 — Interactive Grapher</span>
      <h2 style="color:#50d890">Desmos <em>Graphing</em></h2>
      <p>Full Desmos calculator · plot any function · zoom · trace · explore JEE functions</p>
    </div>

    <!-- Preset panels -->
    <div class="dsm-panel">
      <div class="dsm-panel-hdr"><span class="dsm-panel-hdr-label">⬡ Quick Presets</span><span style="font-family:'Crimson Pro',serif;font-style:italic;font-size:.82rem;color:var(--t3);">click to add to graph</span></div>
      <div class="dsm-panel-body">
        <span class="dsm-group-label">Basic Trig</span>
        <button class="dsm-preset" data-expr="y=\sin\left(x\right)" data-clr="#e8b84b" style="border-color:rgba(232,184,75,.35);color:#e8b84b;">sin x</button>
        <button class="dsm-preset" data-expr="y=\cos\left(x\right)" data-clr="#4b9fe8" style="border-color:rgba(75,159,232,.35);color:#4b9fe8;">cos x</button>
        <button class="dsm-preset" data-expr="y=\tan\left(x\right)" data-clr="#e84b7a" style="border-color:rgba(232,75,122,.35);color:#e84b7a;">tan x</button>
        <button class="dsm-preset" data-expr="y=\csc\left(x\right)" data-clr="#4be8a0" style="border-color:rgba(75,232,160,.35);color:#4be8a0;">cosec x</button>
        <button class="dsm-preset" data-expr="y=\sec\left(x\right)" data-clr="#b84be8" style="border-color:rgba(184,75,232,.35);color:#b84be8;">sec x</button>
        <button class="dsm-preset" data-expr="y=\cot\left(x\right)" data-clr="#e8a04b" style="border-color:rgba(232,160,75,.35);color:#e8a04b;">cot x</button>

        <span class="dsm-group-label">Inverse Trig (ITF)</span>
        <button class="dsm-preset" data-expr="y=\arcsin\left(x\right)" data-clr="#e8b84b" style="border-color:rgba(232,184,75,.35);color:#e8b84b;">sin⁻¹ x</button>
        <button class="dsm-preset" data-expr="y=\arccos\left(x\right)" data-clr="#4b9fe8" style="border-color:rgba(75,159,232,.35);color:#4b9fe8;">cos⁻¹ x</button>
        <button class="dsm-preset" data-expr="y=\arctan\left(x\right)" data-clr="#e84b7a" style="border-color:rgba(232,75,122,.35);color:#e84b7a;">tan⁻¹ x</button>
        <button class="dsm-preset" data-expr="y=\frac{\pi}{2}-\arctan\left(x\right)" data-clr="#4be8a0" style="border-color:rgba(75,232,160,.35);color:#4be8a0;">cot⁻¹ x</button>
        <button class="dsm-preset" data-expr="y=\arccos\left(\frac{1}{x}\right)\left\{x\ge1\right\}" data-clr="#b84be8" style="border-color:rgba(184,75,232,.35);color:#b84be8;">sec⁻¹ x (x≥1)</button>
        <button class="dsm-preset" data-expr="y=\arcsin\left(\frac{1}{x}\right)\left\{x\ge1\right\}" data-clr="#e8a04b" style="border-color:rgba(232,160,75,.35);color:#e8a04b;">cosec⁻¹ x (x≥1)</button>

        <span class="dsm-group-label">ITF Composites — JEE Critical</span>
        <button class="dsm-preset" data-expr="y=\arcsin\left(\sin\left(x\right)\right)" data-clr="#e8b84b" style="border-color:rgba(232,184,75,.35);color:#e8b84b;">sin⁻¹(sin x) — zigzag</button>
        <button class="dsm-preset" data-expr="y=\sin\left(\arcsin\left(x\right)\right)" data-clr="#4b9fe8" style="border-color:rgba(75,159,232,.35);color:#4b9fe8;">sin(sin⁻¹ x) — identity</button>
        <button class="dsm-preset" data-expr="y=\arccos\left(\cos\left(x\right)\right)" data-clr="#e84b7a" style="border-color:rgba(232,75,122,.35);color:#e84b7a;">cos⁻¹(cos x) — zigzag</button>
        <button class="dsm-preset" data-expr="y=\cos\left(\arccos\left(x\right)\right)" data-clr="#4be8a0" style="border-color:rgba(75,232,160,.35);color:#4be8a0;">cos(cos⁻¹ x) — identity</button>
        <button class="dsm-preset" data-expr="y=\arctan\left(\tan\left(x\right)\right)" data-clr="#b84be8" style="border-color:rgba(184,75,232,.35);color:#b84be8;">tan⁻¹(tan x) — sawtooth</button>
        <button class="dsm-preset" data-expr="y=\tan\left(\arctan\left(x\right)\right)" data-clr="#e8a04b" style="border-color:rgba(232,160,75,.35);color:#e8a04b;">tan(tan⁻¹ x) — identity</button>

        <span class="dsm-group-label">Algebra &amp; Calculus</span>
        <button class="dsm-preset" data-expr="y=x^{2}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">x²</button>
        <button class="dsm-preset" data-expr="y=x^{3}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">x³</button>
        <button class="dsm-preset" data-expr="y=\sqrt{x}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">√x</button>
        <button class="dsm-preset" data-expr="y=e^{x}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">eˣ</button>
        <button class="dsm-preset" data-expr="y=\ln\left(x\right)" style="border-color:rgba(255,255,255,.15);color:var(--t2);">ln x</button>
        <button class="dsm-preset" data-expr="y=\left|x\right|" style="border-color:rgba(255,255,255,.15);color:var(--t2);">|x|</button>
        <button class="dsm-preset" data-expr="y=\frac{1}{x}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">1/x</button>
        <button class="dsm-preset" data-expr="y=\frac{\sin\left(x\right)}{x}" style="border-color:rgba(255,255,255,.15);color:var(--t2);">sinc(x)</button>

        <span class="dsm-group-label">JEE Special Curves</span>
        <button class="dsm-preset" data-expr="x^{2}+y^{2}=r^{2}" data-clr="#4b9fe8" style="border-color:rgba(75,159,232,.35);color:#4b9fe8;">Circle x²+y²=r²</button>
        <button class="dsm-preset" data-expr="y^{2}=4ax" data-clr="#e8b84b" style="border-color:rgba(232,184,75,.35);color:#e8b84b;">Parabola y²=4ax</button>
        <button class="dsm-preset" data-expr="\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1" data-clr="#e84b7a" style="border-color:rgba(232,75,122,.35);color:#e84b7a;">Ellipse</button>
        <button class="dsm-preset" data-expr="\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}=1" data-clr="#b84be8" style="border-color:rgba(184,75,232,.35);color:#b84be8;">Hyperbola</button>
        <button class="dsm-preset" data-expr="y=\sin\left(ax+b\right)+c" data-clr="#50d890" style="border-color:rgba(80,216,144,.35);color:#50d890;">a·sin(bx+c)+d</button>
      </div>
      <div class="dsm-toolbar">
        <button class="dsm-toolbar-btn dsm-clear danger">✕ Clear All</button>
        <button class="dsm-toolbar-btn" id="dsm-reset-view">⊞ Reset View</button>
        <button class="dsm-toolbar-btn" id="dsm-toggle-grid">⊟ Grid</button>
        <span style="margin-left:auto;font-family:'JetBrains Mono',monospace;font-size:8px;color:var(--t3);letter-spacing:1.5px;" id="dsm-expr-count">0 EXPRESSIONS</span>
      </div>
    </div>

    <!-- Desmos calculator via iframe -->
    <div id="desmos-wrap" style="position:relative;width:100%;height:calc(100vh - 160px);min-height:560px;border-radius:12px;overflow:hidden;border:1px solid rgba(80,216,144,.18);box-shadow:0 0 60px rgba(80,216,144,.05);">
      <iframe id="desmos-frame"
        src="https://www.desmos.com/calculator"
        style="width:100%;height:100%;border:none;display:block;"
        allowfullscreen
        title="Desmos Graphing Calculator">
      </iframe>
      <div id="desmos-loading" style="position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;background:#06080f;gap:16px;z-index:10;pointer-events:none;">
        <div style="width:44px;height:44px;border:2px solid rgba(80,216,144,.15);border-top-color:#50d890;border-radius:50%;animation:spin 1s linear infinite;"></div>
        <span style="font-family:'JetBrains Mono',monospace;font-size:.7rem;color:#50d890;letter-spacing:.2em;">LOADING DESMOS…</span>
        <span style="font-family:'Crimson Pro',serif;font-style:italic;font-size:.82rem;color:var(--t3);">Requires internet connection</span>
      </div>
    </div>
    <div style="padding:8px 0 48px;font-family:'JetBrains Mono',monospace;font-size:.58rem;color:var(--t3);letter-spacing:.1em;text-align:center;">
      POWERED BY DESMOS GRAPHING CALCULATOR API — <span style="color:rgba(80,216,144,.5);">desmos.com</span>
    </div>
  </div>
</div>

<div id="cur-dot"></div>
<div id="cur-ring"></div>

<script>
/* PROOF FUNCTIONS */
function step(n,hh){return`<div class="pstep"><div class="sn2">${n}</div><div class="st">${hh}</div></div>`;}
function sec2(t,c){return`<div class="ps"><div class="pst">${t}</div>${c}</div>`;}
function note(t){return`<div class="pnote">${t}</div>`;}
function diag(t){return`<div class="pdiag">${t}</div>`;}
function m(t){return`<span class="m">${t}</span>`;}
function h(t){return`<span class="h">${t}</span>`;}

const PROOFS={
"sin-def":{t:"sin θ = Opposite / Hypotenuse",b:sec2("UNIT CIRCLE DEFINITION",
  diag("    P(cosθ, sinθ)\n   /|\n  / | ← opposite (y)\n /θ |\nO───Q\n  adjacent (x)")+
  step(1,`Place point P on the unit circle at angle θ. Coordinates: ${m("P = (cosθ, sinθ)")}.`)+
  step(2,`Drop perpendicular PQ to the x-axis. Length PQ = sinθ = y-coord. Hypotenuse OP = 1.`)+
  step(3,`For any right triangle with hyp r, scale uniformly: ${m("sinθ = opposite / hypotenuse")}. ✓`)+
  note("sin θ is the y-coordinate of the point on the unit circle at angle θ."))},

"cos-def":{t:"cos θ = Adjacent / Hypotenuse",b:sec2("UNIT CIRCLE x-COORDINATE",
  step(1,`On the unit circle, the x-coordinate of P at angle θ equals the adjacent side. With hyp=1: ${m("cosθ = adjacent / hypotenuse")}. ✓`)+
  note("cos is the 'co-sine' — by definition cosθ = sin(90°−θ). It is an even function."))},

"tan-def":{t:"tan θ = sin θ / cos θ",b:sec2("FROM RATIO OF SIN AND COS",
  step(1,`Divide sinθ/cosθ = ${m("(opp/hyp)÷(adj/hyp) = opp/adj")}. ✓`)+
  step(2,`Geometrically, tanθ is the length of the tangent drawn from origin to the unit circle — hence the name ${h("tangent")}.`))},

"cosec-def":{t:"cosec θ = 1 / sin θ",b:sec2("RECIPROCAL DEFINITION",
  step(1,`sinθ = opp/hyp, so its reciprocal is hyp/opp = cosecθ. Defined whenever ${m("sinθ ≠ 0")}, i.e. θ ≠ nπ. ✓`))},
"sec-def":{t:"sec θ = 1 / cos θ",b:sec2("RECIPROCAL DEFINITION",
  step(1,`cosθ = adj/hyp, so its reciprocal hyp/adj = secθ. Undefined when ${m("cosθ = 0")}, i.e. θ = (2n+1)π/2. ✓`))},
"cot-def":{t:"cot θ = cos θ / sin θ",b:sec2("FROM TAN",
  step(1,`${m("cotθ = 1/tanθ = cosθ/sinθ = adj/opp")}. ✓`))},

"q1":{t:"All ratios positive in Quadrant I",b:sec2("COORDINATE SIGNS",
  step(1,`In Q-I: x > 0, y > 0. So sinθ = y/r > 0, cosθ = x/r > 0, tanθ = y/x > 0.`)+
  step(2,`All reciprocals (cosec, sec, cot) are also positive since they are 1/(positive). ✓`))},

"q2":{t:"Only sin, cosec positive in Quadrant II",b:sec2("COORDINATE SIGNS",
  step(1,`In Q-II: x < 0, y > 0. So ${m("sinθ = y/r > 0")}, ${m("cosθ = x/r < 0")}, ${m("tanθ = y/x < 0")}.`)+
  step(2,`cosec = 1/sin > 0, sec = 1/cos < 0, cot = 1/tan < 0. ✓`))},

"q3":{t:"Only tan, cot positive in Quadrant III",b:sec2("COORDINATE SIGNS",
  step(1,`In Q-III: x < 0, y < 0. ${m("sinθ < 0, cosθ < 0, tanθ = (−)/(−) > 0")}.`)+
  step(2,`cot > 0, cosec < 0, sec < 0. ✓`))},

"q4":{t:"Only cos, sec positive in Quadrant IV",b:sec2("COORDINATE SIGNS",
  step(1,`In Q-IV: x > 0, y < 0. ${m("cosθ > 0, sinθ < 0, tanθ < 0")}. sec > 0. ✓`))},

"py1":{t:"sin²θ + cos²θ = 1",b:sec2("PROOF FROM PYTHAGORAS THEOREM",
  step(1,`In a right triangle with opposite=a, adjacent=b, hypotenuse=h: by Pythagoras, ${m("a² + b² = h²")}.`)+
  step(2,`Divide everything by h²: ${m("a²/h² + b²/h² = 1")}.`)+
  step(3,`Since sinθ = a/h and cosθ = b/h: ${m("sin²θ + cos²θ = 1")}. ✓`)+
  note("On the unit circle, (cosθ,sinθ) always lies on x²+y²=1 — so this holds for ALL real θ, not just acute."))},

"py2":{t:"1 + tan²θ = sec²θ",b:sec2("DIVIDE PYTHAGOREAN IDENTITY BY cos²θ",
  step(1,`Start with ${m("sin²θ + cos²θ = 1")}. Divide every term by ${m("cos²θ")} (cosθ ≠ 0):`)+
  step(2,`${m("sin²θ/cos²θ + 1 = 1/cos²θ")} → ${m("tan²θ + 1 = sec²θ")}. ✓`))},

"py3":{t:"1 + cot²θ = cosec²θ",b:sec2("DIVIDE PYTHAGOREAN IDENTITY BY sin²θ",
  step(1,`Divide ${m("sin²θ + cos²θ = 1")} by ${m("sin²θ")}: ${m("1 + cot²θ = cosec²θ")}. ✓`))},

"n-sin":{t:"sin(−θ) = −sin θ  (odd function)",b:sec2("UNIT CIRCLE REFLECTION",
  step(1,`Reflecting angle θ → −θ mirrors P(cosθ,sinθ) across the x-axis to Q(cosθ,−sinθ).`)+
  step(2,`y-coordinate of Q = sin(−θ) = −sinθ. ✓ sin is an ${h("odd function")}.`))},

"n-cos":{t:"cos(−θ) = +cos θ  (even function)",b:sec2("UNIT CIRCLE REFLECTION",
  step(1,`Reflection across x-axis leaves x-coordinate unchanged: ${m("cos(−θ) = cosθ")}. ✓ cos is an ${h("even function")}.`))},

"n-tan":{t:"tan(−θ) = −tan θ",b:sec2("FROM SIN AND COS",
  step(1,`${m("tan(−θ) = sin(−θ)/cos(−θ) = −sinθ/cosθ = −tanθ")}. ✓`))},
"n-cosec":{t:"cosec(−θ) = −cosec θ",b:sec2("RECIPROCAL",step(1,`${m("cosec(−θ) = 1/sin(−θ) = −1/sinθ = −cosecθ")}. ✓`))},
"n-sec":{t:"sec(−θ) = +sec θ",b:sec2("RECIPROCAL",step(1,`${m("sec(−θ) = 1/cos(−θ) = 1/cosθ = secθ")}. ✓`))},
"n-cot":{t:"cot(−θ) = −cot θ",b:sec2("FROM COS/SIN",step(1,`${m("cot(−θ) = cos(−θ)/sin(−θ) = cosθ/(−sinθ) = −cotθ")}. ✓`))},

"c90m-sin":{t:"sin(90°−θ) = cos θ",b:sec2("COMPLEMENTARY ANGLES",
  step(1,`In a right triangle with angles θ and (90°−θ): the side opposite (90°−θ) is the side adjacent to θ.`)+
  step(2,`${m("sin(90°−θ) = adj/hyp = cosθ")}. ✓`)+
  note("This is why sin and cos are called 'co-functions' — each is the other's complement."))},

"c90m-cos":{t:"cos(90°−θ) = sin θ",b:sec2("COMPLEMENTARY ANGLES",step(1,`Side adjacent to (90°−θ) = side opposite θ. ${m("cos(90°−θ) = opp/hyp = sinθ")}. ✓`))},
"c90m-tan":{t:"tan(90°−θ) = cot θ",b:sec2("FROM SIN/COS",step(1,`${m("tan(90°−θ) = sin(90°−θ)/cos(90°−θ) = cosθ/sinθ = cotθ")}. ✓`))},
"c90m-csc":{t:"cosec(90°−θ) = sec θ",b:sec2("RECIPROCAL",step(1,`${m("cosec(90°−θ) = 1/sin(90°−θ) = 1/cosθ = secθ")}. ✓`))},
"c90m-sec":{t:"sec(90°−θ) = cosec θ",b:sec2("RECIPROCAL",step(1,`${m("sec(90°−θ) = 1/cos(90°−θ) = 1/sinθ = cosecθ")}. ✓`))},
"c90m-cot":{t:"cot(90°−θ) = tan θ",b:sec2("FROM COS/SIN",step(1,`${m("cot(90°−θ) = cos(90°−θ)/sin(90°−θ) = sinθ/cosθ = tanθ")}. ✓`))},

"a90p":{t:"sin(90°+θ) = +cos θ",b:sec2("EXPAND USING ADDITION FORMULA",step(1,`${m("sin(90°+θ) = sin90°cosθ + cos90°sinθ = 1·cosθ + 0·sinθ = cosθ")}. ✓`))},
"b90p":{t:"cos(90°+θ) = −sin θ",b:sec2("EXPAND",step(1,`${m("cos(90°+θ) = cos90°cosθ − sin90°sinθ = 0 − sinθ = −sinθ")}. ✓`))},
"c90p":{t:"tan(90°+θ) = −cot θ",b:sec2("RATIO",step(1,`${m("tan(90°+θ) = cosθ/(−sinθ) = −cotθ")}. ✓`))},
"a180m":{t:"sin(180°−θ) = +sin θ",b:sec2("EXPAND",step(1,`${m("sin(180°−θ) = sin180°cosθ − cos180°sinθ = 0−(−1)sinθ = sinθ")}. ✓`))},
"b180m":{t:"cos(180°−θ) = −cos θ",b:sec2("EXPAND",step(1,`${m("cos(180°−θ) = cos180°cosθ + sin180°sinθ = −cosθ + 0 = −cosθ")}. ✓`))},
"c180m":{t:"tan(180°−θ) = −tan θ",b:sec2("RATIO",step(1,`${m("tan(180°−θ) = sinθ/(−cosθ) = −tanθ")}. ✓`))},
"a180p":{t:"sin(180°+θ) = −sin θ",b:sec2("EXPAND",step(1,`${m("sin(180°+θ) = sin180°cosθ + cos180°sinθ = 0+(−1)sinθ = −sinθ")}. ✓`))},
"b180p":{t:"cos(180°+θ) = −cos θ",b:sec2("EXPAND",step(1,`${m("cos(180°+θ) = cos180°cosθ − sin180°sinθ = −cosθ − 0 = −cosθ")}. ✓`))},
"c180p":{t:"tan(180°+θ) = +tan θ  (period of tan = π)",b:sec2("RATIO",step(1,`${m("tan(180°+θ) = (−sinθ)/(−cosθ) = tanθ")}. ✓ This proves tan has period π.`))},
"a360m":{t:"sin(360°−θ) = −sin θ",b:sec2("EXPAND",step(1,`sin(360°−θ) = sin(−θ+360°) = sin(−θ) = −sinθ. (Period 2π) ✓`))},
"b360m":{t:"cos(360°−θ) = +cos θ",b:sec2("EXPAND",step(1,`cos(360°−θ) = cos(−θ) = cosθ. ✓`))},
"c360m":{t:"tan(360°−θ) = −tan θ",b:sec2("RATIO",step(1,`tan(360°−θ) = −sinθ/cosθ = −tanθ. ✓`))},

"sin-add":{t:"sin(A+B) = sinA cosB + cosA sinB",b:sec2("ROTATION MATRIX / COMPLEX EXPONENTIAL",
  step(1,`Consider rotating vector (cosB, sinB) by angle A. The rotation matrix gives new y-coordinate:`)+
  step(2,`${m("y' = sinA·cosB + cosA·sinB")}.`)+
  step(3,`Since rotating (cosB,sinB) by A yields the point at angle A+B, its y-coord = sin(A+B). ✓`)+
  note("Elegant alternative: e^(i(A+B)) = e^(iA)·e^(iB). Compare imaginary parts: sin(A+B) = sinA cosB + cosA sinB."))},

"sin-sub":{t:"sin(A−B) = sinA cosB − cosA sinB",b:sec2("SUBSTITUTE B → −B",
  step(1,`Replace B with −B in sin(A+B):`)+
  step(2,`${m("sin(A+(−B)) = sinA cos(−B) + cosA sin(−B) = sinA cosB − cosA sinB")}. ✓`))},

"cos-add":{t:"cos(A+B) = cosA cosB − sinA sinB",b:sec2("ROTATION MATRIX",
  step(1,`Rotating (cosB,sinB) by A, the new x-coordinate is:`)+
  step(2,`${m("x' = cosA·cosB − sinA·sinB")} = cos(A+B). ✓`)+
  note("Also: Re[e^(i(A+B))] = Re[e^(iA)·e^(iB)] = cosA cosB − sinA sinB."))},

"cos-sub":{t:"cos(A−B) = cosA cosB + sinA sinB",b:sec2("SUBSTITUTE B → −B",
  step(1,`${m("cos(A−B) = cosA cos(−B) − sinA sin(−B) = cosA cosB + sinA sinB")}. ✓`))},

"tan-add":{t:"tan(A+B) = (tanA+tanB)/(1−tanA tanB)",b:sec2("FROM SIN AND COS ADDITION FORMULAS",
  step(1,`${m("tan(A+B) = sin(A+B)/cos(A+B)")}`)+
  step(2,`Numerator: ${m("sinA cosB + cosA sinB")}. Denominator: ${m("cosA cosB − sinA sinB")}.`)+
  step(3,`Divide both by cosA cosB:`)+
  step(4,`${m("= (tanA+tanB)/(1−tanA tanB)")}. ✓`))},

"tan-sub":{t:"tan(A−B) = (tanA−tanB)/(1+tanA tanB)",b:sec2("SUBSTITUTE B → −B",
  step(1,`${m("(tanA+tan(−B))/(1−tanA·tan(−B)) = (tanA−tanB)/(1+tanA tanB)")}. ✓`))},

"cot-add":{t:"cot(A+B) = (cotA cotB−1)/(cotA+cotB)",b:sec2("RECIPROCAL OF TAN(A+B)",
  step(1,`${m("cot(A+B) = 1/tan(A+B) = (1−tanA tanB)/(tanA+tanB)")}.`)+
  step(2,`Multiply top and bottom by cotA cotB: ${m("= (cotA cotB−1)/(cotB+cotA)")}. ✓`))},

"cot-sub":{t:"cot(A−B) = (cotA cotB+1)/(cotB−cotA)",b:sec2("SUBSTITUTE B → −B IN cot(A+B)",
  step(1,`cot(−B) = −cotB. Substituting in cot(A+B) formula gives ${m("(cotA cotB+1)/(cotB−cotA)")}. ✓`))},

"s2p-sp":{t:"sinC+sinD = 2 sin((C+D)/2) cos((C−D)/2)",b:sec2("SUBSTITUTION INTO ADDITION FORMULA",
  step(1,`Let C=A+B, D=A−B. Then A=(C+D)/2, B=(C−D)/2.`)+
  step(2,`${m("sin(A+B)+sin(A−B) = 2sinA cosB")}.`)+
  step(3,`Substituting back: ${m("sinC+sinD = 2sin((C+D)/2)cos((C−D)/2)")}. ✓`))},

"s2p-sm":{t:"sinC−sinD = 2 cos((C+D)/2) sin((C−D)/2)",b:sec2("SAME SUBSTITUTION",
  step(1,`${m("sin(A+B)−sin(A−B) = 2cosA sinB = 2cos((C+D)/2)sin((C−D)/2)")}. ✓`))},

"s2p-cp":{t:"cosC+cosD = 2 cos((C+D)/2) cos((C−D)/2)",b:sec2("SAME SUBSTITUTION",
  step(1,`${m("cos(A+B)+cos(A−B) = 2cosA cosB = 2cos((C+D)/2)cos((C−D)/2)")}. ✓`))},

"s2p-cm":{t:"cosC−cosD = −2 sin((C+D)/2) sin((C−D)/2)",b:sec2("SAME SUBSTITUTION",
  step(1,`${m("cos(A+B)−cos(A−B) = −2sinA sinB = −2sin((C+D)/2)sin((C−D)/2)")}. ✓`))},

"sin2a":{t:"sin 2A = 2 sinA cosA",b:sec2("SET B=A IN SIN ADDITION FORMULA",
  step(1,`${m("sin(A+A) = sinA cosA + cosA sinA = 2sinA cosA")}. ✓`)+
  step(2,`Tan-form: divide ${m("2sinA cosA")} by ${m("cos²A")}: ${m("= 2tanA/sec²A = 2tanA/(1+tan²A)")}. ✓`))},

"cos2a":{t:"cos 2A — all four equivalent forms",b:sec2("DERIVE ALL 4 FORMS",
  step(1,`Form 1 — from cos(A+A): ${m("cos²A − sin²A")}. ✓`)+
  step(2,`Form 2 — replace sin²A=1−cos²A: ${m("cos²A−(1−cos²A) = 2cos²A−1")}. ✓`)+
  step(3,`Form 3 — replace cos²A=1−sin²A: ${m("(1−sin²A)−sin²A = 1−2sin²A")}. ✓`)+
  step(4,`Form 4 — divide Form 1 by cos²A: ${m("(1−tan²A)/sec²A = (1−tan²A)/(1+tan²A)")}. ✓`)+
  note("Use whichever form matches your given info. Forms 2 and 3 are most useful in JEE integration."))},

"tan2a":{t:"tan 2A = 2tanA/(1−tan²A)",b:sec2("SET B=A IN TAN ADDITION",
  step(1,`${m("tan(A+A) = (tanA+tanA)/(1−tanA·tanA) = 2tanA/(1−tan²A)")}. ✓`))},

"sq-forms":{t:"sin²A = (1−cos2A)/2 and cos²A = (1+cos2A)/2",b:sec2("REARRANGE DOUBLE ANGLE FORMULAS",
  step(1,`From ${m("cos2A = 1−2sin²A")}: rearrange → ${m("sin²A = (1−cos2A)/2")}. ✓`)+
  step(2,`From ${m("cos2A = 2cos²A−1")}: rearrange → ${m("cos²A = (1+cos2A)/2")}. ✓`)+
  note("These are extremely important for integrating sin²x and cos²x in JEE problems!"))},

"sin3a":{t:"sin 3A = 3sinA − 4sin³A",b:sec2("EXPAND sin(2A+A)",
  step(1,`${m("sin3A = sin(2A+A) = sin2A cosA + cos2A sinA")}`)+
  step(2,`Substitute: ${m("= 2sinA cosA·cosA + (1−2sin²A)sinA")}`)+
  step(3,`${m("= 2sinA cos²A + sinA − 2sin³A")}`)+
  step(4,`Replace cos²A=1−sin²A: ${m("= 2sinA(1−sin²A)+sinA−2sin³A = 3sinA−4sin³A")}. ✓`))},

"cos3a":{t:"cos 3A = 4cos³A − 3cosA",b:sec2("EXPAND cos(2A+A)",
  step(1,`${m("cos3A = cos(2A+A) = cos2A cosA − sin2A sinA")}`)+
  step(2,`${m("= (2cos²A−1)cosA − 2sinA cosA·sinA")}`)+
  step(3,`${m("= 2cos³A − cosA − 2sin²A cosA")}`)+
  step(4,`Replace sin²A=1−cos²A: ${m("= 4cos³A−3cosA")}. ✓`))},

"tan3a":{t:"tan 3A = (3tanA−tan³A)/(1−3tan²A)",b:sec2("EXPAND tan(2A+A)",
  step(1,`${m("tan3A = (tan2A+tanA)/(1−tan2A·tanA)")}.`)+
  step(2,`Let t=tanA. Substitute ${m("tan2A = 2t/(1−t²)")}:`)+
  step(3,`Numerator: ${m("2t/(1−t²)+t = (3t−t³)/(1−t²)")}. Denominator: ${m("1−2t²/(1−t²) = (1−3t²)/(1−t²)")}.`)+
  step(4,`Divide: ${m("= (3t−t³)/(1−3t²) = (3tanA−tan³A)/(1−3tan²A)")}. ✓`))},

"h-sin":{t:"sin(θ/2) = ±√((1−cosθ)/2)",b:sec2("REARRANGE cos θ = 1−2sin²(θ/2)",
  step(1,`From double-angle: ${m("cosθ = 1−2sin²(θ/2)")}.`)+
  step(2,`Rearrange: ${m("sin²(θ/2) = (1−cosθ)/2")}. Take square root: ${m("sin(θ/2) = ±√((1−cosθ)/2)")}. ✓`)+
  note("Sign depends on the quadrant of θ/2."))},

"h-cos":{t:"cos(θ/2) = ±√((1+cosθ)/2)",b:sec2("REARRANGE cos θ = 2cos²(θ/2)−1",
  step(1,`${m("cosθ = 2cos²(θ/2)−1")} → ${m("cos²(θ/2) = (1+cosθ)/2")} → ${m("cos(θ/2) = ±√((1+cosθ)/2)")}. ✓`))},

"h-tan":{t:"tan(θ/2) — three equivalent forms",b:sec2("ALL THREE FORMS",
  step(1,`Form 1: ${m("tan(θ/2) = sin(θ/2)/cos(θ/2) = ±√((1−cosθ)/(1+cosθ))")}.`)+
  step(2,`Form 2: Multiply top and bottom of Form 1 by ${m("√(1+cosθ)")}:`)+
  step(3,`${m("= (√(1−cosθ)·√(1+cosθ))/(1+cosθ) = √(1−cos²θ)/(1+cosθ) = sinθ/(1+cosθ)")}. ✓`)+
  step(4,`Form 3: Similarly multiply by ${m("√(1−cosθ)")}: get ${m("(1−cosθ)/sinθ")}. ✓`))},

"p2s-sc":{t:"2 sinA cosB = sin(A+B) + sin(A−B)",b:sec2("ADD THE TWO SIN ADDITION FORMULAS",
  step(1,`${m("sin(A+B) = sinA cosB + cosA sinB")}`)+
  step(2,`${m("sin(A−B) = sinA cosB − cosA sinB")}`)+
  step(3,`Add: ${m("sin(A+B)+sin(A−B) = 2sinA cosB")}. ✓`))},

"p2s-cs":{t:"2 cosA sinB = sin(A+B) − sin(A−B)",b:sec2("SUBTRACT",
  step(1,`Subtract sin(A−B) from sin(A+B): ${m("2cosA sinB")}. ✓`))},

"p2s-cc":{t:"2 cosA cosB = cos(A−B) + cos(A+B)",b:sec2("ADD COS FORMULAS",
  step(1,`${m("cos(A−B)+cos(A+B) = (cosA cosB+sinA sinB)+(cosA cosB−sinA sinB) = 2cosA cosB")}. ✓`))},

"p2s-ss":{t:"2 sinA sinB = cos(A−B) − cos(A+B)",b:sec2("SUBTRACT COS FORMULAS",
  step(1,`${m("cos(A−B)−cos(A+B) = 2sinA sinB")}. ✓`))},

"asinbcos":{t:"a·sinθ+b·cosθ = R·sin(θ+φ), R=√(a²+b²)",b:sec2("EXPAND AND COMPARE COEFFICIENTS",
  step(1,`Expand: ${m("R·sin(θ+φ) = R sinθ cosφ + R cosθ sinφ")}.`)+
  step(2,`Compare with a·sinθ+b·cosθ: need ${m("R cosφ = a")} and ${m("R sinφ = b")}.`)+
  step(3,`Square and add: ${m("R²(cos²φ+sin²φ) = a²+b²")} → ${m("R = √(a²+b²)")}. ✓`)+
  step(4,`Divide: ${m("tanφ = b/a")}. Max value = +R (when sin=1), Min = −R. ✓`))},

"iv-comp":{t:"sin⁻¹x + cos⁻¹x = π/2",b:sec2("PROOF FROM COMPLEMENTARY ANGLES",
  step(1,`Let ${m("sin⁻¹x = α")}, so sinα = x, where α ∈ [−π/2, π/2].`)+
  step(2,`Then ${m("cos(π/2−α) = sinα = x")}, and since (π/2−α) ∈ [0,π], we have ${m("cos⁻¹x = π/2−α")}.`)+
  step(3,`Therefore ${m("sin⁻¹x + cos⁻¹x = α+(π/2−α) = π/2")}. ✓`)+
  note("Same logic applies for tan⁻¹+cot⁻¹ and sec⁻¹+cosec⁻¹."))},

"iv-neg":{t:"sin⁻¹(−x)=−sin⁻¹x and cos⁻¹(−x)=π−cos⁻¹x",b:sec2("ODD/EVEN PROPERTIES",
  step(1,`For sin⁻¹: Let sin⁻¹x=α. Then sin(−α)=−x, and −α ∈ [−π/2,π/2], so ${m("sin⁻¹(−x)=−α=−sin⁻¹x")}. ✓`)+
  step(2,`For cos⁻¹: Let cos⁻¹x=α. Then cos(π−α)=−cosα=−x, and (π−α)∈[0,π], so ${m("cos⁻¹(−x)=π−α=π−cos⁻¹x")}. ✓`))},

"iv-rec":{t:"sin⁻¹(1/x) = cosec⁻¹x for |x|≥1",b:sec2("FROM RECIPROCAL RELATION",
  step(1,`Let cosec⁻¹x=θ, so cosecθ=x → sinθ=1/x.`)+
  step(2,`Since θ∈[−π/2,π/2]−{0}, this is within the range of sin⁻¹. So ${m("sin⁻¹(1/x)=θ=cosec⁻¹x")}. ✓`))},

"iv-tadd":{t:"tan⁻¹x+tan⁻¹y = tan⁻¹((x+y)/(1−xy)) when xy<1",b:sec2("USING TAN ADDITION FORMULA",
  step(1,`Let α=tan⁻¹x, β=tan⁻¹y. Then tanα=x, tanβ=y.`)+
  step(2,`${m("tan(α+β) = (tanα+tanβ)/(1−tanα tanβ) = (x+y)/(1−xy)")}.`)+
  step(3,`When xy<1, the sum α+β ∈ (−π/2,π/2), so ${m("α+β = tan⁻¹((x+y)/(1−xy))")}. ✓`)+
  note("When x>0, y>0, xy>1: α+β > π/2, so we add π to adjust to the correct range."))},

"iv-2t":{t:"2tan⁻¹x = sin⁻¹(2x/(1+x²))",b:sec2("USING DOUBLE ANGLE SUBSTITUTION",
  step(1,`Let θ=tan⁻¹x so tanθ=x. Then:`)+
  step(2,`${m("sin2θ = 2tanθ/(1+tan²θ) = 2x/(1+x²")}). So ${m("sin⁻¹(2x/(1+x²)) = 2θ = 2tan⁻¹x")}. ✓`)+
  step(3,`Similarly ${m("cos2θ = (1−tan²θ)/(1+tan²θ) = (1−x²)/(1+x²)")}, giving the cos⁻¹ form. ✓`))},

"gs-sin":{t:"sinθ=sinα → θ = nπ+(−1)ⁿα",b:sec2("PROOF USING SUM-TO-PRODUCT",
  step(1,`${m("sinθ−sinα = 0")} → Use S2P: ${m("2cos((θ+α)/2)sin((θ−α)/2) = 0")}.`)+
  step(2,`Case 1: ${m("sin((θ−α)/2)=0")} → ${m("(θ−α)/2=mπ")} → θ=2mπ+α (even n).`)+
  step(3,`Case 2: ${m("cos((θ+α)/2)=0")} → ${m("(θ+α)/2=(2k+1)π/2")} → θ=(2k+1)π−α (odd n).`)+
  step(4,`Both cases combine into: ${m("θ = nπ+(−1)ⁿα")}. ✓`))},

"gs-cos":{t:"cosθ=cosα → θ = 2nπ±α",b:sec2("PROOF USING SUM-TO-PRODUCT",
  step(1,`${m("cosθ−cosα=0")} → ${m("−2sin((θ+α)/2)sin((θ−α)/2)=0")}.`)+
  step(2,`Either sin((θ−α)/2)=0 → θ=2nπ+α, or sin((θ+α)/2)=0 → θ=2nπ−α. Both: ${m("θ=2nπ±α")}. ✓`))},

"gs-tan":{t:"tanθ=tanα → θ = nπ+α",b:sec2("PROOF",
  step(1,`${m("tanθ=tanα")} → ${m("sinθcosα−cosθsinα=0")} → ${m("sin(θ−α)=0")}.`)+
  step(2,`So θ−α=nπ → ${m("θ=nπ+α")}. ✓ This proves the period of tan is π.`))},

"gs-sin0":{t:"sinθ=0 → θ=nπ",b:sec2("SPECIAL CASE",step(1,`Special case of sinθ=sinα with α=0: ${m("θ=nπ+(−1)ⁿ·0=nπ")}. These are the zero-crossings of the sine wave. ✓`))},
"gs-cos0":{t:"cosθ=0 → θ=(2n+1)π/2",b:sec2("SPECIAL CASE",step(1,`cosθ=cos(π/2): ${m("θ=2nπ±π/2=(4n±1)π/2")}. Simplified: θ=(2k+1)π/2. ✓`))},
"gs-tan0":{t:"tanθ=0 → θ=nπ",b:sec2("SPECIAL CASE",step(1,`tanθ=tan0 → θ=nπ+0=nπ. ✓`))},

"gs-sq":{t:"sin²θ=sin²α → θ=nπ±α",b:sec2("FACTOR",
  step(1,`${m("sin²θ−sin²α=0")} → ${m("sin(θ+α)·sin(θ−α)=0")}.`)+
  step(2,`Either θ+α=nπ or θ−α=nπ → both give ${m("θ=nπ±α")}. ✓ Same for cos² and tan².`))},

"pr-sin":{t:"sinθ·sin(60°−θ)·sin(60°+θ) = (1/4)sin3θ",b:sec2("USING PRODUCT FORMULA",
  step(1,`${m("sin(60°−θ)·sin(60°+θ) = sin²60°−sin²θ = 3/4−sin²θ")}.`)+
  step(2,`Multiply by sinθ: ${m("sinθ(3/4−sin²θ) = (3sinθ−4sin³θ)/4 = sin3θ/4")}. ✓`))},

"pr-cos":{t:"cosθ·cos(60°−θ)·cos(60°+θ) = (1/4)cos3θ",b:sec2("USING PRODUCT FORMULA",
  step(1,`${m("cos(60°−θ)·cos(60°+θ) = cos²θ−sin²60° = cos²θ−3/4")}.`)+
  step(2,`Multiply by cosθ: ${m("cosθ(cos²θ−3/4) = (4cos³θ−3cosθ)/4 = cos3θ/4")}. ✓`))},

"pr-tan":{t:"tanθ·tan(60°−θ)·tan(60°+θ) = tan3θ",b:sec2("FROM SIN AND COS PRODUCTS",
  step(1,`Ratio = ${m("[sinθ·sin(60°−θ)·sin(60°+θ)] / [cosθ·cos(60°−θ)·cos(60°+θ)]")}`)+
  step(2,`= ${m("(sin3θ/4) / (cos3θ/4) = tan3θ")}. ✓`))},

"sine-rule":{t:"a/sinA = b/sinB = c/sinC = 2R",b:sec2("PROOF VIA CIRCUMSCRIBED CIRCLE",
  step(1,`Let O be the circumcenter of △ABC with circumradius R. Draw diameter BD = 2R.`)+
  step(2,`Angle in semicircle: ∠BCD = 90°. In △BCD: ${m("sin(∠BDC) = BC/BD = a/(2R)")}.`)+
  step(3,`∠BDC = ∠A (angles subtended by same chord BC). So ${m("sinA = a/(2R)")} → ${m("a/sinA = 2R")}. ✓`)+
  step(4,`Same argument for b and c. All three equal 2R.`))},

"cos-rule":{t:"cosA = (b²+c²−a²)/2bc",b:sec2("PROOF USING COORDINATES",
  step(1,`Place B at origin, C at (a,0). Then A = (c cosB, c sinB).`)+
  step(2,`${m("b² = AC² = (c cosB−a)² + (c sinB)² = c²−2ac cosB+a²")}.`)+
  step(3,`Rearrange: ${m("cosB = (a²+c²−b²)/(2ac")}). Relabel to get ${m("cosA = (b²+c²−a²)/(2bc)")}. ✓`))},

"area":{t:"Area = ½ab sinC = √(s(s−a)(s−b)(s−c))",b:sec2("TWO PROOFS",
  step(1,`Base = a, height from A = b sinC. Area = ${m("½·a·b sinC")}. ✓`)+
  step(2,`For Heron's formula: express sinC via cosine rule. With s=(a+b+c)/2, extensive algebra gives ${m("Δ = √(s(s−a)(s−b)(s−c))")}. ✓`))},

"ci-tan":{t:"If A+B+C=π: tanA+tanB+tanC = tanA·tanB·tanC",b:sec2("PROOF",
  step(1,`A+B = π−C, so ${m("tan(A+B) = tan(π−C) = −tanC")}.`)+
  step(2,`Expand: ${m("(tanA+tanB)/(1−tanA tanB) = −tanC")}.`)+
  step(3,`${m("tanA+tanB = −tanC(1−tanA tanB) = −tanC+tanA tanB tanC")}.`)+
  step(4,`${m("tanA+tanB+tanC = tanA tanB tanC")}. ✓`))},

"ci-half":{t:"tan(A/2)tan(B/2)+tan(B/2)tan(C/2)+tan(C/2)tan(A/2) = 1",b:sec2("PROOF",
  step(1,`A/2+B/2+C/2 = π/2, so A/2+B/2 = π/2−C/2.`)+
  step(2,`${m("tan(A/2+B/2) = cot(C/2)")}.`)+
  step(3,`Expand tan(A/2+B/2) and cross-multiply: ${m("tanA/2+tanB/2 = cotC/2·(1−tanA/2·tanB/2)")}.`)+
  step(4,`Sum all three symmetric forms; after simplification: sum of products = 1. ✓`))}
};


const _ov=document.getElementById('proof-overlay');
const _pt=document.getElementById('proof-title');
const _pb=document.getElementById('proof-body');
function openProof(key){
  const d=PROOFS[key];
  _pt.innerHTML=d?d.t:'Proof coming soon!';
  _pb.innerHTML=d?d.b:'<div class="pstep"><div class="sn2">i</div><div class="st">Coming soon.</div></div>';
  _ov.classList.add('show');
}
function closeProof(){_ov.classList.remove('show');}
document.getElementById('proof-close').addEventListener('click',closeProof);
_ov.addEventListener('click',e=>{if(e.target===_ov)closeProof();});
document.addEventListener('keydown',e=>{if(e.key==='Escape')closeProof();});
// Wire all [data-p] elements AFTER DOM is ready
document.addEventListener('DOMContentLoaded',()=>{
  document.querySelectorAll('[data-p]').forEach(el=>el.addEventListener('click',()=>openProof(el.dataset.p)));
});
// Also wire immediately in case DOMContentLoaded already fired
document.querySelectorAll('[data-p]').forEach(el=>el.addEventListener('click',()=>openProof(el.dataset.p)));

/* CANVAS GRAPHS */
// ═══════════════════════════════════════════════
//  CANVAS GRAPHS
// ═══════════════════════════════════════════════
const TC=document.getElementById('tc');
const FC={sin:'#e8b84b',cos:'#4b9fe8',tan:'#e84b7a',csc:'#4be8a0',sec:'#b84be8',cot:'#e8a04b'};
let AT=new Set(['sin','cos']);

function resizeCanvas(c){const dpr=window.devicePixelRatio||1,w=c.parentElement.clientWidth,h=380;c.style.width=w+'px';c.style.height=h+'px';c.width=w*dpr;c.height=h*dpr;const cx=c.getContext('2d');cx.scale(dpr,dpr);return[w,h];}

function drawTrig(){
  const ctx=TC.getContext('2d');
  const[W,H]=resizeCanvas(TC);
  ctx.clearRect(0,0,W,H);
  const ox=W/2,oy=H/2,xs=W/(4*Math.PI),ys=H/6,CL=4;
  ctx.strokeStyle='rgba(42,42,58,.8)';ctx.lineWidth=1;
  for(let i=-3;i<=3;i++){const y=oy-i*ys;ctx.beginPath();ctx.moveTo(0,y);ctx.lineTo(W,y);ctx.stroke();}
  for(let i=-6;i<=6;i++){const x=ox+i*Math.PI*xs;ctx.beginPath();ctx.moveTo(x,0);ctx.lineTo(x,H);ctx.stroke();}
  ctx.strokeStyle='rgba(120,120,160,.5)';ctx.lineWidth=1.5;
  ctx.beginPath();ctx.moveTo(0,oy);ctx.lineTo(W,oy);ctx.stroke();
  ctx.beginPath();ctx.moveTo(ox,0);ctx.lineTo(ox,H);ctx.stroke();
  ctx.fillStyle='rgba(120,120,160,.7)';ctx.font='10px JetBrains Mono,monospace';ctx.textAlign='center';
  const pl=['-2π','-3π/2','-π','-π/2','','π/2','π','3π/2','2π'];
  for(let i=-4;i<=4;i++){const lbl=pl[i+4];if(lbl)ctx.fillText(lbl,ox+i*Math.PI*xs,oy+13);}
  for(let i=-2;i<=2;i++){if(!i)continue;ctx.textAlign='right';ctx.fillText(i,ox-6,oy-i*ys+4);}
  const FNS={sin:x=>Math.sin(x),cos:x=>Math.cos(x),tan:x=>Math.tan(x),csc:x=>1/Math.sin(x),sec:x=>1/Math.cos(x),cot:x=>Math.cos(x)/Math.sin(x)};
  for(const[n,fn] of Object.entries(FNS)){
    if(!AT.has(n))continue;
    ctx.strokeStyle=FC[n];ctx.lineWidth=2.2;ctx.beginPath();let pd=false;
    for(let px=0;px<=W*2;px++){const sx=(px/(W*2))*W,mx=(sx-ox)/xs,my=fn(mx);
      if(!isFinite(my)||Math.abs(my)>CL){pd=false;continue;}
      const sy=oy-my*ys;pd?(ctx.lineTo(sx,sy)):(ctx.moveTo(sx,sy),pd=true);}
    ctx.stroke();
  }
  let lx=14;ctx.font='11px JetBrains Mono,monospace';
  for(const n of AT){ctx.fillStyle=FC[n];ctx.fillRect(lx,10,18,3);ctx.fillText(n,lx+24,18);lx+=62;}
}

// Trig toggle buttons (only .ft with data-fn in FC)
document.querySelectorAll('.ft[data-fn]').forEach(b=>{
  b.addEventListener('click',()=>{
    const fn=b.dataset.fn;
    if(!(fn in FC))return;
    b.classList.toggle('on');
    AT.has(fn)?AT.delete(fn):AT.add(fn);
    drawTrig();
  });
});

drawTrig();
window.addEventListener('resize',()=>{drawTrig();if(document.getElementById('itf-ind-canvas'))drawITFInd();if(document.getElementById('itfc'))drawITF();});

/* ITF INDIVIDUAL GRAPHS (sin⁻¹x, cos⁻¹x, etc.) */
const ITFIC=document.getElementById('itf-ind-canvas');
const ITF_IND_COLORS={asin:'#e8b84b',acos:'#4b9fe8',atan:'#e84b7a',acot:'#4be8a0',asec:'#b84be8',acsc:'#e8a04b'};
const ITF_IND_LABELS={asin:'sin⁻¹ x',acos:'cos⁻¹ x',atan:'tan⁻¹ x',acot:'cot⁻¹ x',asec:'sec⁻¹ x',acsc:'cosec⁻¹ x'};
let AITF_IND=new Set(['asin','acos','atan']);

function _itfIndFn(name,x){
  switch(name){
    case 'asin': return(x>=-1&&x<=1)?Math.asin(x):NaN;
    case 'acos': return(x>=-1&&x<=1)?Math.acos(x):NaN;
    case 'atan': return Math.atan(x);
    case 'acot': return Math.PI/2-Math.atan(x);
    case 'asec': return Math.abs(x)>=1?Math.acos(1/x):NaN;
    case 'acsc': return Math.abs(x)>=1?Math.asin(1/x):NaN;
    default: return NaN;
  }
}

function drawITFInd(){
  if(!ITFIC)return;
  const ctx=ITFIC.getContext('2d');
  const[W,H]=resizeCanvas(ITFIC);
  ctx.clearRect(0,0,W,H);
  const PI=Math.PI;
  const ox=W/2,oy=H/2;
  const xs=W/12,ys=H/(2.4*PI); // x: ±6, y: shows ±π comfortably

  // Grid
  ctx.strokeStyle='rgba(42,42,58,.8)';ctx.lineWidth=1;
  // Horizontal lines at -π, -π/2, 0, π/2, π
  [-PI,-PI/2,0,PI/2,PI].forEach(ty=>{const sy=oy-ty*ys;ctx.beginPath();ctx.moveTo(0,sy);ctx.lineTo(W,sy);ctx.stroke();});
  // Vertical lines every unit
  for(let i=-6;i<=6;i++){const sx=ox+i*xs;ctx.beginPath();ctx.moveTo(sx,0);ctx.lineTo(sx,H);ctx.stroke();}

  // Axes
  ctx.strokeStyle='rgba(120,120,160,.5)';ctx.lineWidth=1.5;
  ctx.beginPath();ctx.moveTo(0,oy);ctx.lineTo(W,oy);ctx.stroke();
  ctx.beginPath();ctx.moveTo(ox,0);ctx.lineTo(ox,H);ctx.stroke();

  // Axis labels
  ctx.fillStyle='rgba(120,120,160,.7)';ctx.font='10px JetBrains Mono,monospace';ctx.textAlign='center';
  for(let i=-6;i<=6;i++){if(!i)continue;ctx.fillText(i,ox+i*xs,oy+14);}
  ctx.textAlign='right';
  const yLabs={'-π':-PI,'-π/2':-PI/2,'π/2':PI/2,'π':PI};
  for(const[l,v] of Object.entries(yLabs))ctx.fillText(l,ox-7,oy-v*ys+4);

  // Draw domain boundary indicators
  ctx.strokeStyle='rgba(255,255,255,.06)';ctx.lineWidth=1;ctx.setLineDash([4,4]);
  // x=±1 dashed lines (for asin/acos/asec/acsc domain bounds)
  [-1,1].forEach(xb=>{const sx=ox+xb*xs;ctx.beginPath();ctx.moveTo(sx,0);ctx.lineTo(sx,H);ctx.stroke();});
  ctx.setLineDash([]);

  // Plot functions
  const STEPS=W*4;
  const xMin=(0-ox)/xs, xMax=(W-ox)/xs;
  for(const name of Object.keys(ITF_IND_COLORS)){
    if(!AITF_IND.has(name))continue;
    ctx.strokeStyle=ITF_IND_COLORS[name];ctx.lineWidth=2.5;
    ctx.beginPath();let pd=false;
    let prevY=NaN;
    for(let p=0;p<=STEPS;p++){
      const mx=xMin+(xMax-xMin)*(p/STEPS);
      const my=_itfIndFn(name,mx);
      if(isNaN(my)||!isFinite(my)){pd=false;prevY=NaN;continue;}
      if(pd&&Math.abs(my-prevY)>PI){pd=false;}
      const sx=ox+mx*xs, sy=oy-my*ys;
      pd?(ctx.lineTo(sx,sy)):(ctx.moveTo(sx,sy),pd=true);
      prevY=my;
    }
    ctx.stroke();

    // Endpoint dots for bounded domains
    if(name==='asin'||name==='acos'){
      const pts=[[-1,_itfIndFn(name,-1)],[1,_itfIndFn(name,1)]];
      pts.forEach(([mx,my])=>{if(isNaN(my))return;const sx=ox+mx*xs,sy=oy-my*ys;ctx.beginPath();ctx.arc(sx,sy,4,0,2*Math.PI);ctx.fillStyle=ITF_IND_COLORS[name];ctx.fill();});
    }
    if(name==='asec'||name==='acsc'){
      // Endpoints at x=±1, ±∞ — just show at ±1
      [[-1,_itfIndFn(name,-1)],[1,_itfIndFn(name,1)]].forEach(([mx,my])=>{if(isNaN(my))return;const sx=ox+mx*xs,sy=oy-my*ys;ctx.beginPath();ctx.arc(sx,sy,4,0,2*Math.PI);ctx.fillStyle=ITF_IND_COLORS[name];ctx.fill();});
    }
  }

  // Legend
  let lx=14;ctx.font='11px JetBrains Mono,monospace';
  for(const name of Object.keys(ITF_IND_COLORS)){
    if(!AITF_IND.has(name))continue;
    ctx.fillStyle=ITF_IND_COLORS[name];ctx.fillRect(lx,10,18,3);
    ctx.fillText(ITF_IND_LABELS[name],lx+24,18);lx+=ITF_IND_LABELS[name].length*7+14;
  }
}

// Toggle buttons for ITF individual
document.querySelectorAll('.itf-ind-btn').forEach(b=>{
  b.addEventListener('click',()=>{
    const fn=b.dataset.iifn;
    b.classList.toggle('on');
    AITF_IND.has(fn)?AITF_IND.delete(fn):AITF_IND.add(fn);
    drawITFInd();
  });
});

// Draw on load
if(document.getElementById('itf-ind-canvas'))setTimeout(drawITFInd,120);

/* ITF COMPOSITE GRAPHS */
const ITFC=document.getElementById('itfc');
const ITF_COLORS={
  asin_sin:'#e8b84b',
  acos_cos:'#e84b7a',
  atan_tan:'#b84be8'
};
const ITF_LABELS={
  asin_sin:'sin⁻¹(sin x)',
  acos_cos:'cos⁻¹(cos x)',
  atan_tan:'tan⁻¹(tan x)'
};
let AITF=new Set(['asin_sin']);

function _itfFn(name,x){
  switch(name){
    case 'asin_sin': return Math.asin(Math.sin(x));
    case 'acos_cos': return Math.acos(Math.cos(x));
    case 'atan_tan': {
      const eps=1e-6;
      if(Math.abs(Math.cos(x))<eps)return NaN;
      return Math.atan(Math.tan(x));
    }
    default: return NaN;
  }
}

function drawITF(){
  if(!ITFC)return;
  const ctx2=ITFC.getContext('2d');
  const[W,H]=resizeCanvas(ITFC);
  ctx2.clearRect(0,0,W,H);
  const PI=Math.PI;
  const ox=W/2,oy=H/2;
  const xs=W/(4*PI),ys=H/(1.1*PI); // x: ±2π, y: ±π/2 comfortable

  // Grid lines
  ctx2.strokeStyle='rgba(42,42,58,.8)';ctx2.lineWidth=1;
  const yTicks=[-PI,-PI/2,0,PI/2,PI];
  yTicks.forEach(ty=>{const sy=oy-ty*ys;ctx2.beginPath();ctx2.moveTo(0,sy);ctx2.lineTo(W,sy);ctx2.stroke();});
  for(let i=-4;i<=4;i++){const sx=ox+i*PI*xs;ctx2.beginPath();ctx2.moveTo(sx,0);ctx2.lineTo(sx,H);ctx2.stroke();}

  // Axes
  ctx2.strokeStyle='rgba(120,120,160,.5)';ctx2.lineWidth=1.5;
  ctx2.beginPath();ctx2.moveTo(0,oy);ctx2.lineTo(W,oy);ctx2.stroke();
  ctx2.beginPath();ctx2.moveTo(ox,0);ctx2.lineTo(ox,H);ctx2.stroke();

  // Axis labels
  ctx2.fillStyle='rgba(120,120,160,.7)';ctx2.font='10px JetBrains Mono,monospace';ctx2.textAlign='center';
  const xLbls=['-2π','-3π/2','-π','-π/2','','π/2','π','3π/2','2π'];
  for(let i=-4;i<=4;i++){const lbl=xLbls[i+4];if(lbl)ctx2.fillText(lbl,ox+i*PI*xs,oy+13);}
  ctx2.textAlign='right';
  const yLbls={'-π':-PI,'-π/2':-PI/2,'π/2':PI/2,'π':PI};
  for(const[l,v] of Object.entries(yLbls))ctx2.fillText(l,ox-6,oy-v*ys+4);

  // Draw each active function
  const STEPS=W*3;
  const xMin=(0-ox)/xs, xMax=(W-ox)/xs;
  for(const name of Object.keys(ITF_COLORS)){
    if(!AITF.has(name))continue;
    ctx2.strokeStyle=ITF_COLORS[name];ctx2.lineWidth=2.2;
    ctx2.beginPath();let pd=false;
    let prevY=NaN;
    for(let p=0;p<=STEPS;p++){
      const mx=xMin+(xMax-xMin)*(p/STEPS);
      const my=_itfFn(name,mx);
      if(isNaN(my)||!isFinite(my)){pd=false;prevY=NaN;continue;}
      // Detect discontinuity jump (e.g. atan_tan sawtooth)
      if(pd&&Math.abs(my-prevY)>PI*0.9){pd=false;}
      const sx=ox+mx*xs, sy=oy-my*ys;
      pd?(ctx2.lineTo(sx,sy)):(ctx2.moveTo(sx,sy),pd=true);
      prevY=my;
    }
    ctx2.stroke();
  }

  // Legend
  let lx=14;ctx2.font='11px JetBrains Mono,monospace';
  for(const name of AITF){
    ctx2.fillStyle=ITF_COLORS[name];ctx2.fillRect(lx,10,18,3);
    ctx2.fillText(ITF_LABELS[name],lx+24,18);lx+=ITF_LABELS[name].length*7+16;
  }
}

// ITF toggle buttons
document.querySelectorAll('.itf-btn').forEach(b=>{
  b.addEventListener('click',()=>{
    const fn=b.dataset.ifn;
    b.classList.toggle('on');
    AITF.has(fn)?AITF.delete(fn):AITF.add(fn);
    drawITF();
  });
});

// Initial draw (only if trig section is active on load)
if(document.getElementById('itfc'))setTimeout(drawITF,100);

/* DESMOS MODULE — iframe approach */
(function(){
  const frame=document.getElementById('desmos-frame');
  const loader=document.getElementById('desmos-loading');
  if(frame&&loader){
    frame.addEventListener('load',()=>{
      loader.style.transition='opacity .5s';
      loader.style.opacity='0';
      setTimeout(()=>loader.style.display='none',520);
    });
  }

  // Preset buttons: open Desmos with expression pre-filled (new tab)
  // Map from button label to a Desmos-shareable URL with the expression
  document.querySelectorAll('.dsm-preset').forEach(b=>{
    b.addEventListener('click',()=>{
      if(b.classList.contains('dsm-clear')){
        // Reload iframe to blank Desmos
        if(frame)frame.src='https://www.desmos.com/calculator';
        return;
      }
      const expr=b.dataset.expr;
      if(!expr)return;
      // Encode and open in new tab
      const url='https://www.desmos.com/calculator?'+new URLSearchParams({equations:JSON.stringify([{latex:expr}])});
      // Flash effect
      b.style.transition='background .12s';b.style.background='rgba(80,216,144,.12)';
      setTimeout(()=>b.style.background='',320);
      window.open('https://www.desmos.com/calculator','desmos-popup','width=1000,height=700,menubar=no,toolbar=no');
    });
  });

  // Reset view: reload iframe
  const rst=document.getElementById('dsm-reset-view');
  if(rst)rst.addEventListener('click',()=>{if(frame){frame.src='https://www.desmos.com/calculator';}});

  // Grid toggle: no-op for iframe (user controls inside Desmos)
  const grd=document.getElementById('dsm-toggle-grid');
  if(grd){grd.textContent='↗ Open Full';grd.addEventListener('click',()=>window.open('https://www.desmos.com/calculator','_blank'));}

  const cnt=document.getElementById('dsm-expr-count');
  if(cnt)cnt.textContent='DESMOS GRAPHING CALCULATOR';
})();

/* CONICLAB */

// ═══════════════════════════════════
// STATE
// ═══════════════════════════════════
const cvs = document.getElementById('cvs');
const ctx = cvs.getContext('2d');
let W, H, ox, oy, scale = 60;
let dragging = false, lastMX = 0, lastMY = 0;
let selectedId = null;
let curves = [], nextId = 1;
let mode = 'pan'; // pan | draw_line | draw_circle | draw_point
let drawPts = []; // temp points for draw mode

const S = {
  gridPx:60, showGrid:true, axisLabels:true,
  lw:2, foci:true, verts:true, asym:true, dir:true, curveLabels:true
};

const COLORS = ['#f0c060','#40d0c0','#f06080','#a080f0','#60b8f0','#50d890','#f08040','#e080d0','#80e0a0','#f0a040','#c0e060','#80c0f0'];

// sidebar visible?
let sidebarOpen = true;

// ═══════════════════════════════════
// RESIZE
// ═══════════════════════════════════
function resize() {
  const dpr = devicePixelRatio || 1;
  W = window.innerWidth; H = window.innerHeight;
  cvs.width = W * dpr; cvs.height = H * dpr;
  cvs.style.width = W+'px'; cvs.style.height = H+'px';
  ctx.setTransform(dpr,0,0,dpr,0,0);
  if (!ox) { ox = W/2; oy = H/2; }
  redraw();
}
window.addEventListener('resize', resize);

// ═══════════════════════════════════
// COORD TRANSFORMS
// ═══════════════════════════════════
const sx = x => ox + x*scale;
const sy = y => oy - y*scale;
const wx = X => (X - ox)/scale;
const wy = Y => -(Y - oy)/scale;

// ═══════════════════════════════════
// SIDEBAR
// ═══════════════════════════════════
function toggleSidebar() {
  sidebarOpen = !sidebarOpen;
  document.getElementById('sidebar').classList.toggle('hidden', !sidebarOpen);
}
function hideSidebar() {
  sidebarOpen = false;
  document.getElementById('sidebar').classList.add('hidden');
}

// ═══════════════════════════════════
// DRAW MODE
// ═══════════════════════════════════
function setMode(m) {
  mode = m;
  drawPts = [];
  document.querySelectorAll('.ctb').forEach(b=>b.classList.remove('active'));
  document.getElementById('tb-'+m)?.classList.add('active');
  const ind = document.getElementById('draw-indicator');
  const modeDisp = document.getElementById('mode-display');
  if (m === 'pan') {
    ind.style.display='none'; cvs.style.cursor='crosshair';
    modeDisp.textContent='PAN MODE';
  } else if (m === 'draw_line') {
    ind.style.display='block'; ind.textContent='📏 LINE — Click 2 points on canvas';
    cvs.style.cursor='crosshair'; modeDisp.textContent='DRAW LINE';
  } else if (m === 'draw_circle') {
    ind.style.display='block'; ind.textContent='⭕ CIRCLE — Click centre, then radius point';
    cvs.style.cursor='crosshair'; modeDisp.textContent='DRAW CIRCLE';
  } else if (m === 'draw_point') {
    ind.style.display='block'; ind.textContent='✦ POINT — Click to drop points';
    cvs.style.cursor='crosshair'; modeDisp.textContent='DRAW POINTS';
  }
}

// ═══════════════════════════════════
// REDRAW
// ═══════════════════════════════════
function redraw() {
  ctx.clearRect(0,0,W,H);
  ctx.fillStyle='#080b10'; ctx.fillRect(0,0,W,H);
  if (S.showGrid) drawGrid();
  drawAxes();
  curves.forEach(c => { if(c.visible) drawCurve(c); });
  if (drawPts.length) drawGhostPts();
}

// ─── GRID ───
function drawGrid() {
  const step = scale;
  ctx.strokeStyle='#0f1520'; ctx.lineWidth=0.5;
  const sub = step/5;
  ctx.beginPath();
  for(let x=ox%sub;x<W;x+=sub){ctx.moveTo(x,0);ctx.lineTo(x,H);}
  for(let y=oy%sub;y<H;y+=sub){ctx.moveTo(0,y);ctx.lineTo(W,y);}
  ctx.stroke();
  ctx.strokeStyle='#161e2e'; ctx.lineWidth=1;
  ctx.beginPath();
  for(let x=ox%step;x<W;x+=step){ctx.moveTo(x,0);ctx.lineTo(x,H);}
  for(let y=oy%step;y<H;y+=step){ctx.moveTo(0,y);ctx.lineTo(W,y);}
  ctx.stroke();
  if(S.axisLabels) {
    ctx.fillStyle='#2a3850'; ctx.font='500 10px JetBrains Mono';
    const n0x=Math.ceil((-ox)/scale), n1x=Math.floor((W-ox)/scale);
    ctx.textAlign='center';
    for(let n=n0x;n<=n1x;n++){if(!n)continue;ctx.fillText(n,sx(n),oy+13);}
    ctx.textAlign='right';
    const n0y=Math.ceil(-(oy)/scale), n1y=Math.floor((H-oy)/scale);
    // flip: screen y increases downward, math y increases upward
    const gy0=Math.floor(-(H-oy)/scale), gy1=Math.ceil(oy/scale);
    for(let n=gy0;n<=gy1;n++){if(!n)continue;ctx.fillText(n,ox-5,sy(n)+4);}
  }
}

// ─── AXES ───
function drawAxes() {
  ctx.strokeStyle='#263040'; ctx.lineWidth=1.5;
  ctx.beginPath(); ctx.moveTo(0,oy); ctx.lineTo(W,oy);
  ctx.moveTo(ox,0); ctx.lineTo(ox,H); ctx.stroke();
  ctx.fillStyle='#263040'; arrow(W-1,oy,0); arrow(ox,1,-Math.PI/2);
  ctx.fillStyle='#334466'; ctx.font='600 12px JetBrains Mono';
  ctx.textAlign='left'; ctx.fillText('x',W-16,oy-6);
  ctx.textAlign='center'; ctx.fillText('y',ox+14,12); ctx.fillText('O',ox+10,oy+14);
}
function arrow(x,y,a){ctx.save();ctx.translate(x,y);ctx.rotate(a);ctx.beginPath();ctx.moveTo(0,0);ctx.lineTo(-10,-5);ctx.lineTo(-10,5);ctx.closePath();ctx.fill();ctx.restore();}

// ─── GHOST PTS ───
function drawGhostPts() {
  drawPts.forEach((p,i)=>{
    ctx.save(); ctx.fillStyle=i===0?'#f0c060':'#40d0c0'; ctx.shadowBlur=12; ctx.shadowColor=ctx.fillStyle;
    ctx.beginPath(); ctx.arc(sx(p[0]),sy(p[1]),5,0,2*Math.PI); ctx.fill(); ctx.restore();
    ctx.fillStyle='#e8e0d0'; ctx.font='10px JetBrains Mono';
    ctx.fillText('('+p[0].toFixed(1)+','+p[1].toFixed(1)+')',sx(p[0])+8,sy(p[1])-6);
  });
}

// ═══════════════════════════════════
// CURVE DRAWING
// ═══════════════════════════════════
function drawCurve(c) {
  const θ = (c.rotation||0)*Math.PI/180;
  const sel = c.id===selectedId;
  ctx.save();
  ctx.strokeStyle = c.color;
  ctx.lineWidth = sel ? S.lw+1.5 : S.lw;
  ctx.shadowColor = c.color;
  ctx.shadowBlur = sel ? 14 : 5;

  switch(c.type){
    case 'line':    drawLine(c,θ); break;
    case 'line_g':  drawLineG(c,θ); break;
    case 'circle':  drawCircle(c,θ); break;
    case 'para_r':  drawParaR(c,θ); break;
    case 'para_l':  drawParaL(c,θ); break;
    case 'para_u':  drawParaU(c,θ); break;
    case 'para_d':  drawParaD(c,θ); break;
    case 'ellipse': drawEllipse(c,θ); break;
    case 'hyp':     drawHyp(c,θ); break;
    case 'hyp_c':   drawHypC(c,θ); break;
    case 'rhyp':    drawRHyp(c,θ); break;
    case 'pt':      drawPt(c); break;
  }
  if(c.tans) c.tans.forEach(t=>drawTanNorm(c,t));
  ctx.restore();
}

// ─── ROT HELPERS ───
function rpt(x,y,cx,cy,θ){const dx=x-cx,dy=y-cy;return[cx+dx*Math.cos(θ)-dy*Math.sin(θ),cy+dx*Math.sin(θ)+dy*Math.cos(θ)];}

function path(pts,close=false){
  if(!pts.length)return;
  ctx.beginPath(); let pen=false;
  for(let i=0;i<pts.length;i++){
    const p=pts[i];
    if(!isFinite(p[0])||!isFinite(p[1])){pen=false;continue;}
    if(i>0){const pr=pts[i-1];if(isFinite(pr[0])&&Math.hypot(p[0]-pr[0],p[1]-pr[1])>40){pen=false;}}
    if(!pen){ctx.moveTo(sx(p[0]),sy(p[1]));pen=true;}
    else ctx.lineTo(sx(p[0]),sy(p[1]));
  }
  if(close)ctx.closePath(); ctx.stroke();
}

function dotR(px,py,col,r,lbl){
  ctx.save();ctx.fillStyle=col;ctx.shadowBlur=10;ctx.shadowColor=col;
  ctx.beginPath();ctx.arc(px,py,r,0,2*Math.PI);ctx.fill();
  if(lbl){ctx.font='10px JetBrains Mono';ctx.fillStyle=col;ctx.shadowBlur=0;ctx.fillText(lbl,px+r+3,py-r-2);}
  ctx.restore();
}
function dot(x,y,col,r,lbl){dotR(sx(x),sy(y),col,r,lbl);}

function lbl(c,px,py){
  if(!S.curveLabels)return;
  ctx.save();ctx.font='600 11px JetBrains Mono';ctx.fillStyle=c.color+'bb';ctx.shadowBlur=0;
  ctx.fillText(c.name,px,py-8);ctx.restore();
}

function dashLine(x1,y1,x2,y2,col){
  ctx.save();ctx.strokeStyle=col;ctx.lineWidth=1;ctx.shadowBlur=0;ctx.setLineDash([5,4]);
  ctx.beginPath();ctx.moveTo(sx(x1),sy(y1));ctx.lineTo(sx(x2),sy(y2));ctx.stroke();
  ctx.setLineDash([]);ctx.restore();
}

// ─── LINE  y=mx+b ───
function drawLine(c,θ){
  const {m=1,b=0,h=0,k=0}=c.params;
  const far=Math.max(W,H)/scale*1.5;
  const p1=rpt(-far,m*(-far)+b,h,k,θ), p2=rpt(far,m*far+b,h,k,θ);
  ctx.beginPath();ctx.moveTo(sx(p1[0]),sy(p1[1]));ctx.lineTo(sx(p2[0]),sy(p2[1]));ctx.stroke();
  lbl(c,sx(p2[0]-1),sy(p2[1]));
}

// ─── LINE  ax+by+c=0 ───
function drawLineG(c,θ){
  const {a=1,b=-1,k=0,h=0,ky=0}=c.params;
  const far=Math.max(W,H)/scale*1.5;
  let p1,p2;
  if(Math.abs(b)>1e-9){p1=rpt(-far,(-a*(-far)-k)/b,h,ky,θ);p2=rpt(far,(-a*far-k)/b,h,ky,θ);}
  else{const x0=-k/a;p1=rpt(x0,-far,h,ky,θ);p2=rpt(x0,far,h,ky,θ);}
  ctx.beginPath();ctx.moveTo(sx(p1[0]),sy(p1[1]));ctx.lineTo(sx(p2[0]),sy(p2[1]));ctx.stroke();
}

// ─── CIRCLE ───
function drawCircle(c,θ){
  const {h=0,k=0,r=3}=c.params;
  ctx.beginPath();ctx.arc(sx(h),sy(k),r*scale,0,2*Math.PI);ctx.stroke();
  if(S.verts){dot(h,k,c.color,3,'C('+fmt(h)+','+fmt(k)+')');}
  if(S.foci){
    ctx.save();ctx.strokeStyle=c.color+'40';ctx.lineWidth=0.8;ctx.shadowBlur=0;ctx.setLineDash([2,4]);
    ctx.beginPath();ctx.moveTo(sx(h),sy(k));ctx.lineTo(sx(h+r),sy(k));ctx.stroke();
    ctx.setLineDash([]);ctx.restore();
    ctx.save();ctx.fillStyle=c.color+'80';ctx.font='9px JetBrains Mono';ctx.fillText('r='+fmt(r),sx(h)+4,sy(k+r/2)-3);ctx.restore();
  }
  lbl(c,sx(h),sy(k+r)-6);
}

// ─── PARABOLAS ───
function drawParaR(c,θ){
  const{a=2,h=0,k=0}=c.params; const yext=Math.max(W,H)/scale*1.2;
  const pts=[];for(let i=0;i<=500;i++){const y=yext*2*(i/500-.5);pts.push(rpt(y*y/(4*a)+h,y+k,h,k,θ));}
  path(pts);
  if(S.foci)dot(a+h,k,'#f06080',5,'F('+fmt(a+h)+','+fmt(k)+')');
  if(S.dir)dashLine(-a+h,wy(-10),-a+h,wy(H+10),c.color+'80');
  if(S.verts)dot(h,k,c.color,3,'V');
  lbl(c,sx(h+a*.4),sy(k));
}
function drawParaL(c,θ){
  const{a=2,h=0,k=0}=c.params; const yext=Math.max(W,H)/scale*1.2;
  const pts=[];for(let i=0;i<=500;i++){const y=yext*2*(i/500-.5);pts.push(rpt(-y*y/(4*a)+h,y+k,h,k,θ));}
  path(pts);
  if(S.foci)dot(-a+h,k,'#f06080',5,'F');
  if(S.verts)dot(h,k,c.color,3,'V');
}
function drawParaU(c,θ){
  const{a=2,h=0,k=0}=c.params; const xext=Math.max(W,H)/scale*1.2;
  const pts=[];for(let i=0;i<=500;i++){const x=xext*2*(i/500-.5);pts.push(rpt(x+h,x*x/(4*a)+k,h,k,θ));}
  path(pts);
  if(S.foci)dot(h,a+k,'#f06080',5,'F');
  if(S.verts)dot(h,k,c.color,3,'V');
}
function drawParaD(c,θ){
  const{a=2,h=0,k=0}=c.params; const xext=Math.max(W,H)/scale*1.2;
  const pts=[];for(let i=0;i<=500;i++){const x=xext*2*(i/500-.5);pts.push(rpt(x+h,-x*x/(4*a)+k,h,k,θ));}
  path(pts);
  if(S.foci)dot(h,-a+k,'#f06080',5,'F');
  if(S.verts)dot(h,k,c.color,3,'V');
}

// ─── ELLIPSE ───
function drawEllipse(c,θ){
  const{a=4,b=2.5,h=0,k=0}=c.params;
  const pts=[];for(let i=0;i<=400;i++){const t=2*Math.PI*i/400;pts.push(rpt(a*Math.cos(t)+h,b*Math.sin(t)+k,h,k,θ));}
  path(pts,true);
  const cc=Math.sqrt(Math.max(0,a*a-b*b));
  if(S.foci){const f1=rpt(-cc+h,k,h,k,θ),f2=rpt(cc+h,k,h,k,θ);dotR(sx(f1[0]),sy(f1[1]),'#f06080',5,'F₁');dotR(sx(f2[0]),sy(f2[1]),'#f06080',5,'F₂');}
  if(S.verts){dot(h,k,c.color,3,'C');[rpt(-a+h,k,h,k,θ),rpt(a+h,k,h,k,θ),rpt(h,b+k,h,k,θ),rpt(h,-b+k,h,k,θ)].forEach(v=>dotR(sx(v[0]),sy(v[1]),c.color,3,'')); }
  lbl(c,sx(h+a)+5,sy(k));
}

// ─── HYPERBOLA x²/a² - y²/b² = 1 ───
function drawHyp(c,θ){
  const{a=3,b=2,h=0,k=0}=c.params;
  const xmax=Math.max(Math.abs(wx(0)),Math.abs(wx(W)))*1.3;
  const build=(sign)=>{
    const pts=[];
    for(let i=0;i<=400;i++){const x=a+(xmax-a)*i/400;const yy=b*b*(x*x/a/a-1);if(yy<0)continue;const y=Math.sqrt(yy);pts.push(rpt(sign*x+h,y+k,h,k,θ));}
    for(let i=400;i>=0;i--){const x=a+(xmax-a)*i/400;const yy=b*b*(x*x/a/a-1);if(yy<0)continue;pts.push(rpt(sign*x+h,-Math.sqrt(yy)+k,h,k,θ));}
    return pts;
  };
  path(build(1),true); path(build(-1),true);
  if(S.asym){
    ctx.save();ctx.strokeStyle='#60b8f080';ctx.lineWidth=1;ctx.shadowBlur=0;ctx.setLineDash([5,4]);
    const far=xmax;[1,-1].forEach(s=>{
      const p1=rpt(-far+h,s*far*b/a+k,h,k,θ),p2=rpt(far+h,-s*far*b/a+k,h,k,θ);
      ctx.beginPath();ctx.moveTo(sx(p1[0]),sy(p1[1]));ctx.lineTo(sx(p2[0]),sy(p2[1]));ctx.stroke();
    });
    ctx.setLineDash([]);ctx.restore();
  }
  const cc=Math.sqrt(a*a+b*b);
  if(S.foci){const f1=rpt(-cc+h,k,h,k,θ),f2=rpt(cc+h,k,h,k,θ);dotR(sx(f1[0]),sy(f1[1]),'#f06080',5,'F₁');dotR(sx(f2[0]),sy(f2[1]),'#f06080',5,'F₂');}
  if(S.verts){[rpt(-a+h,k,h,k,θ),rpt(a+h,k,h,k,θ)].forEach((v,i)=>dotR(sx(v[0]),sy(v[1]),c.color,4,i===0?'A\'':'A'));}
}

// ─── CONJ HYPERBOLA -x²/a² + y²/b² = 1 ───
function drawHypC(c,θ){
  const{a=3,b=2,h=0,k=0}=c.params;
  const ymax=Math.max(Math.abs(wy(0)),Math.abs(wy(H)))*1.3;
  const build=(sign)=>{
    const pts=[];
    for(let i=0;i<=400;i++){const y=b+(ymax-b)*i/400;const xx=a*a*(y*y/b/b-1);if(xx<0)continue;const x=Math.sqrt(xx);pts.push(rpt(x+h,sign*y+k,h,k,θ));}
    for(let i=400;i>=0;i--){const y=b+(ymax-b)*i/400;const xx=a*a*(y*y/b/b-1);if(xx<0)continue;pts.push(rpt(-Math.sqrt(xx)+h,sign*y+k,h,k,θ));}
    return pts;
  };
  path(build(1),true); path(build(-1),true);
}

// ─── RECT HYPERBOLA xy=c² ───
function drawRHyp(c,θ){
  const{cc=3,h=0,k=0}=c.params;
  const xmax=Math.max(Math.abs(wx(0)),Math.abs(wx(W)))*1.2;
  const buildBranch=(sign)=>{
    const pts=[];
    for(let i=1;i<=400;i++){const x=sign*0.01+sign*(xmax-0.01)*i/400;const y=cc*cc/x;pts.push(rpt(x+h,y+k,h,k,θ));}
    return pts;
  };
  path(buildBranch(1)); path(buildBranch(-1));
  if(S.asym){
    ctx.save();ctx.strokeStyle='#60b8f080';ctx.lineWidth=1;ctx.shadowBlur=0;ctx.setLineDash([5,4]);
    const far=xmax;const p1=rpt(-far+h,k,h,k,θ),p2=rpt(far+h,k,h,k,θ),p3=rpt(h,-far+k,h,k,θ),p4=rpt(h,far+k,h,k,θ);
    ctx.beginPath();ctx.moveTo(sx(p1[0]),sy(p1[1]));ctx.lineTo(sx(p2[0]),sy(p2[1]));ctx.stroke();
    ctx.beginPath();ctx.moveTo(sx(p3[0]),sy(p3[1]));ctx.lineTo(sx(p4[0]),sy(p4[1]));ctx.stroke();
    ctx.setLineDash([]);ctx.restore();
  }
}

// ─── POINT ───
function drawPt(c){const{x=0,y=0}=c.params;dot(x,y,c.color,6,'('+fmt(x)+','+fmt(y)+')');}

// ═══════════════════════════════════
// TANGENT & NORMAL
// ═══════════════════════════════════
function drawTanNorm(c,tn){
  const θ=(c.rotation||0)*Math.PI/180;
  const {h=0,k=0}=c.params;
  let tx,ty,ts; // tangent point and slope
  const p=tn.param;
  switch(c.type){
    case 'para_r':{const{a=2}=c.params;const t=p;tx=a*t*t+h;ty=2*a*t+k;ts=Math.abs(t)<1e-9?1e9:1/t;break;}
    case 'para_l':{const{a=2}=c.params;const t=p;tx=-a*t*t+h;ty=2*a*t+k;ts=Math.abs(t)<1e-9?1e9:-1/t;break;}
    case 'para_u':{const{a=2}=c.params;const t=p;tx=2*a*t+h;ty=a*t*t+k;ts=t;break;}
    case 'para_d':{const{a=2}=c.params;const t=p;tx=2*a*t+h;ty=-a*t*t+k;ts=-t;break;}
    case 'circle':{const{r=3}=c.params;const ang=p*Math.PI/180;tx=h+r*Math.cos(ang);ty=k+r*Math.sin(ang);const rs=(ty-k)/(tx-h||1e-9);ts=Math.abs(rs)<1e-9?1e9:-1/rs;break;}
    case 'ellipse':{const{a=4,b=2.5}=c.params;const ang=p*Math.PI/180;tx=h+a*Math.cos(ang);ty=k+b*Math.sin(ang);const cosA=Math.cos(ang),sinA=Math.sin(ang);ts=Math.abs(sinA)<1e-9?1e9:-(b*cosA)/(a*sinA);break;}
    case 'hyp':{const{a=3,b=2}=c.params;const ang=p*Math.PI/180;if(Math.abs(Math.cos(ang))<1e-9)return;tx=h+a/Math.cos(ang);ty=k+b*Math.tan(ang);const sinA=Math.sin(ang);ts=Math.abs(sinA)<1e-9?1e9:b/(a*sinA);break;}
    case 'rhyp':{const{cc=3}=c.params;const t=p;if(Math.abs(t)<1e-9)return;tx=cc*t+h;ty=cc/t+k;ts=-1/(t*t);break;}
    case 'line':{const{m=1,b=0}=c.params;tx=p+h;ty=m*(p)+b+k;ts=m;break;}
    default:return;
  }
  if(!isFinite(tx)||!isFinite(ty))return;
  const[rx,ry]=rpt(tx,ty,h,k,θ);
  const psx=sx(rx),psy=sy(ry);
  // rotate slope
  const slopeAngle=Math.atan2(ts,1)+θ;
  const tanSlope=Math.tan(slopeAngle);
  const ext=Math.max(W,H)/scale*1.5;

  const drawLn=(slope,col,dash)=>{
    ctx.save();ctx.strokeStyle=col;ctx.lineWidth=1.8;ctx.shadowBlur=10;ctx.shadowColor=col;
    if(dash)ctx.setLineDash(dash);
    if(Math.abs(slope)>1e5){ctx.beginPath();ctx.moveTo(psx,psy-ext*scale);ctx.lineTo(psx,psy+ext*scale);}
    else{ctx.beginPath();ctx.moveTo(psx-ext*scale,psy+slope*ext*scale);ctx.lineTo(psx+ext*scale,psy-slope*ext*scale);}
    ctx.stroke();ctx.setLineDash([]);ctx.restore();
  };
  drawLn(tanSlope,'#40d0c0',[]);
  const normSlope=Math.abs(tanSlope)<1e-9?1e9:-1/tanSlope;
  drawLn(normSlope,'#f08040',[5,4]);

  dotR(psx,psy,'#40d0c0',5,'');
  ctx.save();ctx.font='500 10px JetBrains Mono';ctx.fillStyle='#40d0c0';ctx.shadowBlur=0;
  ctx.fillText('T('+fmt(rx)+','+fmt(ry)+')',psx+8,psy-8);ctx.restore();
}

function fmt(v){return typeof v==='number'?parseFloat(v.toFixed(3)).toString():v;}

// ═══════════════════════════════════
// TYPE META
// ═══════════════════════════════════
const META={
  line:     {name:'Line',      def:{m:1,b:0},      fields:[{k:'m',l:'slope m',lo:-20,hi:20},{k:'b',l:'y-intercept b',lo:-15,hi:15}]},
  line_g:   {name:'Line (gen)',def:{a:1,b:-1,k:0},  fields:[{k:'a',l:'coeff a',lo:-10,hi:10},{k:'b',l:'coeff b',lo:-10,hi:10},{k:'k',l:'const c',lo:-15,hi:15}]},
  circle:   {name:'Circle',    def:{h:0,k:0,r:3},   fields:[{k:'h',l:'centre h',lo:-15,hi:15},{k:'k',l:'centre k',lo:-15,hi:15},{k:'r',l:'radius r',lo:0.1,hi:15}]},
  para_r:   {name:'Parabola →',def:{a:2,h:0,k:0},   fields:[{k:'a',l:'a (y²=4ax)',lo:0.1,hi:20},{k:'h',l:'vertex h',lo:-15,hi:15},{k:'k',l:'vertex k',lo:-15,hi:15}]},
  para_l:   {name:'Parabola ←',def:{a:2,h:0,k:0},   fields:[{k:'a',l:'a',lo:0.1,hi:20},{k:'h',l:'h',lo:-15,hi:15},{k:'k',l:'k',lo:-15,hi:15}]},
  para_u:   {name:'Parabola ↑',def:{a:2,h:0,k:0},   fields:[{k:'a',l:'a (x²=4ay)',lo:0.1,hi:20},{k:'h',l:'h',lo:-15,hi:15},{k:'k',l:'k',lo:-15,hi:15}]},
  para_d:   {name:'Parabola ↓',def:{a:2,h:0,k:0},   fields:[{k:'a',l:'a',lo:0.1,hi:20},{k:'h',l:'h',lo:-15,hi:15},{k:'k',l:'k',lo:-15,hi:15}]},
  ellipse:  {name:'Ellipse',   def:{a:4,b:2.5,h:0,k:0},fields:[{k:'a',l:'semi-maj a',lo:0.1,hi:20},{k:'b',l:'semi-min b',lo:0.1,hi:20},{k:'h',l:'centre h',lo:-15,hi:15},{k:'k',l:'centre k',lo:-15,hi:15}]},
  hyp:      {name:'Hyperbola', def:{a:3,b:2,h:0,k:0},  fields:[{k:'a',l:'a',lo:0.1,hi:20},{k:'b',l:'b',lo:0.1,hi:20},{k:'h',l:'h',lo:-15,hi:15},{k:'k',l:'k',lo:-15,hi:15}]},
  hyp_c:    {name:'Conj. Hyp', def:{a:3,b:2,h:0,k:0},  fields:[{k:'a',l:'a',lo:0.1,hi:20},{k:'b',l:'b',lo:0.1,hi:20},{k:'h',l:'h',lo:-15,hi:15},{k:'k',l:'k',lo:-15,hi:15}]},
  rhyp:     {name:'Rect. Hyp', def:{cc:3,h:0,k:0},     fields:[{k:'cc',l:'c (xy=c²)',lo:0.1,hi:15},{k:'h',l:'h',lo:-10,hi:10},{k:'k',l:'k',lo:-10,hi:10}]},
  pt:       {name:'Point',     def:{x:0,y:0},           fields:[{k:'x',l:'x',lo:-20,hi:20},{k:'y',l:'y',lo:-20,hi:20}]},
};

const TAN_META={
  para_r:{l:'param t',def:1}, para_l:{l:'param t',def:1},
  para_u:{l:'param t',def:1}, para_d:{l:'param t',def:1},
  circle:{l:'angle θ°',def:45}, ellipse:{l:'angle θ°',def:45},
  hyp:{l:'angle θ°',def:30}, rhyp:{l:'param t',def:1}, line:{l:'x value',def:0}
};

// ═══════════════════════════════════
// CURVE MANAGEMENT
// ═══════════════════════════════════
function addCurve(type, params, name) {
  type = type || document.getElementById('curve-type-sel').value;
  const meta = META[type];
  const id = nextId++;
  const c = {
    id, type,
    name: name || (meta.name+' '+id),
    color: COLORS[curves.length % COLORS.length],
    params: params ? {...params} : {...meta.def},
    rotation: 0, visible: true, tans: []
  };
  curves.push(c);
  selectedId = id;
  renderList();
  redraw();
  // auto-open the new curve
  setTimeout(()=>{
    const el=document.getElementById('ci-'+id);
    if(el)el.classList.add('open');
  },50);
}

function removeCurve(id){curves=curves.filter(c=>c.id!==id);if(selectedId===id)selectedId=null;renderList();redraw();}

function renderList(){
  const list=document.getElementById('curves-list');
  if(!curves.length){list.innerHTML=`<div id="empty-hint"><div class="ico">📐</div>Add a curve above.<br>Tap canvas to hide sidebar.<br>Unlimited curves, tangents & normals.</div>`;updateCount();return;}
  // preserve open state
  const openIds=new Set([...document.querySelectorAll('.ci.open')].map(el=>+el.id.replace('ci-','')));
  list.innerHTML='';
  curves.forEach(c=>{
    const meta=META[c.type];
    const isOpen=openIds.has(c.id)||c.id===selectedId&&openIds.size===0;
    const div=document.createElement('div');
    div.className='ci'+(c.id===selectedId?' sel':'')+(isOpen?' open':'');
    div.id='ci-'+c.id;

    // HEAD
    const head=document.createElement('div');
    head.className='ci-head';
    head.onclick=()=>{selectedId=c.id;div.classList.toggle('open');redraw();};
    head.innerHTML=`<div class="ci-dot" style="background:${c.color};box-shadow:0 0 6px ${c.color}"></div>
      <span class="ci-name">${c.name}</span>
      <span class="ci-badge">${c.type}</span>
      <span class="chev">▾</span>
      <button class="btn-del" onclick="event.stopPropagation();removeCurve(${c.id})">✕</button>`;

    // BODY
    const body=document.createElement('div');
    body.className='ci-body';
    let html='';

    // Visibility
    html+=`<div class="crow"><input type="checkbox" id="vis-${c.id}" ${c.visible?'checked':''} onchange="curves.find(x=>x.id==${c.id}).visible=this.checked;redraw()"><label for="vis-${c.id}">Visible</label></div>`;

    // Name
    html+=`<div class="slbl">Name</div>
      <div style="display:flex;gap:5px;margin-bottom:6px">
        <input style="flex:1;background:#07090e;border:1px solid var(--border2);color:var(--text);padding:4px 7px;border-radius:3px;font-family:'JetBrains Mono',monospace;font-size:0.68rem" value="${c.name}" oninput="curves.find(x=>x.id==${c.id}).name=this.value;redraw()">
      </div>`;

    // Color
    html+=`<div class="slbl">Color</div><div class="swatch-row">${COLORS.map(col=>`<div class="sw ${col===c.color?'active':''}" style="background:${col}" onclick="setCurveColor(${c.id},'${col}',this)"></div>`).join('')}</div>`;

    // Equation / direct input
    html+=`<div class="slbl">Equation (direct input)</div>
      <div class="eqn-box">
        <label>TYPE & APPLY</label>
        <input class="eqn-input" id="eqn-${c.id}" value="${getEqnStr(c)}" placeholder="e.g. a=3 b=2 h=1 k=0  or  y=2x+3" onkeydown="if(event.key==='Enter')applyEqn(${c.id})">
        <div style="display:flex;gap:5px;align-items:center;margin-top:3px">
          <button class="eqn-apply" onclick="applyEqn(${c.id})">↵ Apply</button>
          <span class="eqn-err" id="eqn-err-${c.id}">parse error</span>
        </div>
      </div>`;

    // Parameters with BOTH slider and typed input
    html+=`<div class="slbl">Parameters</div>`;
    meta.fields.forEach(f=>{
      const v=c.params[f.k]||0;
      html+=`<div class="prow">
        <label title="${f.l}">${f.l}</label>
        <input type="range" min="${f.lo}" max="${f.hi}" step="${(f.hi-f.lo)/400}" value="${v}"
          oninput="setP(${c.id},'${f.k}',+this.value);document.getElementById('pv-${c.id}-${f.k}').value=parseFloat(this.value).toFixed(3)">
        <input class="pval" type="number" id="pv-${c.id}-${f.k}" value="${v}"
          step="0.01"
          onchange="setP(${c.id},'${f.k}',+this.value);syncSlider(${c.id},'${f.k}',this.value)"
          onkeydown="if(event.key==='Enter')this.blur()">
      </div>`;
    });

    // Rotation
    html+=`<div class="slbl">Rotation</div>
      <div class="prow">
        <label>θ°</label>
        <input type="range" min="-180" max="180" step="1" value="${c.rotation||0}"
          oninput="setRot(${c.id},+this.value);document.getElementById('rv-${c.id}').value=this.value">
        <input class="pval" type="number" id="rv-${c.id}" value="${c.rotation||0}" step="1"
          onchange="setRot(${c.id},+this.value)" onkeydown="if(event.key==='Enter')this.blur()">
      </div>`;

    // Tangent/Normal
    const tnm=TAN_META[c.type];
    if(tnm){
      html+=`<div class="slbl">Tangent & Normal</div>
        <div class="trow">
          <label>${tnm.l}</label>
          <input type="number" id="tn-${c.id}" value="${tnm.def}" step="0.1">
          <button class="tbtn teal" onclick="addTan(${c.id})">Draw T/N</button>
          <button class="tbtn rose" onclick="clearTans(${c.id})" style="margin-left:3px">Clear</button>
        </div>`;
    }

    // Live equation display
    html+=`<div class="slbl">Current equation</div>
      <div id="ceq-${c.id}" style="font-size:0.65rem;color:var(--teal);background:#06080d;padding:5px 8px;border-radius:3px;border:1px solid var(--border2);word-break:break-all">${getEqnStr(c)}</div>`;

    body.innerHTML=html;
    div.appendChild(head); div.appendChild(body);
    list.appendChild(div);
  });
  updateCount();
}

function getEqnStr(c){
  const p=c.params;
  switch(c.type){
    case 'line':   return `y = ${fmt(p.m)}·x + ${fmt(p.b)}`;
    case 'line_g': return `${fmt(p.a)}x + ${fmt(p.b)}y + ${fmt(p.k)} = 0`;
    case 'circle': return `(x−${fmt(p.h)})² + (y−${fmt(p.k)})² = ${fmt(p.r)}²`;
    case 'para_r': return `(y−${fmt(p.k)})² = ${fmt(4*p.a)}(x−${fmt(p.h)})`;
    case 'para_l': return `(y−${fmt(p.k)})² = −${fmt(4*p.a)}(x−${fmt(p.h)})`;
    case 'para_u': return `(x−${fmt(p.h)})² = ${fmt(4*p.a)}(y−${fmt(p.k)})`;
    case 'para_d': return `(x−${fmt(p.h)})² = −${fmt(4*p.a)}(y−${fmt(p.k)})`;
    case 'ellipse':return `(x−${fmt(p.h)})²/${fmt(p.a)}² + (y−${fmt(p.k)})²/${fmt(p.b)}² = 1`;
    case 'hyp':    return `(x−${fmt(p.h)})²/${fmt(p.a)}² − (y−${fmt(p.k)})²/${fmt(p.b)}² = 1`;
    case 'hyp_c':  return `−(x−${fmt(p.h)})²/${fmt(p.a)}² + (y−${fmt(p.k)})²/${fmt(p.b)}² = 1`;
    case 'rhyp':   return `(x−${fmt(p.h)})(y−${fmt(p.k)}) = ${fmt(p.cc)}²`;
    case 'pt':     return `Point (${fmt(p.x)}, ${fmt(p.y)})`;
    default:return '';
  }
}

// ─── Apply equation from text ───
function applyEqn(id){
  const c=curves.find(x=>x.id===id);
  const errEl=document.getElementById('eqn-err-'+id);
  const input=document.getElementById('eqn-'+id).value.trim();
  errEl.style.display='none';
  try{
    // Parse "key=val key=val ..." syntax
    const kv=/([a-zA-Z]+)\s*=\s*(-?[\d.]+)/g;
    let m, found=false;
    while((m=kv.exec(input))!==null){
      const key=m[1].toLowerCase(), val=parseFloat(m[2]);
      if(key in c.params){c.params[key]=val;found=true;}
      if(key==='rot'||key==='rotation'||key==='theta'){c.rotation=val;found=true;}
    }
    // Also parse "y = mx + b" form for lines
    if(c.type==='line'){
      const lineMatch=input.match(/y\s*=\s*(-?[\d.]+)\s*[*x]?\s*x\s*([+\-]\s*[\d.]+)?/i);
      if(lineMatch){c.params.m=parseFloat(lineMatch[1]);c.params.b=lineMatch[2]?parseFloat(lineMatch[2].replace(/\s/g,'')):0;found=true;}
    }
    if(!found){errEl.style.display='inline';errEl.textContent='use: a=3 b=2 h=1 k=0';}
    renderList(); redraw();
  }catch(e){errEl.style.display='inline';errEl.textContent='parse error';}
}

function setP(id,key,val){
  const c=curves.find(x=>x.id===id);
  if(c){c.params[key]=val;updateEqnDisplay(id);redraw();}
}
function syncSlider(id,key,val){
  // sync range slider if value within range
  const meta=META[curves.find(x=>x.id===id)?.type];
  if(!meta)return;
  const f=meta.fields.find(f=>f.k===key);
  if(!f)return;
  const el=document.querySelector(`#ci-${id} input[type=range][oninput*="'${key}'"]`);
  if(el)el.value=Math.max(f.lo,Math.min(f.hi,+val));
}
function setRot(id,val){const c=curves.find(x=>x.id===id);if(c){c.rotation=val;redraw();}}
function setCurveColor(id,col,el){
  const c=curves.find(x=>x.id===id);if(c)c.color=col;
  el.closest('.swatch-row').querySelectorAll('.sw').forEach(s=>s.classList.remove('active'));
  el.classList.add('active');redraw();
}
function addTan(id){
  const c=curves.find(x=>x.id===id);if(!c)return;
  const v=parseFloat(document.getElementById('tn-'+id).value);
  if(!isFinite(v))return;
  c.tans.push({param:v});redraw();
}
function clearTans(id){const c=curves.find(x=>x.id===id);if(c){c.tans=[];redraw();}}
function updateEqnDisplay(id){
  const el=document.getElementById('ceq-'+id);
  const eqEl=document.getElementById('eqn-'+id);
  const c=curves.find(x=>x.id===id);
  if(el&&c){el.textContent=getEqnStr(c);}
  if(eqEl&&c){eqEl.value=getEqnStr(c);}
}
function updateCount(){document.getElementById('curve-count').textContent=curves.length+' curve'+(curves.length!==1?'s':'');}

// ═══════════════════════════════════
// CANVAS EVENTS
// ═══════════════════════════════════
let lastTouchDist=0;
let touchStartTime=0;

cvs.addEventListener('mousedown', e=>{
  if(mode==='pan'){dragging=true;lastMX=e.clientX;lastMY=e.clientY;cvs.style.cursor='grabbing';}
  else handleCanvasClick(e.offsetX, e.offsetY);
  // hide sidebar on canvas touch
  if(sidebarOpen) hideSidebar();
});
cvs.addEventListener('mousemove', e=>{
  if(dragging&&mode==='pan'){ox+=e.clientX-lastMX;oy+=e.clientY-lastMY;lastMX=e.clientX;lastMY=e.clientY;redraw();}
  document.getElementById('cx-val').textContent=wx(e.offsetX).toFixed(3);
  document.getElementById('cy-val').textContent=wy(e.offsetY).toFixed(3);
  updateSelInfo();
});
cvs.addEventListener('mouseup',()=>{dragging=false;cvs.style.cursor=mode==='pan'?'crosshair':'crosshair';});
cvs.addEventListener('mouseleave',()=>{dragging=false;});
cvs.addEventListener('wheel',e=>{
  e.preventDefault();
  const f=e.deltaY<0?1.12:1/1.12;
  const mx=e.offsetX,my=e.offsetY;
  ox=mx+(ox-mx)*f;oy=my+(oy-my)*f;scale*=f;redraw();
},{passive:false});

// Touch
cvs.addEventListener('touchstart',e=>{
  e.preventDefault();
  touchStartTime=Date.now();
  if(e.touches.length===1){
    const t=e.touches[0];
    lastMX=t.clientX;lastMY=t.clientY;
    if(mode==='pan')dragging=true;
    else{
      const rect=cvs.getBoundingClientRect();
      handleCanvasClick(t.clientX-rect.left,t.clientY-rect.top);
    }
    if(sidebarOpen)hideSidebar();
  } else if(e.touches.length===2){
    dragging=false;
    lastTouchDist=Math.hypot(e.touches[0].clientX-e.touches[1].clientX,e.touches[0].clientY-e.touches[1].clientY);
  }
},{passive:false});
cvs.addEventListener('touchmove',e=>{
  e.preventDefault();
  if(e.touches.length===1&&dragging&&mode==='pan'){
    const t=e.touches[0];ox+=t.clientX-lastMX;oy+=t.clientY-lastMY;lastMX=t.clientX;lastMY=t.clientY;redraw();
  } else if(e.touches.length===2){
    const d=Math.hypot(e.touches[0].clientX-e.touches[1].clientX,e.touches[0].clientY-e.touches[1].clientY);
    const f=d/lastTouchDist;
    const mx=(e.touches[0].clientX+e.touches[1].clientX)/2,my=(e.touches[0].clientY+e.touches[1].clientY)/2;
    ox=mx+(ox-mx)*f;oy=my+(oy-my)*f;scale*=f;lastTouchDist=d;redraw();
  }
},{passive:false});
cvs.addEventListener('touchend',()=>dragging=false);

function handleCanvasClick(px,py){
  const x=parseFloat(wx(px).toFixed(2)),y=parseFloat(wy(py).toFixed(2));
  if(mode==='draw_point'){
    addCurve('pt',{x,y},'Pt('+x+','+y+')');
  } else if(mode==='draw_line'){
    drawPts.push([x,y]);redraw();
    if(drawPts.length===2){
      const [p1,p2]=drawPts;
      const dx=p2[0]-p1[0],dy=p2[1]-p1[1];
      if(Math.abs(dx)<1e-9){addCurve('line_g',{a:1,b:0,k:-p1[0]},'Line '+(nextId));}
      else{const m=dy/dx,b=p1[1]-m*p1[0];addCurve('line',{m:parseFloat(m.toFixed(4)),b:parseFloat(b.toFixed(4))},'Line '+nextId);}
      drawPts=[];
      document.getElementById('draw-indicator').textContent='📏 LINE — Click 2 points on canvas';
    } else {
      document.getElementById('draw-indicator').textContent='📏 LINE — Now click second point';
    }
  } else if(mode==='draw_circle'){
    drawPts.push([x,y]);redraw();
    if(drawPts.length===2){
      const [p1,p2]=drawPts;const r=Math.hypot(p2[0]-p1[0],p2[1]-p1[1]);
      addCurve('circle',{h:p1[0],k:p1[1],r:parseFloat(r.toFixed(4))},'Circle '+nextId);
      drawPts=[];
      document.getElementById('draw-indicator').textContent='⭕ CIRCLE — Click centre, then radius point';
    } else {
      document.getElementById('draw-indicator').textContent='⭕ CIRCLE — Now click radius point';
    }
  }
}

function updateSelInfo(){
  const el=document.getElementById('sel-info');
  if(!selectedId){el.textContent='no selection';return;}
  const c=curves.find(x=>x.id===selectedId);
  if(c)el.textContent=c.name+' | '+getEqnStr(c).slice(0,40);
}

// ═══════════════════════════════════
// CONTROLS
// ═══════════════════════════════════
function zoomIn(){scale*=1.2;redraw();}
function zoomOut(){scale/=1.2;redraw();}
function resetView(){ox=W/2;oy=H/2;scale=60;redraw();}
function toggleGrid(){S.showGrid=!S.showGrid;redraw();}
function clearAll(){if(confirm('Clear all curves?')){curves=[];selectedId=null;drawPts=[];renderList();redraw();}}
function updateSpan(id,v){const el=document.getElementById(id);if(el)el.textContent=v;}

function switchTab(t){
  document.getElementById('tab-curves').style.display=t==='curves'?'flex':'none';
  document.getElementById('tab-settings').style.display=t==='settings'?'block':'none';
  document.getElementById('tab-help').style.display=t==='help'?'block':'none';
  document.querySelectorAll('.tab').forEach((el,i)=>el.classList.toggle('active',['curves','settings','help'][i]===t));
}

// keyboard
document.addEventListener('keydown',e=>{
  if(e.target.tagName==='INPUT')return;
  if(e.key==='r'||e.key==='R')resetView();
  if(e.key==='g'||e.key==='G')toggleGrid();
  if(e.key==='h'||e.key==='H')toggleSidebar();
  if(e.key==='Escape'){setMode('pan');drawPts=[];redraw();}
  if((e.key==='Delete'||e.key==='Backspace')&&selectedId){removeCurve(selectedId);}
});

// ═══════════════════════════════════
// INIT
// ═══════════════════════════════════
function init(){
  resize();
  // starter curves
  addCurve('ellipse',{a:4,b:2.5,h:0,k:0},'Ellipse 1');
  addCurve('para_r',{a:2,h:0,k:0},'Parabola 1');
  addCurve('circle',{h:0,k:0,r:3},'Circle 1');
  // pre-add a tangent on the ellipse
  const el=curves.find(c=>c.type==='ellipse');
  if(el)el.tans.push({param:45});
  selectedId=null;
  renderList();
  redraw();
}
init();


/* NAVIGATION */
const _SECS=['trig','coord','conic','const','cheat','calc','desmos','ptable','rotdyn','thermo','ionic'];
let _cur='trig';
function showSection(id){
  if(id==='hero'){
  _SECS.forEach(s=>{
    const el=document.getElementById('sec-'+s);if(el)el.classList.remove('active');
    const nav=document.getElementById('nav-'+s);if(nav)nav.classList.remove('active');
  });
  document.body.style.overflow='auto';document.documentElement.style.overflow='auto';
  window.scrollTo({top:0,behavior:'smooth'});
  _cur='hero';
  return;
}
  _SECS.forEach(s=>{
    const el=document.getElementById('sec-'+s);if(el)el.classList.remove('active');
    const nav=document.getElementById('nav-'+s);if(nav)nav.classList.remove('active');
  });
  const target=document.getElementById('sec-'+id);if(target)target.classList.add('active');
  const nav=document.getElementById('nav-'+id);if(nav)nav.classList.add('active');
  _cur=id;
  if(id==='conic'){
    document.body.style.overflow='hidden';document.documentElement.style.overflow='hidden';
    const navEl=document.getElementById('topnav');const navH=navEl?navEl.offsetHeight:43;
    const ci=document.getElementById('conic-inner');if(ci){ci.style.height=(window.innerHeight-navH)+'px';ci.style.overflow='hidden';}
    setTimeout(()=>{try{resize();redraw();}catch(e){}},60);
  }else{document.body.style.overflow='auto';document.documentElement.style.overflow='auto';}
  if(id==='trig')setTimeout(()=>{try{drawTrig();drawITFInd();drawITF();}catch(e){}},80);
  const topnav=document.getElementById('topnav');
  if(topnav)window.scrollTo({top:topnav.getBoundingClientRect().top+window.scrollY,behavior:'instant'});
}
window.addEventListener('resize',()=>{
  if(_cur==='conic'){const navEl=document.getElementById('topnav');const navH=navEl?navEl.offsetHeight:43;const ci=document.getElementById('conic-inner');if(ci)ci.style.height=(window.innerHeight-navH)+'px';try{resize();redraw();}catch(e){}}
});

/* CALCULATOR */
let _cExpr='',_cResult='0',_cHist='',_cMem=0,_aMode='deg',_lastAns=0;
function _toR(x){return _aMode==='deg'?x*Math.PI/180:x;}
function _fact(n){if(n<0||n!==Math.floor(n))return NaN;if(n<=1)return 1;let r=1;for(let i=2;i<=n;i++)r*=i;return r;}
function _cEval(expr){
  try{
    const _toRad=_aMode==='deg'?Math.PI/180:1;
    const _toDeg=_aMode==='deg'?180/Math.PI:1;
    let e=expr
      .replace(/\u03c0/g,'Math.PI')
      .replace(/\u00d7/g,'*').replace(/\u00f7/g,'/').replace(/\u2212/g,'-')
      .replace(/sin\u207b\xb9\(/g,'__AS(')
      .replace(/cos\u207b\xb9\(/g,'__AC(')
      .replace(/tan\u207b\xb9\(/g,'__AT(')
      .replace(/sin\(/g,'__sin(')
      .replace(/cos\(/g,'__cos(')
      .replace(/tan\(/g,'__tan(')
      .replace(/__AS\(/g,'__asin(')
      .replace(/__AC\(/g,'__acos(')
      .replace(/__AT\(/g,'__atan(')
      .replace(/log\(/g,'Math.log10(')
      .replace(/ln\(/g,'Math.log(')
      .replace(/\u221a\(/g,'Math.sqrt(')
      .replace(/\u221b\(/g,'Math.cbrt(')
      .replace(/%/g,'/100');
    const helpers=
      'const __sin=x=>Math.sin('+_toRad+'*x);'+
      'const __cos=x=>Math.cos('+_toRad+'*x);'+
      'const __tan=x=>Math.tan('+_toRad+'*x);'+
      'const __asin=x=>Math.asin(x)*'+_toDeg+';'+
      'const __acos=x=>Math.acos(x)*'+_toDeg+';'+
      'const __atan=x=>Math.atan(x)*'+_toDeg+';';
    const r=Function('"use strict";'+helpers+'return('+e+')')();
    return r;
  }catch(err){return null;}
}
function calcPress(a){
  if(a==='ac'){_cExpr='';_cResult='0';_cHist='';_updDisp();return;}
  if(a==='del'){_cExpr=_cExpr.slice(0,-1);_updDisp();return;}
  if(a==='='){
    if(!_cExpr)return;
    const r=_cEval(_cExpr);
    if(r!==null&&isFinite(r)){_lastAns=r;_cHist=_cExpr+' =';_cResult=+r.toPrecision(12)+'';_cExpr='';}
    else{_cResult='Error';_cExpr='';}
    const el=document.getElementById('calc-result');el.classList.add('flash');setTimeout(()=>el.classList.remove('flash'),280);
    _updDisp();return;
  }
  const _app=s=>{_cExpr+=s;_updDisp();};
  const m={mc:()=>{_cMem=0;_updDisp();},mr:()=>_app(_cMem+''),ms:()=>{const r=_cEval(_cExpr||_cResult);if(r!==null)_cMem=r;_updDisp();},
    'm+':()=>{const r=_cEval(_cExpr||_cResult);if(r!==null)_cMem+=r;_updDisp();},'m-':()=>{const r=_cEval(_cExpr||_cResult);if(r!==null)_cMem-=r;_updDisp();},
    pi:()=>_app('π'),e:()=>_app(Math.E+''),ans:()=>_app(_lastAns+''),
    sqrt:()=>_app('√('),cbrt:()=>_app('∛('),sq:()=>_app('**2'),cube:()=>_app('**3'),pow:()=>_app('**'),
    log:()=>_app('log('),ln:()=>_app('ln('),sin:()=>_app('sin('),cos:()=>_app('cos('),tan:()=>_app('tan('),
    asin:()=>_app('sin⁻¹('),acos:()=>_app('cos⁻¹('),atan:()=>_app('tan⁻¹('),
    inv:()=>{_cExpr='1/('+(_cExpr||_cResult)+')';_updDisp();},
    abs:()=>{_cExpr='Math.abs('+(_cExpr||_cResult)+')';_updDisp();},
    fact:()=>{const r=_cEval(_cExpr||_cResult);if(r!==null){const f=_fact(r);_cResult=f+'';_cHist=_cExpr+'! =';_cExpr='';_updDisp();}},
    pct:()=>_app('%'),'+/-':()=>{if(_cExpr)_cExpr='-('+_cExpr+')';else _cResult=(parseFloat(_cResult)*-1)+'';_updDisp();},
  };
  if(m[a]){m[a]();return;}
  _app(a=='+'?'+':a=='−'?'−':a=='×'?'×':a=='÷'?'÷':a);
}
function _updDisp(){
  document.getElementById('calc-history').textContent=_cHist;
  document.getElementById('calc-expr').textContent=_cExpr;
  if(_cExpr){const r=_cEval(_cExpr);document.getElementById('calc-result').textContent=(r!==null&&isFinite(r))?+r.toPrecision(12)+'':_cResult;}
  else document.getElementById('calc-result').textContent=_cResult;
  document.getElementById('mem-ind').textContent=_cMem!==0?'M='+_cMem:'';
  document.getElementById('angle-ind').textContent=_aMode.toUpperCase();
}
function setAngleMode(m){
  _aMode=m;
  document.getElementById('btn-deg').classList.toggle('active',m==='deg');
  document.getElementById('btn-rad').classList.toggle('active',m==='rad');
  _updDisp();
}
document.querySelectorAll('.cb').forEach(btn=>{
  btn.addEventListener('click',function(e){
    const r=document.createElement('span');r.className='cb-ripple';
    const rc=this.getBoundingClientRect(),sz=Math.max(rc.width,rc.height);
    r.style.width=r.style.height=sz+'px';r.style.left=(e.clientX-rc.left-sz/2)+'px';r.style.top=(e.clientY-rc.top-sz/2)+'px';
    this.appendChild(r);setTimeout(()=>r.remove(),420);
    calcPress(this.dataset.action);
  });
});
document.addEventListener('keydown',e=>{
  if(_cur!=='calc')return;const k=e.key;
  if(k>='0'&&k<='9')calcPress(k);
  else if(k==='+')calcPress('+');else if(k==='-')calcPress('−');
  else if(k==='*')calcPress('×');else if(k==='/'){e.preventDefault();calcPress('÷');}
  else if(k==='.')calcPress('.');else if(k==='('||k===')')calcPress(k);
  else if(k==='Enter'||k==='=')calcPress('=');
  else if(k==='Backspace')calcPress('del');else if(k==='Escape')calcPress('ac');
});

/* CURSOR & PARTICLES */
const _dot=document.getElementById('cur-dot');
const _ring=document.getElementById('cur-ring');
let _dx=-20,_dy=-20,_rx=-40,_ry=-40,_rafR;
const _TC=['#e8c060','#f08040','#f06080','#a080f0','#40d0c0','#60b8f0','#50d890'];
document.addEventListener('mousemove',e=>{
  _dx=e.clientX;_dy=e.clientY;
  _dot.style.left=_dx+'px';_dot.style.top=_dy+'px';
  if(!_rafR)_rafR=requestAnimationFrame(_aR);
  _spawnT(e.clientX,e.clientY);
});
function _aR(){_rx+=(_dx-_rx)*.14;_ry+=(_dy-_ry)*.14;_ring.style.left=_rx+'px';_ring.style.top=_ry+'px';_rafR=requestAnimationFrame(_aR);}
let _lt=0,_ti=0;
const _tp=[];
for(let i=0;i<50;i++){const d=document.createElement('div');d.style.cssText='position:fixed;pointer-events:none;border-radius:50%;z-index:99990;opacity:0;transition:opacity .42s,transform .42s';document.body.appendChild(d);_tp.push({el:d,t:null});}
function _spawnT(x,y){
  if(_cur==='conic')return;const now=Date.now();if(now-_lt<38)return;_lt=now;
  const s=_tp[_ti%50];_ti++;const d=s.el;
  const c=_TC[Math.floor(Math.random()*_TC.length)],sz=3+Math.random()*4;
  d.style.left=x+'px';d.style.top=y+'px';d.style.width=sz+'px';d.style.height=sz+'px';
  d.style.background=c;d.style.boxShadow='0 0 '+(sz*2.5)+'px '+c;
  d.style.transform='translate(-50%,-50%) scale(1)';d.style.opacity='.65';
  clearTimeout(s.t);s.t=setTimeout(()=>{d.style.opacity='0';d.style.transform='translate(-50%,-50%) scale(0)';},380);
}
document.addEventListener('click',e=>{if(_cur!=='conic')_burst(e.clientX,e.clientY);});
document.addEventListener('touchstart',e=>{if(_cur!=='conic')_burst(e.touches[0].clientX,e.touches[0].clientY);},{passive:true});
function _burst(x,y){
  const ring=document.createElement('div');
  ring.style.cssText=`position:fixed;pointer-events:none;z-index:99995;width:10px;height:10px;border-radius:50%;border:2px solid #e8c060;box-shadow:0 0 14px #e8c060;left:${x}px;top:${y}px;transform:translate(-50%,-50%);animation:_bR .65s cubic-bezier(.4,0,.2,1) forwards`;
  document.body.appendChild(ring);
  for(let i=0;i<10;i++){
    const p=document.createElement('div'),ang=i*36*Math.PI/180,dist=32+Math.random()*22;
    const c=_TC[i%_TC.length],sz=3+Math.random()*3;
    p.style.cssText=`position:fixed;pointer-events:none;z-index:99994;width:${sz}px;height:${sz}px;border-radius:50%;background:${c};box-shadow:0 0 ${sz*2}px ${c};left:${x}px;top:${y}px;transform:translate(-50%,-50%);--tx:${Math.cos(ang)*dist}px;--ty:${Math.sin(ang)*dist}px;animation:_bP .6s cubic-bezier(.2,1,.3,1) forwards`;
    document.body.appendChild(p);setTimeout(()=>p.remove(),650);
  }
  setTimeout(()=>ring.remove(),700);
}
document.addEventListener('mouseover',e=>{
  if(e.target.closest('button,.ntab,.hmod,.fb,.fi,.cb')){_dot.style.width='5px';_dot.style.height='5px';_dot.style.boxShadow='0 0 20px #e8c060,0 0 40px rgba(232,192,96,.4)';_ring.style.width='44px';_ring.style.height='44px';_ring.style.borderColor='rgba(232,192,96,.9)';}
});
document.addEventListener('mouseout',e=>{
  if(e.target.closest('button,.ntab,.hmod,.fb,.fi,.cb')){_dot.style.width='10px';_dot.style.height='10px';_dot.style.boxShadow='0 0 10px #e8c060,0 0 20px rgba(232,192,96,.3)';_ring.style.width='28px';_ring.style.height='28px';_ring.style.borderColor='rgba(232,192,96,.4)';}
});
document.addEventListener('mousedown',()=>{_dot.style.width='16px';_dot.style.height='16px';_dot.style.boxShadow='0 0 22px #e8c060,0 0 44px rgba(232,192,96,.5)';});
document.addEventListener('mouseup',()=>{_dot.style.width='10px';_dot.style.height='10px';_dot.style.boxShadow='0 0 10px #e8c060,0 0 20px rgba(232,192,96,.3)';});
document.addEventListener('mouseleave',()=>{_dot.style.opacity='0';_ring.style.opacity='0';});
document.addEventListener('mouseenter',()=>{_dot.style.opacity='1';_ring.style.opacity='1';});
if('ontouchstart' in window){_dot.style.display='none';_ring.style.display='none';}

/* Keyframes */
const _ks=document.createElement('style');
_ks.textContent=`
@keyframes _bR{0%{width:10px;height:10px;opacity:1}100%{width:88px;height:88px;opacity:0}}
@keyframes _bP{0%{opacity:1;transform:translate(-50%,-50%) translate(0,0) scale(1)}100%{opacity:0;transform:translate(-50%,-50%) translate(var(--tx),var(--ty)) scale(0)}}
`;
document.head.appendChild(_ks);

/* Ensure scroll */
document.body.style.overflow='auto';
document.documentElement.style.overflow='auto';
</script>

<!-- ══════════════════════════════════════════ PERIODIC TABLE SECTION ══════════════════════════════════════════ -->
<style>
#sec-ptable{display:none;}
#sec-ptable.active{display:block;animation:secIn .38s cubic-bezier(.4,0,.2,1) both;}

/* ── PT WRAPPER ── */
.pt-wrap{max-width:1380px;margin:0 auto;padding:20px 14px 80px;font-family:'JetBrains Mono',monospace;}

/* ── PT HERO BANNER ── */
.pt-banner{text-align:center;padding:28px 0 22px;border-bottom:1px solid #1e2535;margin-bottom:24px;position:relative;overflow:hidden;}
.pt-banner::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse 80% 100% at 50% 0%,rgba(80,232,144,.07) 0%,transparent 70%);pointer-events:none;}
.pt-banner-badge{font-family:'JetBrains Mono',monospace;font-size:.54rem;letter-spacing:.25em;text-transform:uppercase;color:#50e890;margin-bottom:7px;display:block;position:relative;z-index:1;}
.pt-banner h2{font-family:'Syne',sans-serif;font-weight:800;font-size:clamp(1.5rem,4vw,2.5rem);line-height:1.05;position:relative;z-index:1;margin-bottom:6px;background:linear-gradient(120deg,#50e890,#40d0c0 50%,#60b8f0);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;}
.pt-banner p{font-family:'Crimson Pro',serif;font-style:italic;font-size:.93rem;color:#8090a8;position:relative;z-index:1;}

/* ── SUB-TABS ── */
.pt-subtabs{display:flex;gap:4px;border-bottom:1px solid #1e2535;margin-bottom:22px;overflow-x:auto;scrollbar-width:none;}
.pt-subtabs::-webkit-scrollbar{display:none;}
.pt-stab{font-family:'JetBrains Mono',monospace;font-size:.58rem;letter-spacing:.1em;text-transform:uppercase;color:#404e66;cursor:pointer;padding:8px 16px;border-bottom:2px solid transparent;white-space:nowrap;transition:color .2s,border-color .2s;flex-shrink:0;}
.pt-stab:hover{color:#8090a8;}
.pt-stab.active{color:#50e890;border-bottom-color:#50e890;}

/* ── FILTER BAR ── */
.pt-filters{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:16px;align-items:center;}
.pt-flabel{font-size:.54rem;letter-spacing:.18em;text-transform:uppercase;color:#404e66;margin-right:4px;}
.pt-fbtn{font-family:'JetBrains Mono',monospace;font-size:.55rem;letter-spacing:.06em;padding:4px 10px;border-radius:3px;cursor:pointer;border:1px solid transparent;background:rgba(255,255,255,.03);color:#8090a8;transition:all .18s;}
.pt-fbtn:hover{background:rgba(255,255,255,.07);color:#e8e0d0;}
.pt-fbtn.active{background:rgba(80,232,144,.1);color:#50e890;border-color:rgba(80,232,144,.3);}
.pt-search{font-family:'JetBrains Mono',monospace;font-size:.62rem;background:#0d1018;border:1px solid #1e2535;color:#e8e0d0;padding:5px 10px;border-radius:3px;outline:none;width:160px;transition:border-color .2s;}
.pt-search:focus{border-color:#50e890;}
.pt-search::placeholder{color:#404e66;}

/* ── LEGEND ── */
.pt-legend{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:16px;padding:10px 14px;background:#0d1018;border:1px solid #1e2535;border-radius:6px;}
.pt-leg-item{display:flex;align-items:center;gap:5px;font-size:.52rem;color:#8090a8;}
.pt-leg-box{width:11px;height:11px;border-radius:2px;flex-shrink:0;}

/* ── PERIODIC TABLE GRID ── */
.pt-grid-wrap{overflow-x:auto;padding-bottom:8px;}
.pt-grid{display:grid;grid-template-columns:repeat(18,minmax(48px,1fr));gap:2px;min-width:900px;}

/* ── ELEMENT CELL ── */
.el{border-radius:4px;padding:4px 3px 3px;cursor:pointer;position:relative;overflow:hidden;border:1px solid transparent;transition:transform .18s cubic-bezier(.4,0,.2,1),box-shadow .18s,border-color .18s,opacity .22s;aspect-ratio:1;display:flex;flex-direction:column;justify-content:space-between;user-select:none;-webkit-user-select:none;}
.el::after{content:'';position:absolute;inset:0;border-radius:3px;background:radial-gradient(circle at 50% 0%,rgba(255,255,255,.08),transparent 65%);opacity:0;transition:opacity .18s;}
.el:hover{transform:scale(1.18) translateZ(0);z-index:10;box-shadow:0 8px 28px rgba(0,0,0,.7),0 0 0 1px var(--ec,#50e890);border-color:var(--ec,#50e890);}
.el:hover::after{opacity:1;}
.el:active{transform:scale(1.08);}
.el.dim{opacity:.18;}
.el.highlight{opacity:1;box-shadow:0 0 12px var(--ec,#50e890);}
.el-num{font-size:.48rem;color:rgba(255,255,255,.5);line-height:1;}
.el-sym{font-family:'Syne',sans-serif;font-weight:800;font-size:.95rem;line-height:1.1;text-align:center;color:#fff;}
.el-name{font-size:.38rem;text-align:center;color:rgba(255,255,255,.55);line-height:1;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
.el-mass{font-size:.37rem;text-align:center;color:rgba(255,255,255,.4);line-height:1;}

/* Period/Group labels */
.pt-period-label,.pt-group-label{font-family:'JetBrains Mono',monospace;font-size:.5rem;color:#404e66;display:flex;align-items:center;justify-content:center;text-align:center;}

/* ── ELEMENT CATEGORIES → colors ── */
.ec-alkali{background:#1a1208;border-color:#8b4500;--ec:#f08040;}
.ec-alkaline{background:#181508;border-color:#7a6500;--ec:#e8c060;}
.ec-transition{background:#0e1420;border-color:#1e3060;--ec:#60b8f0;}
.ec-post-transition{background:#121a14;border-color:#1e4020;--ec:#50e890;}
.ec-metalloid{background:#131520;border-color:#2a2050;--ec:#a080f0;}
.ec-nonmetal{background:#0e1820;border-color:#105040;--ec:#40d0c0;}
.ec-halogen{background:#1a0e18;border-color:#501050;--ec:#f06080;}
.ec-noble{background:#18101a;border-color:#401460;--ec:#c080f0;}
.ec-lanthanide{background:#1a1010;border-color:#4a1010;--ec:#f06060;}
.ec-actinide{background:#141018;border-color:#301840;--ec:#d060e0;}

/* ── MODAL OVERLAY ── */
#pt-modal-overlay{position:fixed;inset:0;z-index:9998;background:rgba(3,4,10,.92);backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);display:flex;align-items:center;justify-content:center;padding:16px;opacity:0;pointer-events:none;transition:opacity .25s cubic-bezier(.4,0,.2,1);}
#pt-modal-overlay.show{opacity:1;pointer-events:all;}
#pt-modal{background:linear-gradient(135deg,#0f1220 0%,#0d1018 50%,#111526 100%);border:1px solid rgba(80,232,144,.15);border-radius:14px;max-width:640px;width:100%;max-height:90vh;overflow-y:auto;box-shadow:0 40px 100px rgba(0,0,0,.9),0 0 0 1px rgba(80,232,144,.06),inset 0 1px 0 rgba(80,232,144,.1);transform:translateY(24px) scale(.96);transition:transform .3s cubic-bezier(.16,1,.3,1);scrollbar-width:thin;scrollbar-color:#1e2535 transparent;}
#pt-modal-overlay.show #pt-modal{transform:translateY(0) scale(1);}
#pt-modal::-webkit-scrollbar{width:3px;}
#pt-modal::-webkit-scrollbar-thumb{background:#1e2535;border-radius:3px;}
#pt-modal-hdr{padding:20px 22px 16px;border-bottom:1px solid rgba(80,232,144,.1);display:flex;align-items:flex-start;justify-content:space-between;gap:14px;position:sticky;top:0;background:linear-gradient(135deg,#0f1220,#0d1018);backdrop-filter:blur(12px);z-index:2;}
#pt-modal-symbol{font-family:'Syne',sans-serif;font-weight:800;font-size:3.2rem;line-height:1;margin-right:16px;flex-shrink:0;}
#pt-modal-info{flex:1;}
#pt-modal-name{font-family:'Syne',sans-serif;font-size:1.3rem;font-weight:700;color:#e8e0d0;margin-bottom:2px;}
#pt-modal-sub{font-family:'JetBrains Mono',monospace;font-size:.6rem;color:#8090a8;letter-spacing:.12em;}
#pt-modal-close{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);color:#8090a8;font-size:14px;width:30px;height:30px;border-radius:6px;cursor:pointer;display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:all .15s;font-family:sans-serif;}
#pt-modal-close:hover{background:rgba(240,96,128,.15);border-color:rgba(240,96,128,.4);color:#f06080;}
#pt-modal-body{padding:18px 22px 24px;}
.pt-prop-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:16px;}
.pt-prop{background:#0d101a;border:1px solid #1e2535;border-radius:6px;padding:10px 12px;}
.pt-prop-lbl{font-family:'JetBrains Mono',monospace;font-size:.5rem;letter-spacing:.15em;text-transform:uppercase;color:#404e66;margin-bottom:3px;}
.pt-prop-val{font-family:'JetBrains Mono',monospace;font-size:.82rem;color:#e8e0d0;line-height:1.3;}
.pt-conf-block{background:#0d101a;border:1px solid #1e2535;border-radius:6px;padding:10px 12px;margin-bottom:12px;}
.pt-conf-lbl{font-family:'JetBrains Mono',monospace;font-size:.5rem;letter-spacing:.15em;text-transform:uppercase;color:#404e66;margin-bottom:5px;}
.pt-conf-val{font-family:'JetBrains Mono',monospace;font-size:.78rem;color:#60b8f0;word-break:break-all;line-height:1.6;}
.pt-jee-block{background:rgba(80,232,144,.04);border:1px solid rgba(80,232,144,.15);border-radius:6px;padding:10px 12px;margin-bottom:12px;}
.pt-jee-lbl{font-family:'JetBrains Mono',monospace;font-size:.5rem;letter-spacing:.15em;text-transform:uppercase;color:#50e890;margin-bottom:5px;}
.pt-jee-val{font-family:'Crimson Pro',serif;font-size:.88rem;color:#c0d8c0;line-height:1.7;}
.pt-exc-block{background:rgba(240,192,96,.04);border:1px solid rgba(240,192,96,.15);border-radius:6px;padding:10px 12px;}
.pt-exc-lbl{font-family:'JetBrains Mono',monospace;font-size:.5rem;letter-spacing:.15em;text-transform:uppercase;color:#e8c060;margin-bottom:5px;}
.pt-exc-val{font-family:'Crimson Pro',serif;font-size:.88rem;color:#d0c890;line-height:1.7;}

/* ── TRENDS SECTION ── */
.pt-trends{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:14px;margin-top:8px;}
.pt-trend-card{background:#0d1018;border:1px solid #1e2535;border-radius:8px;padding:16px 18px;transition:border-color .2s;}
.pt-trend-card:hover{border-color:#50e890;}
.pt-trend-title{font-family:'Syne',sans-serif;font-size:.85rem;font-weight:700;color:#50e890;margin-bottom:10px;display:flex;align-items:center;gap:6px;}
.pt-trend-arrow{font-size:1.1rem;}
.pt-trend-body{font-family:'JetBrains Mono',monospace;font-size:.67rem;color:#8090a8;line-height:1.85;}
.pt-trend-body .hi{color:#60b8f0;}.pt-trend-body .warn{color:#f08040;}.pt-trend-body .exc{color:#e8c060;}

/* ── EXCEPTIONS SECTION ── */
.pt-exc-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:12px;margin-top:8px;}
.pt-exc-card{background:#0d1018;border:1px solid rgba(232,192,96,.15);border-radius:8px;padding:14px 16px;transition:border-color .2s;}
.pt-exc-card:hover{border-color:rgba(232,192,96,.35);}
.pt-exc-head{font-family:'JetBrains Mono',monospace;font-size:.58rem;letter-spacing:.12em;text-transform:uppercase;color:#e8c060;margin-bottom:8px;}
.pt-exc-row{display:flex;align-items:flex-start;gap:8px;padding:5px 0;border-bottom:1px solid rgba(255,255,255,.04);}
.pt-exc-row:last-child{border-bottom:none;}
.pt-exc-elem{font-family:'Syne',sans-serif;font-weight:700;font-size:.85rem;color:#fff;min-width:32px;flex-shrink:0;}
.pt-exc-text{font-family:'JetBrains Mono',monospace;font-size:.6rem;color:#8090a8;line-height:1.6;}
.pt-exc-text .hi{color:#f06080;}.pt-exc-text .ok{color:#50e890;}.pt-exc-text .note{color:#e8c060;}

/* ── PERIODIC TRENDS ARROWS ── */
.pt-trend-visual{margin:12px 0;padding:12px;background:#06080f;border-radius:6px;border:1px solid #1e2535;}
.ptv-row{display:flex;align-items:center;gap:8px;margin-bottom:6px;}
.ptv-label{font-size:.52rem;color:#404e66;width:110px;flex-shrink:0;}
.ptv-bar{flex:1;height:6px;border-radius:3px;position:relative;}
.ptv-bar-fill{height:100%;border-radius:3px;transition:width .6s cubic-bezier(.4,0,.2,1);}
.ptv-dir{font-size:.52rem;color:#8090a8;white-space:nowrap;}

/* ── ORBITAL FILLING ── */
.pt-orbital-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:10px;margin-top:8px;}
.pt-orb-card{background:#0d1018;border:1px solid #1e2535;border-radius:8px;padding:12px 14px;}
.pt-orb-title{font-family:'JetBrains Mono',monospace;font-size:.55rem;letter-spacing:.12em;text-transform:uppercase;color:#a080f0;margin-bottom:8px;}
.pt-orb-seq{font-family:'JetBrains Mono',monospace;font-size:.7rem;color:#60b8f0;line-height:1.9;letter-spacing:.04em;}
.pt-orb-seq .orb{color:#a080f0;font-weight:700;}.pt-orb-seq .sup{font-size:.5rem;vertical-align:super;}

/* ── HAPTICS ── */
@keyframes ptElPop{0%{transform:scale(1)}40%{transform:scale(1.22)}70%{transform:scale(0.96)}100%{transform:scale(1.18) translateZ(0)}}
@keyframes ptModalIn{0%{opacity:0;transform:translateY(32px) scale(.93)}100%{opacity:1;transform:translateY(0) scale(1)}}
@keyframes ptCellGlow{0%{box-shadow:0 0 0px transparent}50%{box-shadow:0 0 18px var(--ec,#50e890)}100%{box-shadow:0 0 8px var(--ec,#50e890)}}
@keyframes ptFilterPulse{0%{transform:scale(1)}50%{transform:scale(1.06)}100%{transform:scale(1)}}
@keyframes ptSweep{from{opacity:0;transform:translateX(-8px)}to{opacity:1;transform:translateX(0)}}
@keyframes ptRowReveal{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:translateY(0)}}

.el.pop{animation:ptElPop .32s cubic-bezier(.4,0,.2,1);}
.pt-fbtn.pulse{animation:ptFilterPulse .22s ease;}
</style>

<!-- PERIODIC TABLE SECTION HTML -->
<div class="psec" id="sec-ptable">
<div class="pt-wrap">

<div class="pt-banner">
  <span class="pt-banner-badge">08 — Chemistry</span>
  <h2>Interactive Periodic Table</h2>
  <p>All 118 elements · JEE properties · trends · exceptions · electronic configuration</p>
</div>

<!-- Sub-tabs -->
<div class="pt-subtabs">
  <div class="pt-stab active" id="pstab-table" onclick="ptShowTab('table')">Periodic Table</div>
  <div class="pt-stab" id="pstab-trends" onclick="ptShowTab('trends')">Periodic Trends</div>
  <div class="pt-stab" id="pstab-exceptions" onclick="ptShowTab('exceptions')">JEE Exceptions</div>
  <div class="pt-stab" id="pstab-config" onclick="ptShowTab('config')">Electronic Config</div>
</div>

<!-- ═══ TAB: TABLE ═══ -->
<div id="pttab-table">
  <div class="pt-filters">
    <span class="pt-flabel">Filter:</span>
    <button class="pt-fbtn active" onclick="ptFilter('all',this)">All</button>
    <button class="pt-fbtn" onclick="ptFilter('alkali',this)" style="color:#f08040">Alkali Metals</button>
    <button class="pt-fbtn" onclick="ptFilter('alkaline',this)" style="color:#e8c060">Alkaline Earth</button>
    <button class="pt-fbtn" onclick="ptFilter('transition',this)" style="color:#60b8f0">Transition</button>
    <button class="pt-fbtn" onclick="ptFilter('post-transition',this)" style="color:#50e890">Post-Trans</button>
    <button class="pt-fbtn" onclick="ptFilter('metalloid',this)" style="color:#a080f0">Metalloids</button>
    <button class="pt-fbtn" onclick="ptFilter('nonmetal',this)" style="color:#40d0c0">Non-Metals</button>
    <button class="pt-fbtn" onclick="ptFilter('halogen',this)" style="color:#f06080">Halogens</button>
    <button class="pt-fbtn" onclick="ptFilter('noble',this)" style="color:#c080f0">Noble Gases</button>
    <button class="pt-fbtn" onclick="ptFilter('lanthanide',this)" style="color:#f06060">Lanthanides</button>
    <button class="pt-fbtn" onclick="ptFilter('actinide',this)" style="color:#d060e0">Actinides</button>
    <input class="pt-search" id="pt-search-inp" placeholder="Search element…" oninput="ptSearch(this.value)">
  </div>
  <div class="pt-legend">
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#f08040"></div>Alkali Metals</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#e8c060"></div>Alkaline Earth</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#60b8f0"></div>Transition Metals</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#50e890"></div>Post-Transition</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#a080f0"></div>Metalloids</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#40d0c0"></div>Non-Metals</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#f06080"></div>Halogens</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#c080f0"></div>Noble Gases</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#f06060"></div>Lanthanides</div>
    <div class="pt-leg-item"><div class="pt-leg-box" style="background:#d060e0"></div>Actinides</div>
  </div>
  <div class="pt-grid-wrap">
    <div class="pt-grid" id="pt-grid"></div>
  </div>
</div>

<!-- ═══ TAB: TRENDS ═══ -->
<div id="pttab-trends" style="display:none">
  <div class="pt-trends">
    <div class="pt-trend-card" style="animation:ptSweep .35s .05s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">↔</span> Atomic Radius</div>
      <div class="pt-trend-visual">
        <div class="ptv-row"><span class="ptv-label">Across period →</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#60b8f0,#1e2535)"></div></div><span class="ptv-dir">Decreases ↓</span></div>
        <div class="ptv-row"><span class="ptv-label">Down group ↓</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#1e2535,#60b8f0)"></div></div><span class="ptv-dir">Increases ↑</span></div>
      </div>
      <div class="pt-trend-body">
        <span class="hi">Across period:</span> Nuclear charge ↑, same shell → electron cloud contracts.<br>
        <span class="hi">Down group:</span> New shells added → shielding ↑ → radius expands.<br>
        <span class="exc">Exceptions: </span>Cr/Cu config; noble gas radius (van der Waals) unusually large.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .1s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">⚡</span> Ionisation Energy (IE)</div>
      <div class="pt-trend-visual">
        <div class="ptv-row"><span class="ptv-label">Across period →</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#1e2535,#e8c060)"></div></div><span class="ptv-dir">Generally ↑</span></div>
        <div class="ptv-row"><span class="ptv-label">Down group ↓</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#e8c060,#1e2535)"></div></div><span class="ptv-dir">Decreases ↓</span></div>
      </div>
      <div class="pt-trend-body">
        <span class="hi">IE₁ order:</span> Na &lt; Mg &lt; Al &lt; Si &lt; P &gt; S &lt; Cl &lt; Ar<br>
        <span class="warn">Anomaly 1:</span> IE₁(Be) &gt; IE₁(B) — full 2s² vs 1 e⁻ in higher 2p<br>
        <span class="warn">Anomaly 2:</span> IE₁(N) &gt; IE₁(O) — half-filled 2p³ extra stable<br>
        <span class="warn">Anomaly 3:</span> IE₁(Mg) &gt; IE₁(Al); IE₁(P) &gt; IE₁(S)<br>
        <span class="exc">JEE fact:</span> Noble gases highest IE in period; Cs lowest IE of all stable elements.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .15s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">🧲</span> Electronegativity (EN)</div>
      <div class="pt-trend-visual">
        <div class="ptv-row"><span class="ptv-label">Across period →</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#1e2535,#f06080)"></div></div><span class="ptv-dir">Increases ↑</span></div>
        <div class="ptv-row"><span class="ptv-label">Down group ↓</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#f06080,#1e2535)"></div></div><span class="ptv-dir">Decreases ↓</span></div>
      </div>
      <div class="pt-trend-body">
        <span class="hi">Pauling scale:</span> F(4.0) &gt; O(3.5) &gt; N/Cl(3.0) &gt; Br(2.8) &gt; S(2.5)<br>
        <span class="hi">Highest EN:</span> F (most electronegative element)<br>
        <span class="exc">Noble gases</span> not assigned EN on Pauling scale.<br>
        <span class="warn">JEE note:</span> EN determines bond polarity &amp; bond character.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .2s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">⊖</span> Electron Affinity (EA)</div>
      <div class="pt-trend-visual">
        <div class="ptv-row"><span class="ptv-label">Across period →</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#1e2535,#40d0c0)"></div></div><span class="ptv-dir">Generally ↑</span></div>
        <div class="ptv-row"><span class="ptv-label">Down group ↓</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#40d0c0,#1e2535)"></div></div><span class="ptv-dir">Decreases ↓</span></div>
      </div>
      <div class="pt-trend-body">
        <span class="hi">Highest EA:</span> Cl &gt; F (anomaly! F too small → repulsion)<br>
        <span class="warn">Be, N, Mg, noble gases:</span> Positive EA (electron-addition unfavoured)<br>
        <span class="warn">Anomaly:</span> EA(O) &lt; EA(S) for same reason as F &lt; Cl<br>
        <span class="exc">Second EA</span> always positive (endothermic) — against electron-electron repulsion.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .25s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">🔬</span> Metallic Character</div>
      <div class="pt-trend-visual">
        <div class="ptv-row"><span class="ptv-label">Across period →</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#50e890,#1e2535)"></div></div><span class="ptv-dir">Decreases ↓</span></div>
        <div class="ptv-row"><span class="ptv-label">Down group ↓</span><div class="ptv-bar"><div class="ptv-bar-fill" style="width:100%;background:linear-gradient(to right,#1e2535,#50e890)"></div></div><span class="ptv-dir">Increases ↑</span></div>
      </div>
      <div class="pt-trend-body">
        <span class="hi">Most metallic:</span> Cs (excluding radioactive Fr)<br>
        <span class="hi">Least metallic:</span> F (but noble gases are non-metals too)<br>
        <span class="exc">Diagonal relationship:</span> Li–Mg, Be–Al, B–Si show similar properties.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .3s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">📏</span> Ionic Radius Trends</div>
      <div class="pt-trend-body" style="margin-top:8px">
        <span class="hi">Isoelectronic series:</span> Same electrons, increasing Z → smaller.<br>
        e.g. N³⁻ &gt; O²⁻ &gt; F⁻ &gt; Ne &gt; Na⁺ &gt; Mg²⁺ &gt; Al³⁺<br><br>
        <span class="hi">Cation vs neutral:</span> Cation always smaller (loses e⁻, nuclear charge unchanged)<br>
        <span class="hi">Anion vs neutral:</span> Anion always larger (gains e⁻, more repulsion)<br><br>
        <span class="warn">Down a group:</span> Ionic radius increases (additional shells).<br>
        <span class="exc">Lanthanide contraction:</span> 4f electrons poor shielding → 5d/6s contract.
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .35s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">🌡</span> Melting & Boiling Points</div>
      <div class="pt-trend-body" style="margin-top:8px">
        <span class="hi">Period 2/3 trend:</span> Increases across metals (stronger metallic bonding), peaks at group 14 (covalent network), drops sharply for non-metals.<br><br>
        <span class="hi">Highest MP:</span> W (Tungsten) — 3422°C<br>
        <span class="hi">Highest BP of non-metal:</span> C (graphite/diamond) ~3550°C<br>
        <span class="warn">Hg:</span> Only liquid metal at room temp (−38.83°C MP)<br>
        <span class="warn">Ga &amp; Cs:</span> Melt just above room temperature.<br>
        <span class="exc">Anomaly:</span> Ice floats on water (H₂O density anomaly at 4°C due to H-bonding).
      </div>
    </div>
    <div class="pt-trend-card" style="animation:ptSweep .35s .4s both">
      <div class="pt-trend-title"><span class="pt-trend-arrow">📐</span> Oxidation States</div>
      <div class="pt-trend-body" style="margin-top:8px">
        <span class="hi">Max OS</span> = group number (up to 8 for transition metals)<br>
        <span class="hi">Min OS</span> = group number − 8 (for non-metals)<br><br>
        <span class="warn">Special elements:</span><br>
        F: always −1 (most electronegative; no d-orbital)<br>
        O: usually −2; but −1 in peroxides, −½ in O₂⁻, +2 with F<br>
        H: +1 with non-metals; −1 in metal hydrides<br><br>
        <span class="exc">Transition metals:</span> Show multiple OS due to (n-1)d electrons.
      </div>
    </div>
  </div>
</div>

<!-- ═══ TAB: EXCEPTIONS ═══ -->
<div id="pttab-exceptions" style="display:none">
  <div class="pt-exc-grid">
    <div class="pt-exc-card" style="animation:ptSweep .35s .05s both">
      <div class="pt-exc-head">⚡ Electronic Configuration Exceptions</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Cr</div><div class="pt-exc-text">Expected: [Ar] 3d⁴ 4s² <br>Actual: [Ar] <span class="ok">3d⁵ 4s¹</span><br><span class="note">Half-filled d (3d⁵) is extra stable</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Cu</div><div class="pt-exc-text">Expected: [Ar] 3d⁹ 4s² <br>Actual: [Ar] <span class="ok">3d¹⁰ 4s¹</span><br><span class="note">Fully-filled d (3d¹⁰) is extra stable</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Mo</div><div class="pt-exc-text">Expected: [Kr] 4d⁴ 5s² <br>Actual: [Kr] <span class="ok">4d⁵ 5s¹</span><br><span class="note">Like Cr — half-filled 4d⁵ stability</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Ag</div><div class="pt-exc-text">Expected: [Kr] 4d⁹ 5s² <br>Actual: [Kr] <span class="ok">4d¹⁰ 5s¹</span><br><span class="note">Like Cu — fully-filled 4d¹⁰ stability</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Au</div><div class="pt-exc-text">Actual: [Xe] <span class="ok">4f¹⁴ 5d¹⁰ 6s¹</span><br><span class="note">Fully-filled d stability + relativistic effects</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Pd</div><div class="pt-exc-text">Actual: [Kr] <span class="ok">4d¹⁰ 5s⁰</span><br><span class="note">Unique — fully-filled d, empty s orbital</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .1s both">
      <div class="pt-exc-head">📉 Ionisation Energy Anomalies</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Be &gt; B</div><div class="pt-exc-text">IE₁(Be) &gt; IE₁(B)<br><span class="note">Be: full 2s²; B: single 2p¹ electron easier to remove</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">N &gt; O</div><div class="pt-exc-text">IE₁(N) &gt; IE₁(O)<br><span class="note">N: half-filled 2p³ (stable); O: one paired 2p → removed easily</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Mg &gt; Al</div><div class="pt-exc-text">IE₁(Mg) &gt; IE₁(Al)<br><span class="note">Mg: full 3s²; Al: single 3p¹ easier to remove</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">P &gt; S</div><div class="pt-exc-text">IE₁(P) &gt; IE₁(S)<br><span class="note">P: half-filled 3p³; S has one paired 3p electron</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .15s both">
      <div class="pt-exc-head">🧲 Electron Affinity Anomalies</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Cl &gt; F</div><div class="pt-exc-text">EA(Cl) &gt; EA(F)<br><span class="note">F is too small; extra electron repulsion in compact 2p shell</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">S &gt; O</div><div class="pt-exc-text">EA(S) &gt; EA(O)<br><span class="note">Same reason — O 2p shell too compact</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">N, Be</div><div class="pt-exc-text">EA is positive (endothermic)<br><span class="note">N: half-filled 2p³ stable; Be: full 2s², extra e⁻ must go to 2p</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Noble</div><div class="pt-exc-text">EA is positive<br><span class="note">Full octet — extra electron would occupy higher energy shell</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .2s both">
      <div class="pt-exc-head">📏 Size / Radius Anomalies</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Ga &lt; Al</div><div class="pt-exc-text">Ga smaller than expected<br><span class="note">Poor shielding by 3d¹⁰ electrons → Zeff higher for Ga</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Zr ≈ Hf</div><div class="pt-exc-text">Zirconium ≈ Hafnium radius<br><span class="note">Lanthanide contraction cancels shell addition effect</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">In &gt; Tl</div><div class="pt-exc-text">Tl smaller than expected<br><span class="note">Relativistic contraction of 6s orbital</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Li &lt; Na</div><div class="pt-exc-text">Li has smaller atomic radius<br><span class="note">Expected — 2nd shell vs 3rd; but Li resembles Mg (diagonal)</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .25s both">
      <div class="pt-exc-head">🔥 Diagonal Relationships (JEE)</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Li – Mg</div><div class="pt-exc-text"><span class="note">Both form covalent organometallics; Li₃N stable like Mg₃N₂; similar solubility patterns</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Be – Al</div><div class="pt-exc-text"><span class="note">Both amphoteric; form polymeric hydrides; similar charge density</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">B – Si</div><div class="pt-exc-text"><span class="note">Both form covalent halides; hydrolysed by water; semiconducting elements</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .3s both">
      <div class="pt-exc-head">🌡 Melting Point Anomalies</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Hg</div><div class="pt-exc-text">Only liquid metal at RT<br><span class="note">Weak metallic bonding; filled d¹⁰ → poor orbital overlap</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Ga</div><div class="pt-exc-text">MP = 29.76°C (very low)<br><span class="note">Unusual crystal structure with Ga₂ units; weakly metallic</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Cs</div><div class="pt-exc-text">MP = 28.5°C<br><span class="note">Very weak metallic bonding; huge atom, very low IE</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">W</div><div class="pt-exc-text">Highest MP among metals: 3422°C<br><span class="note">6 unpaired electrons → strongest metallic bonding</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .35s both">
      <div class="pt-exc-head">⚗️ Oxidation State Anomalies</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">F</div><div class="pt-exc-text">Only −1 oxidation state<br><span class="note">Most electronegative; no d-orbitals to expand valence shell</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">O in F₂O</div><div class="pt-exc-text">O shows <span class="hi">+2</span> oxidation state<br><span class="note">F is more electronegative than O; assigns +2 to O</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Mn</div><div class="pt-exc-text">Shows +7 OS in KMnO₄<br><span class="note">Highest OS among common transition metals; all 7 electrons used</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Os, Ru</div><div class="pt-exc-text">Show +8 OS (highest possible)<br><span class="note">OsO₄, RuO₄ — rare but important compounds</span></div></div>
    </div>
    <div class="pt-exc-card" style="animation:ptSweep .35s .4s both">
      <div class="pt-exc-head">💡 JEE Special Facts</div>
      <div class="pt-exc-row"><div class="pt-exc-elem">Inert pair</div><div class="pt-exc-text">6s² pair reluctant to participate in bonding in heavier p-block (Tl, Pb, Bi)<br><span class="note">Pb²⁺ more stable than Pb⁴⁺; Tl⁺ more stable than Tl³⁺</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">π-backbond</div><div class="pt-exc-text">SiF₄ more stable than CF₄<br><span class="note">Si has d-orbitals; F lone pairs → Si d-orbital (pπ-dπ)</span></div></div>
      <div class="pt-exc-row"><div class="pt-exc-elem">H position</div><div class="pt-exc-text">H placed in Group 1 AND 17<br><span class="note">1 electron like alkali metals; 1 short of noble gas like halogens</span></div></div>
    </div>
  </div>
</div>

<!-- ═══ TAB: CONFIG ═══ -->
<div id="pttab-config" style="display:none">
  <div class="pt-orbital-grid">
    <div class="pt-orb-card" style="animation:ptSweep .35s .05s both">
      <div class="pt-orb-title">Aufbau Order (n+l rule)</div>
      <div class="pt-orb-seq">
        <span class="orb">1s</span> → <span class="orb">2s</span> → <span class="orb">2p</span> → <span class="orb">3s</span> → <span class="orb">3p</span> → <span class="orb">4s</span> → <span class="orb">3d</span> → <span class="orb">4p</span> → <span class="orb">5s</span> → <span class="orb">4d</span> → <span class="orb">5p</span> → <span class="orb">6s</span> → <span class="orb">4f</span> → <span class="orb">5d</span> → <span class="orb">6p</span> → <span class="orb">7s</span> → <span class="orb">5f</span> → <span class="orb">6d</span>
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .08s both">
      <div class="pt-orb-title">Orbital Capacities</div>
      <div class="pt-orb-seq">
        s-block: 2 electrons (1 orbital)<br>
        p-block: 6 electrons (3 orbitals)<br>
        d-block: 10 electrons (5 orbitals)<br>
        f-block: 14 electrons (7 orbitals)
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .11s both">
      <div class="pt-orb-title">Hund's Rule</div>
      <div class="pt-orb-seq">
        Electrons occupy orbitals singly before pairing. All singly occupied orbitals have same spin (maximise spin multiplicity).<br><br>
        e.g. C(Z=6): 1s² 2s² 2p↑ 2p↑ (not 2p↑↓ 2p⁰)
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .14s both">
      <div class="pt-orb-title">Pauli Exclusion</div>
      <div class="pt-orb-seq">
        No two electrons in an atom can have all four quantum numbers identical.<br><br>
        Each orbital holds max 2 electrons with opposite spins (↑↓).
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .17s both">
      <div class="pt-orb-title">Extra Stability</div>
      <div class="pt-orb-seq">
        Half-filled subshell (s¹, p³, d⁵, f⁷) — symmetric, exchange energy max.<br><br>
        Fully-filled subshell (s², p⁶, d¹⁰, f¹⁴) — symmetric, highly stable.<br><br>
        <span style="color:#e8c060">Cr: 3d⁵4s¹ · Cu: 3d¹⁰4s¹</span>
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .2s both">
      <div class="pt-orb-title">Quantum Numbers</div>
      <div class="pt-orb-seq">
        n (principal): 1,2,3... — shell<br>
        l (azimuthal): 0 to n-1 — subshell<br>
        mₗ (magnetic): −l to +l — orbital<br>
        mₛ (spin): +½ or −½<br><br>
        l=0→s, l=1→p, l=2→d, l=3→f
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .23s both">
      <div class="pt-orb-title">Noble Gas Cores</div>
      <div class="pt-orb-seq">
        He [2]: 1s²<br>
        Ne [10]: [He] 2s² 2p⁶<br>
        Ar [18]: [Ne] 3s² 3p⁶<br>
        Kr [36]: [Ar] 3d¹⁰ 4s² 4p⁶<br>
        Xe [54]: [Kr] 4d¹⁰ 5s² 5p⁶<br>
        Rn [86]: [Xe] 4f¹⁴ 5d¹⁰ 6s² 6p⁶
      </div>
    </div>
    <div class="pt-orb-card" style="animation:ptSweep .35s .26s both">
      <div class="pt-orb-title">Transition Metal Config</div>
      <div class="pt-orb-seq">
        4s fills before 3d (Aufbau)<br>
        but 4s ionised first (experimental)<br><br>
        Fe²⁺: [Ar] 3d⁶ (not 3d⁴4s²)<br>
        Fe³⁺: [Ar] 3d⁵<br><br>
        <span style="color:#f06080">4s ionises before 3d in cation formation</span>
      </div>
    </div>
  </div>
</div>

</div><!-- .pt-wrap -->
</div><!-- #sec-ptable -->

<!-- ELEMENT DETAIL MODAL -->
<div id="pt-modal-overlay">
  <div id="pt-modal">
    <div id="pt-modal-hdr">
      <div style="display:flex;align-items:center;gap:4px;flex:1">
        <div id="pt-modal-symbol" style="color:#50e890">H</div>
        <div id="pt-modal-info">
          <div id="pt-modal-name">Hydrogen</div>
          <div id="pt-modal-sub">Z=1 · Period 1 · Group 1 · Non-Metal</div>
        </div>
      </div>
      <button id="pt-modal-close" onclick="ptCloseModal()">✕</button>
    </div>
    <div id="pt-modal-body"></div>
  </div>
</div>

<script>
/* ═══════════════════════════════════════════════════
   PERIODIC TABLE DATA + LOGIC
═══════════════════════════════════════════════════ */

// Category color map
const PT_CAT_COLOR = {
  'alkali':'#f08040','alkaline':'#e8c060','transition':'#60b8f0',
  'post-transition':'#50e890','metalloid':'#a080f0','nonmetal':'#40d0c0',
  'halogen':'#f06080','noble':'#c080f0','lanthanide':'#f06060','actinide':'#d060e0'
};

// Full element data (118 elements)
const PT_ELEMENTS = [
  // Z, sym, name, mass, cat, period, group, config, jeeNote, exception
  [1,'H','Hydrogen',1.008,'nonmetal',1,1,'1s¹','Most abundant element in universe. Placed in Gr1 AND Gr17.','Only element with no neutrons in most common isotope (protium). Can show +1 and -1 OS.'],
  [2,'He','Helium',4.003,'noble',1,18,'1s²','Lightest noble gas; no known stable compounds.','Only element with no period-1 congener having filled shell at 1s².'],
  [3,'Li','Lithium',6.94,'alkali',2,1,'[He] 2s¹','Diagonal relationship with Mg. Used in batteries.','Smallest alkali metal; anomalously high IE for alkali metal due to small size.'],
  [4,'Be','Beryllium',9.012,'alkaline',2,2,'[He] 2s²','Diagonal relationship with Al. Amphoteric oxide.','IE₁(Be) > IE₁(B) due to full 2s². EA is positive (endothermic addition).'],
  [5,'B','Boron',10.81,'metalloid',2,13,'[He] 2s² 2p¹','Electron deficient; forms Lewis acid. Diagonal with Si.','Only metalloid in period 2. Boranes have multicentre bonds.'],
  [6,'C','Carbon',12.011,'nonmetal',2,14,'[He] 2s² 2p²','Forms more compounds than any other element (organic chemistry).','Allotropes: diamond (hardest), graphite (conductor), fullerene, graphene.'],
  [7,'N','Nitrogen',14.007,'nonmetal',2,15,'[He] 2s² 2p³','N₂ is inert (triple bond, BE=945 kJ/mol). IE₁(N) > IE₁(O).','Half-filled 2p³ is extra stable → IE anomaly. EA of N is positive.'],
  [8,'O','Oxygen',15.999,'nonmetal',2,16,'[He] 2s² 2p⁴','OS usually -2; but -1 in peroxides, +2 in OF₂.','IE₁(O) < IE₁(N) despite higher Z (paired electron in 2p easier to remove).'],
  [9,'F','Fluorine',18.998,'halogen',2,17,'[He] 2s² 2p⁵','Most electronegative element (EN=4.0). Always -1 OS.','EA(F) < EA(Cl) — F too small, electron repulsion dominates. No d-orbitals.'],
  [10,'Ne','Neon',20.180,'noble',2,18,'[He] 2s² 2p⁶','Inert noble gas; no compounds known.','Only noble gas that forms no known stable compounds even under extreme conditions.'],
  [11,'Na','Sodium',22.990,'alkali',3,1,'[Ne] 3s¹','Na⁺ most important cation in biology. NaOH strong base.','Reacts vigorously with water; Na in flame test → yellow.'],
  [12,'Mg','Magnesium',24.305,'alkaline',3,2,'[Ne] 3s²','Diagonal relationship with Li. IE₁(Mg) > IE₁(Al).','Burns in CO₂ and N₂ unlike most metals. Chlorophyll contains Mg.'],
  [13,'Al','Aluminium',26.982,'post-transition',3,13,'[Ne] 3s² 3p¹','Amphoteric metal; diagonal with Be. Most abundant metal in crust.','IE₁(Al) < IE₁(Mg) due to single 3p¹ electron. Al₂O₃ is amphoteric.'],
  [14,'Si','Silicon',28.086,'metalloid',3,14,'[Ne] 3s² 3p²','Semiconductor. Diagonal with B. SiF₄ more stable than CF₄ (pπ-dπ).','Si has d-orbitals unlike C; SiO₂ is polymeric, CO₂ is molecular.'],
  [15,'P','Phosphorus',30.974,'nonmetal',3,15,'[Ne] 3s² 3p³','IE₁(P) > IE₁(S) due to half-filled 3p³. Allotropes: white, red, black.','White P is very reactive (tetrahedral P₄). Red P is polymeric, less reactive.'],
  [16,'S','Sulphur',32.06,'nonmetal',3,16,'[Ne] 3s² 3p⁴','EA(S) > EA(O) due to size anomaly. Multiple allotropes (S₈ most stable).','Expanded octet possible (SF₆ etc.) using 3d orbitals.'],
  [17,'Cl','Chlorine',35.45,'halogen',3,17,'[Ne] 3s² 3p⁵','Highest EA among all elements (EA = 349 kJ/mol). Strong oxidizer.','EA(Cl) > EA(F) — F too small for easy electron addition.'],
  [18,'Ar','Argon',39.948,'noble',3,18,'[Ne] 3s² 3p⁶','Most abundant noble gas in atmosphere (~1%).','Used in welding as inert shield gas; no stable compounds known.'],
  [19,'K','Potassium',39.098,'alkali',4,1,'[Ar] 4s¹','Violet/lilac flame test. Important in biology (K⁺/Na⁺ pump).','Reacts more violently than Na with water; K₂O₂ forms (peroxide).'],
  [20,'Ca','Calcium',40.078,'alkaline',4,2,'[Ar] 4s²','Brick-red flame test. Important in bones (Ca₃(PO₄)₂).','CaO + H₂O → Ca(OH)₂ (slaked lime, strongly exothermic).'],
  [21,'Sc','Scandium',44.956,'transition',4,3,'[Ar] 3d¹ 4s²','First d-block element. Used in aerospace alloys.',''],
  [22,'Ti','Titanium',47.867,'transition',4,4,'[Ar] 3d² 4s²','Lightweight, strong metal. TiO₂ used as white pigment.',''],
  [23,'V','Vanadium',50.942,'transition',4,5,'[Ar] 3d³ 4s²','V₂O₅ catalyst in contact process (SO₂ → SO₃).',''],
  [24,'Cr','Chromium',51.996,'transition',4,6,'[Ar] 3d⁵ 4s¹','Electronic config exception: 3d⁵4s¹ not 3d⁴4s². CrO₄²⁻/Cr₂O₇²⁻.','Half-filled 3d⁵ stability causes configuration exception. Shows +2,+3,+6 OS.'],
  [25,'Mn','Manganese',54.938,'transition',4,7,'[Ar] 3d⁵ 4s²','KMnO₄ strong oxidiser. Shows OS from +2 to +7.','Maximum OS +7 (KMnO₄). Mn²⁺ (pale pink) is most stable ion.'],
  [26,'Fe','Iron',55.845,'transition',4,8,'[Ar] 3d⁶ 4s²','Most important structural metal. Fe³⁺ more stable in acid; Fe²⁺ in neutral.','4s ionises before 3d: Fe²⁺=[Ar]3d⁶, Fe³⁺=[Ar]3d⁵.'],
  [27,'Co','Cobalt',58.933,'transition',4,9,'[Ar] 3d⁷ 4s²','Vitamin B12 contains Co. Used in high-strength alloys.',''],
  [28,'Ni','Nickel',58.693,'transition',4,10,'[Ar] 3d⁸ 4s²','Ni catalyst in hydrogenation of oils. Nickel-metal hydride batteries.',''],
  [29,'Cu','Copper',63.546,'transition',4,11,'[Ar] 3d¹⁰ 4s¹','Config exception: 3d¹⁰4s¹. Cu²⁺ more stable than Cu⁺ in aqueous solution.','Fully-filled 3d¹⁰ stability. Cu⁺ disproportionates in water: 2Cu⁺ → Cu + Cu²⁺.'],
  [30,'Zn','Zinc',65.38,'transition',4,12,'[Ar] 3d¹⁰ 4s²','NOT a true transition metal (d¹⁰ in all states). Galvanising iron.','Zn is sometimes excluded from transition metals (no incomplete d in any ion).'],
  [31,'Ga','Gallium',69.723,'post-transition',4,13,'[Ar] 3d¹⁰ 4s² 4p¹','Melts in hand (MP=29.8°C). Used in semiconductors.','Smaller than expected due to poor 3d¹⁰ shielding. IE₁(Ga) > IE₁(Al) anomaly.'],
  [32,'Ge','Germanium',72.630,'metalloid',4,14,'[Ar] 3d¹⁰ 4s² 4p²','Predicted by Mendeleev as eka-silicon. Semiconductor.','Mendeleev\'s prediction of Ge properties was remarkably accurate.'],
  [33,'As','Arsenic',74.922,'metalloid',4,15,'[Ar] 3d¹⁰ 4s² 4p³','Toxic metalloid. Used in alloys and semiconductors.',''],
  [34,'Se','Selenium',78.971,'nonmetal',4,16,'[Ar] 3d¹⁰ 4s² 4p⁴','Photoconductor used in xerography. EA(Se) < EA(S).',''],
  [35,'Br','Bromine',79.904,'halogen',4,17,'[Ar] 3d¹⁰ 4s² 4p⁵','Only liquid non-metal at room temperature. Strong oxidiser.','One of only two elements liquid at room temperature (other: Hg).'],
  [36,'Kr','Krypton',83.798,'noble',4,18,'[Ar] 3d¹⁰ 4s² 4p⁶','Noble gas; KrF₂ is one of few Kr compounds.',''],
  [37,'Rb','Rubidium',85.468,'alkali',5,1,'[Kr] 5s¹','Reacts explosively with water. Reddish-violet flame test.',''],
  [38,'Sr','Strontium',87.62,'alkaline',5,2,'[Kr] 5s²','Crimson red flame test. Sr-90 is dangerous nuclear waste.',''],
  [39,'Y','Yttrium',88.906,'transition',5,3,'[Kr] 4d¹ 5s²','Used in YBa₂Cu₃O₇ high-temperature superconductor.',''],
  [40,'Zr','Zirconium',91.224,'transition',5,4,'[Kr] 4d² 5s²','Zr ≈ Hf in size due to lanthanide contraction. Nuclear reactor cladding.','Zr and Hf have nearly identical radii (lanthanide contraction effect).'],
  [41,'Nb','Niobium',92.906,'transition',5,5,'[Kr] 4d⁴ 5s¹','Config: 4d⁴5s¹ (not 4d³5s²). Superconducting alloys.','Another configuration exception similar to Cr/Cu pattern.'],
  [42,'Mo','Molybdenum',95.96,'transition',5,6,'[Kr] 4d⁵ 5s¹','Config exception like Cr: 4d⁵5s¹. Essential trace element.','Half-filled 4d⁵ stability. Mo is essential in nitrogen fixation enzymes.'],
  [43,'Tc','Technetium',98,'transition',5,7,'[Kr] 4d⁵ 5s²','First artificial element. No stable isotopes (all radioactive).','Only element in period 4/5/6 with no stable isotopes.'],
  [44,'Ru','Ruthenium',101.07,'transition',5,8,'[Kr] 4d⁷ 5s¹','Shows +8 OS in RuO₄ (highest possible OS). PGM.','RuO₄ is one of very few compounds showing +8 OS.'],
  [45,'Rh','Rhodium',102.906,'transition',5,9,'[Kr] 4d⁸ 5s¹','Platinum group metal. Catalytic converters.',''],
  [46,'Pd','Palladium',106.42,'transition',5,10,'[Kr] 4d¹⁰ 5s⁰','Unique config: 4d¹⁰ 5s⁰. Only element with completely empty valence s.','Only element where d¹⁰ s⁰ is ground state — both half-filled and full d preferred over s.'],
  [47,'Ag','Silver',107.868,'transition',5,11,'[Kr] 4d¹⁰ 5s¹','Config exception like Cu: 4d¹⁰5s¹. Best electrical conductor.','Fully-filled 4d¹⁰ stability. Highest electrical conductivity of all metals.'],
  [48,'Cd','Cadmium',112.414,'transition',5,12,'[Kr] 4d¹⁰ 5s²','Cd²⁺ is toxic; used in Ni-Cd batteries. Like Zn, not true transition metal.',''],
  [49,'In','Indium',114.818,'post-transition',5,13,'[Kr] 4d¹⁰ 5s² 5p¹','Used in ITO (Indium Tin Oxide) for displays. Soft metal.',''],
  [50,'Sn','Tin',118.710,'post-transition',5,14,'[Kr] 4d¹⁰ 5s² 5p²','Sn²⁺ (stannous) and Sn⁴⁺ (stannic). Tin cans, solder.','Sn has 10 stable isotopes — most of any element.'],
  [51,'Sb','Antimony',121.760,'metalloid',5,15,'[Kr] 4d¹⁰ 5s² 5p³','Metalloid; used in flame retardants. Sb₂O₃ amphoteric.',''],
  [52,'Te','Tellurium',127.60,'metalloid',5,16,'[Kr] 4d¹⁰ 5s² 5p⁴','Atomic mass > I (Mendeleev arranged by properties not mass).','Te has higher atomic mass than I but placed before I in the table (properties).'],
  [53,'I','Iodine',126.904,'halogen',5,17,'[Kr] 4d¹⁰ 5s² 5p⁵','Antiseptic. I₂ shows sublimation. Thyroid hormone contains I.','Atomic mass < Te but placed after Te (property-based arrangement).'],
  [54,'Xe','Xenon',131.293,'noble',5,18,'[Kr] 4d¹⁰ 5s² 5p⁶','Forms noble gas compounds: XeF₂, XeF₄, XeO₃. First noble compound.','First noble gas compound ever synthesised (1962 by Neil Bartlett).'],
  [55,'Cs','Caesium',132.905,'alkali',6,1,'[Xe] 6s¹','Lowest IE of all stable elements. MP=28.5°C. Atomic clocks.','Most electropositive stable element. Reacts explosively with water.'],
  [56,'Ba','Barium',137.327,'alkaline',6,2,'[Xe] 6s²','Green flame test. BaSO₄ insoluble (X-ray contrast agent).',''],
  [57,'La','Lanthanum',138.905,'lanthanide',6,3,'[Xe] 5d¹ 6s²','First lanthanide. Used in camera lenses and catalysts.',''],
  [58,'Ce','Cerium',140.116,'lanthanide',6,3,'[Xe] 4f¹ 5d¹ 6s²','Most abundant lanthanide. Used in catalytic converters.',''],
  [59,'Pr','Praseodymium',140.908,'lanthanide',6,3,'[Xe] 4f³ 6s²','Used in green glass and goggles. Neodymium magnets.',''],
  [60,'Nd','Neodymium',144.242,'lanthanide',6,3,'[Xe] 4f⁴ 6s²','Nd₂Fe₁₄B — strongest permanent magnets.',''],
  [61,'Pm','Promethium',145,'lanthanide',6,3,'[Xe] 4f⁵ 6s²','Only lanthanide with no stable isotopes (radioactive).',''],
  [62,'Sm','Samarium',150.36,'lanthanide',6,3,'[Xe] 4f⁶ 6s²','SmCo₅ permanent magnets. Sm-153 cancer treatment.',''],
  [63,'Eu','Europium',151.964,'lanthanide',6,3,'[Xe] 4f⁷ 6s²','Half-filled 4f⁷ stability. Used in phosphors (TV screens).','4f⁷ half-filled subshell — extra stable (like Cr 3d⁵).'],
  [64,'Gd','Gadolinium',157.25,'lanthanide',6,3,'[Xe] 4f⁷ 5d¹ 6s²','4f⁷ half-filled stability. MRI contrast agent.','4f⁷5d¹ instead of 4f⁸ — half-filled f stability.'],
  [65,'Tb','Terbium',158.925,'lanthanide',6,3,'[Xe] 4f⁹ 6s²','Used in solid-state devices and green phosphors.',''],
  [66,'Dy','Dysprosium',162.500,'lanthanide',6,3,'[Xe] 4f¹⁰ 6s²','Used in high-power magnets and nuclear reactors.',''],
  [67,'Ho','Holmium',164.930,'lanthanide',6,3,'[Xe] 4f¹¹ 6s²','Highest magnetic moment of any element.',''],
  [68,'Er','Erbium',167.259,'lanthanide',6,3,'[Xe] 4f¹² 6s²','Used in fibre-optic cables (Er-doped amplifiers).',''],
  [69,'Tm','Thulium',168.934,'lanthanide',6,3,'[Xe] 4f¹³ 6s²','Rarest stable lanthanide. Portable X-ray sources.',''],
  [70,'Yb','Ytterbium',173.045,'lanthanide',6,3,'[Xe] 4f¹⁴ 6s²','Fully-filled 4f¹⁴. Used in atomic clocks.',''],
  [71,'Lu','Lutetium',174.967,'lanthanide',6,3,'[Xe] 4f¹⁴ 5d¹ 6s²','Last lanthanide. Used in PET scan detectors.',''],
  [72,'Hf','Hafnium',178.49,'transition',6,4,'[Xe] 4f¹⁴ 5d² 6s²','Zr ≈ Hf radius (lanthanide contraction). Nuclear control rods.','Inseparable from Zr until 1923 (identical properties due to lanthanide contraction).'],
  [73,'Ta','Tantalum',180.948,'transition',6,5,'[Xe] 4f¹⁴ 5d³ 6s²','Highly corrosion-resistant. Used in capacitors (mobile phones).',''],
  [74,'W','Tungsten',183.84,'transition',6,6,'[Xe] 4f¹⁴ 5d⁴ 6s²','Highest MP of all metals (3422°C). Used in incandescent bulbs.','Highest melting point of any metal. 6 unpaired electrons → strongest metallic bonding.'],
  [75,'Re','Rhenium',186.207,'transition',6,7,'[Xe] 4f¹⁴ 5d⁵ 6s²','Second highest MP (3186°C). Used in jet engine superalloys.',''],
  [76,'Os','Osmium',190.23,'transition',6,8,'[Xe] 4f¹⁴ 5d⁶ 6s²','Densest element (22.59 g/cm³). Shows +8 OS in OsO₄.','Densest naturally occurring element. OsO₄ shows maximum +8 OS.'],
  [77,'Ir','Iridium',192.217,'transition',6,9,'[Xe] 4f¹⁴ 5d⁷ 6s²','Second densest element. Most corrosion-resistant metal.',''],
  [78,'Pt','Platinum',195.084,'transition',6,10,'[Xe] 4f¹⁴ 5d⁹ 6s¹','Config: 5d⁹6s¹. Catalyst in catalytic converters and jewellery.','Another d-s configuration exception.'],
  [79,'Au','Gold',196.967,'transition',6,11,'[Xe] 4f¹⁴ 5d¹⁰ 6s¹','Config: 5d¹⁰6s¹ (like Cu/Ag). Noblest metal; aqua regia dissolves it.','Relativistic effects cause 6s contraction → anomalous colour (yellow) and nobility.'],
  [80,'Hg','Mercury',200.592,'transition',6,12,'[Xe] 4f¹⁴ 5d¹⁰ 6s²','Only liquid metal at RT (MP=−38.8°C). Hg₂²⁺ mercury(I) ion is unique.','Weak metallic bonding due to filled d¹⁰; relativistic effects. Hg₂²⁺ is unusual metal-metal bond.'],
  [81,'Tl','Thallium',204.38,'post-transition',6,13,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p¹','Inert pair effect: Tl⁺ more stable than Tl³⁺. Toxic.','Inert pair effect (6s² reluctant to participate) → Tl⁺ preferred over Tl³⁺.'],
  [82,'Pb','Lead',207.2,'post-transition',6,14,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p²','Inert pair: Pb²⁺ more stable than Pb⁴⁺. PbO₂ is oxidising agent.','Pb²⁺ > Pb⁴⁺ stability (inert pair). End product of most radioactive decay series.'],
  [83,'Bi','Bismuth',208.980,'post-transition',6,15,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p³','Inert pair: Bi³⁺ preferred. Most naturally diamagnetic element.','Bi has longest half-life of any radioactive element (Bi-209).'],
  [84,'Po','Polonium',209,'metalloid',6,16,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p⁴','Radioactive metalloid. Discovered by Marie Curie.',''],
  [85,'At','Astatine',210,'halogen',6,17,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p⁵','Rarest naturally occurring element on Earth. Radioactive halogen.',''],
  [86,'Rn','Radon',222,'noble',6,18,'[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p⁶','Radioactive noble gas; second leading cause of lung cancer.',''],
  [87,'Fr','Francium',223,'alkali',7,1,'[Rn] 7s¹','Most unstable naturally occurring element. Most electropositive.','Half-life only 22 minutes. Estimated <30g on Earth at any time.'],
  [88,'Ra','Radium',226,'alkaline',7,2,'[Rn] 7s²','Radioactive; historically used in glow-in-dark paint (dangerous).',''],
  [89,'Ac','Actinium',227,'actinide',7,3,'[Rn] 6d¹ 7s²','First actinide. Intense radioactivity.',''],
  [90,'Th','Thorium',232.038,'actinide',7,3,'[Rn] 6d² 7s²','Nuclear fuel potential. Th-232 fertile material.',''],
  [91,'Pa','Protactinium',231.036,'actinide',7,3,'[Rn] 5f² 6d¹ 7s²','Rare and toxic actinide.',''],
  [92,'U','Uranium',238.029,'actinide',7,3,'[Rn] 5f³ 6d¹ 7s²','Nuclear fuel (U-235 fissile). U-238 most abundant isotope.','U-235 is fissile; U-238 is fertile (converts to Pu-239 in reactor).'],
  [93,'Np','Neptunium',237,'actinide',7,3,'[Rn] 5f⁴ 6d¹ 7s²','First transuranium element.',''],
  [94,'Pu','Plutonium',244,'actinide',7,3,'[Rn] 5f⁶ 7s²','Nuclear weapon/reactor fuel. Pu-239 most important isotope.',''],
  [95,'Am','Americium',243,'actinide',7,3,'[Rn] 5f⁷ 7s²','Smoke detectors (Am-241). Half-filled 5f⁷ stability.','Half-filled 5f⁷ stability (analogous to Eu).'],
  [96,'Cm','Curium',247,'actinide',7,3,'[Rn] 5f⁷ 6d¹ 7s²','Named for Marie and Pierre Curie. Intense radioactivity.',''],
  [97,'Bk','Berkelium',247,'actinide',7,3,'[Rn] 5f⁹ 7s²','Synthesised at UC Berkeley. Very radioactive.',''],
  [98,'Cf','Californium',251,'actinide',7,3,'[Rn] 5f¹⁰ 7s²','Strong neutron emitter; used in nuclear reactors startup.',''],
  [99,'Es','Einsteinium',252,'actinide',7,3,'[Rn] 5f¹¹ 7s²','Named after Einstein. Only microgram quantities exist.',''],
  [100,'Fm','Fermium',257,'actinide',7,3,'[Rn] 5f¹² 7s²','Named after Fermi. Produced in nuclear explosions.',''],
  [101,'Md','Mendelevium',258,'actinide',7,3,'[Rn] 5f¹³ 7s²','Named after Mendeleev.',''],
  [102,'No','Nobelium',259,'actinide',7,3,'[Rn] 5f¹⁴ 7s²','Fully-filled 5f¹⁴. Named after Nobel.',''],
  [103,'Lr','Lawrencium',266,'actinide',7,3,'[Rn] 5f¹⁴ 7s² 7p¹','Named after Lawrence (cyclotron inventor).',''],
  [104,'Rf','Rutherfordium',267,'transition',7,4,'[Rn] 5f¹⁴ 6d² 7s²','First superheavy element. Named after Rutherford.',''],
  [105,'Db','Dubnium',268,'transition',7,5,'[Rn] 5f¹⁴ 6d³ 7s²','Named after Dubna, Russia.',''],
  [106,'Sg','Seaborgium',269,'transition',7,6,'[Rn] 5f¹⁴ 6d⁴ 7s²','Named after Glenn Seaborg.',''],
  [107,'Bh','Bohrium',270,'transition',7,7,'[Rn] 5f¹⁴ 6d⁵ 7s²','Named after Niels Bohr.',''],
  [108,'Hs','Hassium',277,'transition',7,8,'[Rn] 5f¹⁴ 6d⁶ 7s²','Named after Hesse, Germany.',''],
  [109,'Mt','Meitnerium',278,'transition',7,9,'[Rn] 5f¹⁴ 6d⁷ 7s²','Named after Lise Meitner.',''],
  [110,'Ds','Darmstadtium',281,'transition',7,10,'[Rn] 5f¹⁴ 6d⁸ 7s²','Named after Darmstadt, Germany.',''],
  [111,'Rg','Roentgenium',282,'transition',7,11,'[Rn] 5f¹⁴ 6d¹⁰ 7s¹','Named after Wilhelm Röntgen.',''],
  [112,'Cn','Copernicium',285,'transition',7,12,'[Rn] 5f¹⁴ 6d¹⁰ 7s²','Named after Copernicus.',''],
  [113,'Nh','Nihonium',286,'post-transition',7,13,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p¹','Named after Japan (Nihon). First element discovered in Asia.',''],
  [114,'Fl','Flerovium',289,'post-transition',7,14,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p²','Named after Flerov Laboratory of Nuclear Reactions.',''],
  [115,'Mc','Moscovium',290,'post-transition',7,15,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p³','Named after Moscow Oblast.',''],
  [116,'Lv','Livermorium',293,'post-transition',7,16,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p⁴','Named after Lawrence Livermore National Laboratory.',''],
  [117,'Ts','Tennessine',294,'halogen',7,17,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p⁵','Named after Tennessee state.',''],
  [118,'Og','Oganesson',294,'noble',7,18,'[Rn] 5f¹⁴ 6d¹⁰ 7s² 7p⁶','Heaviest known element. Named after Yuri Oganessian.','May be a solid at room temperature unlike other noble gases (theoretical).']
];

// Grid positions: [period, group] for each element (some elements span f-block)
// Period 6 f-block (lanthanides) at row 8, period 7 f-block (actinides) at row 9
function ptGetGridPos(z, period, group, cat) {
  if(cat === 'lanthanide') return [8, z - 57 + 3]; // row 8, cols 3-17
  if(cat === 'actinide')   return [9, z - 89 + 3]; // row 9, cols 3-17
  return [period, group];
}

// Build the periodic table grid
function ptBuildGrid() {
  const grid = document.getElementById('pt-grid');
  if(!grid) return;
  // Set up 10-row grid (periods 1-7, gap row, lanthanides, actinides)
  grid.style.gridTemplateRows = 'repeat(10,1fr)';
  // Map to hold cells
  const cells = {}; // "row-col" => element
  PT_ELEMENTS.forEach(el => {
    const [z,sym,name,mass,cat,period,group,conf,jee,exc] = el;
    const [row, col] = ptGetGridPos(z, period, group, cat);
    cells[`${row}-${col}`] = el;
  });

  // Clear and rebuild
  grid.innerHTML = '';
  // Period label + rows 1-7
  const ROWS = 10;
  const COLS = 18;
  // We'll do a flat approach: place elements, gaps as empty divs
  // Build a 10x18 matrix
  const mat = Array.from({length:ROWS+1}, ()=>Array(COLS+1).fill(null));
  PT_ELEMENTS.forEach(el => {
    const [z,sym,name,mass,cat,period,group,conf,jee,exc] = el;
    let row, col;
    if(cat==='lanthanide') { row=8; col=z-57+3; }
    else if(cat==='actinide') { row=9; col=z-89+3; }
    else { row=period; col=group; }
    mat[row][col] = el;
  });

  // Render: rows 1..9 (skip row 8-9 gap manually handled below)
  for(let r=1;r<=9;r++) {
    for(let c=1;c<=18;c++) {
      const el = mat[r][c];
      if(r===8 && c===1) {
        // Lanthanide label cell (span conceptually)
        const div = document.createElement('div');
        div.style.cssText='display:flex;align-items:center;justify-content:flex-end;padding-right:4px;';
        div.innerHTML='<span style="font-size:.42rem;color:#f06060;letter-spacing:.06em;writing-mode:vertical-rl;transform:rotate(180deg)">Ln</span>';
        grid.appendChild(div);
      } else if(r===9 && c===1) {
        const div = document.createElement('div');
        div.style.cssText='display:flex;align-items:center;justify-content:flex-end;padding-right:4px;';
        div.innerHTML='<span style="font-size:.42rem;color:#d060e0;letter-spacing:.06em;writing-mode:vertical-rl;transform:rotate(180deg)">An</span>';
        grid.appendChild(div);
      } else if(r>=8 && c===2) {
        const div = document.createElement('div');
        grid.appendChild(div);
      } else if(el) {
        const cell = ptMakeCell(el);
        grid.appendChild(cell);
      } else {
        const gap = document.createElement('div');
        // Add asterisk placeholder in period 6/7, col 3 to indicate f-block
        if((r===6||r===7) && c===3) {
          gap.style.cssText='display:flex;align-items:center;justify-content:center;font-size:.45rem;color:#404e66;border:1px dashed #1e2535;border-radius:3px;';
          gap.textContent = r===6?'57-71':'89-103';
        }
        grid.appendChild(gap);
      }
    }
  }
  // Add reveal animation
  requestAnimationFrame(()=>{
    grid.querySelectorAll('.el').forEach((el,i)=>{
      el.style.opacity='0';
      el.style.animation=`ptRowReveal .22s ${Math.min(i*0.003,0.4)}s both`;
    });
  });
}

function ptMakeCell(elData) {
  const [z,sym,name,mass,cat,period,group,conf,jee,exc] = elData;
  const div = document.createElement('div');
  div.className = `el ec-${cat}`;
  div.style.setProperty('--ec', PT_CAT_COLOR[cat]||'#50e890');
  div.dataset.z = z;
  div.dataset.cat = cat;
  div.innerHTML = `
    <div class="el-num">${z}</div>
    <div class="el-sym">${sym}</div>
    <div class="el-name">${name}</div>
    <div class="el-mass">${typeof mass==='number'?mass.toFixed(mass<10?3:mass<100?3:2):mass}</div>
  `;
  div.addEventListener('click', ()=>ptOpenModal(elData));
  div.addEventListener('mouseenter', ()=>{
    div.classList.add('pop');
    setTimeout(()=>div.classList.remove('pop'),350);
    // Haptic feedback on mobile
    if(navigator.vibrate) navigator.vibrate(8);
  });
  return div;
}

function ptOpenModal(elData) {
  const [z,sym,name,mass,cat,period,group,conf,jee,exc] = elData;
  if(navigator.vibrate) navigator.vibrate([12,6,12]);
  const color = PT_CAT_COLOR[cat]||'#50e890';
  document.getElementById('pt-modal-symbol').textContent = sym;
  document.getElementById('pt-modal-symbol').style.color = color;
  document.getElementById('pt-modal-name').textContent = name;
  document.getElementById('pt-modal-sub').textContent = `Z=${z} · Period ${period} · Group ${group} · ${cat.replace(/-/g,' ').replace(/\b\w/g,c=>c.toUpperCase())}`;

  const props = [
    ['Atomic Number', z],
    ['Symbol', sym],
    ['Atomic Mass', typeof mass==='number'?mass.toFixed(3)+' u':mass],
    ['Category', cat.replace(/-/g,' ').replace(/\b\w/g,c=>c.toUpperCase())],
    ['Period', period],
    ['Group', group],
  ];

  let html = `<div class="pt-prop-grid">` +
    props.map(([l,v])=>`<div class="pt-prop"><div class="pt-prop-lbl">${l}</div><div class="pt-prop-val">${v}</div></div>`).join('') +
    `</div>`;

  html += `<div class="pt-conf-block"><div class="pt-conf-lbl">Electronic Configuration</div><div class="pt-conf-val">${conf}</div></div>`;

  if(jee) {
    html += `<div class="pt-jee-block"><div class="pt-jee-lbl">⚗ JEE Relevance</div><div class="pt-jee-val">${jee}</div></div>`;
  }
  if(exc) {
    html += `<div class="pt-exc-block"><div class="pt-exc-lbl">⚠ Exception / Anomaly</div><div class="pt-exc-val">${exc}</div></div>`;
  }

  document.getElementById('pt-modal-body').innerHTML = html;
  const overlay = document.getElementById('pt-modal-overlay');
  overlay.classList.add('show');
  document.getElementById('pt-modal').style.animation = 'ptModalIn .32s cubic-bezier(.16,1,.3,1)';
}

function ptCloseModal() {
  const overlay = document.getElementById('pt-modal-overlay');
  overlay.classList.remove('show');
  if(navigator.vibrate) navigator.vibrate(6);
}

document.getElementById('pt-modal-overlay').addEventListener('click', e=>{
  if(e.target === document.getElementById('pt-modal-overlay')) ptCloseModal();
});
document.addEventListener('keydown', e=>{ if(e.key==='Escape') ptCloseModal(); });

// ── FILTER ──
let _ptActiveFilter = 'all';
function ptFilter(cat, btn) {
  _ptActiveFilter = cat;
  if(navigator.vibrate) navigator.vibrate(10);
  btn.classList.add('pulse');
  setTimeout(()=>btn.classList.remove('pulse'), 250);
  document.querySelectorAll('.pt-fbtn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  document.querySelectorAll('.el').forEach(el => {
    if(cat==='all') { el.classList.remove('dim','highlight'); }
    else if(el.dataset.cat === cat) { el.classList.remove('dim'); el.classList.add('highlight'); }
    else { el.classList.add('dim'); el.classList.remove('highlight'); }
  });
}

// ── SEARCH ──
function ptSearch(q) {
  q = q.trim().toLowerCase();
  if(!q) {
    document.querySelectorAll('.el').forEach(el=>{ el.classList.remove('dim','highlight'); });
    return;
  }
  PT_ELEMENTS.forEach(elData => {
    const [z,sym,name] = elData;
    const cell = document.querySelector(`.el[data-z="${z}"]`);
    if(!cell) return;
    const match = name.toLowerCase().includes(q) || sym.toLowerCase().includes(q) || String(z)===q;
    if(match) { cell.classList.remove('dim'); cell.classList.add('highlight'); }
    else { cell.classList.add('dim'); cell.classList.remove('highlight'); }
  });
}

// ── SUB-TABS ──
function ptShowTab(tab) {
  ['table','trends','exceptions','config'].forEach(t=>{
    const el = document.getElementById('pttab-'+t);
    const btn = document.getElementById('pstab-'+t);
    if(el) el.style.display = t===tab ? 'block' : 'none';
    if(btn) btn.classList.toggle('active', t===tab);
  });
  if(navigator.vibrate) navigator.vibrate(8);
}

// ── BUILD ON SECTION SHOW ── (handled by unified showSection patch)
</script>

<!-- ════════════════════════════════════════════════════
     ROTATIONAL DYNAMICS SECTION
════════════════════════════════════════════════════ -->
<style>
/* ── ROTDYN GLOBAL STYLES ── */
.rd-wrap { font-family: 'EB Garamond', serif; }
.rd-wrap .rd-sec { padding: 44px 0; border-top: 1px solid rgba(255,107,53,.12); }
.rd-wrap .rd-sec:first-child { border-top: none; }
.rd-sh { display: flex; align-items: baseline; gap: 14px; margin-bottom: 32px; }
.rd-sn { font-family: 'JetBrains Mono', monospace; font-size: 10px; color: #ff6b35; letter-spacing: 2px; opacity: .75; }
.rd-wrap h2 { font-family: 'Syne', sans-serif; font-size: 1.85rem; font-weight: 700; color: #fff; letter-spacing: -.4px; }
.rd-wrap h3 { font-family: 'Syne', sans-serif; font-size: 1.12rem; color: #ff6b35; margin: 24px 0 12px; padding-bottom: 6px; border-bottom: 1px solid rgba(255,107,53,.14); }
.rd-wrap h4 { font-family: 'JetBrains Mono', monospace; font-size: .75rem; letter-spacing: 1.5px; text-transform: uppercase; color: #40d0c0; margin: 16px 0 8px; }

/* formula grid */
.rd-fg { display: grid; grid-template-columns: repeat(auto-fill, minmax(270px, 1fr)); gap: 2px; background: rgba(255,107,53,.06); border: 1px solid rgba(255,107,53,.13); border-radius: 7px; overflow: hidden; margin: 12px 0; }
.rd-fb { background: #050710; padding: 14px 16px 12px; cursor: default; transition: background .18s, transform .14s; border-left: 2px solid transparent; position: relative; }
.rd-fb:hover { background: #0d1020; transform: translateX(3px); border-left-color: #ff6b35; }
.rd-fl { font-family: 'JetBrains Mono', monospace; font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: #8090a8; margin-bottom: 6px; display: flex; justify-content: space-between; }
.rd-fm { font-family: 'JetBrains Mono', monospace; font-size: .88rem; color: #fff; line-height: 1.7; }
.rd-fm .rv  { color: #ff6b35; }
.rd-fm .rb2 { color: #40d0c0; }
.rd-fm .rg  { color: #50d890; }
.rd-fm .rp  { color: #a080f0; }
.rd-fm .re  { color: #8090a8; }

/* trick / property box */
.rd-trick { background: rgba(255,107,53,.05); border: 1px solid rgba(255,107,53,.22); border-radius: 6px; padding: 14px 16px; margin: 12px 0; }
.rd-trick-hdr { font-family: 'JetBrains Mono', monospace; font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: #ff6b35; margin-bottom: 8px; }
.rd-trick-body { font-family: 'Crimson Pro', serif; font-size: .95rem; color: #c0ccd8; line-height: 1.85; }
.rd-trick-body b { color: #ff6b35; }
.rd-trick-body code { font-family: 'JetBrains Mono', monospace; font-size: .82rem; background: rgba(255,255,255,.06); padding: 1px 6px; border-radius: 3px; color: #40d0c0; }

/* misc pattern box */
.rd-pattern { background: rgba(160,128,240,.05); border: 1px solid rgba(160,128,240,.2); border-radius: 6px; padding: 14px 16px; margin: 10px 0; }
.rd-pattern-hdr { font-family: 'JetBrains Mono', monospace; font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: #a080f0; margin-bottom: 8px; display: flex; align-items: center; gap: 6px; }
.rd-pattern-body { font-family: 'JetBrains Mono', monospace; font-size: .82rem; color: #c0ccd8; line-height: 1.9; }
.rd-pattern-body .hl { color: #f5c842; }
.rd-pattern-body .rd-hi { color: #50d890; }

/* note box */
.rd-note { background: rgba(80,216,144,.05); border-left: 3px solid #50d890; padding: 10px 14px; margin: 10px 0; border-radius: 0 5px 5px 0; font-family: 'JetBrains Mono', monospace; font-size: .8rem; color: #50d890; line-height: 1.8; }
.rd-note::before { content: '💡  '; }

/* warn box */
.rd-warn { background: rgba(240,96,128,.05); border-left: 3px solid #f06080; padding: 10px 14px; margin: 10px 0; border-radius: 0 5px 5px 0; font-family: 'JetBrains Mono', monospace; font-size: .8rem; color: #f06080; line-height: 1.8; }
.rd-warn::before { content: '⚠  '; }

/* canvas diagram */
.rd-canvas-wrap { background: #060810; border: 1px solid rgba(255,107,53,.15); border-radius: 8px; overflow: hidden; margin: 16px 0; }
.rd-canvas-title { font-family: 'JetBrains Mono', monospace; font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: #8090a8; padding: 8px 14px; border-bottom: 1px solid rgba(255,107,53,.1); }
.rd-canvas-wrap canvas { display: block; width: 100%; height: auto; }

/* MOI table */
.rd-moi-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(200px,1fr)); gap: 10px; margin: 14px 0; }
.rd-moi-card { background: #070a14; border: 1px solid rgba(255,107,53,.14); border-radius: 8px; padding: 14px; text-align: center; transition: border-color .2s, transform .18s; cursor: default; }
.rd-moi-card:hover { border-color: #ff6b35; transform: translateY(-3px); }
.rd-moi-shape { font-size: 2rem; margin-bottom: 6px; }
.rd-moi-name { font-family: 'JetBrains Mono', monospace; font-size: .65rem; letter-spacing: 1px; text-transform: uppercase; color: #8090a8; margin-bottom: 8px; }
.rd-moi-formula { font-family: 'JetBrains Mono', monospace; font-size: .88rem; color: #ff6b35; margin-bottom: 4px; }
.rd-moi-axis { font-family: 'JetBrains Mono', monospace; font-size: .65rem; color: #40d0c0; }

/* tab navigation inside section */
.rd-tabs { display: flex; gap: 3px; flex-wrap: wrap; margin-bottom: 20px; }
.rd-tab { font-family: 'JetBrains Mono', monospace; font-size: .6rem; letter-spacing: .1em; text-transform: uppercase; color: #404e66; border: 1px solid rgba(255,255,255,.06); padding: 5px 12px; border-radius: 3px; cursor: pointer; background: rgba(255,255,255,.02); transition: all .18s; }
.rd-tab.active { color: #ff6b35; border-color: rgba(255,107,53,.4); background: rgba(255,107,53,.07); }
.rd-tab:hover:not(.active) { color: #8090a8; }

/* fun trick card */
.rd-fun { background: linear-gradient(135deg,rgba(255,107,53,.07) 0%,rgba(160,128,240,.06) 100%); border: 1px solid rgba(255,107,53,.2); border-radius: 10px; padding: 18px 20px; margin: 14px 0; position: relative; overflow: hidden; }
.rd-fun::before { content: ''; position: absolute; top: -20px; right: -20px; width: 80px; height: 80px; border-radius: 50%; background: radial-gradient(circle,rgba(255,107,53,.18),transparent 70%); }
.rd-fun-tag { font-family: 'JetBrains Mono', monospace; font-size: 8px; letter-spacing: 2.5px; text-transform: uppercase; color: #ff6b35; margin-bottom: 8px; }
.rd-fun-title { font-family: 'Syne', sans-serif; font-size: 1rem; font-weight: 700; color: #fff; margin-bottom: 8px; }
.rd-fun-body { font-family: 'Crimson Pro', serif; font-style: italic; font-size: .95rem; color: #c0ccd8; line-height: 1.8; }
.rd-fun-body b { color: #f5c842; font-style: normal; }
.rd-fun-emoji { font-size: 1.6rem; float: right; margin-left: 12px; }

/* question pattern cards */
.rd-qp { display: grid; grid-template-columns: repeat(auto-fill,minmax(300px,1fr)); gap: 10px; margin: 14px 0; }
.rd-qcard { background: #060810; border: 1px solid rgba(160,128,240,.14); border-radius: 8px; padding: 16px; transition: border-color .2s; }
.rd-qcard:hover { border-color: #a080f0; }
.rd-qcard-type { font-family: 'JetBrains Mono', monospace; font-size: 8px; letter-spacing: 2px; text-transform: uppercase; color: #a080f0; margin-bottom: 8px; }
.rd-qcard-q { font-family: 'Crimson Pro', serif; font-size: .95rem; color: #e8e0d0; line-height: 1.75; margin-bottom: 10px; }
.rd-qcard-hint { font-family: 'JetBrains Mono', monospace; font-size: .75rem; color: #50d890; background: rgba(80,216,144,.05); border: 1px solid rgba(80,216,144,.15); padding: 6px 10px; border-radius: 4px; line-height: 1.7; }
.rd-qcard-hint::before { content: '→ '; }

/* misc property row */
.rd-prop-list { display: flex; flex-direction: column; gap: 6px; margin: 12px 0; }
.rd-prop { display: flex; align-items: flex-start; gap: 10px; background: #060810; border: 1px solid rgba(255,255,255,.05); border-radius: 5px; padding: 10px 14px; transition: border-color .18s; }
.rd-prop:hover { border-color: rgba(255,107,53,.3); }
.rd-prop-num { font-family: 'JetBrains Mono', monospace; font-size: .75rem; color: #ff6b35; background: rgba(255,107,53,.12); min-width: 26px; height: 26px; border-radius: 3px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-weight: 700; }
.rd-prop-text { font-family: 'Crimson Pro', serif; font-size: .95rem; color: #c8d0dc; line-height: 1.7; flex: 1; }
.rd-prop-text b { color: #ff6b35; }
.rd-prop-text code { font-family: 'JetBrains Mono', monospace; font-size: .82rem; background: rgba(255,255,255,.06); padding: 1px 5px; border-radius: 3px; color: #40d0c0; }

/* timeline / derivation steps */
.rd-steps { display: flex; flex-direction: column; gap: 8px; margin: 12px 0; }
.rd-step { display: flex; gap: 12px; align-items: flex-start; background: rgba(255,255,255,.02); border-radius: 5px; padding: 10px 14px; border-left: 2px solid transparent; transition: border-color .18s; }
.rd-step:hover { border-left-color: #40d0c0; }
.rd-step-num { font-family: 'JetBrains Mono', monospace; font-size: 9px; color: #40d0c0; background: rgba(64,208,192,.12); min-width: 22px; height: 22px; border-radius: 3px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; margin-top: 1px; font-weight: 700; }
.rd-step-text { font-family: 'Crimson Pro', serif; font-size: .95rem; color: #e0e8f0; line-height: 1.7; }
.rd-step-text .m { font-family: 'JetBrains Mono', monospace; font-size: .82rem; background: rgba(255,255,255,.06); padding: 2px 7px; border-radius: 3px; color: #fff; border: 1px solid rgba(255,255,255,.06); display: inline-block; margin: 1px 2px; }
.rd-step-text .h { color: #50d890; font-family: 'JetBrains Mono', monospace; font-size: .82rem; }
</style>

<div class="psec" id="sec-rotdyn">
<div class="cwrap">

<!-- SECTION HERO BANNER -->
<div class="shero" style="--sc:rgba(255,107,53,.09)">
  <span class="shero-badge">JEE Advanced · Physics · Complete Module</span>
  <h2 style="background:linear-gradient(120deg,#ff6b35,#f5c842,#a080f0);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text">Rotational Dynamics</h2>
  <p>Moment of Inertia · Torque · Angular Momentum · Rolling · JEE patterns · Tricks & Animations</p>
  <div class="snav">
    <a href="#rd1">Kinematics</a>
    <a href="#rd2">Torque & MOI</a>
    <a href="#rd3">Theorems</a>
    <a href="#rd4">Angular Momentum</a>
    <a href="#rd5">Energy</a>
    <a href="#rd6">Rolling</a>
    <a href="#rd7">Rigid Body</a>
    <a href="#rd8">JEE Patterns</a>
    <a href="#rd9">Misc Props</a>
    <a href="#rd10">Tricks</a>
  </div>
</div>

<div class="rd-wrap">

<!-- ══════════════════════════════════════════════════
     ANIMATED DIAGRAMS ROW
══════════════════════════════════════════════════ -->

<div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:16px;margin-bottom:36px;">

  <!-- Rotating Disk Animation -->
  <div class="rd-canvas-wrap">
    <div class="rd-canvas-title">🌀 Angular Velocity · ω = dθ/dt</div>
    <canvas id="rdCanvasDisk" width="280" height="180"></canvas>
  </div>

  <!-- Torque Animation -->
  <div class="rd-canvas-wrap">
    <div class="rd-canvas-title">⚡ Torque · τ = r × F</div>
    <canvas id="rdCanvasTorque" width="280" height="180"></canvas>
  </div>

  <!-- Rolling Motion -->
  <div class="rd-canvas-wrap">
    <div class="rd-canvas-title">⚽ Rolling Without Slipping</div>
    <canvas id="rdCanvasRoll" width="280" height="180"></canvas>
  </div>

</div>

<!-- ═══════════════════════════════════════
     SEC 01: ROTATIONAL KINEMATICS
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd1">
  <div class="rd-sh"><span class="rd-sn">01 —</span><h2>Rotational Kinematics</h2></div>

  <h3>Translational ↔ Rotational Analogy</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Displacement</div><div class="rd-fm"><span class="re">Linear:</span> <span class="rv">x</span> &nbsp;↔&nbsp; <span class="re">Angular:</span> <span class="rb2">θ</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Velocity</div><div class="rd-fm"><span class="re">v</span> &nbsp;↔&nbsp; <span class="rb2">ω = dθ/dt</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Acceleration</div><div class="rd-fm"><span class="re">a</span> &nbsp;↔&nbsp; <span class="rb2">α = dω/dt</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Mass</div><div class="rd-fm"><span class="re">m</span> &nbsp;↔&nbsp; <span class="rv">I (moment of inertia)</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Force</div><div class="rd-fm"><span class="re">F</span> &nbsp;↔&nbsp; <span class="rv">τ (torque)</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Momentum</div><div class="rd-fm"><span class="re">p = mv</span> &nbsp;↔&nbsp; <span class="rv">L = Iω</span></div></div>
    <div class="rd-fb"><div class="rd-fl">KE</div><div class="rd-fm"><span class="re">½mv²</span> &nbsp;↔&nbsp; <span class="rv">½Iω²</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Newton's 2nd</div><div class="rd-fm"><span class="re">F = ma</span> &nbsp;↔&nbsp; <span class="rv">τ = Iα</span></div></div>
  </div>

  <h3>Equations of Rotational Motion (Constant α)</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">1st Equation</div><div class="rd-fm"><span class="rv">ω</span> <span class="re">=</span> <span class="rb2">ω₀</span> <span class="re">+</span> <span class="rg">α</span><span class="re">t</span></div></div>
    <div class="rd-fb"><div class="rd-fl">2nd Equation</div><div class="rd-fm"><span class="rv">θ</span> <span class="re">=</span> <span class="rb2">ω₀</span><span class="re">t</span> <span class="re">+</span> <span class="rg">½αt²</span></div></div>
    <div class="rd-fb"><div class="rd-fl">3rd Equation</div><div class="rd-fm"><span class="rv">ω²</span> <span class="re">=</span> <span class="rb2">ω₀²</span> <span class="re">+</span> <span class="rg">2αθ</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Average ω</div><div class="rd-fm"><span class="rv">θ/t</span> <span class="re">=</span> <span class="rb2">(ω₀ + ω)/2</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Arc Length</div><div class="rd-fm"><span class="rv">s</span> <span class="re">=</span> <span class="rb2">rθ</span> &nbsp;·&nbsp; <span class="rv">v</span> <span class="re">=</span> <span class="rb2">rω</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Centripetal accel</div><div class="rd-fm"><span class="rv">aₓ</span> <span class="re">=</span> <span class="rb2">rω² = v²/r</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Tangential accel</div><div class="rd-fm"><span class="rv">aₜ</span> <span class="re">=</span> <span class="rb2">rα</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Total accel</div><div class="rd-fm"><span class="rv">a</span> <span class="re">=</span> <span class="rb2">√(aₓ² + aₜ²)</span></div></div>
  </div>

  <div class="rd-fun">
    <span class="rd-fun-emoji">🎡</span>
    <div class="rd-fun-tag">🎉 Memory Trick — Analogies</div>
    <div class="rd-fun-title">"Just swap m→I, v→ω, F→τ, p→L !"</div>
    <div class="rd-fun-body">Every linear mechanics formula has a rotational twin. <b>Just replace mass with moment of inertia, velocity with angular velocity, force with torque, and momentum with angular momentum.</b> The math is identical. Once you internalize this symmetry, you basically know both chapters at once! 🤯</div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 02: TORQUE & MOMENT OF INERTIA
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd2">
  <div class="rd-sh"><span class="rd-sn">02 —</span><h2>Torque &amp; Moment of Inertia</h2></div>

  <h3>Torque</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Vector form</div><div class="rd-fm"><span class="rv">τ</span> <span class="re">=</span> <span class="rb2">r × F</span> &nbsp;|τ|<span class="re">=</span><span class="rv">rF sinφ</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Scalar (2D)</div><div class="rd-fm"><span class="rv">τ</span> <span class="re">=</span> <span class="rb2">F × d</span> &nbsp;(d = ⊥ distance)</div></div>
    <div class="rd-fb"><div class="rd-fl">Newton's 2nd (rot)</div><div class="rd-fm"><span class="rv">τ_net</span> <span class="re">=</span> <span class="rb2">Iα</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Direction</div><div class="rd-fm">Right-hand rule: curl fingers r→F; thumb = τ direction</div></div>
    <div class="rd-fb"><div class="rd-fl">Max Torque</div><div class="rd-fm">When <span class="rv">φ = 90°</span> (F ⊥ r) &nbsp;→&nbsp; <span class="rb2">τ = rF</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Zero Torque</div><div class="rd-fm">When φ = 0° or 180° (F ∥ r) &nbsp;→&nbsp; <span class="rb2">τ = 0</span></div></div>
  </div>

  <h3>Moment of Inertia (MOI)</h3>
  <div class="rd-note">MOI = Σmᵢrᵢ² (discrete) or ∫r² dm (continuous) — it's the rotational analogue of mass, representing resistance to angular acceleration.</div>

  <div class="rd-moi-grid">
    <div class="rd-moi-card"><div class="rd-moi-shape">⬤</div><div class="rd-moi-name">Solid Disk / Cylinder</div><div class="rd-moi-formula">I = ½MR²</div><div class="rd-moi-axis">axis: central, ⊥ face</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">⭕</div><div class="rd-moi-name">Thin Ring / Hoop</div><div class="rd-moi-formula">I = MR²</div><div class="rd-moi-axis">axis: central, ⊥ plane</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">🔵</div><div class="rd-moi-name">Solid Sphere</div><div class="rd-moi-formula">I = 2MR²/5</div><div class="rd-moi-axis">axis: diameter</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">🔵</div><div class="rd-moi-name">Hollow Sphere</div><div class="rd-moi-formula">I = 2MR²/3</div><div class="rd-moi-axis">axis: diameter</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">━</div><div class="rd-moi-name">Thin Rod (centre)</div><div class="rd-moi-formula">I = ML²/12</div><div class="rd-moi-axis">axis: ⊥ through centre</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">━</div><div class="rd-moi-name">Thin Rod (end)</div><div class="rd-moi-formula">I = ML²/3</div><div class="rd-moi-axis">axis: ⊥ through end</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">▭</div><div class="rd-moi-name">Rectangular Plate</div><div class="rd-moi-formula">I = M(a²+b²)/12</div><div class="rd-moi-axis">axis: ⊥ through centre</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">📡</div><div class="rd-moi-name">Disk (diameter)</div><div class="rd-moi-formula">I = MR²/4</div><div class="rd-moi-axis">axis: diameter</div></div>
    <div class="rd-moi-card"><div class="rd-moi-shape">🔘</div><div class="rd-moi-name">Hollow Cylinder</div><div class="rd-moi-formula">I = M(R₁²+R₂²)/2</div><div class="rd-moi-axis">axis: central</div></div>
  </div>

  <div class="rd-fun">
    <span class="rd-fun-emoji">🎯</span>
    <div class="rd-fun-tag">🎉 MOI Memory — "2/5, 2/3, 1/2, 1, 1/12, 1/3"</div>
    <div class="rd-fun-title">The Fraction Ladder</div>
    <div class="rd-fun-body">Solid sphere <b>2/5</b> → Hollow sphere <b>2/3</b> → Disk <b>1/2</b> → Ring <b>1</b>. Notice the fractions increase as mass is farther from center! <b>More mass away from axis = harder to rotate = bigger I.</b> Rod: centre <b>1/12</b>, end <b>1/3</b> (end = 4× centre — that's the parallel axis theorem in action!)</div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 03: PARALLEL & PERPENDICULAR AXIS THEOREMS
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd3">
  <div class="rd-sh"><span class="rd-sn">03 —</span><h2>Axis Theorems</h2></div>

  <h3>Parallel Axis Theorem</h3>
  <div class="rd-steps">
    <div class="rd-step"><div class="rd-step-num">①</div><div class="rd-step-text"><span class="m">I = Iₒ + Md²</span> where Iₒ is MOI about COM axis, d = distance between parallel axes.</div></div>
    <div class="rd-step"><div class="rd-step-num">②</div><div class="rd-step-text">The shifted axis is <b>always parallel</b> to the COM axis. You can only add Md², never subtract.</div></div>
    <div class="rd-step"><div class="rd-step-num">③</div><div class="rd-step-text"><span class="h">Key insight:</span> Iₒ is always the <b>minimum</b> MOI for all parallel axes — COM axis minimizes rotational inertia.</div></div>
  </div>
  <div class="rd-note">Rod about end: I = ML²/12 + M(L/2)² = ML²/12 + ML²/4 = ML²/3 ✓ — a classic application!</div>

  <h3>Perpendicular Axis Theorem</h3>
  <div class="rd-steps">
    <div class="rd-step"><div class="rd-step-num">①</div><div class="rd-step-text"><span class="m">Iz = Ix + Iy</span> — <b>only valid for planar (2D) objects</b> (laminas).</div></div>
    <div class="rd-step"><div class="rd-step-num">②</div><div class="rd-step-text">x, y are in-plane axes; z is perpendicular to the lamina through same point.</div></div>
    <div class="rd-step"><div class="rd-step-num">③</div><div class="rd-step-text"><span class="h">Classic:</span> Disk about diameter → I_z = MR²/2, by symmetry Ix = Iy → <span class="m">I_diam = MR²/4</span></div></div>
  </div>
  <div class="rd-warn">Perpendicular axis theorem does NOT apply to 3D objects like solid spheres or cylinders!</div>

  <div class="rd-pattern">
    <div class="rd-pattern-hdr">⚡ JEE TRICK — Combining Theorems</div>
    <div class="rd-pattern-body">
      Ring MOI about tangent = <span class="hl">MR² + MR² = 2MR²</span> (parallel axis, d=R)<br>
      Disk MOI about tangent = <span class="hl">MR²/4 + MR² = 5MR²/4</span> (perp + parallel)<br>
      Disk MOI about edge (⊥ face) = <span class="hl">MR²/2 + MR² = 3MR²/2</span>
    </div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 04: ANGULAR MOMENTUM & CONSERVATION
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd4">
  <div class="rd-sh"><span class="rd-sn">04 —</span><h2>Angular Momentum</h2></div>

  <h3>Definitions & Formulae</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Point mass</div><div class="rd-fm"><span class="rv">L</span> <span class="re">=</span> <span class="rb2">r × p = mvr sinθ</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Rigid body</div><div class="rd-fm"><span class="rv">L</span> <span class="re">=</span> <span class="rb2">Iω</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Newton's 2nd</div><div class="rd-fm"><span class="rv">τ_net</span> <span class="re">=</span> <span class="rb2">dL/dt</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Impulse (angular)</div><div class="rd-fm"><span class="rv">ΔL</span> <span class="re">=</span> <span class="rb2">τ · Δt</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Conservation</div><div class="rd-fm">If <span class="rv">τ_ext = 0</span> → <span class="rb2">L = Iω = constant</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Particle in circle</div><div class="rd-fm"><span class="rv">L</span> <span class="re">=</span> <span class="rb2">mvr</span> (r ⊥ v always)</div></div>
  </div>

  <h3>Conservation of Angular Momentum</h3>
  <div class="rd-steps">
    <div class="rd-step"><div class="rd-step-num">①</div><div class="rd-step-text">When net external torque = 0 → <span class="m">I₁ω₁ = I₂ω₂</span></div></div>
    <div class="rd-step"><div class="rd-step-num">②</div><div class="rd-step-text"><span class="h">Spinning skater:</span> Arms in → I decreases → ω increases (spin faster!) — L conserved.</div></div>
    <div class="rd-step"><div class="rd-step-num">③</div><div class="rd-step-text">Bullet embedding in disk: use angular impulse, not linear momentum for rotational problems!</div></div>
    <div class="rd-step"><div class="rd-step-num">④</div><div class="rd-step-text"><span class="h">Gyroscope precession:</span> τ = dL/dt → L direction changes → precession ω_p = τ/L = Mgr/(Iω)</div></div>
  </div>

  <div class="rd-fun">
    <span class="rd-fun-emoji">🩰</span>
    <div class="rd-fun-tag">🎉 Fun Intuition — The Spinning Skater</div>
    <div class="rd-fun-title">Why does pulling arms in make you spin faster?</div>
    <div class="rd-fun-body">Angular momentum <b>L = Iω</b> is conserved (no external torque on ice). When you pull arms in, I decreases because mass moves closer to the rotation axis. So ω <b>must</b> increase to keep L constant. It's like squeezing a water balloon — push in one dimension, it expands in another! 🎪</div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 05: ROTATIONAL KINETIC ENERGY
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd5">
  <div class="rd-sh"><span class="rd-sn">05 —</span><h2>Rotational Kinetic Energy &amp; Work</h2></div>

  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Rotational KE</div><div class="rd-fm"><span class="rv">KE_rot</span> <span class="re">=</span> <span class="rb2">½Iω²</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Work by torque</div><div class="rd-fm"><span class="rv">W</span> <span class="re">=</span> <span class="rb2">∫τ dθ = τθ</span> (const. τ)</div></div>
    <div class="rd-fb"><div class="rd-fl">Power</div><div class="rd-fm"><span class="rv">P</span> <span class="re">=</span> <span class="rb2">τω</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Work-Energy Theorem</div><div class="rd-fm"><span class="rv">W_net</span> <span class="re">=</span> <span class="rb2">ΔKE_rot = Δ(½Iω²)</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Rolling (total KE)</div><div class="rd-fm"><span class="rv">KE</span> <span class="re">=</span> <span class="rb2">½mv² + ½Iω²</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Rolling KE ratio</div><div class="rd-fm">KE_rot / KE_trans <span class="re">=</span> <span class="rb2">k² / R²</span> (k=rad. of gyration)</div></div>
  </div>

  <div class="rd-note">Radius of gyration k: defined by I = Mk² → k = √(I/M). Think of it as the "effective distance" of mass from axis.</div>

  <h3>Energy Distribution in Rolling</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Solid Sphere</div><div class="rd-fm">KE_rot/KE_total <span class="re">=</span> <span class="rv">2/7</span> &nbsp;·&nbsp; KE_trans = <span class="rg">5/7</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Solid Cylinder</div><div class="rd-fm">KE_rot/KE_total <span class="re">=</span> <span class="rv">1/3</span> &nbsp;·&nbsp; KE_trans = <span class="rg">2/3</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Hollow Sphere</div><div class="rd-fm">KE_rot/KE_total <span class="re">=</span> <span class="rv">2/5</span> &nbsp;·&nbsp; KE_trans = <span class="rg">3/5</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Ring/Hoop</div><div class="rd-fm">KE_rot/KE_total <span class="re">=</span> <span class="rv">1/2</span> &nbsp;·&nbsp; KE_trans = <span class="rg">1/2</span></div></div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 06: ROLLING MOTION
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd6">
  <div class="rd-sh"><span class="rd-sn">06 —</span><h2>Rolling Motion</h2></div>

  <h3>Conditions & Key Relations</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Rolling without slipping</div><div class="rd-fm"><span class="rv">v_cm</span> <span class="re">=</span> <span class="rb2">Rω</span> &nbsp;&amp;&nbsp; <span class="rv">a_cm</span> <span class="re">=</span> <span class="rb2">Rα</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Contact point velocity</div><div class="rd-fm">v_contact <span class="re">=</span> <span class="rv">0</span> (instantaneous rest!)</div></div>
    <div class="rd-fb"><div class="rd-fl">Top point velocity</div><div class="rd-fm">v_top <span class="re">=</span> <span class="rb2">2v_cm</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Acceleration on incline</div><div class="rd-fm"><span class="rv">a</span> <span class="re">=</span> <span class="rb2">g sinθ / (1 + I/MR²)</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Friction (rolling, incline)</div><div class="rd-fm"><span class="rv">f</span> <span class="re">=</span> <span class="rb2">Ma = MgI sinθ/(MR²+I)</span></div></div>
    <div class="rd-fb"><div class="rd-fl">Velocity at bottom</div><div class="rd-fm"><span class="rv">v</span> <span class="re">=</span> <span class="rb2">√(2gh/(1+k²/R²))</span></div></div>
  </div>

  <h3>Race Down the Incline — Who Wins?</h3>
  <div class="rd-fun">
    <span class="rd-fun-emoji">🏁</span>
    <div class="rd-fun-tag">🎉 Classic JEE — Rolling Race!</div>
    <div class="rd-fun-title">Solid Sphere always wins the rolling race!</div>
    <div class="rd-fun-body">
      Acceleration = <b>g sinθ / (1 + k²/R²)</b>. Smaller k²/R² → faster acceleration!<br>
      <b>Solid Sphere: k²/R² = 2/5 → fastest</b><br>
      Solid Cylinder: k²/R² = 1/2 → 2nd<br>
      Hollow Sphere: k²/R² = 2/3 → 3rd<br>
      Ring/Hoop: k²/R² = 1 → slowest 🐢<br>
      (Shape matters, NOT mass or radius — classic trick!)
    </div>
  </div>

  <div class="rd-note">For rolling on incline: friction is STATIC (no slipping), so it does NO work on energy. Energy is conserved using mgh = ½mv² + ½Iω²</div>
</section>

<!-- ═══════════════════════════════════════
     SEC 07: RIGID BODY EQUILIBRIUM
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd7">
  <div class="rd-sh"><span class="rd-sn">07 —</span><h2>Rigid Body Equilibrium &amp; Dynamics</h2></div>

  <h3>Conditions for Equilibrium</h3>
  <div class="rd-fg">
    <div class="rd-fb"><div class="rd-fl">Translational</div><div class="rd-fm"><span class="rv">ΣF</span> <span class="re">=</span> <span class="rb2">0</span> (vector sum)</div></div>
    <div class="rd-fb"><div class="rd-fl">Rotational</div><div class="rd-fm"><span class="rv">Στ</span> <span class="re">=</span> <span class="rb2">0</span> (about ANY point)</div></div>
    <div class="rd-fb"><div class="rd-fl">Couple</div><div class="rd-fm">Two equal, opposite, non-collinear forces → net F=0 but τ ≠ 0</div></div>
    <div class="rd-fb"><div class="rd-fl">Couple moment</div><div class="rd-fm"><span class="rv">τ_couple</span> <span class="re">=</span> <span class="rb2">F × d</span> (same everywhere)</div></div>
    <div class="rd-fb"><div class="rd-fl">COM motion</div><div class="rd-fm">F_net = Ma_cm (even for rotation!)</div></div>
    <div class="rd-fb"><div class="rd-fl">Rotation about COM</div><div class="rd-fm">τ_com = I_com × α (always valid)</div></div>
  </div>

  <h3>Toppling Condition</h3>
  <div class="rd-steps">
    <div class="rd-step"><div class="rd-step-num">①</div><div class="rd-step-text">Object topples when the line of action of weight passes <b>outside</b> the base of support.</div></div>
    <div class="rd-step"><div class="rd-step-num">②</div><div class="rd-step-text">For block on incline: <span class="m">tan θ_topple = b/h</span> (b = base width, h = height to COM)</div></div>
    <div class="rd-step"><div class="rd-step-num">③</div><div class="rd-step-text"><span class="h">Compare:</span> θ_slide (μₛ = tan θ_slide) vs θ_topple. Whichever is smaller happens first!</div></div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 08: JEE MISCELLANEOUS PATTERNS
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd8">
  <div class="rd-sh"><span class="rd-sn">08 —</span><h2>JEE Miscellaneous Question Patterns</h2></div>

  <div class="rd-qp">
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 1 — Bullet + Disk</div>
      <div class="rd-qcard-q">A bullet of mass m, velocity v hits the rim of a disk (mass M, radius R) at rest. It embeds. Find ω.</div>
      <div class="rd-qcard-hint">Use L conservation: mvR = (I_disk + mR²)ω → ω = mvR / (MR²/2 + mR²). L conserved, NOT linear momentum (external forces exist at hinge).</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 2 — Rod + Hinge</div>
      <div class="rd-qcard-q">A uniform rod pivoted at one end is released from horizontal. Find ω at vertical, and hinge reaction.</div>
      <div class="rd-qcard-hint">Energy: MgL/2 = ½(ML²/3)ω² → ω = √(3g/L). Then use F_net = Ma_cm for hinge force. α = 3g/(2L) at horizontal.</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 3 — Spool on Surface</div>
      <div class="rd-qcard-q">A spool with inner radius r, outer radius R pulled by force F at angle θ. Find acceleration and direction of friction.</div>
      <div class="rd-qcard-hint">Torque about contact point = F(R cosθ - r). If +ve, friction is forward (friction assists). Find critical angle where friction = 0: cosθ = r/R.</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 4 — Two Cylinders</div>
      <div class="rd-qcard-q">Cylinder released from rest on rough incline. Find minimum μ for rolling without slipping.</div>
      <div class="rd-qcard-hint">a_cm = g sinθ/(1+I/MR²), f = Ma_cm - Mg sinθ... wait. Set f ≤ μN = μMg cosθ → μ ≥ tanθ/(1 + MR²/I) = tanθ/3 for solid cylinder.</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 5 — Toppling vs Sliding</div>
      <div class="rd-qcard-q">A block of dimensions a×b on rough incline (μ). Find whether it slides or topples first as θ increases.</div>
      <div class="rd-qcard-hint">θ_slide = arctan(μ). θ_topple = arctan(a/2h) where a = base, h = half-height. Compare these angles — smaller one occurs first.</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 6 — COM of Composite</div>
      <div class="rd-qcard-q">MOI of a disk with a circular hole. How to find?</div>
      <div class="rd-qcard-hint">Subtraction principle! I_whole - I_removed_part. Treat hole as negative mass. Use parallel axis theorem for off-center holes. Very common in JEE!</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 7 — Gyroscope / Precession</div>
      <div class="rd-qcard-q">Top of mass M, spin ω, precesses. Find precession angular velocity Ω.</div>
      <div class="rd-qcard-hint">τ = MgR (torque due to gravity). L = Iω. Precession: Ω = τ/L = MgR/(Iω). Direction: torque changes direction of L vector → ΔL = τΔt, so precession ⊥ to both τ and L.</div>
    </div>
    <div class="rd-qcard">
      <div class="rd-qcard-type">🎯 Pattern 8 — String Wrapped</div>
      <div class="rd-qcard-q">String wrapped around cylinder (I), mass m hanging. Find a and T.</div>
      <div class="rd-qcard-hint">For mass: mg - T = ma. For cylinder: TR = Iα = I(a/R) → T = Ia/R². Solve: a = mg/(m + I/R²). Note: T ≠ mg (unlike Atwood without rotation)!</div>
    </div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 09: MISCELLANEOUS PROPERTIES
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd9">
  <div class="rd-sh"><span class="rd-sn">09 —</span><h2>Miscellaneous Properties — Time Savers</h2></div>

  <div class="rd-prop-list">
    <div class="rd-prop"><div class="rd-prop-num">P1</div><div class="rd-prop-text"><b>Torque about contact point</b> for rolling bodies: τ = F × (perpendicular distance from contact) — friction contributes zero torque here (zero moment arm). Greatly simplifies rolling problems!</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P2</div><div class="rd-prop-text"><b>Instantaneous axis of rotation (IAOR)</b>: For rolling, the contact point is the IAOR. Velocity of any point = ω × (distance from IAOR). Top point has v = 2ωR = 2v_cm.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P3</div><div class="rd-prop-text"><b>Pure rolling → static friction does NO work</b>. So use energy conservation freely! But friction still exists as a force and contributes to acceleration equations.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P4</div><div class="rd-prop-text"><b>Angular momentum about any fixed point</b> for a particle: <code>L = mvr sinθ = mv × (⊥ distance from point to velocity line)</code>. This perpendicular distance is called the <b>impact parameter</b>.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P5</div><div class="rd-prop-text"><b>For a system of particles</b>: L_total = L_cm + L_about_cm. The spin part (L_about_cm) is independent of reference point choice!</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P6</div><div class="rd-prop-text"><b>Minimum MOI axis</b>: Iₒ (about COM) is always the minimum MOI. Any parallel axis gives I = Iₒ + Md² > Iₒ. The COM axis is the "easiest to spin" axis.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P7</div><div class="rd-prop-text"><b>Symmetry argument for MOI</b>: If body has 2 axes of symmetry in a plane, Ix = Iy. Then Iz = 2Ix (perpendicular axis theorem). Disk: I_diam = MR²/4, so I_perp = MR²/2 ✓</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P8</div><div class="rd-prop-text"><b>Hollow vs Solid same mass/radius</b>: Always I_hollow > I_solid because mass is farther from axis. So hollow objects accelerate slower on inclines, arrive last in rolling race.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P9</div><div class="rd-prop-text"><b>Slipping to rolling transition</b>: If v_cm ≠ Rω initially, kinetic friction acts until rolling condition v_cm = Rω is reached. Use separate equations for v_cm(t) and ω(t), then equate.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P10</div><div class="rd-prop-text"><b>Radius of gyration shortcut</b>: <code>k² = I/M</code>. Acceleration of rolling = g sinθ/(1 + k²/R²). Just plug k² for the shape. Sphere: 2R²/5, Cylinder: R²/2, Ring: R².</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P11</div><div class="rd-prop-text"><b>Couple has same torque everywhere</b>: The moment of a couple is the same about every point in space. So for couple problems, you don't need to specify the reference point.</div></div>
    <div class="rd-prop"><div class="rd-prop-num">P12</div><div class="rd-prop-text"><b>Angular momentum of projectile</b>: L about launch point = mvₓ × y - mv_y × x = constant? No! Only if torque is zero. Gravity provides torque about any point not on its line of action. L is NOT conserved in projectile motion about launch point.</div></div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SEC 10: TRICKS & FUN METHODS
═══════════════════════════════════════ -->
<section class="rd-sec" id="rd10">
  <div class="rd-sh"><span class="rd-sn">10 —</span><h2>Speed Tricks &amp; Fun Approaches</h2></div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 01 — The "Torque About Contact" Superpower</div>
    <div class="rd-trick-body">For any rolling body on a surface, <b>take torque about the contact point.</b> Friction magically disappears (zero moment arm)! You get one clean equation: <code>τ_contact = I_contact × α</code>. Use parallel axis theorem: I_contact = I_cm + MR². This single equation replaces two (Newton's 2nd for translation + rotation). Saves 50% of work! 🎯</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 02 — Checking Rolling Race Without Calculation</div>
    <div class="rd-trick-body">You don't need to compute accelerations. Just order by <b>k²/R²</b> (smaller = faster). Rank: Solid Sphere (2/5) → Solid Cylinder (1/2) → Hollow Sphere (2/3) → Ring (1). <b>Memorize this order once, use forever.</b> The geometry, not the mass, decides the winner.</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 03 — "Negative Mass" for Holes & Cavities</div>
    <div class="rd-trick-body">MOI of disk with circular hole = I(full disk) − I(removed disk). Place a <b>negative mass</b> where the hole is. For off-center holes, use parallel axis theorem on the "negative disk." This trick extends to COM calculations too: always subtract the removed part.</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 04 — Angular Momentum Direction by Thumb Rule</div>
    <div class="rd-trick-body">Curl right-hand fingers in the direction of rotation → thumb points in direction of <b>L</b> (and ω). This is also the direction from which rotation appears counterclockwise. When torque is perpendicular to L, it changes direction of L but not its magnitude → <b>precession</b>, not spin-up!</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 05 — 5-Second Energy Check for Rolling</div>
    <div class="rd-trick-body">Total KE for rolling = <b>½mv²(1 + k²/R²)</b>. Just multiply translational KE by <code>(1 + k²/R²)</code>. Sphere: 1 + 2/5 = 7/5, so KE = 7/10 mv². Cylinder: 1 + 1/2 = 3/2, KE = 3/4 mv². No need to compute ½Iω² separately!</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 06 — Hinge Reaction Shortcut</div>
    <div class="rd-trick-body">For a rod/bar pivoted at one end, at the moment of release:<br>α = 3g/(2L) (horizontal rod). <b>Hinge reaction = Mg/4</b> (horizontal) and varies with angle. At any angle θ from vertical: use <code>F_net = Ma_cm = M(L/2)α</code> for radial and tangential separately. Don't guess — split into components!</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 07 — Slipping Detection Rule</div>
    <div class="rd-trick-body">At contact point: if <b>v_cm > Rω</b>, the bottom slides forward → friction acts <b>backward</b>. If <b>v_cm &lt; Rω</b>, bottom slides backward → friction acts <b>forward</b>. Rolling without slipping: v_cm = Rω exactly. Use this to instantly know friction direction in any rolling/slipping problem!</div>
  </div>

  <div class="rd-trick">
    <div class="rd-trick-hdr">🚀 TRICK 08 — The "Constant L" Pattern Spotter</div>
    <div class="rd-trick-body">Look for these keywords in JEE problems: "suddenly", "collapses", "pulls in", "free to rotate", "smooth pivot/hinge" → these mean <b>angular momentum is conserved</b>! But beware: "rough surface", "string tension", "normal force" can provide external torques. Always check τ_ext about the axis before conserving L.</div>
  </div>

  <!-- Animation canvas for MOI visualization -->
  <div class="rd-canvas-wrap" style="margin-top:24px;">
    <div class="rd-canvas-title">🎡 Interactive — Parallel Axis Theorem Visualized</div>
    <canvas id="rdCanvasPAT" width="560" height="200"></canvas>
  </div>

</section>

</div><!-- .rd-wrap -->
</div><!-- .cwrap -->
</div><!-- #sec-rotdyn -->

<script>
// ── ROTATIONAL DYNAMICS ANIMATIONS ──

let _rdAnimStarted = false;

function rdStartAnimations() {
  if (_rdAnimStarted) return;
  _rdAnimStarted = true;
  rdAnimDisk();
  rdAnimTorque();
  rdAnimRoll();
  rdAnimPAT();
}

// ─ 1) Spinning Disk ─
function rdAnimDisk() {
  const canvas = document.getElementById('rdCanvasDisk');
  if (!canvas) return;
  const ctx = canvas.getContext('2d');
  const W = canvas.width, H = canvas.height;
  let angle = 0, omega = 1.8; // rad/s sim

  function draw() {
    ctx.clearRect(0, 0, W, H);
    const cx = W / 2, cy = H / 2, R = 65;

    // Background glow
    const grd = ctx.createRadialGradient(cx, cy, 0, cx, cy, R);
    grd.addColorStop(0, 'rgba(255,107,53,0.08)');
    grd.addColorStop(1, 'rgba(255,107,53,0)');
    ctx.fillStyle = grd;
    ctx.beginPath();
    ctx.arc(cx, cy, R + 10, 0, Math.PI * 2);
    ctx.fill();

    // Disk body
    ctx.save();
    ctx.translate(cx, cy);
    ctx.rotate(angle);
    ctx.beginPath();
    ctx.arc(0, 0, R, 0, Math.PI * 2);
    ctx.fillStyle = 'rgba(255,107,53,0.15)';
    ctx.strokeStyle = '#ff6b35';
    ctx.lineWidth = 1.5;
    ctx.fill();
    ctx.stroke();

    // Spokes
    for (let i = 0; i < 6; i++) {
      const a = (i / 6) * Math.PI * 2;
      ctx.beginPath();
      ctx.moveTo(0, 0);
      ctx.lineTo(Math.cos(a) * R, Math.sin(a) * R);
      ctx.strokeStyle = 'rgba(255,107,53,0.5)';
      ctx.lineWidth = 1;
      ctx.stroke();
    }

    // Marker dot
    ctx.beginPath();
    ctx.arc(R - 8, 0, 5, 0, Math.PI * 2);
    ctx.fillStyle = '#f5c842';
    ctx.fill();

    ctx.restore();

    // Center dot
    ctx.beginPath();
    ctx.arc(cx, cy, 4, 0, Math.PI * 2);
    ctx.fillStyle = '#40d0c0';
    ctx.fill();

    // Labels
    ctx.fillStyle = '#8090a8';
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('ω = ' + omega.toFixed(1) + ' rad/s', 8, 20);
    ctx.fillText('θ = ' + (angle % (Math.PI * 2) * 180 / Math.PI).toFixed(0) + '°', 8, 34);

    // Arrow for omega
    ctx.save();
    ctx.translate(cx + R + 18, cy);
    ctx.strokeStyle = '#ff6b35';
    ctx.lineWidth = 1.5;
    ctx.beginPath();
    ctx.moveTo(0, -20);
    ctx.lineTo(0, 20);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(-5, -15);
    ctx.lineTo(0, -22);
    ctx.lineTo(5, -15);
    ctx.strokeStyle = '#f5c842';
    ctx.stroke();
    ctx.fillStyle = '#ff6b35';
    ctx.font = '9px JetBrains Mono, monospace';
    ctx.fillText('ω', 6, 4);
    ctx.restore();

    angle += omega * 0.016;
    requestAnimationFrame(draw);
  }
  draw();
}

// ─ 2) Torque Animation ─
function rdAnimTorque() {
  const canvas = document.getElementById('rdCanvasTorque');
  if (!canvas) return;
  const ctx = canvas.getContext('2d');
  const W = canvas.width, H = canvas.height;
  let t = 0;

  function draw() {
    ctx.clearRect(0, 0, W, H);
    const pivotX = W / 2, pivotY = H / 2;
    const armLen = 80;

    // Arm angle oscillates
    const armAngle = -Math.PI / 4 + Math.sin(t * 0.6) * 0.35;

    // Arm
    const ax = pivotX + Math.cos(armAngle) * armLen;
    const ay = pivotY + Math.sin(armAngle) * armLen;

    ctx.strokeStyle = '#40d0c0';
    ctx.lineWidth = 3;
    ctx.beginPath();
    ctx.moveTo(pivotX, pivotY);
    ctx.lineTo(ax, ay);
    ctx.stroke();

    // r label
    ctx.fillStyle = '#40d0c0';
    ctx.font = '11px JetBrains Mono, monospace';
    ctx.fillText('r', (pivotX + ax) / 2 - 12, (pivotY + ay) / 2 - 6);

    // Force arrow (downward from tip)
    const fLen = 55;
    ctx.strokeStyle = '#ff6b35';
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.moveTo(ax, ay);
    ctx.lineTo(ax, ay + fLen);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(ax - 6, ay + fLen - 10);
    ctx.lineTo(ax, ay + fLen);
    ctx.lineTo(ax + 6, ay + fLen - 10);
    ctx.stroke();
    ctx.fillStyle = '#ff6b35';
    ctx.fillText('F', ax + 6, ay + fLen / 2);

    // Dashed perpendicular line
    const perpX = pivotX;
    const perpY = ay;
    ctx.setLineDash([4, 4]);
    ctx.strokeStyle = 'rgba(160,128,240,0.5)';
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.moveTo(pivotX, pivotY);
    ctx.lineTo(perpX, perpY);
    ctx.lineTo(ax, ay);
    ctx.stroke();
    ctx.setLineDash([]);

    // Torque arc
    ctx.strokeStyle = '#a080f0';
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.arc(pivotX, pivotY, 30, armAngle - 0.5, armAngle + 0.3);
    ctx.stroke();

    // Pivot
    ctx.beginPath();
    ctx.arc(pivotX, pivotY, 6, 0, Math.PI * 2);
    ctx.fillStyle = '#e8c060';
    ctx.fill();

    // Labels
    ctx.fillStyle = '#a080f0';
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('τ = r × F', 6, 18);
    ctx.fillStyle = '#8090a8';
    ctx.fillText('d = r sinφ', 6, 32);

    t += 0.016;
    requestAnimationFrame(draw);
  }
  draw();
}

// ─ 3) Rolling without Slipping ─
function rdAnimRoll() {
  const canvas = document.getElementById('rdCanvasRoll');
  if (!canvas) return;
  const ctx = canvas.getContext('2d');
  const W = canvas.width, H = canvas.height;
  const R = 36;
  let cx = R + 10, angle = 0;
  const v_cm = 1.4; // pixels per frame
  const omega = v_cm / R;

  function draw() {
    ctx.clearRect(0, 0, W, H);

    // Ground line
    const gy = H - 28;
    ctx.strokeStyle = 'rgba(255,107,53,0.25)';
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.moveTo(0, gy);
    ctx.lineTo(W, gy);
    ctx.stroke();

    const cy2 = gy - R;

    // Circle
    ctx.save();
    ctx.translate(cx, cy2);
    ctx.rotate(angle);
    ctx.beginPath();
    ctx.arc(0, 0, R, 0, Math.PI * 2);
    ctx.fillStyle = 'rgba(64,208,192,0.12)';
    ctx.strokeStyle = '#40d0c0';
    ctx.lineWidth = 2;
    ctx.fill();
    ctx.stroke();

    // Cross
    ctx.strokeStyle = 'rgba(64,208,192,0.6)';
    ctx.lineWidth = 1.2;
    ctx.beginPath();
    ctx.moveTo(-R, 0); ctx.lineTo(R, 0);
    ctx.moveTo(0, -R); ctx.lineTo(0, R);
    ctx.stroke();

    // Marker
    ctx.beginPath();
    ctx.arc(R - 7, 0, 4, 0, Math.PI * 2);
    ctx.fillStyle = '#f5c842';
    ctx.fill();

    ctx.restore();

    // v_cm arrow
    ctx.strokeStyle = '#ff6b35';
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.moveTo(cx, cy2);
    ctx.lineTo(cx + 38, cy2);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(cx + 32, cy2 - 5);
    ctx.lineTo(cx + 38, cy2);
    ctx.lineTo(cx + 32, cy2 + 5);
    ctx.stroke();
    ctx.fillStyle = '#ff6b35';
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('v_cm', cx + 14, cy2 - 6);

    // Top point arrow (2v_cm)
    ctx.strokeStyle = '#a080f0';
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.moveTo(cx, cy2 - R);
    ctx.lineTo(cx + 60, cy2 - R);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(cx + 54, cy2 - R - 5);
    ctx.lineTo(cx + 60, cy2 - R);
    ctx.lineTo(cx + 54, cy2 - R + 5);
    ctx.stroke();
    ctx.fillStyle = '#a080f0';
    ctx.fillText('2v_cm', cx + 18, cy2 - R - 6);

    // Contact point label
    ctx.fillStyle = '#50d890';
    ctx.beginPath();
    ctx.arc(cx, gy, 4, 0, Math.PI * 2);
    ctx.fill();
    ctx.font = '9px JetBrains Mono, monospace';
    ctx.fillText('v=0', cx + 5, gy + 14);

    // Labels bottom
    ctx.fillStyle = '#8090a8';
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('v_cm = Rω', 8, H - 8);

    cx += v_cm;
    angle += omega;
    if (cx > W + R) { cx = -R; }

    requestAnimationFrame(draw);
  }
  draw();
}

// ─ 4) Parallel Axis Theorem visual ─
function rdAnimPAT() {
  const canvas = document.getElementById('rdCanvasPAT');
  if (!canvas) return;
  const ctx = canvas.getContext('2d');
  const W = canvas.width, H = canvas.height;
  let t = 0;

  function draw() {
    ctx.clearRect(0, 0, W, H);

    // Title
    ctx.fillStyle = '#8090a8';
    ctx.font = '10px JetBrains Mono, monospace';

    // LEFT: CM axis
    const cx1 = 110, cy = H / 2, R = 60;
    ctx.beginPath();
    ctx.arc(cx1, cy, R, 0, Math.PI * 2);
    ctx.fillStyle = 'rgba(255,107,53,0.1)';
    ctx.strokeStyle = '#ff6b35';
    ctx.lineWidth = 1.5;
    ctx.fill();
    ctx.stroke();

    // CM axis
    ctx.strokeStyle = '#40d0c0';
    ctx.lineWidth = 2;
    ctx.setLineDash([]);
    ctx.beginPath();
    ctx.moveTo(cx1, cy - R - 20);
    ctx.lineTo(cx1, cy + R + 20);
    ctx.stroke();
    ctx.fillStyle = '#40d0c0';
    ctx.fillText('COM axis', cx1 + 5, cy - R - 8);
    ctx.fillStyle = '#ff6b35';
    ctx.fillText('I₀ = ½MR²', cx1 - 35, cy + R + 30);

    // CENTER: arrow
    ctx.fillStyle = '#a080f0';
    ctx.font = '16px sans-serif';
    ctx.fillText('→', W / 2 - 10, cy + 5);
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('+ Md²', W / 2 - 18, cy + 20);

    // RIGHT: parallel axis
    const cx2 = 390, d = 75;
    ctx.beginPath();
    ctx.arc(cx2 - d, cy, R, 0, Math.PI * 2);
    ctx.fillStyle = 'rgba(255,107,53,0.07)';
    ctx.strokeStyle = 'rgba(255,107,53,0.4)';
    ctx.lineWidth = 1.5;
    ctx.fill();
    ctx.stroke();

    // Parallel axis (shifted)
    ctx.strokeStyle = '#a080f0';
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.moveTo(cx2, cy - R - 20);
    ctx.lineTo(cx2, cy + R + 20);
    ctx.stroke();

    // d arrow
    ctx.strokeStyle = '#f5c842';
    ctx.lineWidth = 1.5;
    ctx.beginPath();
    ctx.moveTo(cx2 - d, cy + R + 10);
    ctx.lineTo(cx2, cy + R + 10);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(cx2 - d + 8, cy + R + 5);
    ctx.lineTo(cx2 - d, cy + R + 10);
    ctx.lineTo(cx2 - d + 8, cy + R + 15);
    ctx.stroke();
    ctx.beginPath();
    ctx.moveTo(cx2 - 8, cy + R + 5);
    ctx.lineTo(cx2, cy + R + 10);
    ctx.lineTo(cx2 - 8, cy + R + 15);
    ctx.stroke();
    ctx.fillStyle = '#f5c842';
    ctx.font = '11px JetBrains Mono, monospace';
    ctx.fillText('d', cx2 - d / 2 - 4, cy + R + 7);

    // Labels
    ctx.fillStyle = '#a080f0';
    ctx.font = '10px JetBrains Mono, monospace';
    ctx.fillText('parallel axis', cx2 + 4, cy - R - 8);
    ctx.fillStyle = '#50d890';
    ctx.fillText('I = I₀ + Md²', cx2 - d - 30, cy + R + 30);

    // Animated pulse on new axis
    const pulse = 0.5 + 0.5 * Math.sin(t * 3);
    ctx.beginPath();
    ctx.arc(cx2, cy, 6, 0, Math.PI * 2);
    ctx.fillStyle = `rgba(160,128,240,${pulse})`;
    ctx.fill();

    t += 0.016;
    requestAnimationFrame(draw);
  }
  draw();
}

// ═══════════════════════════════════════════════════════════════
//  SHARED STYLES — THERMODYNAMICS & IONIC EQUILIBRIUM (injected)
// ═══════════════════════════════════════════════════════════════
</script>
<style>
.chem-wrap{font-family:'EB Garamond',serif;}
.chem-sec{padding:44px 0;border-top:1px solid rgba(224,90,255,.1);}
.ionic-sec{padding:44px 0;border-top:1px solid rgba(34,238,168,.1);}
.chem-sec:first-child,.ionic-sec:first-child{border-top:none;}
.chem-sh{display:flex;align-items:baseline;gap:14px;margin-bottom:30px;}
.chem-sn{font-family:'JetBrains Mono',monospace;font-size:10px;color:#e05aff;letter-spacing:2px;opacity:.75;}
.ionic-sn{font-family:'JetBrains Mono',monospace;font-size:10px;color:#22eea8;letter-spacing:2px;opacity:.75;}
.chem-wrap h2{font-family:'Syne',sans-serif;font-size:1.8rem;font-weight:700;color:#fff;letter-spacing:-.4px;}
.chem-wrap h3{font-family:'Syne',sans-serif;font-size:1.08rem;color:#e05aff;margin:22px 0 11px;padding-bottom:5px;border-bottom:1px solid rgba(224,90,255,.14);}
.ionic-wrap h3{font-family:'Syne',sans-serif;font-size:1.08rem;color:#22eea8;margin:22px 0 11px;padding-bottom:5px;border-bottom:1px solid rgba(34,238,168,.14);}
.chem-wrap h4{font-family:'JetBrains Mono',monospace;font-size:.73rem;letter-spacing:1.5px;text-transform:uppercase;color:#60b8f0;margin:14px 0 7px;}
/* formula grids */
.ch-fg{display:grid;grid-template-columns:repeat(auto-fill,minmax(255px,1fr));gap:2px;background:rgba(224,90,255,.05);border:1px solid rgba(224,90,255,.12);border-radius:7px;overflow:hidden;margin:12px 0;}
.io-fg{display:grid;grid-template-columns:repeat(auto-fill,minmax(255px,1fr));gap:2px;background:rgba(34,238,168,.04);border:1px solid rgba(34,238,168,.11);border-radius:7px;overflow:hidden;margin:12px 0;}
.ch-fb{background:#050710;padding:12px 15px 10px;border-left:2px solid transparent;transition:background .18s,transform .14s;}
.ch-fb:hover{background:#0d1020;transform:translateX(3px);border-left-color:#e05aff;}
.io-fb{background:#040c10;padding:12px 15px 10px;border-left:2px solid transparent;transition:background .18s,transform .14s;}
.io-fb:hover{background:#081814;transform:translateX(3px);border-left-color:#22eea8;}
.ch-fl{font-family:'JetBrains Mono',monospace;font-size:8.5px;letter-spacing:1.8px;text-transform:uppercase;color:#8090a8;margin-bottom:5px;}
.ch-fm{font-family:'JetBrains Mono',monospace;font-size:.85rem;color:#fff;line-height:1.7;}
.ch-fm .cv{color:#e05aff;}.ch-fm .cg{color:#50d890;}.ch-fm .cb{color:#60b8f0;}.ch-fm .cy{color:#f5c842;}.ch-fm .cr{color:#f06080;}.ch-fm .ce{color:#8090a8;}
.io-fm{font-family:'JetBrains Mono',monospace;font-size:.85rem;color:#fff;line-height:1.7;}
.io-fm .iv{color:#22eea8;}.io-fm .iy{color:#f5c842;}.io-fm .ib{color:#60b8f0;}.io-fm .ir{color:#f06080;}.io-fm .ip{color:#e05aff;}.io-fm .ie{color:#8090a8;}
/* notes */
.ch-note{background:rgba(80,216,144,.05);border-left:3px solid #50d890;padding:10px 14px;margin:10px 0;border-radius:0 5px 5px 0;font-family:'JetBrains Mono',monospace;font-size:.78rem;color:#50d890;line-height:1.8;}
.ch-note::before{content:'💡  ';}
.io-note{background:rgba(34,238,168,.05);border-left:3px solid #22eea8;padding:10px 14px;margin:10px 0;border-radius:0 5px 5px 0;font-family:'JetBrains Mono',monospace;font-size:.78rem;color:#22eea8;line-height:1.8;}
.io-note::before{content:'💡  ';}
.ch-warn{background:rgba(240,96,128,.05);border-left:3px solid #f06080;padding:10px 14px;margin:10px 0;border-radius:0 5px 5px 0;font-family:'JetBrains Mono',monospace;font-size:.78rem;color:#f06080;line-height:1.8;}
.ch-warn::before{content:'⚠  ';}
/* steps */
.ch-steps{display:flex;flex-direction:column;gap:7px;margin:12px 0;}
.ch-step{display:flex;gap:11px;align-items:flex-start;background:rgba(255,255,255,.02);border-radius:5px;padding:10px 14px;border-left:2px solid transparent;transition:border-color .18s;}
.ch-step:hover{border-left-color:#e05aff;}
.io-step{display:flex;gap:11px;align-items:flex-start;background:rgba(255,255,255,.02);border-radius:5px;padding:10px 14px;border-left:2px solid transparent;transition:border-color .18s;}
.io-step:hover{border-left-color:#22eea8;}
.ch-step-n{font-family:'JetBrains Mono',monospace;font-size:9px;color:#e05aff;background:rgba(224,90,255,.12);min-width:22px;height:22px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px;font-weight:700;}
.io-step-n{font-family:'JetBrains Mono',monospace;font-size:9px;color:#22eea8;background:rgba(34,238,168,.12);min-width:22px;height:22px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px;font-weight:700;}
.ch-step-t{font-family:'Crimson Pro',serif;font-size:.94rem;color:#e0e8f0;line-height:1.7;flex:1;}
.ch-step-t .m{font-family:'JetBrains Mono',monospace;font-size:.8rem;background:rgba(255,255,255,.06);padding:2px 6px;border-radius:3px;color:#fff;border:1px solid rgba(255,255,255,.06);display:inline-block;margin:1px 2px;}
.ch-step-t .h{color:#22eea8;font-family:'JetBrains Mono',monospace;font-size:.8rem;}
.ch-step-t .hp{color:#e05aff;font-family:'JetBrains Mono',monospace;font-size:.8rem;}
/* fun cards */
.ch-fun{background:linear-gradient(135deg,rgba(224,90,255,.07) 0%,rgba(96,184,240,.05) 100%);border:1px solid rgba(224,90,255,.2);border-radius:10px;padding:17px 20px;margin:13px 0;position:relative;overflow:hidden;}
.ch-fun::before{content:'';position:absolute;top:-18px;right:-18px;width:75px;height:75px;border-radius:50%;background:radial-gradient(circle,rgba(224,90,255,.18),transparent 70%);}
.io-fun{background:linear-gradient(135deg,rgba(34,238,168,.06) 0%,rgba(96,184,240,.05) 100%);border:1px solid rgba(34,238,168,.2);border-radius:10px;padding:17px 20px;margin:13px 0;position:relative;overflow:hidden;}
.io-fun::before{content:'';position:absolute;top:-18px;right:-18px;width:75px;height:75px;border-radius:50%;background:radial-gradient(circle,rgba(34,238,168,.16),transparent 70%);}
.ch-fun-tag,.io-fun-tag{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2.5px;text-transform:uppercase;margin-bottom:7px;}
.ch-fun-tag{color:#e05aff;}.io-fun-tag{color:#22eea8;}
.ch-fun-title,.io-fun-title{font-family:'Syne',sans-serif;font-size:.96rem;font-weight:700;color:#fff;margin-bottom:7px;}
.ch-fun-emoji,.io-fun-emoji{font-size:1.5rem;float:right;margin-left:12px;}
.ch-fun-body,.io-fun-body{font-family:'Crimson Pro',serif;font-style:italic;font-size:.93rem;color:#c0ccd8;line-height:1.8;}
.ch-fun-body b,.io-fun-body b{font-style:normal;color:#f5c842;}
/* props */
.ch-props{display:flex;flex-direction:column;gap:6px;margin:12px 0;}
.ch-prop{display:flex;align-items:flex-start;gap:10px;background:#060810;border:1px solid rgba(255,255,255,.04);border-radius:5px;padding:10px 14px;transition:border-color .18s;}
.ch-prop:hover{border-color:rgba(224,90,255,.28);}
.io-prop{display:flex;align-items:flex-start;gap:10px;background:#040c10;border:1px solid rgba(255,255,255,.04);border-radius:5px;padding:10px 14px;transition:border-color .18s;}
.io-prop:hover{border-color:rgba(34,238,168,.28);}
.ch-pn{font-family:'JetBrains Mono',monospace;font-size:.72rem;color:#e05aff;background:rgba(224,90,255,.11);min-width:26px;height:26px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0;font-weight:700;}
.io-pn{font-family:'JetBrains Mono',monospace;font-size:.72rem;color:#22eea8;background:rgba(34,238,168,.1);min-width:26px;height:26px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0;font-weight:700;}
.ch-pt{font-family:'Crimson Pro',serif;font-size:.93rem;color:#c8d0dc;line-height:1.72;flex:1;}
.ch-pt b{color:#e05aff;}.ch-pt .gb{color:#22eea8;}.ch-pt code{font-family:'JetBrains Mono',monospace;font-size:.8rem;background:rgba(255,255,255,.06);padding:1px 5px;border-radius:3px;color:#60b8f0;}
.io-pt{font-family:'Crimson Pro',serif;font-size:.93rem;color:#c8d0dc;line-height:1.72;flex:1;}
.io-pt b{color:#22eea8;}.io-pt .rb{color:#f06080;}.io-pt code{font-family:'JetBrains Mono',monospace;font-size:.8rem;background:rgba(255,255,255,.06);padding:1px 5px;border-radius:3px;color:#60b8f0;}
/* QP */
.ch-qp{display:grid;grid-template-columns:repeat(auto-fill,minmax(290px,1fr));gap:10px;margin:13px 0;}
.ch-qcard{background:#060810;border:1px solid rgba(224,90,255,.13);border-radius:8px;padding:14px;transition:border-color .2s;}
.ch-qcard:hover{border-color:#e05aff;}
.io-qcard{background:#040c10;border:1px solid rgba(34,238,168,.12);border-radius:8px;padding:14px;transition:border-color .2s;}
.io-qcard:hover{border-color:#22eea8;}
.ch-qtype{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2px;text-transform:uppercase;color:#e05aff;margin-bottom:7px;}
.io-qtype{font-family:'JetBrains Mono',monospace;font-size:8px;letter-spacing:2px;text-transform:uppercase;color:#22eea8;margin-bottom:7px;}
.ch-qq{font-family:'Crimson Pro',serif;font-size:.93rem;color:#e8e0d0;line-height:1.75;margin-bottom:9px;}
.ch-qhint{font-family:'JetBrains Mono',monospace;font-size:.73rem;color:#50d890;background:rgba(80,216,144,.05);border:1px solid rgba(80,216,144,.14);padding:6px 10px;border-radius:4px;line-height:1.7;}
.ch-qhint::before{content:'→ ';}
/* graph */
.ch-graph{background:#050a10;border:1px solid rgba(224,90,255,.14);border-radius:8px;overflow:hidden;margin:16px 0;}
.io-graph{background:#040c0a;border:1px solid rgba(34,238,168,.13);border-radius:8px;overflow:hidden;margin:16px 0;}
.ch-graph-title,.io-graph-title{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:#8090a8;padding:8px 14px;border-bottom:1px solid rgba(255,255,255,.05);}
.ch-graph canvas,.io-graph canvas{display:block;width:100%;}
/* table */
.ch-tbl{width:100%;border-collapse:collapse;font-family:'JetBrains Mono',monospace;font-size:.79rem;margin:13px 0;}
.ch-tbl th{background:rgba(224,90,255,.08);color:#e05aff;font-size:8.5px;letter-spacing:1.5px;text-transform:uppercase;padding:9px 11px;text-align:left;border-bottom:1px solid rgba(224,90,255,.12);}
.ch-tbl td{padding:8px 11px;border-bottom:1px solid rgba(30,37,53,.5);background:#050710;transition:background .12s;}
.ch-tbl tr:hover td{background:#0a0e18;}
.ch-tbl td:first-child{color:#60b8f0;}
.io-tbl{width:100%;border-collapse:collapse;font-family:'JetBrains Mono',monospace;font-size:.79rem;margin:13px 0;}
.io-tbl th{background:rgba(34,238,168,.07);color:#22eea8;font-size:8.5px;letter-spacing:1.5px;text-transform:uppercase;padding:9px 11px;text-align:left;border-bottom:1px solid rgba(34,238,168,.12);}
.io-tbl td{padding:8px 11px;border-bottom:1px solid rgba(20,50,40,.5);background:#040c10;transition:background .12s;}
.io-tbl tr:hover td{background:#071410;}
.io-tbl td:first-child{color:#60b8f0;}
/* pattern box */
.ch-pattern{background:rgba(224,90,255,.04);border:1px solid rgba(224,90,255,.18);border-radius:6px;padding:13px 15px;margin:10px 0;}
.io-pattern{background:rgba(34,238,168,.04);border:1px solid rgba(34,238,168,.17);border-radius:6px;padding:13px 15px;margin:10px 0;}
.ch-pattern-hdr{font-family:'JetBrains Mono',monospace;font-size:8.5px;letter-spacing:2px;text-transform:uppercase;color:#e05aff;margin-bottom:7px;}
.io-pattern-hdr{font-family:'JetBrains Mono',monospace;font-size:8.5px;letter-spacing:2px;text-transform:uppercase;color:#22eea8;margin-bottom:7px;}
.ch-pattern-body,.io-pattern-body{font-family:'JetBrains Mono',monospace;font-size:.79rem;color:#c0ccd8;line-height:1.95;}
.ch-pattern-body .hl,.io-pattern-body .hl{color:#f5c842;}
.ch-pattern-body .gh,.io-pattern-body .gh{color:#50d890;}
/* pH strip */
.ph-strip{display:flex;height:28px;border-radius:5px;overflow:hidden;margin:12px 0;}
.ph-cell{flex:1;display:flex;align-items:center;justify-content:center;font-family:'JetBrains Mono',monospace;font-size:.64rem;font-weight:700;}
</style>

<!-- THERMODYNAMICS SECTION -->
<div class="psec" id="sec-thermo">
<div class="cwrap">
<div class="shero" style="--sc:rgba(224,90,255,.09)">
  <span class="shero-badge">JEE Advanced · Physical Chemistry · Complete Module</span>
  <h2 style="background:linear-gradient(120deg,#e05aff,#60b8f0,#f5c842);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text">Thermodynamics</h2>
  <p>Laws · Enthalpy · Entropy · Gibbs Energy · Hess's Law · Graphs · JEE Tricks &amp; Patterns</p>
  <div class="snav"><a href="#th1">Basics</a><a href="#th2">Laws</a><a href="#th3">Enthalpy</a><a href="#th4">Entropy</a><a href="#th5">Gibbs</a><a href="#th6">Cp&amp;Cv</a><a href="#th7">Graphs</a><a href="#th8">JEE Patterns</a><a href="#th9">Misc Props</a><a href="#th10">Tricks</a></div>
</div>
<div class="chem-wrap">

<section class="chem-sec" id="th1">
  <div class="chem-sh"><span class="chem-sn">01 —</span><h2>Fundamental Concepts</h2></div>
  <div class="ch-fg">
    <div class="ch-fb"><div class="ch-fl">System Types</div><div class="ch-fm">Open (E+M), Closed (E only), Isolated (neither)</div></div>
    <div class="ch-fb"><div class="ch-fl">State Functions</div><div class="ch-fm"><span class="cv">U, H, S, G</span> — path-independent. <span class="cb">q, w</span> — path-dependent</div></div>
    <div class="ch-fb"><div class="ch-fl">First Law</div><div class="ch-fm"><span class="cv">ΔU</span> <span class="ce">=</span> <span class="cb">q + w</span> &nbsp;(IUPAC: w +ve when done ON system)</div></div>
    <div class="ch-fb"><div class="ch-fl">Work (expansion)</div><div class="ch-fm"><span class="cv">w</span> <span class="ce">=</span> <span class="cr">−P_ext ΔV</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Isochoric</div><div class="ch-fm">ΔV = 0 → <span class="cv">w = 0</span> → <span class="cv">ΔU = q_v</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Isobaric</div><div class="ch-fm">P = const → <span class="cv">q_p = ΔH</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Isothermal ideal gas</div><div class="ch-fm">ΔT=0 → <span class="cv">ΔU=0</span> → <span class="cv">q = −w</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Adiabatic</div><div class="ch-fm">q = 0 → <span class="cv">ΔU = w</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Rev. isothermal work</div><div class="ch-fm"><span class="cv">w_rev</span> <span class="ce">=</span> <span class="cb">−nRT ln(V₂/V₁)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Irrev. work (const P)</div><div class="ch-fm"><span class="cv">w_irrev</span> <span class="ce">=</span> <span class="cr">−P_ext(V₂−V₁)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Free expansion</div><div class="ch-fm">P_ext = 0 → <span class="cv">w = 0, ΔU = 0, q = 0</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Max work</div><div class="ch-fm">|w_rev| &gt; |w_irrev| always for expansion</div></div>
  </div>
  <div class="ch-note">For ideal gas: ΔU depends only on T. At constant T → ΔU = 0 regardless of path.</div>
</section>

<section class="chem-sec" id="th2">
  <div class="chem-sh"><span class="chem-sn">02 —</span><h2>Laws of Thermodynamics</h2></div>
  <h3>Second Law &amp; Entropy</h3>
  <div class="ch-steps">
    <div class="ch-step"><div class="ch-step-n">2L</div><div class="ch-step-t"><span class="m">ΔS_universe ≥ 0</span> for all real processes. = 0 for reversible, &gt; 0 for irreversible.</div></div>
    <div class="ch-step"><div class="ch-step-n">3L</div><div class="ch-step-t">Entropy of perfectly crystalline substance = 0 at 0 K → absolute entropies always positive.</div></div>
  </div>
  <div class="ch-warn">Sign convention: IUPAC → w = +ve when work done ON system. q = +ve when heat absorbed BY system. Opposite of older conventions!</div>
</section>

<section class="chem-sec" id="th3">
  <div class="chem-sh"><span class="chem-sn">03 —</span><h2>Enthalpy &amp; Hess's Law</h2></div>
  <div class="ch-fg">
    <div class="ch-fb"><div class="ch-fl">Definition</div><div class="ch-fm"><span class="cv">H = U + PV</span> &nbsp;·&nbsp; <span class="cv">ΔH = ΔU + Δn_g RT</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Exothermic</div><div class="ch-fm"><span class="cr">ΔH &lt; 0</span> — heat released</div></div>
    <div class="ch-fb"><div class="ch-fl">Endothermic</div><div class="ch-fm"><span class="cg">ΔH &gt; 0</span> — heat absorbed</div></div>
    <div class="ch-fb"><div class="ch-fl">Bond Enthalpy</div><div class="ch-fm"><span class="cv">ΔH_rxn</span> = Σ(bonds broken) − Σ(bonds formed)</div></div>
    <div class="ch-fb"><div class="ch-fl">Hess's Law</div><div class="ch-fm"><span class="cv">ΔH_rxn</span> = ΣΔH°f(products) − ΣΔH°f(reactants)</div></div>
    <div class="ch-fb"><div class="ch-fl">Neutralisation (SA+SB)</div><div class="ch-fm">Always <span class="cr">−57.1 kJ/mol</span> at 25°C</div></div>
    <div class="ch-fb"><div class="ch-fl">Resonance energy</div><div class="ch-fm">ΔH°f(from bond E) − ΔH°f(from combustion). Always −ve for aromatics.</div></div>
    <div class="ch-fb"><div class="ch-fl">Standard state</div><div class="ch-fm">ΔH°f of element in std state = 0. Diamond ≠ 0 (graphite = 0).</div></div>
  </div>
  <h3>Standard Enthalpies Reference Table</h3>
  <table class="ch-tbl">
    <thead><tr><th>Type</th><th>Symbol</th><th>Key Point</th></tr></thead>
    <tbody>
      <tr><td>Formation</td><td>ΔH°f</td><td>1 mol compound from elements in std state</td></tr>
      <tr><td>Combustion</td><td>ΔH°c</td><td>Complete combustion in O₂ (always negative)</td></tr>
      <tr><td>Atomisation</td><td>ΔH°at</td><td>Always endothermic (+ve)</td></tr>
      <tr><td>Hydration</td><td>ΔH°hyd</td><td>Always exothermic (−ve)</td></tr>
      <tr><td>Lattice (LE)</td><td>U</td><td>Always endothermic if defined as MX→M⁺+X⁻</td></tr>
      <tr><td>Solution</td><td>ΔH°sol</td><td>= LE − hydration; can be + or −</td></tr>
    </tbody>
  </table>
</section>

<section class="chem-sec" id="th4">
  <div class="chem-sh"><span class="chem-sn">04 —</span><h2>Entropy</h2></div>
  <div class="ch-fg">
    <div class="ch-fb"><div class="ch-fl">Clausius</div><div class="ch-fm"><span class="cv">dS = δq_rev/T</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Isothermal ideal gas</div><div class="ch-fm"><span class="cv">ΔS = nR ln(V₂/V₁) = nR ln(P₁/P₂)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Phase change</div><div class="ch-fm"><span class="cv">ΔS = ΔH_transition/T</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Heating</div><div class="ch-fm"><span class="cv">ΔS = nCp ln(T₂/T₁)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Boltzmann</div><div class="ch-fm"><span class="cv">S = k_B ln W</span> (W = microstates)</div></div>
    <div class="ch-fb"><div class="ch-fl">Surroundings</div><div class="ch-fm"><span class="cv">ΔS_surr = −ΔH_sys/T</span></div></div>
    <div class="ch-fb"><div class="ch-fl">S(gas)>>S(liq)>S(s)</div><div class="ch-fm">Entropy increases: solid→liquid→gas; Δn_g &gt; 0 → ΔS &gt; 0</div></div>
    <div class="ch-fb"><div class="ch-fl">Trouton's Rule</div><div class="ch-fm">ΔS_vap ≈ 88 J/mol·K for most liquids (exceptions: H₂O, EtOH)</div></div>
  </div>
</section>

<section class="chem-sec" id="th5">
  <div class="chem-sh"><span class="chem-sn">05 —</span><h2>Gibbs Free Energy &amp; Spontaneity</h2></div>
  <div class="ch-fg">
    <div class="ch-fb"><div class="ch-fl">Definition</div><div class="ch-fm"><span class="cv">G = H − TS</span> &nbsp;·&nbsp; <span class="cv">ΔG = ΔH − TΔS</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Spontaneous</div><div class="ch-fm"><span class="cg">ΔG &lt; 0</span> → spontaneous; <span class="cr">ΔG &gt; 0</span> → non-spontaneous</div></div>
    <div class="ch-fb"><div class="ch-fl">Equilibrium</div><div class="ch-fm"><span class="cv">ΔG = 0</span> at equilibrium</div></div>
    <div class="ch-fb"><div class="ch-fl">ΔG° &amp; K</div><div class="ch-fm"><span class="cv">ΔG° = −RT ln K</span></div></div>
    <div class="ch-fb"><div class="ch-fl">ΔG vs ΔG°</div><div class="ch-fm"><span class="cv">ΔG = ΔG° + RT ln Q</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Max non-PV work</div><div class="ch-fm"><span class="cv">w_max = ΔG</span> (const T, P)</div></div>
    <div class="ch-fb"><div class="ch-fl">Crossover T</div><div class="ch-fm"><span class="cv">T* = ΔH/ΔS</span> where ΔG flips sign</div></div>
    <div class="ch-fb"><div class="ch-fl">Cell potential link</div><div class="ch-fm"><span class="cv">ΔG° = −nFE°cell</span></div></div>
  </div>
  <h3>Spontaneity Table</h3>
  <table class="ch-tbl">
    <thead><tr><th>ΔH</th><th>ΔS</th><th>ΔG = ΔH−TΔS</th><th>Spontaneous?</th></tr></thead>
    <tbody>
      <tr><td>−</td><td>+</td><td style="color:#50d890">Always −</td><td>✅ At all T</td></tr>
      <tr><td>+</td><td>−</td><td style="color:#f06080">Always +</td><td>❌ Never</td></tr>
      <tr><td>−</td><td>−</td><td>− at low T</td><td>✅ Low T only</td></tr>
      <tr><td>+</td><td>+</td><td>− at high T</td><td>✅ High T only</td></tr>
    </tbody>
  </table>
  <div class="ch-graph">
    <div class="ch-graph-title">📈 ΔG = ΔH − TΔS — All Four Cases</div>
    <canvas id="thermoGGraph" width="540" height="210"></canvas>
  </div>
</section>

<section class="chem-sec" id="th6">
  <div class="chem-sh"><span class="chem-sn">06 —</span><h2>Heat Capacity, Kirchhoff &amp; Adiabatic</h2></div>
  <div class="ch-fg">
    <div class="ch-fb"><div class="ch-fl">Cp − Cv</div><div class="ch-fm"><span class="cv">Cp − Cv = R</span> (ideal gas)</div></div>
    <div class="ch-fb"><div class="ch-fl">γ = Cp/Cv</div><div class="ch-fm">Monoatomic: <span class="cv">5/3</span> · Diatomic: <span class="cv">7/5</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Kirchhoff's Law</div><div class="ch-fm"><span class="cv">ΔH(T₂) = ΔH(T₁) + ΔCp(T₂−T₁)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Adiabatic rev.</div><div class="ch-fm"><span class="cv">PV^γ = const</span> · <span class="cv">TV^(γ−1) = const</span></div></div>
    <div class="ch-fb"><div class="ch-fl">Adiabatic work</div><div class="ch-fm"><span class="cv">w = nCv(T₂−T₁)</span></div></div>
    <div class="ch-fb"><div class="ch-fl">P-V slope comparison</div><div class="ch-fm">Adiabatic slope = <span class="cv">γ × isothermal slope</span> (steeper)</div></div>
  </div>
</section>

<section class="chem-sec" id="th7">
  <div class="chem-sh"><span class="chem-sn">07 —</span><h2>Key Graphs</h2></div>
  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:14px;">
    <div class="ch-graph"><div class="ch-graph-title">P–V Diagram: Four Processes</div><canvas id="thermoPVGraph" width="250" height="200"></canvas></div>
    <div class="ch-graph"><div class="ch-graph-title">Enthalpy Profile: Exo vs Endo</div><canvas id="thermoEnergyGraph" width="250" height="200"></canvas></div>
  </div>
  <div class="ch-note">Area under P-V curve = work done BY gas (= −w in IUPAC). Isothermal curve encloses MORE area than adiabatic for same expansion → isothermal does more work.</div>
</section>

<section class="chem-sec" id="th8">
  <div class="chem-sh"><span class="chem-sn">08 —</span><h2>JEE Question Patterns</h2></div>
  <div class="ch-qp">
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 1 — ΔH vs ΔU</div><div class="ch-qq">Find ΔH − ΔU for CH₄(g) + 2O₂(g) → CO₂(g) + 2H₂O(l)</div><div class="ch-qhint">Δn_g = 1 − 3 = −2 (count only gaseous moles; liquid H₂O excluded). ΔH − ΔU = −2RT ≈ −4958 J at 300K.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 2 — Hess's Law Combo</div><div class="ch-qq">Given ΔH for A→B, B→C, C→D. Find ΔH for A→D.</div><div class="ch-qhint">Simply add the three: ΔH(A→D) = ΔH₁ + ΔH₂ + ΔH₃. If any step is reversed, flip its sign first. Intermediate species cancel.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 3 — Spontaneity Temperature</div><div class="ch-qq">ΔH = +120 kJ, ΔS = +400 J/K. At what T is process spontaneous?</div><div class="ch-qhint">T > ΔH/ΔS = 120000/400 = 300 K. Convert ΔH to J first! Very common unit trap in JEE.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 4 — Irreversible Work</div><div class="ch-qq">1 mol gas expands against P_ext = 1 atm from 10L to 50L. Find w, q, ΔU (isothermal ideal).</div><div class="ch-qhint">w = −1×(50−10) = −40 L·atm = −4054 J. ΔU=0 (isothermal ideal). q = +4054 J (heat absorbed).</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 5 — Bond Enthalpy</div><div class="ch-qq">CH₄ + 2O₂ → CO₂ + 2H₂O(g). Use bond enthalpies.</div><div class="ch-qhint">Broken: 4×C-H(413) + 2×O=O(498) = 2648 kJ. Formed: 2×C=O(741)×2 + 4×O-H(463) = 4816 kJ. ΔH = 2648−4816 = −802 kJ.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 6 — ΔG° from K</div><div class="ch-qq">K = 100 at 298K. Find ΔG°.</div><div class="ch-qhint">ΔG° = −RT ln K = −8.314 × 298 × ln(100) = −8.314 × 298 × 4.605 ≈ −11.4 kJ/mol.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 7 — Born-Haber</div><div class="ch-qq">Find lattice enthalpy of NaCl given: ΔHf, sub(Na), IE(Na), ½×diss(Cl₂), EA(Cl).</div><div class="ch-qhint">ΔHf = sub + IE + ½diss + EA + U(lattice). Solve for U. All terms except U can be measured directly.</div></div>
    <div class="ch-qcard"><div class="ch-qtype">🎯 Pattern 8 — Entropy Sign</div><div class="ch-qq">Rank by entropy: N₂(g) at 1 atm 300K, N₂(g) at 2 atm 300K, N₂(l) at 300K.</div><div class="ch-qhint">S(g,1atm) > S(g,2atm) [lower P = higher V = more disorder]. S(g) >> S(l). Order: liquid < 2atm gas < 1atm gas.</div></div>
  </div>
</section>

<section class="chem-sec" id="th9">
  <div class="chem-sh"><span class="chem-sn">09 —</span><h2>Miscellaneous Properties</h2></div>
  <div class="ch-props">
    <div class="ch-prop"><div class="ch-pn">M1</div><div class="ch-pt"><b>ΔH neutralisation (WA or WB)</b>: Less than 57.1 kJ/mol because ionisation of weak species is endothermic, reducing net heat released.</div></div>
    <div class="ch-prop"><div class="ch-pn">M2</div><div class="ch-pt"><b>Entropy of mixing</b>: <code>ΔS_mix = −nR Σxᵢ ln xᵢ</code> — always positive. Mixing is always spontaneous for ideal gases and ideal solutions.</div></div>
    <div class="ch-prop"><div class="ch-pn">M3</div><div class="ch-pt"><b>Joule-Thomson effect</b>: Ideal gas: no temperature change (μ_JT = 0). Real gases cool below inversion temperature. Used in gas liquefaction.</div></div>
    <div class="ch-prop"><div class="ch-pn">M4</div><div class="ch-pt"><b>Adiabatic > Isothermal slope on P-V</b>: Slope of adiabatic = γ × slope of isothermal at any point. Adiabat is always steeper than isotherm passing through same point.</div></div>
    <div class="ch-prop"><div class="ch-pn">M5</div><div class="ch-pt"><b>Cyclic process</b>: ΔU = 0, ΔH = 0, ΔS = 0, ΔG = 0 (all state functions). q = −w. This is an important JEE pattern.</div></div>
    <div class="ch-prop"><div class="ch-pn">M6</div><div class="ch-pt"><b>K > 1 ↔ ΔG° negative</b>: Large K (≫1) → very negative ΔG° → essentially complete reaction. K ≈ 1 → ΔG° ≈ 0. K &lt;&lt; 1 → ΔG° very positive.</div></div>
    <div class="ch-prop"><div class="ch-pn">M7</div><div class="ch-pt"><b>Internal energy of ideal gas</b>: U = nCvT. Depends ONLY on temperature. ΔU = nCvΔT regardless of process (isochoric, isothermal, isobaric, adiabatic).</div></div>
    <div class="ch-prop"><div class="ch-pn">M8</div><div class="ch-pt"><b>Extensive vs Intensive</b>: U, H, S, G, V are extensive (proportional to amount). T, P, density, molar quantities are intensive. Molar entropy S° is intensive.</div></div>
    <div class="ch-prop"><div class="ch-pn">M9</div><div class="ch-pt"><b>ΔG and reversible work</b>: Maximum non-PV work obtainable from a process = −ΔG at constant T and P. For electrochemical cells: max electrical work = −ΔG = nFE°.</div></div>
    <div class="ch-prop"><div class="ch-pn">M10</div><div class="ch-pt"><b>Standard state reminder</b>: 1 bar, 298 K. Note 1 bar ≠ 1 atm (1 atm = 1.01325 bar). ΔH°f of all elements in standard state = 0 by definition.</div></div>
  </div>
</section>

<section class="chem-sec" id="th10">
  <div class="chem-sh"><span class="chem-sn">10 —</span><h2>Speed Tricks &amp; Strategies</h2></div>
  <div class="ch-fun">
    <span class="ch-fun-emoji">⚡</span>
    <div class="ch-fun-tag">🚀 Trick 01 — Count Δn_g First</div>
    <div class="ch-fun-title">Always start by counting gaseous mole change</div>
    <div class="ch-fun-body"><b>Δn_g = moles gaseous products − moles gaseous reactants.</b> Liquids and solids are ignored. This instantly gives ΔH − ΔU = Δn_g RT. Half the JEE thermodynamics MCQs test exactly this.</div>
  </div>
  <div class="ch-fun">
    <span class="ch-fun-emoji">📊</span>
    <div class="ch-fun-tag">🚀 Trick 02 — Spontaneity in 2 Seconds</div>
    <div class="ch-fun-title">Learn the 2×2 spontaneity grid cold</div>
    <div class="ch-fun-body">−ΔH &amp; +ΔS → <b>always spontaneous</b>. +ΔH &amp; −ΔS → <b>never spontaneous</b>. Same sign → temperature decides. Crossover T* = ΔH/ΔS. Takes 2 seconds once memorised.</div>
  </div>
  <div class="ch-fun">
    <span class="ch-fun-emoji">🔗</span>
    <div class="ch-fun-tag">🚀 Trick 03 — Hess's Law: Target First</div>
    <div class="ch-fun-title">Write target equation first, then manipulate given equations</div>
    <div class="ch-fun-body">Never start randomly combining. Look at <b>each species in target → find it in given equations → scale and flip as needed → cancel intermediates</b>. Systematic = zero mistakes.</div>
  </div>
  <div class="ch-fun">
    <span class="ch-fun-emoji">🌡️</span>
    <div class="ch-fun-tag">🚀 Trick 04 — Isothermal Does More Work</div>
    <div class="ch-fun-title">|w_rev isothermal| > |w_adiabatic| for same ΔV</div>
    <div class="ch-fun-body">In isothermal: gas absorbs heat to maintain T → more work done. In adiabatic: gas cools → less force available → less work. <b>Bigger area under P-V curve = more work.</b> Isothermal always has bigger area than adiabatic between same volumes.</div>
  </div>
  <div class="ch-pattern">
    <div class="ch-pattern-hdr">⚡ Critical Quick-Reference</div>
    <div class="ch-pattern-body">
      <span class="hl">ΔH = ΔU + Δn_g RT</span> · <span class="hl">ΔG° = −RT ln K</span> · <span class="hl">ΔG = ΔG° + RT ln Q</span><br>
      <span class="hl">T* = ΔH/ΔS</span> · <span class="hl">ΔS_surr = −ΔH_sys/T</span> · <span class="hl">ΔS = nR ln(V₂/V₁)</span><br>
      <span class="gh">w_rev = −nRT ln(V₂/V₁)</span> · <span class="gh">w_irr = −P_ext ΔV</span> · <span class="gh">ΔG° = −nFE°</span>
    </div>
  </div>
</section>

</div></div></div>

<!-- IONIC EQUILIBRIUM SECTION -->
<div class="psec" id="sec-ionic">
<div class="cwrap">
<div class="shero" style="--sc:rgba(34,238,168,.08)">
  <span class="shero-badge">JEE Advanced · Physical Chemistry · Complete Module</span>
  <h2 style="background:linear-gradient(120deg,#22eea8,#60b8f0,#e05aff);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text">Ionic Equilibrium</h2>
  <p>Acids &amp; Bases · pH · Ka/Kb · Buffers · Solubility · Hydrolysis · JEE Tricks &amp; Patterns</p>
  <div class="snav"><a href="#io1">Theories</a><a href="#io2">pH &amp; pKa</a><a href="#io3">Weak Acids/Bases</a><a href="#io4">Hydrolysis</a><a href="#io5">Buffers</a><a href="#io6">Ksp</a><a href="#io7">Graphs</a><a href="#io8">JEE Patterns</a><a href="#io9">Misc Props</a><a href="#io10">Tricks</a></div>
</div>
<div class="ionic-wrap chem-wrap">

<section class="ionic-sec" id="io1">
  <div class="chem-sh"><span class="ionic-sn">01 —</span><h2>Acid–Base Theories</h2></div>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">Arrhenius Acid/Base</div><div class="io-fm">Acid → H⁺; Base → OH⁻ in water</div></div>
    <div class="io-fb"><div class="ch-fl">Brønsted Acid</div><div class="io-fm">Proton <span class="iv">donor</span> (HF, HCl, CH₃COOH)</div></div>
    <div class="io-fb"><div class="ch-fl">Brønsted Base</div><div class="io-fm">Proton <span class="iv">acceptor</span> (NH₃, H₂O, F⁻)</div></div>
    <div class="io-fb"><div class="ch-fl">Lewis Acid</div><div class="io-fm">Electron pair <span class="iy">acceptor</span>: BF₃, AlCl₃, Fe³⁺, H⁺</div></div>
    <div class="io-fb"><div class="ch-fl">Lewis Base</div><div class="io-fm">Electron pair <span class="iy">donor</span>: NH₃, H₂O, F⁻, CO</div></div>
    <div class="io-fb"><div class="ch-fl">Conjugate pair</div><div class="io-fm">HA ⇌ H⁺ + A⁻ · HA/A⁻ are conjugate pair</div></div>
    <div class="io-fb"><div class="ch-fl">Ka × Kb</div><div class="io-fm"><span class="iv">Ka × Kb = Kw</span> for conjugate acid-base pair</div></div>
    <div class="io-fb"><div class="ch-fl">Amphoteric</div><div class="io-fm">H₂O, HCO₃⁻, H₂PO₄⁻, HSO₄⁻ — both acid &amp; base</div></div>
  </div>
  <div class="io-note">Strongest acid → weakest conjugate base. Lewis acid/base concept is most general (includes non-protic systems).</div>
</section>

<section class="ionic-sec" id="io2">
  <div class="chem-sh"><span class="ionic-sn">02 —</span><h2>pH, pOH, pKa, pKb</h2></div>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">pH</div><div class="io-fm"><span class="iv">pH = −log[H⁺]</span></div></div>
    <div class="io-fb"><div class="ch-fl">pOH</div><div class="io-fm"><span class="iv">pOH = −log[OH⁻]</span></div></div>
    <div class="io-fb"><div class="ch-fl">pH + pOH = 14</div><div class="io-fm">At 25°C. Kw = [H⁺][OH⁻] = 10⁻¹⁴</div></div>
    <div class="io-fb"><div class="ch-fl">pKa + pKb = 14</div><div class="io-fm">For conjugate pair at 25°C</div></div>
    <div class="io-fb"><div class="ch-fl">Strong acid</div><div class="io-fm"><span class="iv">pH = −log C</span> (complete dissociation)</div></div>
    <div class="io-fb"><div class="ch-fl">Strong base</div><div class="io-fm"><span class="iv">pOH = −log C</span> then pH = 14 − pOH</div></div>
    <div class="io-fb"><div class="ch-fl">Lower pKa</div><div class="io-fm">Stronger acid (pKa↓ = Ka↑ = more dissociation)</div></div>
    <div class="io-fb"><div class="ch-fl">Kw vs T</div><div class="io-fm">Kw increases with T → pH of pure water decreases with T (still neutral)</div></div>
  </div>
  <!-- pH strip -->
  <div class="ph-strip">
    <div class="ph-cell" style="background:#b71c1c;color:#fff">0</div><div class="ph-cell" style="background:#d32f2f;color:#fff">1</div><div class="ph-cell" style="background:#e53935;color:#fff">2</div><div class="ph-cell" style="background:#f44336;color:#fff">3</div><div class="ph-cell" style="background:#ef9a9a;color:#222">4</div><div class="ph-cell" style="background:#ffcc80;color:#222">5</div><div class="ph-cell" style="background:#fff176;color:#222">6</div><div class="ph-cell" style="background:#e8f5e9;color:#222">7</div><div class="ph-cell" style="background:#b2dfdb;color:#222">8</div><div class="ph-cell" style="background:#80cbc4;color:#222">9</div><div class="ph-cell" style="background:#26a69a;color:#fff">10</div><div class="ph-cell" style="background:#00897b;color:#fff">11</div><div class="ph-cell" style="background:#00695c;color:#fff">12</div><div class="ph-cell" style="background:#004d40;color:#fff">13</div><div class="ph-cell" style="background:#002622;color:#fff">14</div>
  </div>
  <div style="display:flex;justify-content:space-between;font-family:'JetBrains Mono',monospace;font-size:.64rem;color:#8090a8;margin-bottom:12px;"><span>← Acidic</span><span>Neutral (7)</span><span>Basic →</span></div>
</section>

<section class="ionic-sec" id="io3">
  <div class="chem-sh"><span class="ionic-sn">03 —</span><h2>Weak Acids &amp; Bases</h2></div>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">Ka expression</div><div class="io-fm"><span class="iv">Ka = [H⁺][A⁻]/[HA]</span></div></div>
    <div class="io-fb"><div class="ch-fl">[H⁺] weak acid</div><div class="io-fm"><span class="iv">[H⁺] = √(Ka·C)</span> (if α &lt;&lt; 1)</div></div>
    <div class="io-fb"><div class="ch-fl">pH weak acid</div><div class="io-fm"><span class="iv">pH = ½(pKa − log C)</span></div></div>
    <div class="io-fb"><div class="ch-fl">Degree α</div><div class="io-fm"><span class="iv">α = √(Ka/C)</span> (Ostwald dilution law)</div></div>
    <div class="io-fb"><div class="ch-fl">[OH⁻] weak base</div><div class="io-fm"><span class="iv">[OH⁻] = √(Kb·C)</span></div></div>
    <div class="io-fb"><div class="ch-fl">pH weak base</div><div class="io-fm">pOH = ½(pKb − log C) then pH = 14 − pOH</div></div>
    <div class="io-fb"><div class="ch-fl">Polyprotic: pH</div><div class="io-fm">Use Ka₁ only (Ka₂, Ka₃ negligible)</div></div>
    <div class="io-fb"><div class="ch-fl">Intermediate HA⁻</div><div class="io-fm"><span class="iv">pH = ½(pKa₁ + pKa₂)</span></div></div>
  </div>
  <div class="ch-warn">√(Ka·C) approximation valid only when α &lt; 5%. If C is very small or Ka is large, solve full quadratic: x² + Ka·x − Ka·C = 0.</div>
</section>

<section class="ionic-sec" id="io4">
  <div class="chem-sh"><span class="ionic-sn">04 —</span><h2>Salt Hydrolysis</h2></div>
  <table class="io-tbl">
    <thead><tr><th>Salt Type</th><th>Example</th><th>pH</th><th>Hydrolysis</th></tr></thead>
    <tbody>
      <tr><td>SA + SB</td><td>NaCl</td><td>= 7</td><td>None</td></tr>
      <tr><td>WA + SB</td><td>CH₃COONa</td><td>&gt; 7 (basic)</td><td>Anionic (A⁻ + H₂O ⇌ HA + OH⁻)</td></tr>
      <tr><td>SA + WB</td><td>NH₄Cl</td><td>&lt; 7 (acidic)</td><td>Cationic (BH⁺ + H₂O ⇌ B + H₃O⁺)</td></tr>
      <tr><td>WA + WB</td><td>CH₃COONH₄</td><td>≈ 7 if Ka=Kb</td><td>Both hydrolyse</td></tr>
    </tbody>
  </table>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">WA salt (CH₃COONa)</div><div class="io-fm"><span class="iv">pH = 7 + ½pKa − ½log C</span></div></div>
    <div class="io-fb"><div class="ch-fl">WB salt (NH₄Cl)</div><div class="io-fm"><span class="iv">pH = 7 − ½pKb + ½log C</span></div></div>
    <div class="io-fb"><div class="ch-fl">WA + WB salt</div><div class="io-fm"><span class="iv">pH = 7 + ½(pKa − pKb)</span></div></div>
    <div class="io-fb"><div class="ch-fl">Hydrolysis const Kh</div><div class="io-fm"><span class="iv">Kh = Kw/Ka</span> (for WA salt)</div></div>
    <div class="io-fb"><div class="ch-fl">Degree of hydrolysis h</div><div class="io-fm"><span class="iv">h = √(Kw/(Ka·C))</span></div></div>
    <div class="io-fb"><div class="ch-fl">Hydrolysis increases with</div><div class="io-fm">Dilution (C↓), Temperature↑, weaker acid/base</div></div>
  </div>
  <div class="io-note">Rule: Only the ion derived from the WEAK species hydrolyses. Na⁺ (from NaOH, strong) — no hydrolysis. CH₃COO⁻ (from CH₃COOH, weak) — hydrolyses.</div>
</section>

<section class="ionic-sec" id="io5">
  <div class="chem-sh"><span class="ionic-sn">05 —</span><h2>Buffer Solutions</h2></div>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">Henderson-Hasselbalch</div><div class="io-fm"><span class="iv">pH = pKa + log([A⁻]/[HA])</span></div></div>
    <div class="io-fb"><div class="ch-fl">Basic buffer</div><div class="io-fm"><span class="iv">pOH = pKb + log([BH⁺]/[B])</span></div></div>
    <div class="io-fb"><div class="ch-fl">Max buffer capacity</div><div class="io-fm">At <span class="iv">pH = pKa</span> (equal concentrations)</div></div>
    <div class="io-fb"><div class="ch-fl">Buffer range</div><div class="io-fm"><span class="iv">pH = pKa ± 1</span></div></div>
    <div class="io-fb"><div class="ch-fl">Half-equivalence point</div><div class="io-fm">[HA] = [A⁻] → <span class="iv">pH = pKa</span></div></div>
    <div class="io-fb"><div class="ch-fl">Add strong acid</div><div class="io-fm">A⁻ + H⁺ → HA · recalculate moles ratio</div></div>
    <div class="io-fb"><div class="ch-fl">Add strong base</div><div class="io-fm">HA + OH⁻ → A⁻ + H₂O · recalculate</div></div>
    <div class="io-fb"><div class="ch-fl">Volume doesn't matter</div><div class="io-fm">Buffer ratio = moles ratio (volume cancels!)</div></div>
  </div>
  <div class="io-fun">
    <span class="io-fun-emoji">🧪</span>
    <div class="io-fun-tag">🎉 Buffer — The Chemical Sponge</div>
    <div class="io-fun-title">A buffer absorbs H⁺ and OH⁻ without large pH change</div>
    <div class="io-fun-body">A⁻ absorbs added H⁺ (forms HA). HA absorbs added OH⁻ (forms A⁻ + H₂O). The <b>ratio [A⁻]/[HA] shifts slightly</b> but since log function is slow-changing, pH changes very little. <b>The reservoir is the key!</b> No reservoir → no buffer action.</div>
  </div>
</section>

<section class="ionic-sec" id="io6">
  <div class="chem-sh"><span class="ionic-sn">06 —</span><h2>Solubility Product (Ksp)</h2></div>
  <div class="io-fg">
    <div class="io-fb"><div class="ch-fl">AgCl type (AB)</div><div class="io-fm"><span class="iv">Ksp = s²</span> → s = √Ksp</div></div>
    <div class="io-fb"><div class="ch-fl">PbCl₂ type (AB₂)</div><div class="io-fm"><span class="iv">Ksp = 4s³</span> → s = (Ksp/4)^(1/3)</div></div>
    <div class="io-fb"><div class="ch-fl">Ag₂CrO₄ type (A₂B)</div><div class="io-fm"><span class="iv">Ksp = 4s³</span> → s = (Ksp/4)^(1/3)</div></div>
    <div class="io-fb"><div class="ch-fl">AlF₃ type (AB₃)</div><div class="io-fm"><span class="iv">Ksp = 27s⁴</span> → s = (Ksp/27)^(1/4)</div></div>
    <div class="io-fb"><div class="ch-fl">Precipitation</div><div class="io-fm">Q > Ksp → precipitate forms</div></div>
    <div class="io-fb"><div class="ch-fl">Common ion effect</div><div class="io-fm">Adding common ion → solubility ↓</div></div>
    <div class="io-fb"><div class="ch-fl">Selective precipitation</div><div class="io-fm">Smaller Ksp precipitates first (at lower [precipitant])</div></div>
    <div class="io-fb"><div class="ch-fl">pH effect</div><div class="io-fm">Metal hydroxides: solubility ↑ at lower pH</div></div>
  </div>
  <div class="ch-warn">NEVER compare Ksp directly across different formula types! AgCl (Ksp=10⁻¹⁰) vs Ag₂CrO₄ (Ksp=10⁻¹²): Ag₂CrO₄ has smaller Ksp but LARGER molar solubility! Always convert to s first.</div>
</section>

<section class="ionic-sec" id="io7">
  <div class="chem-sh"><span class="ionic-sn">07 —</span><h2>Key Graphs</h2></div>
  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:14px;">
    <div class="io-graph"><div class="io-graph-title">Titration: Strong Acid + Strong Base</div><canvas id="ionicTitration1" width="250" height="215"></canvas></div>
    <div class="io-graph"><div class="io-graph-title">Titration: Weak Acid + Strong Base</div><canvas id="ionicTitration2" width="250" height="215"></canvas></div>
    <div class="io-graph"><div class="io-graph-title">α &amp; [H⁺] vs Concentration</div><canvas id="ionicAlpha" width="250" height="215"></canvas></div>
  </div>
  <div class="io-note">Weak acid titration: gradual rise in buffer region, steep jump at equivalence (above 7), half-equivalence point gives pKa directly.</div>
</section>

<section class="ionic-sec" id="io8">
  <div class="chem-sh"><span class="ionic-sn">08 —</span><h2>JEE Question Patterns</h2></div>
  <div class="ch-qp">
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 1 — Mixed Strong Acids</div><div class="ch-qq">50 mL 0.1M HCl + 50 mL 0.1M H₂SO₄. Find pH.</div><div class="ch-qhint">Total H⁺ = (0.1×50 + 0.2×50)/100 = 0.15 M. pH = −log(0.15) ≈ 0.82. H₂SO₄ gives 2 H⁺ per molecule!</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 2 — Buffer + Strong Acid</div><div class="ch-qq">Buffer: 0.1 mol CH₃COOH + 0.1 mol CH₃COONa in 1L. Add 0.01 mol HCl. pH? (pKa=4.74)</div><div class="ch-qhint">HCl reacts: A⁻ → 0.09 mol, HA → 0.11 mol. pH = 4.74 + log(0.09/0.11) = 4.74 − 0.087 ≈ 4.65.</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 3 — Ksp + Common Ion</div><div class="ch-qq">Ksp(AgCl)=10⁻¹⁰. Solubility in 0.1M NaCl?</div><div class="ch-qhint">s × 0.1 = 10⁻¹⁰ → s = 10⁻⁹ M. Compare pure water: s = 10⁻⁵ M. Common ion reduced solubility 10,000×!</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 4 — Salt Hydrolysis pH</div><div class="ch-qq">pH of 0.1M CH₃COONa? Ka = 1.8×10⁻⁵.</div><div class="ch-qhint">Kh = 10⁻¹⁴/1.8×10⁻⁵ = 5.56×10⁻¹⁰. [OH⁻] = √(5.56×10⁻¹¹) ≈ 7.46×10⁻⁶. pOH=5.13, pH=8.87.</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 5 — Precipitation Check</div><div class="ch-qq">Equal vols 10⁻³M AgNO₃ and 10⁻³M NaCl mixed. Ksp(AgCl)=10⁻¹⁰. Precipitate?</div><div class="ch-qhint">After mixing: [Ag⁺]=[Cl⁻]=5×10⁻⁴ M. Q=(5×10⁻⁴)²=2.5×10⁻⁷ >> 10⁻¹⁰. Yes, precipitate forms.</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 6 — pKa from Titration</div><div class="ch-qq">pH at half-equivalence point = 5.3. Find Ka.</div><div class="ch-qhint">At half-equiv: pH = pKa = 5.3. Ka = 10⁻⁵·³ = 5×10⁻⁶. The simplest JEE trick — frequently missed!</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 7 — Amphoteric Salt pH</div><div class="ch-qq">pH of 0.1M NaHCO₃? Ka₁=4.3×10⁻⁷, Ka₂=4.7×10⁻¹¹.</div><div class="ch-qhint">pH = ½(pKa₁ + pKa₂) = ½(6.37 + 10.33) = 8.35. This formula is independent of concentration!</div></div>
    <div class="io-qcard"><div class="io-qtype">🎯 Pattern 8 — Ksp Comparison Trap</div><div class="ch-qq">Which is more soluble: AgCl (Ksp=10⁻¹⁰) or Ag₂CrO₄ (Ksp=10⁻¹²)?</div><div class="ch-qhint">AgCl: s=10⁻⁵ M. Ag₂CrO₄: s=(10⁻¹²/4)^(1/3)≈6.3×10⁻⁵ M. Ag₂CrO₄ MORE soluble despite smaller Ksp! Different formula types!</div></div>
  </div>
</section>

<section class="ionic-sec" id="io9">
  <div class="chem-sh"><span class="ionic-sn">09 —</span><h2>Miscellaneous Properties</h2></div>
  <div class="ch-props">
    <div class="io-prop"><div class="io-pn">M1</div><div class="io-pt"><b>Ostwald dilution law</b>: α = √(Ka/C). Diluting increases α but decreases [H⁺]. <span class="rb">Diluting a weak acid raises its pH</span> (opposite of what students expect).</div></div>
    <div class="io-prop"><div class="io-pn">M2</div><div class="io-pt"><b>Acid strength order (HX)</b>: HI &gt; HBr &gt; HCl &gt;&gt; HF. Bond strength dominates. For oxyacids: more O atoms = more acidic. H₂SO₄ &gt; H₂SO₃; HClO₄ &gt; HClO₃ &gt; HClO.</div></div>
    <div class="io-prop"><div class="io-pn">M3</div><div class="io-pt"><b>Solubility rules (must-know)</b>: All NO₃⁻ soluble. Chlorides except AgCl, PbCl₂, Hg₂Cl₂. Sulfates except BaSO₄, PbSO₄, SrSO₄. Carbonates insoluble except Na⁺, K⁺, NH₄⁺ salts.</div></div>
    <div class="io-prop"><div class="io-pn">M4</div><div class="io-pt"><b>Very dilute strong acid pH</b>: 10⁻⁷ M HCl → pH ≠ 7. Water contributes 10⁻⁷ M H⁺. Total [H⁺] ≈ 1.414×10⁻⁷ → pH ≈ 6.85. Never below 6 for any acid in water.</div></div>
    <div class="io-prop"><div class="io-pn">M5</div><div class="io-pt"><b>Buffer capacity max</b>: At [HA] = [A⁻] (ratio = 1, pH = pKa). Buffer works within pKa ± 1. Outside this range, it's no longer an effective buffer.</div></div>
    <div class="io-prop"><div class="io-pn">M6</div><div class="io-pt"><b>Indicators</b>: Choose indicator with pKIn ≈ equivalence point pH. Phenolphthalein (pKIn≈9): WA+SB titrations. Methyl orange (pKIn≈4): SA+WB titrations. Litmus: not ideal for precise work.</div></div>
    <div class="io-prop"><div class="io-pn">M7</div><div class="io-pt"><b>Amphiprotic species pH</b>: For HA⁻ (from H₂A): pH = ½(pKa₁ + pKa₂). This is independent of concentration — a unique property of amphoteric intermediate salts.</div></div>
    <div class="io-prop"><div class="io-pn">M8</div><div class="io-pt"><b>Ksp and temperature</b>: Most ionic compound dissolution is endothermic → Ksp increases with T → higher solubility at higher T. Exceptions exist (e.g. Ca(OH)₂ retrograde solubility).</div></div>
    <div class="io-prop"><div class="io-pn">M9</div><div class="io-pt"><b>Isoelectric point</b>: pH at which amino acid/protein carries no net charge. pH = ½(pKa₁ + pKa₂). At this pH, minimum solubility and zero net migration in electric field.</div></div>
    <div class="io-prop"><div class="io-pn">M10</div><div class="io-pt"><b>Hydrolysis degree increases with dilution</b>: h = √(Kw/(Ka·C)). As C↓, h↑. But [OH⁻] = h·C = √(Kw·C/Ka) decreases with dilution. Paradox — degree goes up but concentration goes down.</div></div>
  </div>
</section>

<section class="ionic-sec" id="io10">
  <div class="chem-sh"><span class="ionic-sn">10 —</span><h2>Speed Tricks &amp; Strategies</h2></div>
  <div class="io-fun">
    <span class="io-fun-emoji">📐</span>
    <div class="io-fun-tag">🚀 Trick 01 — pH Formula Map (6 Situations)</div>
    <div class="io-fun-title">Identify situation → plug in matching formula</div>
    <div class="io-fun-body">
      <b>Strong acid:</b> pH = −log C &nbsp;&nbsp;
      <b>Weak acid:</b> pH = ½(pKa − log C)<br>
      <b>WA salt (e.g. CH₃COONa):</b> pH = 7 + ½pKa − ½log C<br>
      <b>Buffer:</b> pH = pKa + log([A⁻]/[HA])<br>
      <b>Amphoteric (HA⁻):</b> pH = ½(pKa₁ + pKa₂)<br>
      <b>Half-equiv point:</b> pH = pKa &nbsp;&nbsp; Zero derivation needed!
    </div>
  </div>
  <div class="io-fun">
    <span class="io-fun-emoji">🎯</span>
    <div class="io-fun-tag">🚀 Trick 02 — Ksp Comparison: Always Convert to s First</div>
    <div class="io-fun-title">Never compare Ksp directly across different salt formulas</div>
    <div class="io-fun-body">This is the most common JEE trap in ionic equilibrium. <b>Always compute molar solubility s and compare those.</b> AB type: s=√Ksp. AB₂ type: s=(Ksp/4)^(1/3). The one with smaller Ksp can have larger s if it's an AB₂ type vs AB type.</div>
  </div>
  <div class="io-fun">
    <span class="io-fun-emoji">⚖️</span>
    <div class="io-fun-tag">🚀 Trick 03 — Buffer: Moles First, Molarity Never</div>
    <div class="io-fun-title">Work in moles for buffer shift calculations</div>
    <div class="io-fun-body">When acid/base is added to buffer: do stoichiometry in <b>moles</b>, not molarity. The H-H equation uses the ratio [A⁻]/[HA] which equals the ratio of moles (volume cancels). <b>No need to recompute concentrations</b> if volume doesn't change drastically.</div>
  </div>
  <div class="io-fun">
    <span class="io-fun-emoji">🧲</span>
    <div class="io-fun-tag">🚀 Trick 04 — Hydrolysis: Weak Partner Rule</div>
    <div class="io-fun-title">"Only the ion from the WEAK species hydrolyses"</div>
    <div class="io-fun-body">CH₃COO⁻ → from weak CH₃COOH → hydrolyses → basic. NH₄⁺ → from weak NH₃ → hydrolyses → acidic. Na⁺ from strong NaOH → no hydrolysis. Cl⁻ from strong HCl → no hydrolysis. <b>This one rule handles all salt hydrolysis questions instantly.</b></div>
  </div>
  <div class="io-pattern">
    <div class="io-pattern-hdr">⚡ Critical Quick-Reference</div>
    <div class="io-pattern-body">
      <span class="hl">pH + pOH = 14</span> · <span class="hl">pKa + pKb = 14</span> · <span class="hl">Ka × Kb = Kw = 10⁻¹⁴</span><br>
      <span class="hl">[H⁺] = √(Ka·C)</span> · <span class="hl">pH = ½(pKa − log C)</span> · <span class="hl">Half-equiv: pH = pKa</span><br>
      <span class="hl">H-H: pH = pKa + log([A⁻]/[HA])</span> · <span class="hl">Kh = Kw/Ka</span><br>
      <span class="gh">AB: s=√Ksp</span> · <span class="gh">AB₂: s=(Ksp/4)^⅓</span> · <span class="gh">WA+WB: pH=7+½(pKa−pKb)</span>
    </div>
  </div>
</section>

</div></div></div>

<!-- CANVAS GRAPH SCRIPTS -->
<script>
function drawThermoGGraph(){
  const c=document.getElementById('thermoGGraph');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  const pL=50,pR=20,pT=24,pB=38,gW=W-pL-pR,gH=H-pT-pB;
  ctx.fillStyle='#050a10';ctx.fillRect(0,0,W,H);
  ctx.strokeStyle='#1e2a38';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='9px JetBrains Mono,monospace';
  ctx.fillText('T (K) →',pL+gW-42,pT+gH+28);
  ctx.save();ctx.translate(13,pT+gH/2+10);ctx.rotate(-Math.PI/2);ctx.fillText('ΔG',0,0);ctx.restore();
  const zY=pT+gH*0.5;
  ctx.strokeStyle='#1e2a38';ctx.setLineDash([4,4]);
  ctx.beginPath();ctx.moveTo(pL,zY);ctx.lineTo(pL+gW,zY);ctx.stroke();ctx.setLineDash([]);
  ctx.fillStyle='#404e66';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('0',pL-16,zY+4);
  const cases=[{dH:-1,dS:1,col:'#50d890',lbl:'−H+S: Always ✓'},{dH:1,dS:-1,col:'#f06080',lbl:'+H−S: Never ✗'},{dH:-1,dS:-1,col:'#60b8f0',lbl:'−H−S: Low T'},{dH:1,dS:1,col:'#f5c842',lbl:'+H+S: High T'}];
  cases.forEach(({dH,dS,col,lbl},i)=>{
    ctx.strokeStyle=col;ctx.lineWidth=2;
    ctx.beginPath();
    for(let px=0;px<=gW;px++){const T=px/gW,dG=dH*0.7-T*dS*0.85,y=zY-dG*gH*0.44;px===0?ctx.moveTo(pL+px,y):ctx.lineTo(pL+px,y);}
    ctx.stroke();
    ctx.fillStyle=col;ctx.font='8px JetBrains Mono,monospace';ctx.fillText(lbl,pL+4,pT+12+i*13);
  });
}
function drawThermoPVGraph(){
  const c=document.getElementById('thermoPVGraph');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  const pL=40,pR=14,pT=20,pB=34,gW=W-pL-pR,gH=H-pT-pB;
  ctx.fillStyle='#050a10';ctx.fillRect(0,0,W,H);
  ctx.strokeStyle='#1e2a38';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('V →',pL+gW-18,pT+gH+24);
  ctx.save();ctx.translate(11,pT+gH/2+6);ctx.rotate(-Math.PI/2);ctx.fillText('P →',0,0);ctx.restore();
  const V1=0.08,V2=0.9,P1=0.9,P2=0.1;
  const toX=v=>pL+(v-V1)/(V2-V1)*gW,toY=p=>pT+(1-(p-P2)/(P1-P2))*gH;
  // Isothermal
  ctx.strokeStyle='#60b8f0';ctx.lineWidth=1.8;ctx.beginPath();
  let f=true;for(let v=V1;v<=V2;v+=0.008){const p=V1*P1/v;if(p<P2||p>1.1)continue;const x=toX(v),y=toY(p);f?ctx.moveTo(x,y):ctx.lineTo(x,y);f=false;}
  ctx.stroke();
  // Adiabatic
  const g=5/3,Ca=P1*Math.pow(V1,g);
  ctx.strokeStyle='#a080f0';ctx.lineWidth=1.8;ctx.beginPath();f=true;
  for(let v=V1;v<=V2;v+=0.008){const p=Ca/Math.pow(v,g);if(p<P2||p>1.1)continue;const x=toX(v),y=toY(p);f?ctx.moveTo(x,y):ctx.lineTo(x,y);f=false;}
  ctx.stroke();
  // Isobaric
  ctx.strokeStyle='#f5c842';ctx.lineWidth=1.4;ctx.setLineDash([4,3]);
  const iP=0.45;ctx.beginPath();ctx.moveTo(toX(V1),toY(iP));ctx.lineTo(toX(V2),toY(iP));ctx.stroke();
  // Isochoric
  ctx.strokeStyle='#f06080';
  const iV=0.45;ctx.beginPath();ctx.moveTo(toX(iV),toY(P1));ctx.lineTo(toX(iV),toY(P2));ctx.stroke();ctx.setLineDash([]);
  const leg=[['Iso-T','#60b8f0'],['Adiab','#a080f0'],['Iso-P','#f5c842'],['Iso-V','#f06080']];
  leg.forEach(([l,col],i)=>{ctx.fillStyle=col;ctx.font='7.5px JetBrains Mono,monospace';ctx.fillText('— '+l,pL+2,pT+10+i*11);});
}
function drawThermoEnergyGraph(){
  const c=document.getElementById('thermoEnergyGraph');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  ctx.fillStyle='#050a10';ctx.fillRect(0,0,W,H);
  const pL=28,pR=10,pT=16,pB=26,gW=W-pL-pR,gH=H-pT-pB;
  ctx.strokeStyle='#1e2a38';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('Reaction →',pL,pT+gH+20);
  const ex=[[0,.7],[.15,.72],[.35,.22],[.5,.25],[.65,.1],[1,.1]];
  ctx.strokeStyle='#f06080';ctx.lineWidth=2;ctx.beginPath();
  ex.forEach(([x,y],i)=>{const px=pL+x*gW,py=pT+(1-y)*gH;i===0?ctx.moveTo(px,py):ctx.lineTo(px,py);});ctx.stroke();
  const en=[[0,.1],[.15,.12],[.35,.68],[.5,.71],[.65,.58],[1,.7]];
  ctx.strokeStyle='#60b8f0';ctx.lineWidth=2;ctx.beginPath();
  en.forEach(([x,y],i)=>{const px=pL+x*gW,py=pT+(1-y)*gH;i===0?ctx.moveTo(px,py):ctx.lineTo(px,py);});ctx.stroke();
  ctx.fillStyle='#f06080';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('Exo(ΔH<0)',pL+gW*0.6,pT+gH*0.2);
  ctx.fillStyle='#60b8f0';ctx.fillText('Endo(ΔH>0)',pL+gW*0.52,pT+gH*0.72);
}
function drawTitration1(){
  const c=document.getElementById('ionicTitration1');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  ctx.fillStyle='#040c0a';ctx.fillRect(0,0,W,H);
  const pL=40,pR=12,pT=16,pB=34,gW=W-pL-pR,gH=H-pT-pB;
  ctx.strokeStyle='#1a3028';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('Vol NaOH →',pL+gW/2-28,pT+gH+26);
  ctx.save();ctx.translate(11,pT+gH/2+8);ctx.rotate(-Math.PI/2);ctx.fillText('pH',0,0);ctx.restore();
  for(let ph=0;ph<=14;ph+=2){const y=pT+(1-ph/14)*gH;ctx.fillStyle='#404e66';ctx.font='7.5px JetBrains Mono,monospace';ctx.fillText(ph,pL-16,y+4);ctx.strokeStyle='#0e1e18';ctx.lineWidth=.4;ctx.beginPath();ctx.moveTo(pL,y);ctx.lineTo(pL+gW,y);ctx.stroke();}
  const toY=ph=>pT+(1-ph/14)*gH;
  ctx.strokeStyle='#22eea8';ctx.lineWidth=2;ctx.beginPath();
  for(let i=0;i<=100;i++){const x=pL+(i/100)*gW;let ph;
    if(i<44)ph=1+i*0.04;else if(i<48)ph=2.76+(i-44)*0.8;else if(i===50)ph=7;else if(i<54)ph=7+(i-50)*0.8;else ph=10.2+(i-54)*0.08;
    ph=Math.max(0,Math.min(14,ph));i===0?ctx.moveTo(x,toY(ph)):ctx.lineTo(x,toY(ph));}
  ctx.stroke();
  const eqX=pL+gW*0.495;ctx.strokeStyle='#f5c842';ctx.lineWidth=1;ctx.setLineDash([3,3]);ctx.beginPath();ctx.moveTo(eqX,pT);ctx.lineTo(eqX,pT+gH);ctx.stroke();ctx.setLineDash([]);
  ctx.fillStyle='#f5c842';ctx.font='7.5px JetBrains Mono,monospace';ctx.fillText('eq pt pH=7',eqX+3,toY(7)-4);
}
function drawTitration2(){
  const c=document.getElementById('ionicTitration2');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  ctx.fillStyle='#040c0a';ctx.fillRect(0,0,W,H);
  const pL=40,pR=12,pT=16,pB=34,gW=W-pL-pR,gH=H-pT-pB;
  ctx.strokeStyle='#1a3028';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('Vol NaOH →',pL+gW/2-28,pT+gH+26);
  ctx.save();ctx.translate(11,pT+gH/2+8);ctx.rotate(-Math.PI/2);ctx.fillText('pH',0,0);ctx.restore();
  for(let ph=0;ph<=14;ph+=2){const y=pT+(1-ph/14)*gH;ctx.fillStyle='#404e66';ctx.font='7.5px JetBrains Mono,monospace';ctx.fillText(ph,pL-16,y+4);ctx.strokeStyle='#0e1e18';ctx.lineWidth=.4;ctx.beginPath();ctx.moveTo(pL,y);ctx.lineTo(pL+gW,y);ctx.stroke();}
  const toY=ph=>pT+(1-ph/14)*gH;
  ctx.strokeStyle='#60b8f0';ctx.lineWidth=2;ctx.beginPath();
  for(let i=0;i<=100;i++){const x=pL+(i/100)*gW;let ph;
    if(i<4)ph=3+i*0.06;else if(i<48)ph=3.24+(i-4)*0.033;else if(i===50)ph=4.7;else if(i<88)ph=4.7+(i-50)*0.062;else if(i<93)ph=7.1+(i-88)*0.52;else ph=9.7+(i-93)*0.18;
    ph=Math.max(0,Math.min(14,ph));i===0?ctx.moveTo(x,toY(ph)):ctx.lineTo(x,toY(ph));}
  ctx.stroke();
  const hX=pL+gW*0.5,hY=toY(4.7);
  ctx.strokeStyle='#e05aff';ctx.lineWidth=1;ctx.setLineDash([3,3]);ctx.beginPath();ctx.moveTo(hX,pT);ctx.lineTo(hX,pT+gH);ctx.stroke();ctx.setLineDash([]);
  ctx.beginPath();ctx.arc(hX,hY,4,0,Math.PI*2);ctx.fillStyle='#e05aff';ctx.fill();
  ctx.fillStyle='#e05aff';ctx.font='7px JetBrains Mono,monospace';ctx.fillText('½eq: pH=pKa',hX+5,hY+4);
  const eqX=pL+gW*0.905;ctx.strokeStyle='#f5c842';ctx.lineWidth=1;ctx.setLineDash([3,3]);ctx.beginPath();ctx.moveTo(eqX,pT);ctx.lineTo(eqX,pT+gH);ctx.stroke();ctx.setLineDash([]);
  ctx.fillStyle='#f5c842';ctx.font='7px JetBrains Mono,monospace';ctx.fillText('eq>7',eqX+2,toY(8.7)-4);
}
function drawAlphaGraph(){
  const c=document.getElementById('ionicAlpha');if(!c)return;
  const ctx=c.getContext('2d'),W=c.width,H=c.height;
  ctx.fillStyle='#040c0a';ctx.fillRect(0,0,W,H);
  const pL=40,pR=12,pT=16,pB=34,gW=W-pL-pR,gH=H-pT-pB;
  ctx.strokeStyle='#1a3028';ctx.lineWidth=1;
  ctx.beginPath();ctx.moveTo(pL,pT);ctx.lineTo(pL,pT+gH);ctx.lineTo(pL+gW,pT+gH);ctx.stroke();
  ctx.fillStyle='#8090a8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('Conc (C) →',pL+gW/2-28,pT+gH+26);
  ctx.save();ctx.translate(11,pT+gH/2+14);ctx.rotate(-Math.PI/2);ctx.fillText('α, [H⁺]',0,0);ctx.restore();
  const Ka=1e-5,maxC=0.5;
  ctx.strokeStyle='#22eea8';ctx.lineWidth=2;ctx.beginPath();
  for(let i=1;i<=200;i++){const C=i/200*maxC+0.001,alpha=Math.min(1,Math.sqrt(Ka/C)),x=pL+((C-0.001)/maxC)*gW,y=pT+(1-alpha)*gH;i===1?ctx.moveTo(x,y):ctx.lineTo(x,y);}
  ctx.stroke();
  ctx.strokeStyle='#f5c842';ctx.lineWidth=1.5;ctx.setLineDash([4,3]);ctx.beginPath();
  for(let i=1;i<=200;i++){const C=i/200*maxC+0.001,H=Math.sqrt(Ka*C),norm=H/Math.sqrt(Ka*maxC)*0.45,x=pL+((C-0.001)/maxC)*gW,y=pT+(1-norm)*gH;i===1?ctx.moveTo(x,y):ctx.lineTo(x,y);}
  ctx.stroke();ctx.setLineDash([]);
  ctx.fillStyle='#22eea8';ctx.font='8px JetBrains Mono,monospace';ctx.fillText('α = √(Ka/C)',pL+4,pT+13);
  ctx.fillStyle='#f5c842';ctx.fillText('[H⁺]=√(Ka·C)',pL+4,pT+25);
}

// ── Unified showSection extension ──
(function(){
  const _base = window.showSection;
  let _ptBuiltLocal = false, _tDrewThermo = false, _tDrewIonic = false;
  window.showSection = function(id) {
    _base(id);
    if (id === 'ptable' && !_ptBuiltLocal) {
      _ptBuiltLocal = true;
      setTimeout(ptBuildGrid, 60);
    }
    if (id === 'rotdyn') {
      setTimeout(() => { try { rdStartAnimations(); } catch(e) {} }, 100);
    }
    if (id === 'thermo' && !_tDrewThermo) {
      _tDrewThermo = true;
      setTimeout(() => {
        try { drawThermoGGraph(); } catch(e) {}
        try { drawThermoPVGraph(); } catch(e) {}
        try { drawThermoEnergyGraph(); } catch(e) {}
      }, 80);
    }
    if (id === 'ionic' && !_tDrewIonic) {
      _tDrewIonic = true;
      setTimeout(() => {
        try { drawTitration1(); } catch(e) {}
        try { drawTitration2(); } catch(e) {}
        try { drawAlphaGraph(); } catch(e) {}
      }, 80);
    }
  };
})();

/* ── SNAV ANCHOR FIX: smooth scroll within sections ── */
document.addEventListener('click', function(e) {
  const anchor = e.target.closest('a[href^="#"]');
  if (!anchor) return;
  const target = document.querySelector(anchor.getAttribute('href'));
  if (target) {
    e.preventDefault();
    setTimeout(() => {
      const topnav = document.getElementById('topnav');
      const navH = topnav ? topnav.offsetHeight : 0;
      const y = target.getBoundingClientRect().top + window.scrollY - navH - 12;
      window.scrollTo({ top: y, behavior: 'smooth' });
    }, 30);
  }
});

</script>
</body></html>
