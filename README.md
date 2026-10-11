<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Rapture Studios | Roblox Developer Portfolio</title>
<meta name="description" content="Rapture Studios (rapture-rblx): Roblox soundtracks, sound effects and scripting. Games worked on and games in development.">
<meta property="og:title" content="Rapture Studios">
<meta property="og:description" content="Roblox soundtracks, SFX and scripts. Bloomville, Cursed Cargo and more.">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='14' fill='%230b0d10'/%3E%3Cpath d='M20 48V16h14a10 10 0 0 1 3 19.6L46 48h-8l-7-11h-5v11z M26 22v9h8a4.5 4.5 0 0 0 0-9z' fill='%2362ff8a'/%3E%3C/svg%3E">
<style>
:root{
  --bg:#0a0c0f; --bg2:#10141a; --card:#131820; --line:#222a35;
  --text:#e9eef5; --mute:#8f9bad; --accent:#62ff8a; --accent2:#7c5cff;
  --radius:18px; --max:1120px;
  --display:"Space Grotesk","Segoe UI",system-ui,sans-serif;
  --body:"Inter",system-ui,-apple-system,"Segoe UI",sans-serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:80px}
body{background:var(--bg);color:var(--text);font-family:var(--body);line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:hidden}
a{color:inherit;text-decoration:none}
img{display:block;max-width:100%}
.wrap{max-width:var(--max);margin:0 auto;padding:0 20px}
section{padding:96px 0}
h1,h2,h3{font-family:var(--display);line-height:1.1;letter-spacing:-.02em}
.eyebrow{font:600 .78rem/1 var(--display);letter-spacing:.18em;text-transform:uppercase;color:var(--accent);margin-bottom:14px;display:block}
h2{font-size:clamp(1.9rem,4.5vw,3rem);margin-bottom:14px}
.lead{color:var(--mute);max-width:620px;font-size:1.05rem}

/* nav */
nav{position:fixed;inset:0 0 auto 0;z-index:50;backdrop-filter:blur(14px);background:rgba(10,12,15,.72);border-bottom:1px solid var(--line)}
nav .wrap{display:flex;align-items:center;justify-content:space-between;height:64px}
.logo{font:700 1.1rem var(--display);display:flex;align-items:center;gap:10px}
.logo i{width:12px;height:12px;border-radius:3px;background:var(--accent);box-shadow:0 0 14px var(--accent)}
.links{display:flex;gap:26px;font-size:.92rem;color:var(--mute)}
.links a:hover{color:var(--text)}
@media(max-width:640px){.links{gap:16px;font-size:.84rem}.logo span{display:none}}

