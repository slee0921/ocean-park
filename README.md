<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Ocean Park Digital Marketing</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Inter+Tight:wght@600;700;800&display=swap">
<style>
/* VOICE: a student team's case-study site, clear and confident, easy to present from by scrolling
   IDEA: an editorial microsite for the report — hero, sticky section nav, chapters that unfold as you scroll
   PICTURE: the park entrance photo as hero; the team's screenshots and live charts inside each chapter
   COLOUR and TYPE: the deck's palette — cream ground, navy ink, steel-blue panels, platform colours; Inter Tight headings, Inter body
   LAYOUT: full-width bands, content up to 1200px, two-column rows that stack under 820px */
:root{color-scheme:light;--bg:#F5F3EF;--paper:#fff;--ink:#2E3A46;--navy:#23476B;--blue:#4D7FA3;--grey:#5F6B78;--line:#D5DEE5;--p1:#DCE7EE;--p2:#CFDDE6;--coral:#C25F3B;--ct:#3D6FD1;--gg:#E0703C;--ta:#3E9E6E;--sea:#54A5BE}
*{box-sizing:border-box;min-width:0}
html{scroll-behavior:smooth;scroll-padding-top:76px;overflow-x:clip}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}.rv{opacity:1!important;transform:none!important}}
body{margin:0;background:var(--bg);color:var(--ink);font:17px/1.6 Inter,system-ui,sans-serif;overflow-x:clip}
h1,h2,h3{font-family:"Inter Tight",Inter,sans-serif;color:var(--navy);margin:0;line-height:1.1;text-wrap:balance}
a{color:var(--blue)}
img{max-width:100%;display:block}
button{font:inherit;color:inherit;cursor:pointer}
:focus-visible{outline:3px solid var(--blue);outline-offset:3px;border-radius:4px}
.wrap{max-width:1200px;margin:0 auto;padding:0 max(4vw,18px)}
/* header */
.nav{position:sticky;top:0;z-index:10;background:rgba(245,243,239,.9);backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
.nav .wrap{display:flex;align-items:center;gap:20px;height:64px}
.brand{display:flex;gap:8px;align-items:center;font:800 17px "Inter Tight",sans-serif;color:var(--navy);text-decoration:none;white-space:nowrap}
.links{display:flex;gap:4px;margin-left:auto;overflow-x:auto;scrollbar-width:none}
.links a{flex:none;text-decoration:none;color:var(--grey);font-weight:600;font-size:15px;padding:10px 14px;border-radius:999px;min-height:44px;display:flex;align-items:center}
.links a.on{background:var(--navy);color:#fff}
.links a:hover:not(.on){background:var(--p1);color:var(--navy)}
.prog{position:absolute;left:0;bottom:-1px;height:3px;width:0;background:var(--sea)}
/* hero */
.hero{position:relative;min-height:min(86vh,760px);display:grid;align-items:end;overflow:hidden;background:#cfe3ee}
.hero .ph{position:absolute;inset:0 0 0 38%;background:url(img/cover.jpg) 50% 35%/cover}
.hero::after{content:"";position:absolute;inset:0;background:linear-gradient(90deg,rgba(245,243,239,1) 0%,rgba(245,243,239,1) 38%,rgba(245,243,239,0) 62%),linear-gradient(0deg,rgba(245,243,239,1) 0%,rgba(245,243,239,0) 26%)}
.hero .wrap{position:relative;z-index:1;width:100%;padding-top:70px;padding-bottom:56px}
.tagline{display:flex;gap:10px;align-items:center;font:800 16px "Inter Tight",sans-serif;color:var(--navy);letter-spacing:.5px}
.hero h1{font-size:clamp(56px,10vw,120px);font-weight:800;letter-spacing:-3px;line-height:.95;margin:18px 0 8px}
.hero .sub{font-size:clamp(22px,3vw,32px);color:var(--navy);margin:0 0 36px}
.team{display:grid;grid-template-columns:repeat(3,auto);gap:4px 28px;width:max-content;max-width:100%;font-size:16px;color:var(--navy);border-top:3px solid var(--blue);padding-top:14px}
.team b{grid-column:1/-1;font-size:14px;letter-spacing:1px}
.agenda{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:14px;margin-top:-30px;position:relative;z-index:2}
.agenda a{background:var(--paper);border-radius:14px;padding:18px 20px;text-decoration:none;color:var(--navy);box-shadow:0 8px 24px rgba(35,71,107,.1);transition:transform .2s,box-shadow .2s;display:block}
.agenda a:hover{transform:translateY(-3px);box-shadow:0 14px 30px rgba(35,71,107,.16)}
.agenda b{display:block;font:800 34px "Inter Tight",sans-serif;color:var(--blue)}
.agenda span{font-weight:700;font-size:16px}
/* chapters */
.chap{padding:96px 0 40px}
.chead{display:flex;align-items:flex-end;gap:22px;margin-bottom:42px;border-bottom:1px solid var(--line);padding-bottom:22px}
.chead .n{font:800 clamp(64px,9vw,112px)/.85 "Inter Tight",sans-serif;color:transparent;-webkit-text-stroke:2px var(--blue)}
.chead h2{font-size:clamp(34px,5vw,56px);font-weight:800;letter-spacing:-1px}
.chead p{margin:6px 0 0;color:var(--grey);max-width:60ch}
.sub2{display:flex;align-items:center;gap:14px;margin:64px 0 24px}
.sub2 h3{font-size:clamp(24px,3vw,32px)}
.sub2 .tag{font-size:13px;font-weight:700;color:var(--blue);background:var(--p1);padding:4px 12px;border-radius:999px;white-space:nowrap}
.lede{font-size:19px;max-width:70ch;margin:-8px 0 28px}
/* blocks */
.row{display:grid;grid-template-columns:minmax(0,1fr) minmax(0,1.05fr);gap:44px;align-items:center;padding:34px 0;border-bottom:1px solid var(--line)}
.row.flip>:first-child{order:2}
.row h4{font:700 26px/1.2 "Inter Tight",sans-serif;color:var(--navy);margin:0 0 16px}
.row h4 small{display:block;font:700 13px Inter,sans-serif;color:var(--blue);letter-spacing:1px;margin-bottom:6px}
.card{background:var(--p1);border-radius:16px;padding:20px 24px}
.card.dark{background:var(--navy);color:#fff}.card.dark h5{color:#9EC3DA}
.card.mid{background:var(--p2)}
.card h5{margin:0 0 4px;font-size:13px;letter-spacing:1.5px;color:var(--blue)}
.card h6{margin:0 0 6px;font-size:18px;color:var(--navy)}
.flow{display:flex;justify-content:center;color:var(--blue);padding:6px 0}
ul{margin:0;padding-left:20px}li{margin:4px 0}ul ul{list-style:circle}
.shots{display:flex;gap:16px;justify-content:center;align-items:flex-start}
.shot{border-radius:10px;border:1px solid #D9DFE5;background:#fff;box-shadow:0 10px 30px rgba(35,71,107,.14);cursor:zoom-in;transition:transform .25s}
.shot:hover{transform:translateY(-4px)}
.shots .shot{max-height:460px;width:auto}
.recs{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:22px;align-items:start}
.rec{background:var(--paper);border-radius:18px;padding:26px;box-shadow:0 6px 20px rgba(35,71,107,.08);display:flex;flex-direction:column;gap:16px}
.rec h4{margin:0;font:700 22px/1.2 "Inter Tight",sans-serif;color:var(--navy)}
.rec h4 small{display:block;font:700 13px Inter,sans-serif;color:var(--blue);letter-spacing:1px;margin-bottom:4px}
.rec ul{font-weight:600;color:var(--navy)}.rec ul ul{color:var(--blue);font-weight:500}
.pill{border-radius:12px;padding:14px 18px;text-align:center;font-weight:700;letter-spacing:.8px}
.pill.l{background:var(--p1);color:var(--blue)}.pill.m{background:var(--blue);color:#fff}.pill.d{background:var(--navy);color:#fff}
.outcome{color:var(--blue);font-weight:700;text-align:center;font-size:20px;line-height:1.5}
/* social */
.tabs{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:26px}
.tabs button{border:1px solid var(--line);background:var(--paper);border-radius:999px;padding:10px 20px;min-height:44px;font-weight:700;color:var(--navy);display:flex;gap:8px;align-items:center}
.tabs button[aria-selected=true]{background:var(--navy);color:#fff;border-color:var(--navy)}
.dot{display:inline-block;width:11px;height:11px;border-radius:50%;flex:none}
.plat{display:grid;grid-template-columns:minmax(0,.9fr) minmax(0,1.1fr);gap:44px;align-items:center}
.plat .imgs{display:grid;gap:16px;justify-items:center}
.plat .imgs .shot{max-height:300px;width:auto}
.pt{display:flex;gap:18px;padding:20px 0;border-top:1px solid var(--line)}.pt:first-child{border-top:0}
.num{flex:none;width:42px;height:42px;border-radius:50%;background:var(--blue);color:#fff;display:grid;place-items:center;font-weight:700;font-size:15px}
.num.s{width:32px;height:32px;font-size:13px}
.pt b{display:block;color:var(--navy);font-size:19px}
.feature{display:grid;grid-template-columns:minmax(0,1.1fr) minmax(0,1fr);gap:28px;align-items:start}
.stats{display:flex;gap:30px;flex-wrap:wrap}
.stat{color:var(--navy)}.stat b{display:block;font:800 clamp(34px,4vw,46px)/1 "Inter Tight",sans-serif}
.callout{display:flex;gap:18px;align-items:center;background:var(--navy);color:#fff;border-radius:16px;padding:20px 24px;font-weight:700}
/* sentiment */
.sec{display:flex;align-items:center;gap:12px;margin:0 0 14px}.sec h4{margin:0;font:700 22px "Inter Tight",sans-serif;color:var(--navy)}
.grid2{display:grid;grid-template-columns:minmax(0,1fr) minmax(0,1fr);gap:28px}
.panel{background:var(--paper);border-radius:18px;padding:24px;box-shadow:0 6px 20px rgba(35,71,107,.07)}
.big{font:800 clamp(32px,4vw,44px)/1 "Inter Tight",sans-serif;color:var(--navy);white-space:nowrap}
.rr{display:grid;grid-template-columns:minmax(0,1.3fr) 80px minmax(0,1.4fr);gap:12px;align-items:center;padding:12px 0;border-bottom:1px solid var(--line)}
.rr.h{font-size:13px;font-weight:700;color:var(--navy);padding-top:0}
.bar{height:12px;border-radius:6px;background:#E6E9EC;position:relative;overflow:hidden;flex:1}
.bar i{position:absolute;inset:0 auto 0 0;width:0;background:var(--coral);border-radius:6px;transition:width 1s .2s}
.three{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:24px}
.legend{display:flex;gap:16px;flex-wrap:wrap;font-size:14px}.legend span{display:flex;gap:6px;align-items:center}
.note{font-size:13px;color:var(--grey);margin-top:16px}
.quote{background:#fff;border:1px solid #E3E6EA;border-radius:12px;padding:12px 16px;margin-bottom:10px}
.emo{display:grid;grid-template-columns:minmax(0,1.2fr) minmax(0,.9fr) minmax(0,1.2fr);gap:10px;padding:14px 4px;border-bottom:1px solid var(--line);align-items:start}
.steps>div{display:flex;gap:16px;position:relative;padding-bottom:22px}
.steps>div:not(:last-child)::before{content:"";position:absolute;left:27px;top:56px;bottom:0;border-left:1.5px solid #9DB3C9}
.ring{flex:none;width:56px;height:56px;border-radius:50%;border:2px solid var(--navy);display:grid;place-items:center;font-size:26px;color:var(--navy);background:var(--bg)}
.booking{border:1.5px solid #9DB3C9;border-radius:14px;background:#fff;padding:16px 20px}
.booking>div{display:flex;gap:14px;align-items:center;padding:12px 4px;border-bottom:1px solid var(--line)}
.booking>div:last-child{border:0}
svg.i{width:1em;height:1em;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round;flex:none}
.fig svg{width:100%;height:auto;overflow:visible;display:block}
/* refs + end */
.refs p{padding-left:32px;text-indent:-32px;margin:0 0 18px;overflow-wrap:anywhere}
.end{margin-top:80px;background:var(--navy);color:#fff;position:relative;overflow:hidden}
.end::before{content:"";position:absolute;right:-120px;top:-140px;width:520px;height:480px;border-radius:46% 54% 40% 60%;background:radial-gradient(circle at 30% 30%,#53C3C9,#2F5E9C 70%);opacity:.6;filter:blur(20px)}
.end .wrap{position:relative;padding-top:90px;padding-bottom:90px}
.end h2{color:#fff;font-size:clamp(48px,8vw,96px);font-weight:500;letter-spacing:-2px;line-height:.95}.end h2 b{display:block;font-weight:800}
.end p{color:#C9DCE8;margin-top:22px}
/* reveal */
.rv{opacity:0;transform:translateY(26px);transition:opacity .7s,transform .7s}
.rv.in{opacity:1;transform:none}
/* lightbox */
.lb{position:fixed;inset:0;background:rgba(15,28,42,.86);display:none;align-items:center;justify-content:center;z-index:30;padding:20px}
.lb.on{display:flex}.lb img{max-width:94vw;max-height:88vh;border-radius:8px;background:#fff}
.lb button{position:absolute;top:16px;right:16px;width:44px;height:44px;border-radius:50%;border:0;background:#fff;font-size:18px}
.next{position:fixed;right:22px;bottom:22px;z-index:9;width:52px;height:52px;border-radius:50%;border:0;background:var(--navy);color:#fff;font-size:24px;display:grid;place-items:center;box-shadow:0 8px 20px rgba(35,71,107,.3)}
@media(max-width:820px){.hero .ph{inset:0 0 45% 0}.row,.row.flip,.plat,.feature,.grid2,.recs{grid-template-columns:minmax(0,1fr)}.row.flip>:first-child{order:0}.agenda{grid-template-columns:repeat(2,minmax(0,1fr));margin-top:16px}.three{grid-template-columns:minmax(0,1fr)}.hero::after{background:linear-gradient(0deg,rgba(245,243,239,1) 0%,rgba(245,243,239,.92) 55%,rgba(245,243,239,.2) 100%)}.team{grid-template-columns:repeat(2,auto)}.shots .shot{max-height:360px}.links a{padding:10px}.brand span{display:none}}
@media(max-width:520px){body{font-size:16px}.emo{grid-template-columns:minmax(0,1fr) minmax(0,1fr)}.emo>:last-child{grid-column:1/-1}.rr{grid-template-columns:minmax(0,1fr) 60px minmax(0,1fr)}.next{display:none}}
</style>
</head>
<body>

<header class="nav"><div class="wrap">
  <a class="brand" href="#top"><svg class="i" viewBox="0 0 24 24" style="font-size:24px;color:var(--blue)"><path d="M2 12l5 5L18 6M9 15l2 2L22 6"/></svg><span>MASTERS</span></a>
  <nav class="links" aria-label="Sections"><a href="#webpage">01 Webpage</a><a href="#social">02 Social media</a><a href="#sentiment">03 Online sentiment</a><a href="#refs">Reference</a></nav>
</div><i class="prog" id="prog"></i></header>

<section class="hero" id="top">
  <div class="ph" role="img" aria-label="Ocean Park Hong Kong entrance"></div>
  <div class="wrap">
    <div class="tagline"><svg class="i" viewBox="0 0 24 24" style="font-size:26px;color:var(--blue)"><path d="M2 12l5 5L18 6M9 15l2 2L22 6"/></svg>TEAM: MASTERS</div>
    <h1>Ocean Park</h1>
    <p class="sub">Digital Marketing Strategy</p>
    <div class="team"><b>TEAM MASTERS</b><span>Soyoon Lee</span><span>Cheung Wai Wai</span><span>Gu Xiang</span><span>Duan Zhangjiayi</span><span>Yao Yuan</span><span>Ip Po Man</span></div>
  </div>
</section>
<div class="wrap"><nav class="agenda" aria-label="Agenda">
  <a href="#webpage"><b>01</b><span>WEBPAGE</span></a><a href="#social"><b>02</b><span>SOCIAL MEDIA</span></a><a href="#sentiment"><b>03</b><span>ONLINE SENTIMENT</span></a><a href="#sent-recs"><b>04</b><span>CONCLUSION</span></a></nav></div>

<!-- 01 WEBPAGE -->
<section class="chap" id="webpage"><div class="wrap">
  <div class="chead rv"><span class="n">01</span><div><h2>WEBPAGE</h2></div></div>
  <div class="sub2 rv"><h3>Issues</h3><span class="tag">4 issues</span></div>
  <div id="issues"></div>
  <div class="sub2 rv"><h3>Recommendations</h3><span class="tag">Webpage</span></div>
  <div class="recs">
    <article class="rec rv"><h4><small>RECOMMENDATION 1</small>Streamlining Navigation</h4>
      <img class="shot" src="img/rec1.jpg" alt="Mock-up of a streamlined Plan Your Visit page">
      <ul><li>Plan Your Visit<ul><li>Opening hours</li><li>Daily schedules</li><li>Transport</li><li>Park Maps</li></ul></li><li>Tickets &amp; Offers</li><li>Attractions &amp; Experiences</li><li>Membership</li><li>Conservation &amp; Education</li></ul></article>
    <article class="rec rv"><h4><small>RECOMMENDATION 2</small>Improving Content Prioritization</h4>
      <div class="pill l">Compact Sections &gt; Discrete Sections</div><div class="pill m">Priortize Selected Promotions</div><div class="pill d">“Buy Ticket” Call-to-Action</div>
      <div class="outcome">Clearer Visual Hierarchy<div class="flow"><i data-i="chev"></i></div>Reduce Information Overload</div></article>
    <article class="rec rv"><h4><small>RECOMMENDATION 3</small>Legacy Content Governance</h4>
      <ul><li>2026/07/01: Suspension <span style="color:var(--blue)">of the Ocean Park Hong Kong App</span></li><li>Accessible Legacy Guest Service Page → Outdated Download Instructions</li><li>301 redirects</li><li>Obsolete pages should be removed</li></ul>
      <div class="pill d">Information Consistency<div class="flow" style="color:#fff"><i data-i="chev"></i></div>Confusion↓ &amp; Reliability↑</div></article>
    <article class="rec rv"><h4><small>RECOMMENDATION 4</small>User Intent &amp; Mobile Ticketing Improvement</h4>
      <ul><li><span style="color:var(--blue)">Align</span> Search Results <span style="color:var(--blue)">with</span> Different User Intentions<ul><li>“香港 海洋公园” → Official Simplified Chinese homepage</li><li>Ticket-related → Ticket Selection</li></ul></li><li>Headlines show Clear Differences</li><li>Consitent Mobile Experience<ul><li>Visual Styling</li><li>Responsive Navigation</li><li>Clearer Language Options</li></ul></li><li>Loading Performance</li></ul>
      <div class="pill m">Localized Titles &amp; Searching Indexing (SEO)<div class="flow" style="color:#fff"><i data-i="chev"></i></div>Improve Organic Visibility</div>
      <div class="pill d">Seamless Transition from Information Searching to Ticketing<div class="flow" style="color:#fff"><i data-i="chev"></i></div>Reduce Confusion &amp; Potential Abandonment</div></article>
  </div>
</div></section>

<!-- 02 SOCIAL -->
<section class="chap" id="social"><div class="wrap">
  <div class="chead rv"><span class="n">02</span><div><h2>SOCIAL MEDIA</h2></div></div>
  <div class="sub2 rv"><h3>Social Media Performance</h3></div>
  <div class="tabs rv" role="tablist" id="tabs"></div>
  <div class="panel rv" id="platPanel" role="tabpanel"></div>

  <div class="sub2 rv"><h3>Social Media Campaign Study</h3><span class="tag">OCEAN PARK - “Panda Monium”</span></div>
  <div class="feature rv">
    <div><img class="shot" src="img/panda.jpg" alt="Panda twins first birthday campaign poster" style="border:0;border-radius:20px;width:100%">
      <img src="img/award.jpg" alt="Winner of MarTech APAC NEXT Awards 2026 Hong Kong and iab HK" style="height:96px;width:auto;margin-top:14px;mix-blend-mode:multiply"></div>
    <div style="display:grid;gap:16px">
      <div class="card"><h6>“PANDA FAMILY”</h6><ul><li>Panda family: Ying ying, Le le (the parents); Jia jia, De de (twins, born in HK); An an, Ke ke (new arrivals)</li><li>Personification of pandas</li></ul></div>
      <div class="card mid"><h6>OMNI-STRATEGY</h6><ul><li>As mentioned, the social media matrix of Ocean Park covers large variety of consumer segments.</li></ul></div>
      <div class="callout"><i data-i="bulb" style="font-size:40px"></i>SOCIAL MEDIA SERVES AS AN AMPLIFIER OF THE EFFECT OF THIS CUTE CAMPAIGN.</div>
    </div>
  </div>
  <div class="grid2" style="margin-top:28px">
    <div class="panel rv"><div class="sec"><span class="num s">01</span><h4>LIVE-STREAMS: MULTI PLATFORMS</h4></div>
      <div class="stats" style="margin:6px 0 16px"><div class="stat"><i data-i="eye" style="font-size:30px"></i><b>29.8M</b></div><div class="stat"><i data-i="phone" style="font-size:30px"></i><b>17.6M</b></div><div class="stat"><i data-i="thumb" style="font-size:30px"></i><b>21.4K</b></div></div>
      <ul><li>Streamed the panda twins’ first birthday party across major platforms</li><li>Reached both mainland, local, and international audiences → supported global brand awareness</li><li>Live format also encouraged real-time engagement and social buzz.</li></ul></div>
    <div class="panel rv"><div class="sec"><span class="num s">02</span><h4>DEDICATED ACCOUNT: @PANDAHKOFFICIAL</h4></div>
      <div style="display:flex;gap:20px;align-items:center;margin:6px 0 16px;flex-wrap:wrap"><img class="shot" src="img/phk.jpg" alt="@pandahkofficial profile" style="height:100px;width:auto;border:0">
        <div class="stats"><div class="stat"><i data-i="userplus" style="font-size:30px"></i><b>75K</b></div><div class="stat"><i data-i="thumb" style="font-size:30px"></i><b>1.7+M</b></div></div></div>
      <ul><li>Build distinctive brand IP through personalities, family roles and human-like emotion</li><li>Creates an emotional connection</li><li>Maintains long-term engagement through regular update - “virtual panda raising”→ Consumer Loyalty</li></ul></div>
  </div>
  <div class="callout rv" style="margin-top:22px"><i data-i="bulb" style="font-size:34px"></i>Ocean Park’s multi-channel strategy builds broad awareness and audience loyalty, but focusing resources on high-performing platforms and tailoring content to each audience could improve engagement quality.</div>
</div></section>

<!-- 03 SENTIMENT -->
<section class="chap" id="sentiment"><div class="wrap">
  <div class="chead rv"><span class="n">03</span><div><h2>ONLINE SENTIMENT</h2></div></div>

  <div class="sub2 rv"><h3>Rating Overview</h3></div>
  <p class="lede rv">Ctrip and Google Maps reviewers rate the park highly. TripAdvisor reviewers are far more critical, and their ratings have not returned to pre-COVID levels.</p>
  <div class="grid2">
    <div class="panel rv"><div class="sec"><span class="num s">01</span><h4>Ratings by platform</h4></div>
      <div class="rr h"><span>Platform</span><span>Avg rating</span><span>Negative share <span style="color:var(--grey);font-weight:500">(1–2★)</span></span></div><div id="rateRows"></div></div>
    <div class="panel rv"><div class="sec"><span class="num s">02</span><h4>TripAdvisor rating by year</h4></div>
      <div class="fig"><svg id="line" viewBox="0 0 600 215" role="img" aria-label="TripAdvisor average stars by year, 2017 to 2026"></svg></div>
      <div style="font-size:14px;margin-top:6px"><b style="color:var(--coral)">COVID low</b> <span style="color:var(--grey)">park closed for almost a third of FY2021–22 (Ng, 2022)</span></div></div>
  </div>
  <div class="panel rv" style="margin-top:24px;background:var(--p2);box-shadow:none"><div class="sec"><span class="num s">03</span><h4>Why TripAdvisor reviewers are harsher</h4></div>
    <div class="three">
      <div><b style="color:var(--navy);display:flex;gap:8px;align-items:center"><span class="dot" style="background:var(--ta)"></span>Different audience</b><div class="big" style="margin:6px 0">79%</div><div style="font-size:15px">of TripAdvisor reviewers with a listed home live outside HK, mainland China and Taiwan</div></div>
      <div><b style="color:var(--navy);display:flex;gap:8px;align-items:center"><span class="dot" style="background:var(--ta)"></span>Stricter on vlaue</b><div class="big" style="margin:6px 0">24% vs 6-8%</div><div style="font-size:15px">of recent written reviews criticise price or ageing facilities (vs Ctrip and Google)</div></div>
      <div><b style="color:var(--navy);display:flex;gap:8px;align-items:center"><span class="dot" style="background:var(--gg)"></span>Low-effort ratings</b><div class="big" style="margin:6px 0">768 of 1,378</div><div style="font-size:15px">Google Maps reviews in 2026 are stars only, with no text</div></div></div></div>
  <p class="note">Comparison sample: Ctrip 1,710 and Google Maps 1,378 reviews (2026), TripAdvisor 145 (2023–26). Trend uses 2,050 dated TripAdvisor reviews, 2017–26. Home location self-reported by 105 TripAdvisor reviewers.</p>

  <div class="sub2 rv"><h3>Topics and Emotions</h3></div>
  <p class="lede rv">Family visits led on Ctrip and rides led on Google Maps and TripAdvisor. Enjoyment was the most common emotion on all three.</p>
  <div class="grid2">
    <div class="panel rv"><div class="sec"><span class="num s">01</span><h4>Most-mentioned topics</h4></div>
      <div style="font-size:14px;color:var(--grey)">Share of written reviews mentioning each topic</div>
      <div class="legend" style="margin:8px 0"><span><i class="dot" style="background:var(--ct)"></i>Ctrip</span><span><i class="dot" style="background:var(--gg)"></i>Google Maps</span><span><i class="dot" style="background:var(--ta)"></i>TripAdvisor</span><span style="margin-left:auto;font-weight:700;color:var(--navy)">Overall</span></div>
      <div class="fig"><svg id="topics" viewBox="0 0 560 150" role="img" aria-label="Topic shares by platform"></svg></div></div>
    <div class="panel rv"><div class="sec"><span class="num s">02</span><h4>Leading positive and negative emotions</h4></div>
      <div class="emo" style="background:var(--p1);border-radius:10px;border:0;font-size:13px;font-weight:700;color:var(--navy);padding:10px 12px"><span>Emotion</span><span>Reviews<small style="display:block;font-weight:500;color:var(--grey)">Share of all reviews</small></span><span>Most frequent topic<small style="display:block;font-weight:500;color:var(--grey)">Share within emotion</small></span></div>
      <div class="emo"><b style="color:var(--navy);display:flex;gap:8px"><i data-i="smile" style="font-size:24px;color:#4E8B95"></i>Enjoyment</b><span style="color:#3F7A83;font-weight:700">368 (14.9%)<i style="display:block;height:5px;width:90%;background:#4E8B95;border-radius:3px;margin-top:4px"></i></span><span><b style="color:var(--navy)">Family and children</b><br><small>154 of 368 (41.8%)</small></span></div>
      <div class="emo" style="border:0"><b style="color:var(--navy);display:flex;gap:8px"><i data-i="frown" style="font-size:24px;color:var(--coral)"></i>Disappointment or regret</b><span style="color:var(--coral);font-weight:700">73 (3.0%)<i style="display:block;height:5px;width:18%;background:var(--coral);border-radius:3px;margin-top:4px"></i></span><span><b style="color:var(--navy)">Rides</b><br><small>27 of 73 (37.0%)</small></span></div></div>
  </div>
  <div class="sec rv" style="margin-top:28px"><span class="num s">03</span><h4>Specific topics that stand out</h4></div>
  <div class="grid2">
    <div class="card rv" style="display:flex;gap:16px;align-items:center"><img src="img/icon-panda.jpg" alt="" style="width:56px;border-radius:50%"><div><b style="color:var(--navy);font-size:20px">Pandas</b> <b style="color:var(--navy);font-size:15px">334 reviews (13.5%)</b><br><i>“the main reason for my visit”</i> <small style="color:var(--grey)">TripAdvisor</small></div></div>
    <div class="card rv" style="display:flex;gap:16px;align-items:center"><img src="img/icon-pumpkin.jpg" alt="" style="width:56px;border-radius:50%"><div><b style="color:var(--navy);font-size:20px">Halloween</b> <b style="color:var(--navy);font-size:15px">43 reviews (1.7%)</b><br><i>“Halloween Fest is the only reason I go each year.”</i> <small style="color:var(--grey)">Ctrip</small></div></div>
  </div>
  <div class="card mid rv" style="margin-top:24px;display:grid;grid-template-columns:minmax(0,1fr) minmax(0,.9fr);gap:24px" id="conc">
    <div><div class="sec" style="margin-bottom:4px"><span class="num s">04</span><h4>Concerns in four- and five-star reviews</h4></div>
      <div style="font-size:14px">Share of highly rated written reviews with mixed or negative comments</div>
      <div class="stats" style="margin-top:10px"><div class="stat"><small style="display:flex;gap:6px;align-items:center"><i class="dot" style="background:var(--ct)"></i><b style="font:700 14px Inter">Ctrip</b></small><b>12.4%</b></div><div class="stat"><small style="display:flex;gap:6px;align-items:center"><i class="dot" style="background:var(--gg)"></i><b style="font:700 14px Inter">Google Maps</b></small><b>16.9%</b></div><div class="stat"><small style="display:flex;gap:6px;align-items:center"><i class="dot" style="background:var(--ta)"></i><b style="font:700 14px Inter">TripAdvisor</b></small><b>39.4%</b></div></div></div>
    <div class="quote" style="margin:0"><div style="display:flex;justify-content:space-between;gap:10px"><b style="color:var(--navy)">TripAdvisor reviewer</b><b style="color:var(--ta);white-space:nowrap">5/5 ●●●●●</b></div><small style="color:var(--grey)">9 Dec 2024</small><div style="font-weight:700;color:var(--navy)">Nice family outing place</div>“My 6-year-old son loved the jellyfish display but was greatly disappointed that he was not allowed to take the bumper car ride”</div>
  </div>
  <p class="note">Sample of 2,465 written reviews • Ctrip 1,710 (69.4%), Google Maps 610 (24.7%), TripAdvisor 145 (5.9%). Ctrip and Google Maps cover 2026, TripAdvisor 2023–26.</p>

  <div class="sub2 rv"><h3>Complaints</h3></div>
  <p class="lede rv">Closed rides and price are the only complaints in the top three on every platform. Some visitors only learn about closures once they arrive.</p>
  <div class="grid2" style="grid-template-columns:minmax(0,1.25fr) minmax(0,1fr)">
    <div class="panel rv"><div class="sec"><span class="num s">01</span><h4>Most common complaints</h4></div>
      <div style="font-size:14px">Share of 1–3★ written reviews mentioning each topic</div>
      <div class="legend" style="margin:8px 0"><span><i class="dot" style="background:var(--ct)"></i>Ctrip</span><span><i class="dot" style="background:var(--gg)"></i>Google Maps</span><span><i class="dot" style="background:var(--ta)"></i>TripAdvisor</span></div>
      <div class="fig"><svg id="compl" viewBox="0 0 640 330" role="img" aria-label="Complaint shares by platform"></svg></div></div>
    <div class="rv"><div class="sec"><span class="num s">02</span><h4>Closures in visitors' words</h4></div>
      <div class="quote"><small style="display:flex;gap:6px;align-items:center"><i class="dot" style="background:var(--ct)"></i><b style="color:var(--navy)">Ctrip</b> <span style="color:var(--grey)">3★ · Jul 2026</span></small><i>"Roller coaster was closed the day we went"</i></div>
      <div class="quote"><small style="display:flex;gap:6px;align-items:center"><i class="dot" style="background:var(--ta)"></i><b style="color:var(--navy)">TripAdvisor</b> <span style="color:var(--grey)">2★ · Apr 2026</span></small><i>"disappointing overall as the park's main rides are largely closed"</i></div>
      <div class="card mid" style="margin-top:18px"><div class="sec"><span class="num s">03</span><h4>Told too late</h4></div>
        <div class="big" style="color:var(--coral)">~1 in 10</div><div style="margin-top:6px">TripAdvisor closure complaints say visitors were not told before arriving</div>
        <div style="font-size:14px;color:var(--grey);margin-top:10px">Most date from 2017–2019, and closures are listed on the website, so the information exists but is easy to miss.</div></div></div>
  </div>
  <p class="note">Sample: 1–3★ written reviews — Ctrip 99 (2026), Google Maps 101 (2026), TripAdvisor 46 (2023–26). Keyword tagging; a review can mention several topics. Closure figure based on 128 TripAdvisor closure complaints, 2017–26.</p>

  <div class="sub2 rv" id="sent-recs"><h3>Recommendations</h3><span class="tag">Online sentiment</span></div>
  <p class="lede rv">Visitors reported unexpected closures and raised concerns even in four- and five-star reviews.</p>
  <div class="grid2">
    <div class="panel rv"><div class="sec"><span class="num">01</span><h4>Show ride availability at booking</h4></div>
      <div class="booking"><div style="border:1.5px solid #9DB3C9;border-radius:10px;padding:10px 14px;margin-bottom:6px"><i data-i="cal" style="font-size:24px;color:var(--navy)"></i>Select a visit date<i data-i="chev" style="margin-left:auto;font-size:20px"></i></div>
        <div><i data-i="ban" style="font-size:26px;color:var(--coral)"></i>Flag scheduled closures</div><div><i data-i="arrow" style="font-size:26px;color:#3F7A83"></i>Suggest open alternatives</div><div><i data-i="ruler" style="font-size:26px;color:var(--navy)"></i>Show age and height requirements</div></div></div>
    <div class="panel rv"><div class="sec"><span class="num">02</span><h4>Reply across all star ratings</h4></div><div class="steps" id="steps"></div></div>
  </div>
  <div class="card rv" style="margin-top:22px;display:flex;flex-wrap:wrap;gap:14px 36px;align-items:center;font-size:17px"><b style="font:700 21px 'Inter Tight',sans-serif;color:var(--navy)">Track monthly by platform</b><span>Priority reviews answered (%)</span><span>Median time to first reply</span></div>
</div></section>

<section class="chap" id="refs" style="padding-top:64px"><div class="wrap refs">
  <div class="sub2" style="margin-top:0"><h3>Reference</h3></div>
  <p>Ctrip. (n.d.). 香港海洋公园 [Ocean Park Hong Kong] [Visitor reviews]. Retrieved November 17, 2026, from <a href="https://you.ctrip.com/sight/hongkong38/3339.html">https://you.ctrip.com/sight/hongkong38/3339.html</a></p>
  <p>Google. (n.d.). Ocean Park Hong Kong [Visitor ratings and reviews]. Google Maps. Retrieved November 20, 2026, from <a href="https://www.google.com/maps/search/?api=1&amp;query=Ocean+Park+Hong+Kong&amp;query_place_id=ChIJ4SEGMiQABDQRRhn7SYWq0fM">https://www.google.com/maps/search/?api=1&amp;query=Ocean+Park+Hong+Kong&amp;query_place_id=ChIJ4SEGMiQABDQRRhn7SYWq0fM</a></p>
  <p>Tripadvisor. (n.d.). Ocean Park [Visitor reviews]. Retrieved November 20, 2026, from <a href="https://www.tripadvisor.com/Attraction_Review-g294217-d317431-Reviews-Ocean_Park-Hong_Kong.html">https://www.tripadvisor.com/Attraction_Review-g294217-d317431-Reviews-Ocean_Park-Hong_Kong.html</a></p>
</div></section>

<footer class="end"><div class="wrap">
  <h2>THANK YOU<b>VERY MUCH</b></h2>
  <p>TEAM MASTERS · Soyoon Lee · Cheung Wai Wai · Gu Xiang · Duan Zhangjiayi · Yao Yuan · Ip Po Man</p>
</div></footer>

<button class="next" id="nextB" aria-label="Next section"><svg class="i" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg></button>
<div class="lb" id="lb"><button aria-label="Close">✕</button><img id="lbImg" alt=""></div>

<script>
{
const IC={eye:'<path d="M2 12s3-7 10-7 10 7 10 7-3 7-10 7-10-7-10-7Z"/><circle cx="12" cy="12" r="3"/>',
phone:'<rect x="5" y="2" width="14" height="20" rx="2"/><path d="M9 6h6M9 10h6M9 14h6M12 18h.01"/>',
thumb:'<path d="M7 10v12"/><path d="M15 5.88 14 10h5.83a2 2 0 0 1 1.92 2.56l-2.33 8A2 2 0 0 1 17.5 22H4a2 2 0 0 1-2-2v-8a2 2 0 0 1 2-2h2.76a2 2 0 0 0 1.79-1.11L12 2a3.13 3.13 0 0 1 3 3.88Z"/>',
userplus:'<path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M19 8v6M22 11h-6"/>',
bulb:'<path d="M15 14c.2-1 .7-1.7 1.5-2.5 1-.9 1.5-2.2 1.5-3.5A6 6 0 0 0 6 8c0 1 .2 2.2 1.5 3.5.7.7 1.3 1.5 1.5 2.5"/><path d="M9 18h6M10 22h4"/>',
chev:'<path d="m6 9 6 6 6-6"/>',cal:'<rect x="3" y="4" width="18" height="18" rx="2"/><path d="M16 2v4M8 2v4M3 10h18"/>',ban:'<circle cx="12" cy="12" r="10"/><path d="m4.9 4.9 14.2 14.2"/>',
arrow:'<path d="M5 12h14M12 5l7 7-7 7"/>',ruler:'<path d="M21.3 15.3a2.4 2.4 0 0 1 0 3.4l-2.6 2.6a2.4 2.4 0 0 1-3.4 0L2.7 8.7a2.41 2.41 0 0 1 0-3.4l2.6-2.6a2.41 2.41 0 0 1 3.4 0Z"/><path d="m14.5 12.5 2-2M11.5 9.5l2-2M8.5 6.5l2-2M17.5 15.5l2-2"/>',
msg:'<path d="M7.9 20A9 9 0 1 0 4 16.1L2 22Z"/><path d="M8 12h.01M12 12h.01M16 12h.01"/>',wrench:'<path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/>',
reply:'<path d="m9 17-5-5 5-5"/><path d="M20 18v-2a4 4 0 0 0-4-4H4"/>',smile:'<circle cx="12" cy="12" r="10"/><path d="M8 14s1.5 2 4 2 4-2 4-2M9 9h.01M15 9h.01"/>',frown:'<circle cx="12" cy="12" r="10"/><path d="M16 16s-1.5-2-4-2-4 2-4 2M9 9h.01M15 9h.01"/>',
users:'<path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87M16 3.13a4 4 0 0 1 0 7.75"/>',
wheel:'<circle cx="12" cy="12" r="2"/><path d="M12 2v4M6.8 15l-3.5 2M20.7 7l-3.5 2M6.8 9 3.3 7M20.7 17l-3.5-2M9 22l3-8 3 8M8 22h8"/><path d="M18 18.7a9 9 0 1 0-12 0"/>',
fish:'<path d="M6.5 12c.94-3.46 4.94-6 8.5-6 3.56 0 6.06 2.54 7 6-.94 3.47-3.44 6-7 6s-7.56-2.53-8.5-6Z"/><path d="M18 12v.5M7 10.67C7 8 5.58 5.97 2.73 5.5c-1 1.5-1 5 .23 6.5-1.24 1.5-1.24 5-.23 6.5C5.58 18.03 7 16 7 13.33"/>'};
const svgI=n=>`<svg class="i" viewBox="0 0 24 24" aria-hidden="true">${IC[n]||''}</svg>`;

/* issues */
const ISS=[
{t:'Overlapping Navigation',p:'Lack of clear, dedicated structure',pb:'<li>Navigation labels overlap in function<ul><li>e.g., "Tickets" vs. "Ticket &amp; Offer"</li><li>e.g., "A Day at the Park" overlaps with shortcuts like "Attractions" and "Schedule."</li></ul></li>',
 ib:'<li>Increases unnecessary <b>cognitive load</b></li><li><b>Slows down the consumer journey</b> for simple tasks (buying tickets, checking hours)</li><li>Reduces <b>user-friendliness</b> and <b>consistency</b></li>',im:['i1']},
{t:'Excessive Promotional Density',p:'Poor Content Prioritization',pb:'<li>Homepage displays too many modules simultaneously<ul><li>(offers, conservation, membership, etc.)</li></ul></li><li>Core items (ticket price, opening hours, map) <b>compete for attention</b> with heavy promotional material</li>',
 ib:'<li><b>Dilutes the visibility</b> of functional information</li><li>Users must filter out "noise" to make a decision</li><li>Homepage tries to serve too many objectives, making the main conversion path <b>invisible</b></li>',im:['i2']},
{t:'Inconsistent Legacy Content',p:'Content Governance &amp; Legacy Pages',pb:'<li>Legacy web pages still describe the Ocean Park Mobile App as available, while the new site says it is suspended.</li><li>Old pages remain retrievable via search engines.</li>',
 ib:'<li><b>Confusion</b>: Users may try to download a non-existent app.</li><li><b>Trust Damage</b>: Inconsistent descriptions damage trust in the website\'s accuracy.</li>',im:['i3']},
{t:'Search-Intent Mismatch &amp; Mobile Friction',p:'Sponsored ads and landing pages do not align with user intent',pb:'<li>General info search leads to a ticketing subdomain (intent mismatch).</li><li>The ticketing page has inconsistent styling, awkward labels, and a large stacked menu.</li><li>Loading delays and interface changes create friction.</li>',
 ib:'<li>Visitors seeking general info are forced into a transaction page prematurely.</li><li>Perceived loading delays and interface friction lead to <b>user abandonment</b> and <b>reduced confidence</b>.</li>',im:['i4a','i4b']}];
document.getElementById('issues').innerHTML=ISS.map((d,i)=>`<article class="row rv${i%2?' flip':''}">
 <div><h4><small>ISSUE ${i+1}</small>${d.t}</h4><div class="card"><h5>THE PROBLEM</h5><h6>${d.p}</h6><ul>${d.pb}</ul></div><div class="flow">${svgI('chev')}</div><div class="card dark"><h5>IMPACT</h5><ul>${d.ib}</ul></div></div>
 <div class="shots">${d.im.map(k=>`<img class="shot" src="img/${k}.jpg" alt="Screenshot for issue ${i+1}" style="${d.im.length>1?'max-width:48%':''}">`).join('')}</div></article>`).join('');

/* platforms */
const PL=[
{n:'Xiaohongshu',c:'#FF2442',im:['xhs1','xhs2'],r:[['Content Style','Highly platform-native, visually appealing, and lifestyle-oriented (e.g., "Old-School Date" spots, monthly park calendars, and "Family Autumn Routes")'],['Performance','Excellent. The account boasts 89k followers and high "Saves/Collects" on posts, indicating strong utility value to mainland tourists.'],['','It serves as a powerful tool for market research as it has understanding tourist needs and driving direct sales.']]},
{n:'Instagram',c:'#C13584',im:['ig1','ig2'],r:[['Content Style','Visual-first, focusing heavily on animal IP (especially the pandas) and seasonal events.'],['Performance','Strong engagement. The platform is used to establish an "emotional bond" with local audiences.'],['','It effectively maintains the local brand identity, though it lacks deep two-way "Listening" or community dialogue compared to Xiaohongshu.']]},
{n:'Facebook',c:'#1877F2',im:['fb1','fb2'],r:[['Content Style','Traditional, informational, and announcement-heavy.'],['Performance','Moderate. While it still functions as a core platform for older demographics, its emotional resonance and organic reach are decaying among younger users.'],['','It is no longer the highly interactive hub it once was and requires a strategic revamp to avoid feeling like a legacy platform.']]},
{n:'YouTube',c:'#FF0000',im:['yt1','yt2'],r:[['Content Style','Split between high-budget, cinematic seasonal ads and raw, educational conservation videos.'],['Performance','Extreme inconsistency . Seasonal campaigns such as Halloween 2026 rake in massive views. However, core educational videos such as conservation video barely break 143 views.'],['','Content is "good" in production quality, but the marketing is only effective for commercial events. They need more engaging formats (like Shorts) to match their campaign success.']]}];
const tabs=document.getElementById('tabs'),pp=document.getElementById('platPanel');
tabs.innerHTML=PL.map((d,i)=>`<button role="tab" id="tab${i}" aria-selected="${i===0}" aria-controls="platPanel"><span class="dot" style="background:${d.c}"></span>${d.n}</button>`).join('');
function plat(i){const d=PL[i];tabs.querySelectorAll('button').forEach((b,k)=>b.setAttribute('aria-selected',k===i));pp.setAttribute('aria-labelledby','tab'+i);
 pp.innerHTML=`<div class="plat"><div class="imgs">${d.im.map(k=>`<img class="shot" src="img/${k}.jpg" alt="${d.n} screenshot">`).join('')}</div>
 <div>${d.r.map((r,j)=>`<div class="pt"><span class="num">0${j+1}</span><div>${r[0]?`<b>${r[0]}</b>`:''}${r[1]}</div></div>`).join('')}</div></div>`;}
tabs.addEventListener('click',e=>{const b=e.target.closest('button');if(b)plat([...tabs.children].indexOf(b))});
tabs.addEventListener('keydown',e=>{const bs=[...tabs.children],i=bs.indexOf(document.activeElement);if(i<0)return;if(e.key==='ArrowRight'||e.key==='ArrowLeft'){e.preventDefault();const n=(i+(e.key==='ArrowRight'?1:3))%4;plat(n);bs[n].focus()}});
plat(0);

/* rating rows */
document.getElementById('rateRows').innerHTML=[['Ctrip','2026','var(--ct)','4.67',.02],['Google Maps','2026','var(--gg)','4.44',.06],['TripAdvisor','2023–26','var(--ta)','3.77',.22]].map((r,i)=>`<div class="rr">
 <span style="display:flex;gap:8px;align-items:center;flex-wrap:wrap"><i class="dot" style="background:${r[2]}"></i><b style="color:var(--navy)">${r[0]}</b><small style="color:var(--grey)">${r[1]}</small></span>
 <span class="big" style="font-size:28px;color:${i==2?'var(--coral)':'var(--navy)'}">${r[3]}</span>
 <span style="display:flex;align-items:center;gap:10px"><span class="bar"><i data-w="${r[4]/.25*100}%"></i></span><b style="color:var(--coral);width:38px;text-align:right">${Math.round(r[4]*100)}%</b></span></div>`).join('');

/* line */
{const v=[4.17,4.25,3.96,3.86,2.95,3.00,3.63,3.73,3.94,3.84],yrs=[2017,2018,2019,2020,2021,2022,2023,2024,2025,2026];
 const X=i=>36+i*60,Y=x=>182-(x-2.5)/2*160;let s='';
 [2.5,3,3.5,4,4.5].forEach(t=>s+=`<line x1="30" x2="590" y1="${Y(t)}" y2="${Y(t)}" stroke="#E3E6EA"/><text x="0" y="${Y(t)+4}" font-size="12" fill="#5F6B78">${t.toFixed(1)}</text>`);
 s+=`<rect x="${X(4)-24}" y="14" width="${X(5)-X(4)+48}" height="170" rx="8" fill="#C25F3B" opacity=".08"/>`;
 s+=`<polyline id="pl" points="${v.map((x,i)=>X(i)+','+Y(x)).join(' ')}" fill="none" stroke="#3E9E6E" stroke-width="3" stroke-linejoin="round" pathLength="1" stroke-dasharray="1" stroke-dashoffset="1" style="transition:stroke-dashoffset 1.6s ease"/>`;
 v.forEach((x,i)=>s+=`<g><title>${yrs[i]}: ${x.toFixed(2)} stars</title><circle cx="${X(i)}" cy="${Y(x)}" r="5" fill="#3E9E6E" stroke="#fff" stroke-width="2"/><text x="${X(i)}" y="${Y(x)-11}" text-anchor="middle" font-size="13" font-weight="${i==4||i==1?700:500}" fill="${i==4?'#C25F3B':'#2E3A46'}">${x.toFixed(2)}</text><text x="${X(i)}" y="208" text-anchor="middle" font-size="12" fill="#5F6B78">${yrs[i]}</text></g>`);
 document.getElementById('line').innerHTML=s;}

/* dot plots */
const COL=['#3D6FD1','#E0703C','#3E9E6E'],PN=['Ctrip','Google Maps','TripAdvisor'];
function dots(id,rows,max,x0,w,rh,y0,extra){let s='';const X=v=>x0+w*v/max;
 for(let t=0;t<=max+1e-9;t+=.1)s+=`<line x1="${X(t)}" x2="${X(t)}" y1="${y0-16}" y2="${y0+(rows.length-1)*rh+16}" stroke="#E3E6EA"/><text x="${X(t)}" y="${y0+(rows.length-1)*rh+34}" text-anchor="middle" font-size="12" fill="#5F6B78">${Math.round(t*100)}%</text>`;
 rows.forEach((r,i)=>{const y=y0+i*rh,mn=Math.min(...r.v),mx=Math.max(...r.v);
  s+=`<text x="${r.ic?30:0}" y="${y+(r.tag?-2:5)}" font-size="15" font-weight="${r.b?700:500}" fill="#23476B">${r.l}</text>`;
  if(r.ic)s+=`<g transform="translate(2,${y-11}) scale(.9)" stroke="#4D7FA3" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">${IC[r.ic]}</g>`;
  if(r.tag)s+=`<text x="0" y="${y+15}" font-size="12" font-weight="700" fill="#C25F3B">${r.tag}</text>`;
  s+=`<line x1="${X(mn)}" x2="${X(mx)}" y1="${y}" y2="${y}" stroke="#B5C0CA" stroke-width="2"/>`;
  r.v.forEach((v,j)=>s+=`<circle cx="${X(v)}" cy="${y}" r="7.5" fill="${COL[j]}" stroke="#fff" stroke-width="1.5"><title>${PN[j]}: ${(v*100).toFixed(1)}%</title></circle>`);
  if(extra)s+=extra(r,y);});
 document.getElementById(id).innerHTML=s;}
dots('topics',[{l:'Family and children',ic:'users',b:1,v:[.253,.193,.400],o:'24.7%'},{l:'Rides',ic:'wheel',v:[.144,.251,.434],o:'18.8%'},{l:'Aquarium and marine life',ic:'fish',v:[.125,.138,.331],o:'14.0%'}],.5,230,250,44,20,
 (r,y)=>`<text x="560" y="${y+7}" text-anchor="end" font-size="21" font-weight="700" fill="#23476B">${r.o}</text>`);
dots('compl',[{l:'Closed rides',b:1,tag:'top 3 on every platform',v:[.18,.17,.30]},{l:'Price / value',b:1,tag:'top 3 on every platform',v:[.23,.15,.28]},{l:'Old facilities',v:[.24,.14,.17]},{l:'Staff',v:[.13,.14,.39]},{l:'Food',v:[.11,.12,.26]}],.4,190,430,58,22);

document.getElementById('steps').innerHTML=[['msg','Reply publicly','Guest Relations acknowledges the concern and offers a next step.'],['wrench','Escalate recurring issues','Send repeated complaints to Operations for investigation.'],['reply','Update the original reply','Tell readers what action the park has confirmed.']]
 .map(r=>`<div><span class="ring">${svgI(r[0])}</span><div><b style="font-size:19px;color:var(--navy)">${r[1]}</b><div>${r[2]}</div></div></div>`).join('');

document.querySelectorAll('i[data-i]').forEach(e=>e.outerHTML=svgI(e.dataset.i).replace('<svg ',`<svg style="${e.getAttribute('style')||''}" `));

/* reveal + charts on view */
const io=new IntersectionObserver(es=>es.forEach(e=>{if(!e.isIntersecting)return;const t=e.target;t.classList.add('in');
 t.querySelectorAll('.bar i').forEach(b=>b.style.width=b.dataset.w);const pl=t.querySelector('#pl');if(pl)pl.style.strokeDashoffset='0';io.unobserve(t)}),{threshold:.15});
document.querySelectorAll('.rv').forEach(el=>io.observe(el));

/* nav: scrollspy + progress */
const links=[...document.querySelectorAll('.links a')],secs=links.map(a=>document.querySelector(a.getAttribute('href'))),prog=document.getElementById('prog');
function onScroll(){const h=document.documentElement,y=h.scrollTop;prog.style.width=(y/(h.scrollHeight-h.clientHeight)*100||0)+'%';
 let k=-1;secs.forEach((s,i)=>{if(s.getBoundingClientRect().top<140)k=i});links.forEach((a,i)=>a.classList.toggle('on',i===k));}
addEventListener('scroll',onScroll,{passive:true});onScroll();

/* next-section button + keys (for presenting) */
const stops=[...document.querySelectorAll('#top,.chead,.sub2,.end')];
function step(dir){const y=scrollY+90;let t=dir>0?stops.find(s=>s.getBoundingClientRect().top+scrollY>y+10):[...stops].reverse().find(s=>s.getBoundingClientRect().top+scrollY<y-10);if(t)t.scrollIntoView({behavior:matchMedia('(prefers-reduced-motion:reduce)').matches?'auto':'smooth'})}
document.getElementById('nextB').onclick=()=>step(1);
addEventListener('keydown',e=>{if(e.metaKey||e.ctrlKey||e.altKey||e.target.closest('[role=tab]'))return;
 if(e.key==='Escape')lb.classList.remove('on');else if(e.key==='n'||e.key==='ArrowRight'){e.preventDefault();step(1)}else if(e.key==='p'||e.key==='ArrowLeft'){e.preventDefault();step(-1)}});

/* lightbox */
const lb=document.getElementById('lb'),li=document.getElementById('lbImg');
document.addEventListener('click',e=>{const im=e.target.closest('img.shot');if(im){li.src=im.src;li.alt=im.alt;lb.classList.add('on')}});
lb.addEventListener('click',e=>{if(e.target!==li)lb.classList.remove('on')});
}
</script>
</body>
</html>
