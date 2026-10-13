<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Rapture Studios | Roblox Builder, Music, SFX &amp; Scripts</title>
<meta name="description" content="Rapture Studios: Roblox builds, music, sound effects and scripts. See prices and portfolio.">
<meta property="og:title" content="Rapture Studios">
<meta property="og:description" content="Roblox builds, music, SFX and scripts.">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='14' fill='%230b0d10'/%3E%3Cpath d='M20 48V16h14a10 10 0 0 1 3 19.6L46 48h-8l-7-11h-5v11z M26 22v9h8a4.5 4.5 0 0 0 0-9z' fill='%2362ff8a'/%3E%3C/svg%3E">
<style>
:root{--bg:#0a0c0f;--bg2:#10141a;--card:#131820;--line:#222a35;--text:#eef2f8;--mute:#8f9bad;--accent:#62ff8a;
 --display:"Space Grotesk","Segoe UI",system-ui,sans-serif;--body:"Inter",system-ui,-apple-system,"Segoe UI",sans-serif}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--text);font-family:var(--body);line-height:1.5;-webkit-font-smoothing:antialiased;min-height:100svh;display:flex;flex-direction:column;overflow-x:hidden}
body::before{content:"";position:fixed;inset:0;z-index:-1;pointer-events:none;
 background:radial-gradient(55% 45% at 85% 10%,rgba(124,92,255,.2),transparent 70%),radial-gradient(45% 40% at 5% 95%,rgba(98,255,138,.1),transparent 70%)}
a{color:inherit;text-decoration:none}
button{font:inherit;color:inherit}
img{display:block;max-width:100%}
[hidden]{display:none!important}
.wrap{max-width:1120px;margin:0 auto;padding:0 20px;width:100%}