/* hero */
.hero{min-height:100svh;display:flex;align-items:center;padding:120px 0 72px;position:relative;isolation:isolate}
.hero::before{content:"";position:absolute;inset:0;z-index:-1;
  background:radial-gradient(60% 50% at 80% 20%,rgba(124,92,255,.22),transparent 70%),radial-gradient(50% 45% at 10% 90%,rgba(98,255,138,.12),transparent 70%),
  linear-gradient(var(--line) 1px,transparent 1px) 0 0/56px 56px,linear-gradient(90deg,var(--line) 1px,transparent 1px) 0 0/56px 56px;
  -webkit-mask-image:radial-gradient(80% 80% at 50% 40%,#000 30%,transparent 100%);mask-image:radial-gradient(80% 80% at 50% 40%,#000 30%,transparent 100%);opacity:.9}
.tag{display:inline-flex;gap:10px;align-items:center;border:1px solid var(--line);background:var(--bg2);border-radius:999px;padding:7px 14px;font-size:.82rem;color:var(--mute);margin-bottom:26px}
.tag b{color:var(--accent);font-weight:600}
.hero h1{font-size:clamp(2.8rem,9vw,6.4rem);max-width:12ch}
.hero h1 em{font-style:normal;background:linear-gradient(90deg,var(--accent),#b6ffcb 50%,var(--accent2));-webkit-background-clip:text;background-clip:text;color:transparent}
.hero p{margin:24px 0 34px;max-width:560px;color:var(--mute);font-size:1.15rem}
.btns{display:flex;gap:12px;flex-wrap:wrap}
.btn{display:inline-flex;align-items:center;gap:8px;padding:13px 22px;border-radius:12px;font-weight:600;font-size:.95rem;border:1px solid var(--line);background:var(--bg2);transition:.2s;cursor:pointer;color:var(--text);font-family:inherit}
.btn:hover{transform:translateY(-2px);border-color:#3a4658}
.btn.primary{background:var(--accent);color:#04120a;border-color:var(--accent)}
.btn.primary:hover{box-shadow:0 8px 30px rgba(98,255,138,.3)}

/* work cards */
.grid3{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:18px;margin-top:44px}
.card{background:var(--card);border:1px solid var(--line);border-radius:var(--radius);padding:28px;transition:.25s}
.card:hover{border-color:#34405a;transform:translateY(-3px)}
.card .ico{width:46px;height:46px;border-radius:12px;display:grid;place-items:center;background:rgba(98,255,138,.1);color:var(--accent);margin-bottom:18px}
.card:nth-child(2) .ico{background:rgba(124,92,255,.14);color:#a592ff}
.card h3{font-size:1.3rem;margin-bottom:8px}
.card p{color:var(--mute);font-size:.97rem}
.chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:16px}
.chip{font-size:.76rem;padding:4px 10px;border-radius:999px;border:1px solid var(--line);color:var(--mute)}

/* project */
.alt{background:var(--bg2);border-block:1px solid var(--line)}
.proj{display:grid;grid-template-columns:minmax(0,5fr) minmax(0,6fr);gap:44px;align-items:center;margin-top:44px}
@media(max-width:860px){.proj{grid-template-columns:1fr}}
.cover{border-radius:var(--radius);overflow:hidden;border:1px solid var(--line);aspect-ratio:1/1;max-width:460px;width:100%;box-shadow:0 30px 80px rgba(124,92,255,.18)}
.cover img{width:100%;height:100%;object-fit:cover}
.status{display:inline-flex;align-items:center;gap:8px;font-size:.78rem;font-weight:600;padding:5px 12px;border-radius:999px;margin-bottom:14px;letter-spacing:.04em}
.status.done{background:rgba(98,255,138,.1);color:var(--accent)}
.status.wip{background:rgba(255,184,76,.12);color:#ffb84c}
.status::before{content:"";width:7px;height:7px;border-radius:50%;background:currentColor}
.status.wip::before{animation:pulse 1.6s infinite}
@keyframes pulse{50%{opacity:.25}}
.proj h3{font-size:clamp(1.8rem,4vw,2.6rem);margin-bottom:12px}
.proj p{color:var(--mute);margin-bottom:12px}
.roles{display:flex;gap:8px;flex-wrap:wrap;margin-top:18px}

/* player */
.player{margin-top:26px;border:1px solid var(--line);border-radius:14px;background:var(--bg);overflow:hidden}
.ph{padding:12px 16px;font:600 .75rem var(--display);letter-spacing:.14em;text-transform:uppercase;color:var(--mute);border-bottom:1px solid var(--line);display:flex;justify-content:space-between}
.track{display:grid;grid-template-columns:42px 1fr auto;gap:14px;align-items:center;padding:12px 16px;border-bottom:1px solid var(--line);transition:background .2s}
.track:last-child{border-bottom:0}
.track.on{background:rgba(98,255,138,.05)}
.pbtn{width:42px;height:42px;border-radius:50%;border:0;background:var(--accent);color:#04120a;display:grid;place-items:center;cursor:pointer;transition:.2s}
.pbtn:hover{transform:scale(1.07)}
.pbtn svg{width:16px;height:16px;fill:currentColor}
.pbtn .pa{display:none}.track.playing .pbtn .pl{display:none}.track.playing .pbtn .pa{display:block}
.tt{min-width:0}
.tt b{display:block;font-weight:600;font-size:.95rem}
.tt small{color:var(--mute);font-size:.78rem}
.bar{height:5px;border-radius:5px;background:var(--line);margin-top:8px;cursor:pointer;position:relative}
.bar i{position:absolute;inset:0 auto 0 0;width:0;border-radius:5px;background:linear-gradient(90deg,var(--accent),var(--accent2))}
.tm{font:.78rem ui-monospace,Menlo,monospace;color:var(--mute)}

/* gallery */
.gal{display:grid;grid-template-columns:repeat(6,1fr);gap:14px;margin-top:40px}
.gal button{border:1px solid var(--line);background:var(--card);padding:0;border-radius:14px;overflow:hidden;cursor:zoom-in;position:relative;grid-column:span 2;aspect-ratio:16/10;color:inherit;font:inherit}
.gal button:nth-child(1){grid-column:span 4;aspect-ratio:auto}
.gal button:nth-child(2){grid-column:span 2}
.gal button:nth-child(n+3){grid-column:span 3}
.gal button img{width:100%;height:100%;object-fit:cover;transition:transform .5s}
.gal button:hover img{transform:scale(1.05)}
.gal span{position:absolute;left:0;right:0;bottom:0;padding:26px 14px 10px;font-size:.82rem;font-weight:500;text-align:left;background:linear-gradient(transparent,rgba(0,0,0,.78))}
@media(max-width:700px){.gal{grid-template-columns:1fr 1fr}.gal button,.gal button:nth-child(n){grid-column:span 1;aspect-ratio:4/3}.gal button:nth-child(1){grid-column:span 2}}
.concept{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px;margin-top:30px}
.concept div{padding:18px;border-radius:14px;border:1px solid var(--line);background:var(--card)}
.concept b{font:600 1rem var(--display);display:block;margin-bottom:4px;color:var(--accent)}
.concept span{font-size:.9rem;color:var(--mute)}
#lb{position:fixed;inset:0;z-index:100;background:rgba(4,6,8,.94);display:none;align-items:center;justify-content:center;flex-direction:column;gap:14px;padding:20px}
#lb.open{display:flex}
#lb img{max-height:80vh;max-width:96vw;border-radius:10px}
#lb p{color:var(--mute);font-size:.9rem}
#lb button{position:absolute;top:18px;right:20px;background:var(--card);color:var(--text);border:1px solid var(--line);width:42px;height:42px;border-radius:50%;font-size:1.3rem;cursor:pointer}

/* contact */
.contact{text-align:center}
.contact .lead{margin:0 auto 30px}
.contact .btns{justify-content:center}
footer{border-top:1px solid var(--line);padding:28px 0;color:var(--mute);font-size:.85rem}
footer .wrap{display:flex;justify-content:space-between;flex-wrap:wrap;gap:10px}
.reveal{opacity:0;transform:translateY(24px);transition:opacity .7s,transform .7s}
.reveal.in{opacity:1;transform:none}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.reveal{opacity:1;transform:none}html{scroll-behavior:auto}}
</style>
</head>
<body>

<nav><div class="wrap">
  <a class="logo" href="#top"><i></i><span>Rapture Studios</span></a>
  <div class="links"><a href="#work">Work</a><a href="#games">Games</a><a href="#wip">In development</a><a href="#contact">Contact</a></div>
</div></nav>

<header class="hero" id="top"><div class="wrap">
  <div class="tag"><b>rapture-rblx</b> · Roblox developer</div>
  <h1>Sound, scripts &amp; <em>worlds</em> for Roblox.</h1>
  <p>I'm Daniel, the developer behind Rapture Studios. I make soundtracks, sound effects and game scripts for Roblox experiences.</p>
  <div class="btns">
    <a class="btn primary" href="#games">See my games</a>
    <a class="btn" href="#bloomville-music">Listen to soundtracks</a>
  </div>
</div></header>

<section id="work"><div class="wrap">
  <span class="eyebrow">What I do</span>
  <h2>Examples of work</h2>
  <p class="lead">Everything an experience needs to sound and play right, from music to the code behind it.</p>
  <div class="grid3">
    <div class="card reveal"><div class="ico"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18V5l12-2v13"/><circle cx="6" cy="18" r="3"/><circle cx="18" cy="16" r="3"/></svg></div>
      <h3>Soundtracks</h3><p>Looping, themed music built for specific islands and moods. Hear the Bloomville tracks <a href="#bloomville-music" style="color:var(--accent)">below</a>.</p>
      <div class="chips"><span class="chip">Themed loops</span><span class="chip">Seasonal music</span><span class="chip">Game ready</span></div></div>
    <div class="card reveal"><div class="ico"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M11 5 6 9H2v6h4l5 4z"/><path d="M15.5 8.5a5 5 0 0 1 0 7M19 5a10 10 0 0 1 0 14"/></svg></div>
      <h3>Sound effects</h3><p>SFX for gameplay feedback, ambience and upgrades, from small UI clicks to big moments.</p>
      <div class="chips"><span class="chip">Gameplay SFX</span><span class="chip">Ambience</span><span class="chip">UI sounds</span></div></div>
    <div class="card reveal"><div class="ico"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m16 18 6-6-6-6M8 6l-6 6 6 6"/></svg></div>
      <h3>Scripts</h3><p>Luau scripting for game systems, features and tools that run reliably in live servers.</p>
      <div class="chips"><span class="chip">Luau</span><span class="chip">Game systems</span><span class="chip">Roblox Studio</span></div></div>
  </div>
</div></section>

<section id="games" class="alt"><div class="wrap">
  <span class="eyebrow">Games I've worked on</span>
  <h2>Released work</h2>
  <div class="proj">
    <div class="cover reveal"><img src="assets/bloomville.jpg" alt="Bloomville key art: a pumpkin-filled Halloween town with bats and an hourglass"></div>
    <div class="reveal">
      <span class="status done">Worked on</span>
      <h3>Bloomville</h3>
      <p>A Roblox experience with a cosy, seasonal town that changes with the calendar, from Halloween pumpkins and bats to a main island and a desert.</p>
      <p>I composed the soundtrack, with a separate theme for each area.</p>
      <div class="roles"><span class="chip">Soundtrack</span><span class="chip">Roblox</span></div>
      <div class="player" id="bloomville-music">
        <div class="ph"><span>Bloomville soundtrack</span><span>4 tracks</span></div>
        <div id="tracks"></div>
      </div>
    </div>
  </div>
</div></section>

<section id="wip"><div class="wrap">
  <span class="eyebrow">Games I'm working on</span>
  <h2>In development</h2>
  <div class="reveal" style="margin-top:36px">
    <span class="status wip">In development</span>
    <h3 style="font-size:clamp(2rem,5vw,3.4rem);margin-bottom:12px">Cursed Cargo</h3>
    <p class="lead">A co-op delivery game where your packages are alive and cursed. Load up the van, work as a team and get every parcel to its door. <b style="color:var(--accent)">No returns. No refunds.</b></p>
  </div>
  <div class="gal" id="gal">
    <button><img src="assets/aerial.jpg" alt="Aerial view of the Cursed Cargo town"><span>The town from above</span></button>
    <button><img src="assets/van.jpg" alt="Black Cursed Cargo delivery van"><span>The delivery van</span></button>
    <button><img src="assets/boxes.jpg" alt="Cursed Cargo packages on a rooftop"><span>The cursed packages</span></button>
    <button><img src="assets/houses.jpg" alt="Brick houses on a residential street"><span>Delivery addresses</span></button>
    <button><img src="assets/depot.jpg" alt="The depot garage with three roller doors"><span>The depot</span></button>
    <button><img src="assets/street.jpg" alt="Main street looking toward the mountains"><span>Main street</span></button>
  </div>
  <div class="concept reveal">
    <div><b>Co-op</b><span>Work with friends to get every delivery done.</span></div>
    <div><b>Living packages</b><span>Cursed parcels that don't want to be delivered.</span></div>
    <div><b>Drive and deliver</b><span>A custom van, a depot and a whole town to cover.</span></div>
  </div>
</div></section>

<section id="contact" class="alt contact"><div class="wrap">
  <span class="eyebrow">Get in touch</span>
  <h2>Need sound or scripts for your game?</h2>
  <p class="lead">I'm open to Roblox soundtrack, SFX and scripting work. Join the studio Discord or follow along on YouTube and TikTok.</p>
  <div class="btns">
    <a class="btn primary" href="https://discord.gg/arvm99rawt" target="_blank" rel="noopener">Join Rapture Studios on Discord</a>
    <a class="btn" href="https://youtube.com/@raprblx" target="_blank" rel="noopener">YouTube</a>
    <a class="btn" href="https://www.tiktok.com/@rapturedevelopment?_r=1&amp;_t=ZN-9AS47enZy5u" target="_blank" rel="noopener">TikTok</a>
  </div>
</div></section>

<footer><div class="wrap"><span>&copy; <span id="yr"></span> Rapture Studios</span><span>rapture-rblx</span></div></footer>

<div id="lb" role="dialog" aria-modal="true" aria-label="Image viewer"><button aria-label="Close">&times;</button><img alt=""><p></p></div>

<script>
const TRACKS=[
  {title:"Main Island",sub:"Bloomville · Main theme",src:"assets/main.mp3"},
  {title:"Halloween Island",sub:"Bloomville · Seasonal theme",src:"assets/halloween.mp3"},
  {title:"Fall (Backing)",sub:"Bloomville · Autumn backing track",src:"assets/fall.mp3"},
  {title:"Desert (Backing)",sub:"Bloomville · Desert backing track",src:"assets/desert.mp3"}
];
const PLAY='<svg class="pl" viewBox="0 0 24 24"><path d="M7 4v16l14-8z"/></svg><svg class="pa" viewBox="0 0 24 24"><path d="M6 4h4v16H6zM14 4h4v16h-4z"/></svg>';
const audio=new Audio();audio.preload="none";let cur=-1;const rows=[],blobs={};
const fmt=s=>isFinite(s)?Math.floor(s/60)+":"+String(Math.floor(s%60)).padStart(2,"0"):"0:00";
const box=document.getElementById("tracks");
TRACKS.forEach((t,i)=>{
  const r=document.createElement("div");r.className="track";
  r.innerHTML=`<button class="pbtn" aria-label="Play ${t.title}">${PLAY}</button><div class="tt"><b>${t.title}</b><small>${t.sub}</small><div class="bar"><i></i></div></div><span class="tm">0:00</span>`;
  r.querySelector(".pbtn").onclick=()=>toggle(i);
  r.querySelector(".bar").onclick=e=>{if(cur!==i||!audio.duration)return;const b=e.currentTarget.getBoundingClientRect();audio.currentTime=(e.clientX-b.left)/b.width*audio.duration};
  box.appendChild(r);rows.push(r);
});
async function load(i){
  if(!blobs[i]){try{blobs[i]=URL.createObjectURL(await (await fetch(TRACKS[i].src)).blob())}catch(e){blobs[i]=TRACKS[i].src}}
  return blobs[i];
}
async function toggle(i){
  if(cur===i){audio.paused?audio.play():audio.pause();return}
  if(cur>-1){rows[cur].classList.remove("playing","on");rows[cur].querySelector("i").style.width="0"}
  cur=i;audio.src=await load(i);rows[i].classList.add("on");audio.play();
}
audio.onplay=()=>rows[cur]&&rows[cur].classList.add("playing");
audio.onpause=()=>rows[cur]&&rows[cur].classList.remove("playing");
audio.onended=()=>{if(cur<TRACKS.length-1)toggle(cur+1);else{rows[cur].classList.remove("playing")}};
audio.ontimeupdate=()=>{if(cur<0)return;const r=rows[cur];r.querySelector("i").style.width=(audio.currentTime/audio.duration*100||0)+"%";r.querySelector(".tm").textContent=fmt(audio.currentTime)+" / "+fmt(audio.duration)};

// gallery lightbox
const lb=document.getElementById("lb"),lbi=lb.querySelector("img"),lbp=lb.querySelector("p");
document.querySelectorAll("#gal button").forEach(b=>b.onclick=()=>{const im=b.querySelector("img");lbi.src=im.src;lbi.alt=im.alt;lbp.textContent=b.querySelector("span").textContent;lb.classList.add("open")});
lb.onclick=e=>{if(e.target!==lbi)lb.classList.remove("open")};
addEventListener("keydown",e=>{if(e.key==="Escape")lb.classList.remove("open")});

// reveal on scroll
const io=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){e.target.classList.add("in");io.unobserve(e.target)}}),{threshold:.12});
document.querySelectorAll(".reveal").forEach(el=>io.observe(el));
document.getElementById("yr").textContent=new Date().getFullYear();
</script>
</body>
</html>