/* top bar */
.top{height:64px;display:flex;align-items:center;border-bottom:1px solid var(--line)}
.top .wrap{display:flex;align-items:center;justify-content:space-between}
.brand{font:700 1.1rem var(--display);display:flex;align-items:center;gap:10px}
.brand i{width:12px;height:12px;border-radius:3px;background:var(--accent);box-shadow:0 0 14px var(--accent)}
.back{background:var(--bg2);border:1px solid var(--line);border-radius:999px;padding:8px 16px;font-weight:600;font-size:.9rem;cursor:pointer}
.back:hover{border-color:#3a4658}

main{flex:1;display:flex;flex-direction:column}
.view{flex:1;display:flex;flex-direction:column;padding:34px 0 48px;animation:in .35s ease}
@keyframes in{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}

/* home */
#home{justify-content:center}
#home h1{font:700 clamp(2.6rem,8vw,5.5rem)/1 var(--display);letter-spacing:-.03em;text-align:center;margin-bottom:34px}
.skills{display:grid;grid-template-columns:repeat(4,1fr);gap:16px}
.skill{--c:var(--accent);position:relative;display:flex;flex-direction:column;justify-content:space-between;min-height:clamp(220px,34vh,320px);padding:26px;border-radius:24px;background:linear-gradient(160deg,color-mix(in srgb,var(--c) 16%,var(--card)),var(--card) 70%);border:1px solid color-mix(in srgb,var(--c) 30%,var(--line));transition:.25s;overflow:hidden}
.skill:hover,.skill:focus-visible{transform:translateY(-6px);border-color:var(--c);box-shadow:0 18px 50px color-mix(in srgb,var(--c) 25%,transparent);outline:0}
.skill .ico{width:64px;height:64px;border-radius:18px;display:grid;place-items:center;background:color-mix(in srgb,var(--c) 18%,transparent);color:var(--c)}
.skill .ico svg{width:34px;height:34px}
.skill b{font:700 clamp(1.6rem,3vw,2.2rem)/1.05 var(--display);letter-spacing:-.02em}
.skill .go{position:absolute;top:24px;right:24px;font-size:1.5rem;color:var(--c);transition:.25s}
.skill:hover .go{transform:translateX(4px)}
@media(max-width:900px){.skills{grid-template-columns:1fr 1fr;gap:12px}.skill{min-height:170px;padding:18px;border-radius:20px}.skill .ico{width:50px;height:50px;border-radius:14px}.skill .ico svg{width:26px;height:26px}.skill .go{top:16px;right:16px}}

/* skill panel */
.panel{--c:var(--accent)}
.phead{display:flex;flex-wrap:wrap;align-items:flex-end;justify-content:space-between;gap:22px;padding-bottom:26px;border-bottom:1px solid var(--line)}
.ptitle{font:700 clamp(2.2rem,6vw,3.6rem)/1 var(--display);letter-spacing:-.03em;display:flex;align-items:center;gap:16px}
.ptitle .ico{width:56px;height:56px;border-radius:16px;display:grid;place-items:center;background:color-mix(in srgb,var(--c) 18%,transparent);color:var(--c);flex:none}
.ptitle .ico svg{width:30px;height:30px}
.price{text-align:right}
.price small{display:block;color:var(--mute);font-size:.8rem;font-weight:600;letter-spacing:.14em;text-transform:uppercase}
.price b{font:700 clamp(2.8rem,9vw,5rem)/1 var(--display);letter-spacing:-.03em;color:var(--c)}
.price b.ask{font-size:clamp(1.8rem,5vw,2.8rem)}
@media(max-width:640px){.price{text-align:left;width:100%}}
.styles{display:flex;flex-wrap:wrap;gap:10px;padding:22px 0}
.styles span{padding:9px 18px;border-radius:999px;font-weight:600;font-size:1rem;background:color-mix(in srgb,var(--c) 12%,transparent);border:1px solid color-mix(in srgb,var(--c) 35%,transparent);color:var(--text)}
.group{margin-top:26px}
.group h3{font:700 1.15rem var(--display);margin-bottom:12px;display:flex;align-items:center;gap:10px}
.group h3 em{font-style:normal;font-size:.72rem;font-weight:600;padding:3px 10px;border-radius:999px;background:rgba(255,184,76,.12);color:#ffb84c}
.thumbs{display:grid;grid-template-columns:repeat(auto-fill,minmax(210px,1fr));gap:12px}
.thumb{padding:0;border:1px solid var(--line);border-radius:14px;overflow:hidden;cursor:zoom-in;background:var(--card);aspect-ratio:16/10}
.thumb img{width:100%;height:100%;object-fit:cover;transition:transform .5s}
.thumb:hover img{transform:scale(1.06)}
.empty{margin-top:26px;padding:34px;border:1px dashed var(--line);border-radius:18px;text-align:center;color:var(--mute);font-size:1.05rem}

/* player */
.mhead{display:flex;align-items:center;gap:16px;margin-bottom:14px}
.mhead img{width:72px;height:72px;border-radius:16px;object-fit:cover;border:1px solid var(--line)}
.mhead h3{margin:0}
.player{border:1px solid var(--line);border-radius:16px;background:var(--bg2);overflow:hidden}
.track{display:grid;grid-template-columns:48px 1fr auto;gap:14px;align-items:center;padding:14px 16px;border-bottom:1px solid var(--line);transition:background .2s}
.track:last-child{border-bottom:0}
.track.on{background:color-mix(in srgb,var(--c) 7%,transparent)}
.pbtn{width:48px;height:48px;border-radius:50%;border:0;background:var(--c);color:#0a0c0f;display:grid;place-items:center;cursor:pointer;transition:.2s}
.pbtn:hover{transform:scale(1.07)}
.pbtn svg{width:18px;height:18px;fill:currentColor}
.pbtn .pa{display:none}.track.playing .pbtn .pl{display:none}.track.playing .pbtn .pa{display:block}
.tt{min-width:0}.tt b{display:block;font-weight:600}
.bar{height:5px;border-radius:5px;background:var(--line);margin-top:9px;cursor:pointer;position:relative}
.bar i{position:absolute;inset:0 auto 0 0;width:0;border-radius:5px;background:var(--c)}
.tm{font:.78rem ui-monospace,Menlo,monospace;color:var(--mute)}

/* contacts */
.contact{border-top:1px solid var(--line);background:rgba(10,12,15,.85);backdrop-filter:blur(10px);padding:16px 0}
.contact .wrap{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px}
.contact strong{font:700 1.05rem var(--display)}
.cbtns{display:flex;gap:10px;flex-wrap:wrap}
.btn{display:inline-flex;align-items:center;gap:8px;padding:11px 20px;border-radius:12px;font-weight:600;font-size:.95rem;border:1px solid var(--line);background:var(--bg2);transition:.2s}
.btn:hover{transform:translateY(-2px);border-color:#3a4658}
.btn.primary{background:var(--accent);color:#04120a;border-color:var(--accent)}
.btn.primary:hover{box-shadow:0 8px 30px rgba(98,255,138,.3)}
@media(max-width:560px){.contact .wrap{justify-content:center}.contact strong{width:100%;text-align:center}.cbtns{justify-content:center}.btn{padding:10px 16px}}

#lb{position:fixed;inset:0;z-index:100;background:rgba(4,6,8,.94);display:none;align-items:center;justify-content:center;padding:20px}
#lb.open{display:flex}
#lb img{max-height:88vh;max-width:96vw;border-radius:10px}
#lb button{position:absolute;top:18px;right:20px;background:var(--card);color:var(--text);border:1px solid var(--line);width:42px;height:42px;border-radius:50%;font-size:1.3rem;cursor:pointer}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>

<header class="top"><div class="wrap">
  <a class="brand" href="#"><i></i>Rapture Studios</a>
  <button class="back" id="back" hidden>&larr; Back</button>
</div></header>

<main class="wrap" id="main">
  <section class="view" id="home">
    <h1>My skills</h1>
    <div class="skills" id="skills"></div>
  </section>
  <section class="view panel" id="panel" hidden></section>
</main>

<footer class="contact"><div class="wrap">
  <strong>Hire me</strong>
  <div class="cbtns">
    <a class="btn primary" href="https://discord.gg/arvm99rawt" target="_blank" rel="noopener">Discord</a>
    <a class="btn" href="https://youtube.com/@raprblx" target="_blank" rel="noopener">YouTube</a>
    <a class="btn" href="https://www.tiktok.com/@rapturedevelopment?_r=1&amp;_t=ZN-9AS47enZy5u" target="_blank" rel="noopener">TikTok</a>
  </div>
</div></footer>

<div id="lb" role="dialog" aria-modal="true" aria-label="Image viewer"><button aria-label="Close">&times;</button><img alt=""></div>

<script>
/* ============ EDIT HERE ============
   price: your lowest price for that skill, e.g. "£10". Leave "" to show "DM for price".
   styles: short tags shown big (genres for music, styles for builds). */
const SKILLS = {
  builds:  {name:"Builds",  color:"#62ff8a", price:"", styles:["Roleplay cities","Horror interiors","Desert & war maps","Terrain"]},
  music:   {name:"Music",   color:"#a592ff", price:"", styles:["Seasonal","Halloween","Desert","Looping themes"]},
  sfx:     {name:"SFX",     color:"#ffb84c", price:"", styles:["Gameplay","Ambience","UI sounds"]},
  scripts: {name:"Scripts", color:"#4cc9ff", price:"", styles:["Luau","Game systems","Tools"]}
};
const ICONS = {
  builds:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 8 12 3 3 8v8l9 5 9-5z"/><path d="m3 8 9 5 9-5M12 13v8"/></svg>',
  music:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18V5l12-2v13"/><circle cx="6" cy="18" r="3"/><circle cx="18" cy="16" r="3"/></svg>',
  sfx:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M11 5 6 9H2v6h4l5 4z"/><path d="M15.5 8.5a5 5 0 0 1 0 7M19 5a10 10 0 0 1 0 14"/></svg>',
  scripts:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m16 18 6-6-6-6M8 6l-6 6 6 6"/></svg>'
};
const BUILDS = [
  {title:"Orlando State Roleplay", imgs:[["assets/orl-bridge.jpg","Rail bridge"],["assets/orl-highway.jpg","Highway interchange"],["assets/orl-city.jpg","City streets"],["assets/orl-airport.jpg","Airport"]]},
  {title:"Harold Hill Asylum", imgs:[["assets/asylum-clearance.jpg","Clearance checkpoint"],["assets/asylum-medical.jpg","Medical room"],["assets/asylum-containment.jpg","Containment chamber"]]},
  {title:"Desert Wars", imgs:[["assets/desert-compound.jpg","Compound by the lake"],["assets/desert-camp.jpg","Base camp"],["assets/desert-hills.jpg","Hills"]]},
  {title:"Cursed Cargo", tag:"In development", imgs:[["assets/aerial.jpg","Town"],["assets/van.jpg","Delivery van"],["assets/boxes.jpg","Packages"],["assets/houses.jpg","Houses"],["assets/depot.jpg","Depot"],["assets/street.jpg","Main street"]]}
];
const MUSIC = {title:"Bloomville", cover:"assets/bloomville.jpg", tracks:[
  {title:"Main Island",src:"assets/main.mp3"},{title:"Halloween Island",src:"assets/halloween.mp3"},
  {title:"Fall (Backing)",src:"assets/fall.mp3"},{title:"Desert (Backing)",src:"assets/desert.mp3"}]};
/* ============ END EDIT ============ */

const $=s=>document.querySelector(s);
const home=$("#home"),panel=$("#panel"),back=$("#back");

// home buttons
$("#skills").innerHTML=Object.entries(SKILLS).map(([k,s])=>
  `<a class="skill" href="#${k}" style="--c:${s.color}"><span class="ico">${ICONS[k]}</span><b>${s.name}</b><span class="go">&rarr;</span></a>`).join("");

// audio
const audio=new Audio();audio.preload="none";let cur=-1,rows=[],blobs={},TR=[];
const fmt=s=>isFinite(s)?Math.floor(s/60)+":"+String(Math.floor(s%60)).padStart(2,"0"):"0:00";
const PLAY='<svg class="pl" viewBox="0 0 24 24"><path d="M7 4v16l14-8z"/></svg><svg class="pa" viewBox="0 0 24 24"><path d="M6 4h4v16H6zM14 4h4v16h-4z"/></svg>';
async function load(i){if(!blobs[i]){try{blobs[i]=URL.createObjectURL(await (await fetch(TR[i].src)).blob())}catch(e){blobs[i]=TR[i].src}}return blobs[i]}
async function toggle(i){
  if(cur===i){audio.paused?audio.play():audio.pause();return}
  if(cur>-1&&rows[cur]){rows[cur].classList.remove("playing","on");rows[cur].querySelector("i").style.width="0"}
  cur=i;audio.src=await load(i);rows[i].classList.add("on");audio.play();
}
audio.onplay=()=>rows[cur]&&rows[cur].classList.add("playing");
audio.onpause=()=>rows[cur]&&rows[cur].classList.remove("playing");
audio.onended=()=>{if(cur<TR.length-1)toggle(cur+1);else rows[cur]&&rows[cur].classList.remove("playing")};
audio.ontimeupdate=()=>{if(cur<0||!rows[cur])return;const r=rows[cur];r.querySelector("i").style.width=(audio.currentTime/audio.duration*100||0)+"%";r.querySelector(".tm").textContent=fmt(audio.currentTime)+" / "+fmt(audio.duration)};

function musicHTML(){
  TR=MUSIC.tracks;
  return `<div class="group"><div class="mhead"><img src="${MUSIC.cover}" alt="${MUSIC.title}"><h3>${MUSIC.title}</h3></div><div class="player">`+
   TR.map((t,i)=>`<div class="track"><button class="pbtn" aria-label="Play ${t.title}">${PLAY}</button><div class="tt"><b>${t.title}</b><div class="bar"><i></i></div></div><span class="tm">0:00</span></div>`).join("")+`</div></div>`;
}
function buildsHTML(){
  return BUILDS.map(g=>`<div class="group"><h3>${g.title}${g.tag?`<em>${g.tag}</em>`:""}</h3><div class="thumbs">`+
   g.imgs.map(([s,a])=>`<button class="thumb"><img src="${s}" alt="${a}" loading="lazy"></button>`).join("")+`</div></div>`).join("");
}

function show(key){
  audio.pause();audio.removeAttribute("src");cur=-1;rows=[];
  const s=SKILLS[key];
  if(!s){panel.hidden=true;home.hidden=false;back.hidden=true;document.title="Rapture Studios | Roblox Builder, Music, SFX & Scripts";window.scrollTo(0,0);return}
  home.hidden=true;panel.hidden=false;back.hidden=false;
  panel.style.setProperty("--c",s.color);
  const price=s.price?`<small>From</small><b>${s.price}</b>`:`<small>Price</small><b class="ask">DM me</b>`;
  let body="";
  if(key==="builds")body=buildsHTML();
  else if(key==="music")body=musicHTML();
  else body=`<div class="empty">Examples on request. Message me.</div>`;
  panel.innerHTML=`<div class="phead"><div class="ptitle"><span class="ico">${ICONS[key]}</span>${s.name}</div><div class="price">${price}</div></div>`+
   `<div class="styles">${s.styles.map(x=>`<span>${x}</span>`).join("")}</div>`+body;
  rows=[...panel.querySelectorAll(".track")];
  rows.forEach((r,i)=>{
    r.querySelector(".pbtn").onclick=()=>toggle(i);
    r.querySelector(".bar").onclick=e=>{if(cur!==i||!audio.duration)return;const b=e.currentTarget.getBoundingClientRect();audio.currentTime=(e.clientX-b.left)/b.width*audio.duration};
  });
  document.title=s.name+" | Rapture Studios";window.scrollTo(0,0);
}
function route(){show(location.hash.replace("#",""))}
addEventListener("hashchange",route);route();
back.onclick=()=>{location.hash=""; history.replaceState(null,"",location.pathname+location.search); route()};
$(".brand").onclick=e=>{e.preventDefault();history.replaceState(null,"",location.pathname+location.search);route()};

// lightbox
const lb=$("#lb"),lbi=lb.querySelector("img");
panel.addEventListener("click",e=>{const t=e.target.closest(".thumb");if(!t)return;const im=t.querySelector("img");lbi.src=im.src;lbi.alt=im.alt;lb.classList.add("open")});
lb.onclick=e=>{if(e.target!==lbi)lb.classList.remove("open")};
addEventListener("keydown",e=>{if(e.key==="Escape")lb.classList.remove("open")});
</script>
</body>
</html>
