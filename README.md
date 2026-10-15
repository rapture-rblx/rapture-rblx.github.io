<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#111410">
  <title>Rapture Studios | Worlds with feeling.</title>
  <meta name="description" content="Rapture Studios creates Roblox worlds, original music, sound effects and Luau scripts. Explore the portfolio and talk about your next project.">
  <meta property="og:title" content="Rapture Studios — Worlds with feeling.">
  <meta property="og:description" content="Roblox builds, original music, SFX and scripts. Made to bring your ideas to life.">
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='14' fill='%23111410'/%3E%3Cpath d='M20 48V16h14a10 10 0 0 1 3 19.6L46 48h-8l-7-11h-5v11z M26 22v9h8a4.5 4.5 0 0 0 0-9z' fill='%239df6b1'/%3E%3C/svg%3E">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Manrope:wght@400;500;600;700;800&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root{--bg:#111410;--surface:#191d17;--surface-2:#22271e;--ink:#f0f1e7;--muted:#a5ad9d;--line:#343b2f;--accent:#9df6b1;--display:"Space Grotesk","Arial Black",Arial,sans-serif;--body:"Manrope","Segoe UI",sans-serif;--mono:"DM Mono",Consolas,monospace;--gutter:clamp(20px,4.5vw,76px);--radius:5px}
    *,*::before,*::after{box-sizing:border-box}
    html{scroll-behavior:smooth;scroll-padding-top:110px}
    body{margin:0;background:var(--bg);color:var(--ink);font-family:var(--body);font-size:15px;line-height:1.65;-webkit-font-smoothing:antialiased}
    body.modal-open{overflow:hidden}
    ::selection{background:var(--accent);color:var(--bg)}
    a{color:inherit;text-decoration:none}
    button,input{font:inherit}
    button{color:inherit;cursor:pointer}
    button,a,input{-webkit-tap-highlight-color:transparent}
    button{border:0}
    img,svg{display:block;max-width:100%}
    h1,h2,h3,p{margin:0}
    [hidden]{display:none!important}
    :focus-visible{outline:2px solid var(--accent);outline-offset:6px}
    .shell{width:min(100%,1600px);padding-inline:var(--gutter);margin-inline:auto}
    .mono{font-family:var(--mono);font-size:10px;line-height:1.5;letter-spacing:.14em;text-transform:uppercase}
    .eyebrow{display:flex;align-items:center;gap:10px;color:var(--muted)}
    .eyebrow::before{content:"";width:7px;height:7px;background:var(--accent);flex:none}
    .arrow{width:19px;height:19px;flex:none;stroke:currentColor;stroke-width:1.6;fill:none}
    .skip{position:fixed;left:20px;top:-100px;z-index:200;padding:12px 20px;background:var(--accent);color:var(--bg)}
    .skip:focus{top:12px}
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}

    /* Navigation */
    .top{position:sticky;top:0;z-index:30;background:rgba(17,20,16,.92);backdrop-filter:blur(18px);border-bottom:1px solid var(--line)}
    .top-inner{height:90px;display:flex;align-items:center;justify-content:space-between;gap:30px}
    .brand{display:flex;align-items:center;gap:12px;flex-shrink:0}
    .brand-mark{width:36px;height:40px;color:var(--accent)}
    .brand-name{font:700 17px/.96 var(--display);letter-spacing:-.05em}
    .brand-name span{display:block;font:400 9px/1 var(--mono);letter-spacing:.28em;margin-top:7px;text-transform:uppercase}
    .nav{display:flex;align-items:center;gap:32px;margin-left:auto;margin-right:25px}
    .nav a{font-size:12px;color:var(--muted);transition:color .2s}
    .nav a:hover,.nav a[aria-current]{color:var(--ink)}
    .nav a::after{content:"";display:block;width:0;height:1px;background:var(--accent);transition:width .25s}
    .nav a:hover::after{width:100%}
    .nav-cta{display:flex;align-items:center;gap:22px;font-size:12px;font-weight:700;border:1px solid #69755c;padding:11px 17px;border-radius:var(--radius);transition:background .2s,color .2s}
    .nav-cta:hover{background:var(--accent);color:var(--bg);border-color:var(--accent)}
    .menu-toggle{display:none;background:transparent;width:38px;height:38px;align-items:center;justify-content:center;border:1px solid var(--line);border-radius:var(--radius)}
    .menu-toggle svg{width:20px;stroke:currentColor}

    /* Buttons */
    .button{display:inline-flex;align-items:center;justify-content:center;gap:30px;min-height:52px;padding:14px 21px;border:1px solid var(--line);border-radius:var(--radius);font-size:12px;font-weight:800;background:transparent;transition:background .2s,transform .2s,color .2s}
    .button:hover{background:var(--surface-2);transform:translateY(-2px)}
    .button.primary{background:var(--accent);color:#112116;border-color:var(--accent)}
    .button.primary:hover{background:#b4ffc4}
    .text-link{display:inline-flex;align-items:center;gap:15px;font-size:12px;font-weight:700;padding-block:8px;border-bottom:1px solid #69755c}
    .text-link .arrow{transition:transform .2s}
    .text-link:hover .arrow{transform:translate(3px,-3px)}

    /* Hero */
    .hero{position:relative;display:grid;grid-template-columns:1.08fr 1fr;align-items:center;gap:32px;padding-block:75px 58px;min-height:670px}
    .hero-copy{position:relative;z-index:2}
    .hero h1{font:700 clamp(62px,7.35vw,118px)/.96 var(--display);letter-spacing:-.075em;margin:31px 0 27px}
    .hero h1 span{display:block}
    .hero h1 em{color:var(--accent);font-style:normal}
    .hero-description{color:var(--muted);font-size:14px;max-width:350px;line-height:1.85}
    .hero-actions{display:flex;align-items:center;gap:27px;margin-top:30px}
    .hero-actions .text-link{border:0;color:var(--muted)}
    .hero-art{position:relative;align-self:stretch;min-height:510px;display:flex;align-items:center;justify-content:center;perspective:1000px;isolation:isolate}
    .hero-art::before{content:"";position:absolute;inset:35px 0;background:radial-gradient(ellipse at center,#28432a55,transparent 65%);z-index:-1}
    .art-grid{position:absolute;inset:22px -10px;background-image:linear-gradient(#78956b0e 1px,transparent 1px),linear-gradient(90deg,#78956b0e 1px,transparent 1px);background-size:38px 38px;mask-image:radial-gradient(ellipse,black 25%,transparent 70%)}
    .world{width:100%;overflow:visible;transform:rotate(-4deg);animation:world-float 9s ease-in-out infinite}
    .world .signal{animation:signal 4s ease-in-out infinite}
    .art-top,.art-bottom{position:absolute;left:10%;right:0;display:flex;justify-content:space-between;color:#9dac91;z-index:2;font-size:9px;letter-spacing:.08em}
    .art-top{top:32px}.art-bottom{bottom:30px}
    .art-top span:last-child{color:var(--accent)}
    .art-caption{position:absolute;bottom:90px;left:3%;display:flex;align-items:center;gap:10px;border:1px solid #57654b;background:#161c14e6;padding:10px 14px;backdrop-filter:blur(10px);font-size:10px;letter-spacing:0;color:var(--ink);transform:rotate(-4deg)}
    .art-caption .cross{font:300 22px/1 var(--display);color:var(--accent)}
    .hero-bottom{border-top:1px solid var(--line);padding-block:20px;display:flex;justify-content:space-between;align-items:center;color:var(--muted)}
    .hero-bottom .scroll-note{display:flex;align-items:center;gap:12px;font-size:9px}
    .hero-bottom .scroll-note .arrow{transform:rotate(90deg);width:14px}
    .discipline-line{display:flex;align-items:center;gap:18px;font-size:9px;letter-spacing:.14em}
    .discipline-line i{width:3px;height:3px;background:var(--accent)}

    /* Sections */
    .section{padding-block:90px}
    .section-head{display:flex;justify-content:space-between;align-items:flex-end;gap:30px;margin-bottom:36px}
    .section-label{font:400 10px/1 var(--mono);letter-spacing:.12em;color:var(--muted);text-transform:uppercase;margin-bottom:20px;display:flex;gap:13px;align-items:center}
    .section-label span{color:var(--accent)}
    .section h2,.panel h1{font:500 clamp(38px,4.2vw,65px)/1.04 var(--display);letter-spacing:-.055em}
    .section-head p{color:var(--muted);font-size:13px;max-width:310px;margin-top:16px}

    /* Selected projects */
    .work-section{padding-top:73px}
    .project-grid{display:grid;grid-template-columns:1fr 1fr;gap:36px 26px}
    .project-card{min-width:0;display:block}
    .project-image{position:relative;aspect-ratio:1.62;overflow:hidden;border-radius:var(--radius);background:#222a20;isolation:isolate;border:1px solid #384132}
    .project-image img{width:100%;height:100%;object-fit:cover;transition:transform .7s cubic-bezier(.2,.65,.2,1);position:relative;z-index:1}
    .project-card:hover img{transform:scale(1.035)}
    .project-image::after{content:"";position:absolute;inset:50% 0 0;z-index:2;background:linear-gradient(transparent,#0e160b55);pointer-events:none}
    .project-tag{position:absolute;top:16px;left:16px;z-index:3;background:#111a11d9;border:1px solid #c0dfb330;color:#d8e6cd;padding:6px 9px;font:400 9px/1.2 var(--mono);letter-spacing:.07em;text-transform:uppercase;backdrop-filter:blur(8px)}
    .project-open{position:absolute;bottom:17px;right:17px;z-index:3;width:38px;height:38px;display:grid;place-items:center;background:var(--ink);border-radius:50%;color:var(--bg);transition:background .2s,transform .2s}
    .project-card:hover .project-open{background:var(--accent);transform:rotate(45deg)}
    .project-meta{display:flex;justify-content:space-between;align-items:center;gap:15px;padding-top:18px}
    .project-meta h3{font:500 clamp(18px,2vw,24px)/1.15 var(--display);letter-spacing:-.035em}
    .project-meta p{color:var(--muted);font-size:11px;margin-top:7px}
    .project-num{font:400 11px var(--mono);color:#88967b}
    .fallback-art{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;flex-direction:column;gap:15px;background-color:#222c20;background-image:linear-gradient(30deg,#789d5710 12%,transparent 12.5%,transparent 87%,#789d5710 87.5%),linear-gradient(150deg,#789d5710 12%,transparent 12.5%,transparent 87%,#789d5710 87.5%),linear-gradient(30deg,#789d5710 12%,transparent 12.5%,transparent 87%,#789d5710 87.5%),linear-gradient(150deg,#789d5710 12%,transparent 12.5%,transparent 87%,#789d5710 87.5%);background-size:100px 174px;background-position:0 0,0 0,50px 87px,50px 87px;color:#b1c8a2}
    .fallback-art .placeholder-mark{width:57px;height:57px;color:#94af7d;opacity:.65}
    .fallback-art strong{font:500 clamp(15px,1.9vw,26px) var(--display);letter-spacing:-.04em;max-width:90%;text-align:center}
    .fallback-art small{font:400 9px var(--mono);text-transform:uppercase;letter-spacing:.1em;opacity:.65}
    .project-card:nth-child(2) .fallback-art{background-color:#282a27;filter:saturate(.2)}
    .project-card:nth-child(3) .fallback-art{background-color:#302b20;color:#c3b99a;filter:sepia(.3)}
    .project-card:nth-child(4) .fallback-art{background-color:#242c2c;filter:hue-rotate(40deg)}

    /* Services */
    .services-section{border-top:1px solid var(--line);border-bottom:1px solid var(--line);background:#171b14}
    .services-grid{display:grid;grid-template-columns:repeat(4,1fr);border-top:1px solid var(--line);border-bottom:1px solid var(--line)}
    .service{--c:var(--accent);padding:30px 24px 27px;border-right:1px solid var(--line);position:relative;display:flex;flex-direction:column;min-height:300px;transition:background .25s}
    .service:first-child{padding-left:0}.service:last-child{padding-right:0;border-right:0}
    .service:hover{background:color-mix(in srgb,var(--c) 5%,transparent)}
    .service-top{display:flex;align-items:center;justify-content:space-between;margin-bottom:41px;color:var(--c)}
    .service-icon{width:30px;height:30px}.service-icon svg{width:100%;height:100%}
    .service-index{font:400 10px var(--mono);color:var(--muted)}
    .service h3{font:500 27px/1 var(--display);letter-spacing:-.04em}
    .service p{font-size:12px;color:var(--muted);line-height:1.9;margin-top:15px;max-width:210px}
    .service-bottom{display:flex;justify-content:space-between;align-items:center;margin-top:auto;padding-top:30px;font:400 9px var(--mono);letter-spacing:.07em;text-transform:uppercase;color:var(--c)}
    .service-bottom .arrow{transition:transform .2s}.service:hover .arrow{transform:translate(3px,-3px)}

    /* Music preview */
    .sound-section{display:grid;grid-template-columns:.9fr 1fr;gap:clamp(30px,8vw,130px);align-items:center}
    .sound-intro>p{color:var(--muted);font-size:13px;line-height:1.9;max-width:360px;margin-top:24px}
    .sound-intro>.text-link{margin-top:25px}
    .sound-visual{border:1px solid var(--line);border-radius:var(--radius);background:var(--surface);padding:30px;position:relative;overflow:hidden}
    .sound-top{display:flex;gap:17px;align-items:center}
    .cover-art{width:80px;height:80px;position:relative;flex:none;background:#354030;overflow:hidden;border-radius:2px;display:grid;place-items:center}
    .cover-art svg{width:34px;color:var(--accent)}
    .cover-art img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
    .sound-top h3{font:500 25px var(--display);letter-spacing:-.04em}
    .sound-top p{font:400 9px var(--mono);letter-spacing:.1em;text-transform:uppercase;color:var(--muted);margin-top:5px}
    .waveform{display:flex;gap:4px;align-items:center;justify-content:center;height:105px;margin-top:20px;overflow:hidden}
    .waveform span{flex:1;max-width:5px;min-width:2px;height:var(--h);background:var(--accent);opacity:.75;border-radius:1px;transform-origin:center;animation:wave 1.8s ease-in-out infinite alternate;animation-delay:var(--d);animation-play-state:paused}
    .sound-visual:hover .waveform span{animation-play-state:running}
    .sound-bottom{display:flex;justify-content:space-between;align-items:center;border-top:1px solid var(--line);padding-top:20px;color:var(--muted)}
    .sound-bottom span{font-size:9px}
    .listen-link{width:38px;height:38px;display:grid;place-items:center;background:var(--accent);color:var(--bg);border-radius:50%}
    .listen-link svg{width:14px;height:14px;fill:currentColor;margin-left:2px}

    /* Contact */
    .contact{background:var(--accent);color:#142219;padding-block:66px 25px;position:relative;overflow:hidden}
    .contact .section-label{color:#3d6547;margin-bottom:23px}.contact .section-label span{color:#142219}
    .contact-main{display:flex;align-items:center;justify-content:space-between;gap:36px;padding-bottom:50px}
    .contact h2{font:500 clamp(45px,6vw,90px)/1 var(--display);letter-spacing:-.065em}
    .contact h2 span{display:block}
    .contact-cta{display:flex;align-items:center;gap:25px;background:#15231a;color:var(--ink);padding:20px 27px;border-radius:var(--radius);font-size:13px;font-weight:700;white-space:nowrap;transition:transform .2s,background .2s}
    .contact-cta:hover{background:#284131;transform:translateY(-3px)}
    .contact-note{font-size:11px;margin-top:12px;text-align:right;color:#3a6044}
    .footer-bottom{border-top:1px solid #15231a40;display:flex;align-items:center;justify-content:space-between;gap:20px;padding-top:25px;font-size:10px}
    .socials{display:flex;gap:24px}.socials a{display:flex;gap:6px;align-items:center}.socials .arrow{width:11px;height:11px}
    .socials a:hover{text-decoration:underline;text-underline-offset:4px}
    .copyright{color:#365a3e}
    .footer-sign{display:flex;gap:8px;align-items:center;font:500 11px var(--display);letter-spacing:-.02em}
    .footer-sign .brand-mark{width:18px;height:20px;color:#15231a}

    /* Service views retain the original #builds, #music, #sfx and #scripts URLs. */
    .panel{--c:var(--accent);padding-top:40px;padding-bottom:90px;min-height:75vh}
    .back{display:inline-flex;gap:9px;align-items:center;background:transparent;color:var(--muted);font:400 10px var(--mono);text-transform:uppercase;letter-spacing:.06em;padding:10px 0;margin-bottom:40px}
    .back .arrow{width:15px;transform:rotate(180deg)}.back:hover{color:var(--ink)}
    .panel-heading{display:flex;justify-content:space-between;align-items:flex-end;gap:35px;border-bottom:1px solid var(--line);padding-bottom:34px}
    .panel-heading h1{font-size:clamp(58px,7.3vw,110px);line-height:.95;margin-top:20px}
    .panel-heading p{color:var(--muted);font-size:13px;max-width:490px;margin-top:22px}
    .panel .section-label span{color:var(--c)}
    .quote{flex:none;display:flex;flex-direction:column;align-items:flex-start;gap:9px;border:1px solid var(--line);padding:20px 25px;min-width:190px;border-radius:var(--radius)}
    .quote small{color:var(--muted);font:400 9px var(--mono);text-transform:uppercase;letter-spacing:.12em}
    .quote strong{display:flex;align-items:center;gap:20px;color:var(--c);font:500 21px var(--display);letter-spacing:-.03em}
    .quote:hover{border-color:var(--c)}
    .styles{display:flex;gap:8px;flex-wrap:wrap;margin:25px 0 45px}
    .styles span{font:400 10px var(--mono);color:var(--muted);padding:8px 12px;border:1px solid var(--line);border-radius:3px}
    .project-group{margin-top:48px;scroll-margin-top:120px}
    .group-head{display:flex;justify-content:space-between;align-items:center;gap:20px;margin-bottom:19px}
    .group-title{display:flex;flex-wrap:wrap;align-items:center;gap:13px}
    .group-title h2{font:500 clamp(24px,3vw,36px)/1.15 var(--display);letter-spacing:-.04em}
    .group-count{font:400 10px var(--mono);color:var(--muted);white-space:nowrap}
    .status{font:400 8px var(--mono);letter-spacing:.04em;text-transform:uppercase;color:#e7cc91;border:1px solid #5c533e;padding:5px 8px}
    .thumbs{display:grid;grid-template-columns:repeat(3,1fr);gap:15px}
    .thumb{padding:0;background:var(--surface);border:1px solid var(--line);border-radius:var(--radius);overflow:hidden;text-align:left;cursor:zoom-in}
    .thumb-image{display:block;aspect-ratio:1.6;position:relative;overflow:hidden}
    .thumb-image img{position:relative;z-index:1;width:100%;height:100%;object-fit:cover;transition:transform .5s}
    .thumb:hover img{transform:scale(1.04)}
    .thumb-caption{display:flex;align-items:center;justify-content:space-between;padding:12px 14px;font-size:11px;color:var(--muted)}
    .thumb-caption .arrow{width:14px;height:14px;color:var(--c)}
    .thumb .fallback-art strong{font-size:15px}.thumb .placeholder-mark{width:35px;height:35px}

    /* Audio player */
    .music-layout{display:grid;grid-template-columns:320px 1fr;gap:50px;margin-top:40px}
    .album-cover{aspect-ratio:1;position:relative;overflow:hidden;background:#2c3627;border:1px solid #46523c;border-radius:var(--radius)}
    .album-cover img{position:relative;z-index:1;width:100%;height:100%;object-fit:cover}
    .album-note{color:var(--muted);font:400 9px/1.8 var(--mono);letter-spacing:.08em;text-transform:uppercase;margin-top:15px}
    .player-title{display:flex;align-items:center;justify-content:space-between;gap:15px;margin-bottom:24px}
    .player-title h2{font:500 34px/1 var(--display);letter-spacing:-.05em}
    .player-title>span{font:400 9px var(--mono);color:var(--muted);text-transform:uppercase;letter-spacing:.08em}
    .track{display:grid;grid-template-columns:42px 1fr 82px;gap:17px;align-items:center;border-top:1px solid var(--line);padding:22px 0;transition:background .2s}
    .track:last-child{border-bottom:1px solid var(--line)}
    .pbtn{width:42px;height:42px;border-radius:50%;border:1px solid #56604c;background:transparent;color:var(--ink);display:grid;place-items:center;transition:background .2s,color .2s}
    .pbtn:hover,.track.playing .pbtn{background:var(--c);border-color:var(--c);color:#16141d}
    .pbtn svg{width:14px;height:14px;fill:currentColor}
    .pbtn .pa{display:none}
    .track.playing .pbtn .pl{display:none}
    .track.playing .pbtn .pa{display:block}
    .track-info{min-width:0}
    .track-info strong{font-size:12px;font-weight:600;display:block}
    .track-info small{display:block;color:var(--muted);font:400 8px var(--mono);letter-spacing:.06em;text-transform:uppercase;margin-top:4px}
    .seek{width:100%;height:18px;display:block;margin:7px 0 0;accent-color:var(--c);cursor:pointer}
    .seek:disabled{opacity:.35;cursor:default}
    .time{font:400 9px var(--mono);color:var(--muted);text-align:right}
    .audio-message{color:#e6bb80;font-size:12px;min-height:23px;margin-top:14px}

    /* SFX and scripts */
    .request-panel{display:grid;grid-template-columns:1fr 1fr;border:1px solid var(--line);border-radius:var(--radius);margin-top:45px;overflow:hidden}
    .request-copy{padding:45px}
    .request-copy h2{font:500 clamp(28px,4vw,43px)/1.1 var(--display);letter-spacing:-.04em}
    .request-copy p{color:var(--muted);font-size:13px;line-height:1.9;margin:20px 0 27px;max-width:390px}
    .request-art{min-height:280px;background:color-mix(in srgb,var(--c) 5%,var(--surface));display:flex;align-items:center;justify-content:center;position:relative;border-left:1px solid var(--line);overflow:hidden}
    .request-art::before,.request-art::after{content:"";position:absolute;width:230px;height:230px;border:1px solid color-mix(in srgb,var(--c) 18%,transparent);border-radius:50%}
    .request-art::after{width:330px;height:330px}
    .request-art .service-icon{width:80px;height:80px;color:var(--c)}
    .request-art .mono{position:absolute;bottom:20px;color:var(--muted);font-size:8px}

    /* Image viewer */
    dialog{padding:0;border:1px solid #59644f;border-radius:6px;background:#111410;color:var(--ink);max-width:min(1200px,calc(100vw - 32px));width:fit-content;max-height:calc(100dvh - 32px);overflow:auto}
    dialog::backdrop{background:#060a07ec;backdrop-filter:blur(8px)}
    .lightbox-top{display:flex;align-items:center;justify-content:space-between;padding:14px 18px;gap:30px;font:400 10px var(--mono);color:var(--muted)}
    .close{width:32px;height:32px;background:var(--surface-2);border:1px solid var(--line);border-radius:50%;font-size:22px;line-height:1}
    .lightbox-stage{position:relative;min-width:min(700px,calc(100vw - 34px));min-height:180px;display:grid;place-items:center;background:#0c100b}
    .lightbox-stage img{max-height:72dvh;max-width:100%;object-fit:contain}
    .lightbox-error{padding:50px 25px;color:var(--muted);text-align:center;font-size:13px}
    .lightbox-bottom{display:flex;align-items:center;justify-content:space-between;gap:15px;padding:13px 18px}
    .lightbox-caption{font-size:12px}
    .lightbox-count{color:var(--muted);font:400 10px var(--mono);margin-left:9px}
    .lightbox-controls{display:flex;gap:8px}
    .lightbox-controls button{display:grid;place-items:center;width:36px;height:36px;background:var(--surface-2);border:1px solid var(--line);border-radius:3px}
    .lightbox-controls button:first-child .arrow{transform:rotate(180deg)}
    .lightbox-controls button:disabled{opacity:.3;cursor:default}

    /* Motion */
    .view-enter{animation:enter .4s ease both}
    @keyframes enter{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
    @keyframes world-float{0%,100%{transform:translateY(0) rotate(-4deg)}50%{transform:translateY(-12px) rotate(-2deg)}}
    @keyframes signal{0%,100%{opacity:.5}50%{opacity:1}}
    @keyframes wave{from{transform:scaleY(.45)}to{transform:scaleY(1)}}

    /* Responsive layouts */
    @media(min-width:1600px){
      .hero{min-height:730px}
      .hero-art{min-height:570px}
    }

    @media(max-width:1100px){
      .nav{gap:23px;margin-right:0}
      .hero{gap:15px;min-height:600px;padding-top:55px}
      .hero-art{min-height:450px}
      .hero h1{font-size:clamp(65px,8vw,95px)}
      .hero-actions{gap:18px}
      .hero-actions .button{gap:17px}
      .service{padding-inline:20px}
      .service h3{font-size:24px}
      .service p{font-size:11px}
      .music-layout{grid-template-columns:260px 1fr;gap:35px}
      .sound-section{gap:45px}
      .contact-main{gap:30px}
    }

    @media(max-width:800px){
      .top-inner{height:74px;gap:20px}
      .nav{gap:20px}
      .nav-cta{padding:9px 12px;gap:12px}
      .hero{padding-top:48px;min-height:560px;grid-template-columns:1.1fr 1fr;gap:0}
      .hero h1{font-size:clamp(60px,8.5vw,78px)}
      .hero-art{min-height:400px}
      .art-top,.art-bottom{font-size:7px;left:0}
      .art-caption{bottom:65px;font-size:8px;padding:7px 9px;left:0}
      .hero-description{font-size:12px;max-width:290px}
      .hero-actions{flex-wrap:wrap;gap:10px}
      .hero-actions .text-link{font-size:10px}
      .hero-actions .button{min-height:47px;font-size:11px}
      .eyebrow{font-size:8px}
      .section{padding-block:65px}
      .services-grid{grid-template-columns:1fr 1fr}
      .service{min-height:270px;padding:26px!important}
      .service:nth-child(2){border-right:0}
      .service:nth-child(-n+2){border-bottom:1px solid var(--line)}
      .service-top{margin-bottom:25px}
      .service p{font-size:12px}
      .section-head{gap:20px}
      .project-grid{gap:30px 18px}
      .project-meta h3{font-size:20px}
      .sound-section{grid-template-columns:1fr 1fr;gap:35px}
      .sound-visual{padding:22px}
      .sound-top{gap:12px}
      .cover-art{width:60px;height:60px}
      .sound-top h3{font-size:22px}
      .contact-main{align-items:flex-start}
      .contact-cta{padding:17px 20px;font-size:11px;gap:16px}
      .contact-note{font-size:9px}
      .contact h2{font-size:clamp(44px,6.3vw,70px)}
      .thumbs{grid-template-columns:repeat(2,1fr)}
      .music-layout{grid-template-columns:200px 1fr;gap:25px}
      .track{gap:12px;grid-template-columns:38px 1fr 65px}
      .pbtn{width:38px;height:38px}
      .time{font-size:8px}
      .player-title{align-items:flex-start;flex-direction:column;gap:9px}
      .request-copy{padding:30px}
      .footer-bottom{flex-wrap:wrap}
      .copyright{order:3;width:100%}
    }

    @media(max-width:600px){
      .top-inner{height:70px;gap:13px}
      .brand-name{font-size:15px}
      .brand-mark{width:29px;height:33px}
      .brand-name span{font-size:7px}
      .nav-cta{margin-left:auto;font-size:10px;padding:9px 11px;gap:10px}
      .nav-cta .arrow{width:15px}
      .menu-toggle{display:flex;flex:none}
      .nav{display:none;position:absolute;top:70px;left:0;right:0;margin:0;padding:20px var(--gutter);border-bottom:1px solid var(--line);background:var(--bg)}
      .nav.open{display:flex;justify-content:space-between}
      .nav a{font-size:13px}
      .hero{grid-template-columns:1fr;padding-top:45px;padding-bottom:25px;gap:0}
      .hero h1{font-size:clamp(63px,12.3vw,84px);margin-block:25px 20px;max-width:100%}
      .hero-description{font-size:13px;max-width:330px}
      .eyebrow{font-size:8px}
      .hero-actions{gap:22px;margin-top:25px}
      .hero-actions .text-link{font-size:11px}
      .hero-art{min-height:340px;max-width:420px;width:100%;margin:8px auto 0}
      .world{max-height:380px}
      .art-top{top:15px;left:7%;right:4%;font-size:7px}
      .art-bottom{bottom:15px;left:7%;right:4%;font-size:7px}
      .art-caption{bottom:65px;left:8%;font-size:8px}
      .hero-bottom{padding-block:17px}
      .discipline-line{gap:11px;font-size:7px;letter-spacing:.06em}
      .hero-bottom .scroll-note{font-size:7px;gap:5px}
      .hero-bottom .scroll-note .arrow{width:11px}
      .section{padding-block:55px}
      .section-head{align-items:flex-start;gap:20px}
      .section-label{font-size:9px;margin-bottom:17px}
      .section h2{font-size:40px}
      .section-head .text-link{font-size:10px;gap:8px;white-space:nowrap;margin-top:30px}
      .section-head p{font-size:12px}
      .project-grid{grid-template-columns:1fr;gap:30px}
      .project-image{aspect-ratio:1.55}
      .project-meta{padding-top:14px}
      .project-meta h3{font-size:24px}
      .project-tag{font-size:8px;left:12px;top:12px}
      .project-open{width:34px;height:34px}
      .fallback-art strong{font-size:23px}
      .services-section .section-head{display:block}
      .services-section .section-head p{max-width:330px}
      .service{padding:24px 17px!important;min-height:260px}
      .service:nth-child(odd){padding-left:0!important}
      .service:nth-child(even){padding-right:0!important}
      .service h3{font-size:25px}
      .service p{font-size:11px}
      .service-bottom{font-size:8px}
      .service-icon{width:27px;height:27px}
      .sound-section{grid-template-columns:1fr;gap:30px}
      .sound-intro>p{margin-top:20px}
      .sound-visual{padding:25px}
      .cover-art{width:70px;height:70px}
      .sound-top h3{font-size:27px}
      .contact{padding-top:50px}
      .contact-main{flex-direction:column;gap:30px;padding-bottom:40px}
      .contact h2{font-size:clamp(48px,10.5vw,65px)}
      .contact-note{text-align:left;font-size:10px}
      .contact-cta{font-size:12px;gap:40px}
      .footer-bottom{gap:20px;font-size:9px}
      .socials{gap:16px}
      .copyright{font-size:8px}
      .panel{padding-top:24px;padding-bottom:55px}
      .back{margin-bottom:28px}
      .panel-heading{display:block;padding-bottom:25px}
      .panel-heading h1{font-size:64px;margin-top:12px}
      .panel-heading p{font-size:12px}
      .quote{margin-top:25px;width:fit-content;min-width:0;padding:12px 17px;gap:4px}
      .quote strong{font-size:19px}
      .styles{gap:6px;margin-block:20px 30px}
      .styles span{font-size:9px;padding:7px 9px}
      .project-group{margin-top:36px}
      .group-head{align-items:flex-start;gap:12px}
      .group-title h2{font-size:25px}
      .group-count{font-size:8px;padding-top:5px}
      .thumbs{gap:10px}
      .thumb-caption{padding:10px;font-size:9px;gap:6px}
      .thumb-caption .arrow{width:11px;flex:none}
      .thumb .fallback-art{gap:6px}
      .thumb .fallback-art strong{font-size:12px}
      .thumb .fallback-art small{font-size:7px}
      .thumb .placeholder-mark{width:25px;height:25px}
      .music-layout{grid-template-columns:1fr;gap:30px;margin-top:30px}
      .album{display:flex;gap:20px;align-items:flex-end}
      .album-cover{width:130px;flex:none}
      .album-note{max-width:160px;margin:0}
      .player-title{flex-direction:row;align-items:center}
      .player-title h2{font-size:30px}
      .player-title>span{font-size:8px}
      .track{grid-template-columns:40px 1fr 70px;gap:14px;padding-block:18px}
      .pbtn{width:40px;height:40px}
      .track-info strong{font-size:12px}
      .request-panel{grid-template-columns:1fr}
      .request-copy{padding:28px 24px}
      .request-art{min-height:210px;border-top:1px solid var(--line);border-left:0}
      .request-art::before{width:150px;height:150px}
      .request-art::after{width:240px;height:240px}
      .request-art .service-icon{width:60px;height:60px}
      .lightbox-top{padding:10px 12px;font-size:8px;gap:12px}
      .lightbox-bottom{padding:12px}
      .lightbox-caption{font-size:10px}
      .lightbox-count{font-size:8px;display:block;margin:3px 0 0}
    }

    @media(max-width:360px){
      :root{--gutter:16px}
      .top-inner{gap:10px}
      .brand{gap:8px}
      .brand-name{font-size:14px}
      .nav-cta{padding:8px;font-size:9px;gap:5px}
      .menu-toggle{width:32px;height:32px}
      .hero h1{font-size:61px}
      .hero-art{min-height:300px}
      .hero-actions{gap:16px}
      .section h2{font-size:35px}
      .section-head .text-link{font-size:9px;gap:5px}
      .section-head .text-link .arrow{width:13px}
      .service h3{font-size:23px}
      .track{gap:10px;grid-template-columns:36px 1fr 62px}
      .pbtn{width:36px;height:36px}
      .socials{gap:12px}
      .footer-sign{font-size:10px}
    }

    @media(prefers-reduced-motion:reduce){
      html{scroll-behavior:auto}
      *,*::before,*::after{animation:none!important;transition:none!important}
    }
  </style>
</head>

<body>
  <a class="skip" href="#main">Skip to content</a>

  <svg width="0" height="0" style="position:absolute" aria-hidden="true">
    <defs>
      <symbol id="arrow" viewBox="0 0 24 24">
        <path d="M5 19 19 5M5 5h14v14"/>
      </symbol>
      <symbol id="arrow-right" viewBox="0 0 24 24">
        <path d="M4 12h15m-6-6 6 6-6 6"/>
      </symbol>
      <symbol id="mark" viewBox="0 0 40 44">
        <path fill="currentColor" d="M2 42V2h20c10 0 16 5 16 13 0 6-3 10-9 12l11 15H28L16 25h6c5 0 7-3 7-7s-2-7-7-7H12v31z"/>
      </symbol>
      <symbol id="cube" viewBox="0 0 24 24">
        <path d="m12 2 10 6v9l-10 6-10-6V8zM2 8l10 6 10-6M12 14v9" fill="none" stroke="currentColor" stroke-width="1.2" stroke-linejoin="round"/>
      </symbol>
    </defs>
  </svg>

  <header class="top">
    <div class="shell top-inner">
      <a class="brand" href="#home" aria-label="Rapture Studios home">
        <svg class="brand-mark" aria-hidden="true"><use href="#mark"/></svg>
        <span class="brand-name">RAPTURE<span>Studios</span></span>
      </a>

      <nav class="nav" id="navigation" aria-label="Main navigation">
        <a href="#work">Selected work</a>
        <a href="#services">Services</a>
        <a href="#music">Music</a>
      </nav>

      <a class="nav-cta" href="https://discord.gg/arvm99rawt" target="_blank" rel="noopener">
        Let’s talk
        <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
      </a>

      <button class="menu-toggle" aria-expanded="false" aria-controls="navigation" aria-label="Open navigation">
        <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
          <path d="M4 8h16M4 16h16" stroke-width="1.5"/>
        </svg>
      </button>
    </div>
  </header>

  <main id="main" tabindex="-1">
    <div id="home">
      <div class="shell">
        <section class="hero" aria-labelledby="hero-title">
          <div class="hero-copy">
            <p class="eyebrow mono">Independent Roblox creative</p>
            <h1 id="hero-title" tabindex="-1">
              <span>WORLDS</span>
              <span>WITH</span>
              <span><em>FEELING.</em></span>
            </h1>

            <p class="hero-description">
              Places to get lost in. Sounds that stay with you.
              I build the details that bring your Roblox experience to life.
            </p>

            <div class="hero-actions">
              <a class="button primary" href="#work">
                Explore my work
                <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
              </a>
              <a class="text-link" href="#services">
                Find your next piece
                <svg class="arrow" aria-hidden="true"><use href="#arrow-right"/></svg>
              </a>
            </div>
          </div>

          <div class="hero-art" aria-hidden="true">
            <div class="art-grid"></div>

            <div class="art-top mono">
              <span>R / STUDIO EXPLORATIONS</span>
              <span>[ WORLD_01 ]</span>
            </div>

            <svg class="world" viewBox="0 0 620 560" fill="none">
              <defs>
                <linearGradient id="slab" x1="120" y1="250" x2="500" y2="470" gradientUnits="userSpaceOnUse">
                  <stop stop-color="#c1f1b3"/>
                  <stop offset="1" stop-color="#719961"/>
                </linearGradient>
                <linearGradient id="face" x1="170" y1="150" x2="370" y2="410" gradientUnits="userSpaceOnUse">
                  <stop stop-color="#425b38"/>
                  <stop offset="1" stop-color="#263b21"/>
                </linearGradient>
                <linearGradient id="glass" x1="260" y1="170" x2="410" y2="370" gradientUnits="userSpaceOnUse">
                  <stop stop-color="#a5ffc5" stop-opacity=".5"/>
                  <stop offset="1" stop-color="#7ccc90" stop-opacity=".08"/>
                </linearGradient>
                <pattern id="grid" width="22" height="22" patternUnits="userSpaceOnUse" patternTransform="matrix(1 .5 -1 .5 310 190)">
                  <path d="M22 0H0V22" stroke="#34482c" stroke-width=".8" opacity=".5"/>
                </pattern>
              </defs>

              <ellipse cx="316" cy="450" rx="207" ry="55" fill="#060b05" opacity=".35"/>
              <path d="m60 325 250-130 250 130-250 130z" stroke="#7b9c66" stroke-opacity=".4" stroke-dasharray="4 6"/>
              <path d="m60 350 250-130 250 130-250 130z" stroke="#7b9c66" stroke-opacity=".18"/>
              <path d="m114 323 196-102 196 102v42L310 467 114 365z" fill="#23321d" stroke="#73995c"/>
              <path d="m114 323 196 102v42L114 365z" fill="#3c4f30"/>
              <path d="m114 323 196-102 196 102-196 102z" fill="url(#slab)" stroke="#d1fac6"/>
              <path d="m114 323 196-102 196 102-196 102z" fill="url(#grid)"/>
              <path d="m136 327 174 89 174-89M310 425v42" stroke="#a5d48d" stroke-opacity=".6"/>
              <path d="m164 299 61-32 61 32v48l-61 32-61-32z" fill="#45613a" stroke="#b1db9e"/>
              <path d="m164 299 61 32v48l-61-32z" fill="#5f8050"/>
              <path d="m164 299 61-32 61 32-61 32z" fill="#bce5a8"/>
              <path d="m179 301 46-24 46 24-46 24z" stroke="#6f9259"/>
              <path d="m237 194 96-50 96 50v156l-96 50-96-50z" fill="url(#face)" stroke="#b0d698" stroke-width="1.2"/>
              <path d="m237 194 96 50v156l-96-50z" fill="#527343"/>
              <path d="m237 194 96-50 96 50-96 50z" fill="#dce9bc"/>
              <path d="m257 195 76-39 76 39-76 39z" fill="#8da371" stroke="#516d42"/>
              <path d="m257 195 76 17 76-17-76 39z" fill="#b5cd9b"/>
              <path d="M333 244v156M254 224v113m19-103v113m19-103v113m19-103v113M350 243v130m20-140v130m20-141v130m20-141v130" stroke="#b9df9c" stroke-opacity=".3"/>
              <path d="m238 247 95 50 95-50m-190 53 95 50 95-50" stroke="#c6dfad" stroke-opacity=".3"/>
              <path d="m333 286 121-63v91l-121 63z" fill="url(#glass)" stroke="#9df6b1"/>
              <path d="m333 286-22-11 121-63 22 11m-143 52v91l22 11" stroke="#9df6b1" stroke-opacity=".7"/>
              <path d="m370 266 24-13v56l-24 13z" fill="#b2ffd0" opacity=".25"/>
              <path d="m203 227 45 23v63l-45-23z" fill="#d9e8ba" stroke="#f0f5db"/>
              <path d="m203 227 21-11 45 23-21 11m0 0 21-11v63l-21 11" fill="#9fb284" stroke="#d6e4bc"/>
              <path d="m390 354 41-22 41 22v31l-41 21-41-21z" fill="#395b35" stroke="#a0cd8e"/>
              <path d="m390 354 41-22 41 22-41 21z" fill="#c3e7ad"/>
              <path d="m390 354 41 21v31" stroke="#a0cd8e"/>
              <path d="m145 349 16 8m-6-11 16 8m-6-11 16 8m-6-11 16 8" stroke="#192d16" stroke-width="3"/>
              <path d="M333 143v-38m-9 5 9-5 9 5" stroke="#b5e09d" stroke-dasharray="3 4"/>
              <path d="m320 93 13-7 13 7-13 7z" fill="#9df6b1" class="signal"/>
              <path d="M120 236H75v45m413-105h45v45M504 405h35v-40" stroke="#a3c18a" stroke-opacity=".6"/>
              <path d="M78 239h-6m3-3v6m455-63h6m-3-3v6m3 220h6m-3-3v6" stroke="#d5e7c2"/>
              <circle cx="125" cy="236" r="3" fill="#9df6b1" class="signal"/>
              <circle cx="485" cy="176" r="3" fill="#9df6b1" class="signal"/>
              <path d="m202 424 85 44m47-5 120-63" stroke="#849874" stroke-dasharray="2 6"/>
            </svg>

            <div class="art-caption mono">
              <span class="cross">+</span>
              A little detail. A whole new world.
            </div>

            <div class="art-bottom mono">
              <span>BUILT FROM AN IDEA.</span>
              <span>IMAGINATION → EXPERIENCE</span>
            </div>
          </div>
        </section>

        <div class="hero-bottom">
          <div class="discipline-line mono">
            <span>BUILD</span><i></i>
            <span>COMPOSE</span><i></i>
            <span>DESIGN</span><i></i>
            <span>DEVELOP</span>
          </div>

          <a class="scroll-note mono" href="#work">
            Scroll to explore
            <svg class="arrow" aria-hidden="true"><use href="#arrow-right"/></svg>
          </a>
        </div>

        <section class="section work-section" id="work" aria-labelledby="work-title">
          <div class="section-head">
            <div>
              <div class="section-label"><span>01 /</span> Selected work</div>
              <h2 id="work-title" tabindex="-1">A world of possibilities.</h2>
            </div>

            <a class="text-link" href="#builds">
              All builds
              <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
            </a>
          </div>

          <div class="project-grid" id="project-grid"></div>
        </section>
      </div>

      <section class="section services-section" id="services" aria-labelledby="services-title">
        <div class="shell">
          <div class="section-head">
            <div>
              <div class="section-label"><span>02 /</span> The toolkit</div>
              <h2 id="services-title" tabindex="-1">Every layer matters.</h2>
            </div>

            <p>
              From the first landscape to the final sound.
              Explore what I can bring to your next experience.
            </p>
          </div>

          <div class="services-grid" id="skills"></div>
        </div>
      </section>

      <section class="shell section sound-section" aria-labelledby="sound-title">
        <div class="sound-intro">
          <div class="section-label"><span>03 /</span> Press play</div>
          <h2 id="sound-title">Set the scene.<br>Find the feeling.</h2>
          <p>
            A world has a sound of its own. Explore original music for Bloomville,
            from the main island to seasonal themes and desert backdrops.
          </p>
          <a class="text-link" href="#music">
            Enter the listening room
            <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
          </a>
        </div>

        <div class="sound-visual">
          <div class="sound-top">
            <div class="cover-art">
              <svg aria-hidden="true"><use href="#cube"/></svg>
              <img src="assets/bloomville.jpg" alt="Bloomville album artwork" loading="lazy" data-fallback>
            </div>
            <div>
              <h3>Bloomville</h3>
              <p>Original game music</p>
            </div>
          </div>

          <div class="waveform" id="waveform" aria-hidden="true"></div>

          <div class="sound-bottom">
            <span class="mono">04 TRACKS / A DIFFERENT ATMOSPHERE</span>
            <a class="listen-link" href="#music" aria-label="Listen to Bloomville">
              <svg viewBox="0 0 16 16" aria-hidden="true">
                <path d="M3 1v14l12-7z"/>
              </svg>
            </a>
          </div>
        </div>
      </section>
    </div>

    <section class="shell panel" id="panel" hidden></section>

    <noscript>
      <div class="shell section">
        <h2>Explore Rapture Studios</h2>
        <p>
          Enable JavaScript to open the project galleries and music player.
          You can also contact me on
          <a href="https://discord.gg/arvm99rawt">Discord</a>
          for examples and prices.
        </p>
      </div>
    </noscript>
  </main>

  <footer class="contact" id="contact">
    <div class="shell">
      <div class="section-label">
        <span>LET’S MAKE SOMETHING</span> / YOUR NEXT PROJECT
      </div>

      <div class="contact-main">
        <h2>Got a world<span>in mind?</span></h2>
        <div>
          <a class="contact-cta" href="https://discord.gg/arvm99rawt" target="_blank" rel="noopener">
            Let’s build it together
            <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
          </a>
          <p class="contact-note">Send the idea. Let’s talk details on Discord.</p>
        </div>
      </div>

      <div class="footer-bottom">
        <a class="footer-sign" href="#home">
          <svg class="brand-mark" aria-hidden="true"><use href="#mark"/></svg>
          RAPTURE STUDIOS
        </a>

        <p class="copyright">
          © <span id="year"></span> Rapture Studios. Made with intention.
        </p>

        <div class="socials">
          <a href="https://discord.gg/arvm99rawt" target="_blank" rel="noopener">
            Discord
            <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
          </a>
          <a href="https://youtube.com/@raprblx" target="_blank" rel="noopener">
            YouTube
            <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
          </a>
          <a href="https://www.tiktok.com/@rapturedevelopment?_r=1&amp;_t=ZN-9AS47enZy5u" target="_blank" rel="noopener">
            TikTok
            <svg class="arrow" aria-hidden="true"><use href="#arrow"/></svg>
          </a>
        </div>
      </div>
    </div>
  </footer>

  <dialog id="lightbox" aria-labelledby="lightbox-project" aria-describedby="lightbox-caption">
    <div class="lightbox-top">
      <span id="lightbox-project"></span>
      <button class="close" aria-label="Close image viewer" autofocus>×</button>
    </div>

    <div class="lightbox-stage">
      <img id="lightbox-image" alt="">
      <p class="lightbox-error" hidden>This image is currently unavailable.</p>
    </div>

    <div class="lightbox-bottom">
      <div>
        <span class="lightbox-caption" id="lightbox-caption"></span>
        <span class="lightbox-count" id="lightbox-count"></span>
      </div>

      <div class="lightbox-controls">
        <button id="image-prev" aria-label="Previous image">
          <svg class="arrow" aria-hidden="true"><use href="#arrow-right"/></svg>
        </button>
        <button id="image-next" aria-label="Next image">
          <svg class="arrow" aria-hidden="true"><use href="#arrow-right"/></svg>
        </button>
      </div>
    </div>
  </dialog>

  <script>
    'use strict';

    /* ================= YOUR CONTENT =================
       Keep this HTML beside your existing assets folder.
       No assets have been renamed.

       Set a price (for example "£10") to show a starting price.
       Empty prices invite a quote.

       No build step is required.
    */

    const SKILLS = {
      builds: {
        name: 'Builds',
        color: '#9df6b1',
        price: '',
        styles: [
          'Roleplay cities',
          'Horror interiors',
          'Desert & war maps',
          'Terrain'
        ],
        description: 'Distinct places with their own atmosphere. From sprawling roleplay cities to the details of a horror interior.',
        short: 'Places with character. Cities, landscapes and everything in between.',
        action: 'Explore the worlds'
      },
      music: {
        name: 'Music',
        color: '#b5a5f4',
        price: '',
        styles: [
          'Seasonal',
          'Halloween',
          'Desert',
          'Looping themes'
        ],
        description: 'Original music that gives your world a mood, a rhythm and a sense of place.',
        short: 'Original themes and looping soundtracks that set the mood.',
        action: 'Find your soundtrack'
      },
      sfx: {
        name: 'SFX',
        color: '#efc18a',
        price: '',
        styles: [
          'Gameplay',
          'Ambience',
          'UI sounds'
        ],
        description: 'The small sounds that make an experience feel alive. Gameplay, ambience and interface audio.',
        short: 'The clicks, cues and atmosphere that make every moment feel right.',
        action: 'Explore sound design'
      },
      scripts: {
        name: 'Scripts',
        color: '#95cddc',
        price: '',
        styles: [
          'Luau',
          'Game systems',
          'Tools'
        ],
        description: 'Luau scripts, game systems and tools to bring the moving parts of your experience together.',
        short: 'Game systems and Luau tools that put your ideas into motion.',
        action: 'See what’s possible'
      }
    };

    const BUILDS = [
      {
        title: 'Orlando State Roleplay',
        type: 'Roleplay / City',
        slug: 'orlando',
        imgs: [
          ['assets/orl-bridge.jpg', 'Rail bridge'],
          ['assets/orl-highway.jpg', 'Highway interchange'],
          ['assets/orl-city.jpg', 'City streets'],
          ['assets/orl-airport.jpg', 'Airport']
        ],
        featured: 2
      },
      {
        title: 'Harold Hill Asylum',
        type: 'Horror / Interiors',
        slug: 'asylum',
        imgs: [
          ['assets/asylum-clearance.jpg', 'Clearance checkpoint'],
          ['assets/asylum-medical.jpg', 'Medical room'],
          ['assets/asylum-containment.jpg', 'Containment chamber']
        ],
        featured: 0
      },
      {
        title: 'Desert Wars',
        type: 'Environment / Terrain',
        slug: 'desert-wars',
        imgs: [
          ['assets/desert-compound.jpg', 'Compound by the lake'],
          ['assets/desert-camp.jpg', 'Base camp'],
          ['assets/desert-hills.jpg', 'Hills']
        ],
        featured: 0
      },
      {
        title: 'Cursed Cargo',
        type: 'World / Props',
        slug: 'cursed-cargo',
        tag: 'In development',
        imgs: [
          ['assets/aerial.jpg', 'Town'],
          ['assets/van.jpg', 'Delivery van'],
          ['assets/boxes.jpg', 'Packages'],
          ['assets/houses.jpg', 'Houses'],
          ['assets/depot.jpg', 'Depot'],
          ['assets/street.jpg', 'Main street']
        ],
        featured: 0
      }
    ];

    const MUSIC = {
      title: 'Bloomville',
      cover: 'assets/bloomville.jpg',
      tracks: [
        {
          title: 'Main Island',
          src: 'assets/main.mp3',
          type: 'Island theme'
        },
        {
          title: 'Halloween Island',
          src: 'assets/halloween.mp3',
          type: 'Seasonal theme'
        },
        {
          title: 'Fall (Backing)',
          src: 'assets/fall.mp3',
          type: 'Seasonal backing'
        },
        {
          title: 'Desert (Backing)',
          src: 'assets/desert.mp3',
          type: 'Desert backing'
        }
      ]
    };

    /* ================= END YOUR CONTENT ================= */

    const ICONS = {
      builds: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"><path d="m12 2 10 6v9l-10 6-10-6V8zM2 8l10 6 10-6M12 14v9"/></svg>',
      music: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"><path d="M9 18V5l12-2v13M9 9l12-2"/><circle cx="6" cy="18" r="3"/><circle cx="18" cy="16" r="3"/></svg>',
      sfx: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"><path d="M2 10v4m4-7v10m4-14v18m4-16v14m4-11v8m4-5v2"/></svg>',
      scripts: '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"><path d="m7 6-6 6 6 6m10-12 6 6-6 6M14 3l-4 18"/></svg>'
    };

    const $ = (selector, root = document) => root.querySelector(selector);

    const esc = value => String(value).replace(
      /[&<>"']/g,
      character => ({
        '&': '&amp;',
        '<': '&lt;',
        '>': '&gt;',
        '"': '&quot;',
        "'": '&#39;'
      }[character])
    );

    const arrow = (right = false) =>
      `<svg class="arrow" aria-hidden="true">
        <use href="#${right ? 'arrow-right' : 'arrow'}"/>
      </svg>`;

    const placeholder = title =>
      `<span class="fallback-art" aria-hidden="true">
        <svg class="placeholder-mark"><use href="#cube"/></svg>
        <strong>${esc(title)}</strong>
        <small>Preview unavailable</small>
      </span>`;

    const home = $('#home');
    const panel = $('#panel');

    let currentView = null;
    let pendingProject = null;
    let lastGalleryTrigger = null;

    $('#year').textContent = new Date().getFullYear();

    // Homepage projects
    $('#project-grid').innerHTML = BUILDS.map((project, index) => {
      const [src, alt] = project.imgs[project.featured];

      return `
        <a
          class="project-card"
          href="#builds"
          data-project="${project.slug}"
          aria-label="View ${esc(project.title)} gallery"
        >
          <div class="project-image">
            ${placeholder(project.title)}
            <img
              src="${src}"
              alt="${esc(alt)} — ${esc(project.title)}"
              loading="lazy"
              data-fallback
            >
            <span class="project-tag">${esc(project.tag || project.type)}</span>
            <span class="project-open">${arrow()}</span>
          </div>
          <div class="project-meta">
            <div>
              <h3>${esc(project.title)}</h3>
              <p>${esc(project.type)}</p>
            </div>
            <span class="project-num">0${index + 1}</span>
          </div>
        </a>
      `;
    }).join('');

    // Homepage services
    $('#skills').innerHTML = Object.entries(SKILLS).map(([key, skill], index) => `
      <a class="service" href="#${key}" style="--c:${skill.color}">
        <div class="service-top">
          <span class="service-icon" aria-hidden="true">${ICONS[key]}</span>
          <span class="service-index">0${index + 1}</span>
        </div>
        <h3>${esc(skill.name)}</h3>
        <p>${esc(skill.short)}</p>
        <span class="service-bottom">
          ${esc(skill.action)}
          ${arrow()}
        </span>
      </a>
    `).join('');

    // Decorative music waveform
    $('#waveform').innerHTML = Array.from({length: 55}, (_, index) => `
      <span style="
        --h:${14 + Math.abs(Math.sin(index * 1.73) * Math.cos(index * .31)) * 74}px;
        --d:${-(index % 13) * .15}s
      "></span>
    `).join('');

    function setupImageFallbacks(root = document) {
      root.querySelectorAll('img[data-fallback]').forEach(img => {
        img.addEventListener('error', () => {
          img.hidden = true;
        }, {once: true});

        if (img.complete && img.naturalWidth === 0) {
          img.hidden = true;
        }
      });
    }

    setupImageFallbacks();

    // Mobile navigation
    const menuButton = $('.menu-toggle');
    const navigation = $('#navigation');

    function closeMenu() {
      navigation.classList.remove('open');
      menuButton.setAttribute('aria-expanded', 'false');
      menuButton.setAttribute('aria-label', 'Open navigation');
    }

    menuButton.addEventListener('click', () => {
      const open = navigation.classList.toggle('open');
      menuButton.setAttribute('aria-expanded', String(open));
      menuButton.setAttribute(
        'aria-label',
        open ? 'Close navigation' : 'Open navigation'
      );

      if (open) {
        navigation.querySelector('a').focus();
      }
    });

    document.addEventListener('keydown', event => {
      if (event.key === 'Escape' && navigation.classList.contains('open')) {
        closeMenu();
        menuButton.focus();
      }
    });

    const desktopNav = matchMedia('(min-width: 601px)');

    desktopNav.addEventListener('change', () => {
      if (desktopNav.matches) closeMenu();
    });

    document.addEventListener('click', event => {
      const link = event.target.closest('a[href^="#"]');

      if (
        !link ||
        event.ctrlKey ||
        event.metaKey ||
        event.shiftKey ||
        event.altKey
      ) {
        return;
      }

      if (link.classList.contains('skip')) {
        event.preventDefault();
        closeMenu();

        const target = currentView === 'home'
          ? $('#hero-title')
          : $('#panel-title');

        target.focus({preventScroll: true});
        target.scrollIntoView({block: 'start', behavior: 'instant'});
        return;
      }

      closeMenu();

      if (link.dataset.project) {
        pendingProject = link.dataset.project;
      }

      if (link.hash === location.hash) {
        event.preventDefault();
        route(true);
      }
    });

    // Audio player
    // Direct relative URLs work with local files and hosting.
    const audio = new Audio();
    audio.preload = 'none';

    let currentTrack = -1;
    let audioRequest = 0;

    const playIcon = `
      <svg class="pl" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M7 4v16l14-8z"/>
      </svg>
      <svg class="pa" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M6 4h4v16H6zM14 4h4v16h-4z"/>
      </svg>
    `;

    const formatTime = seconds => Number.isFinite(seconds)
      ? `${Math.floor(seconds / 60)}:${String(Math.floor(seconds % 60)).padStart(2, '0')}`
      : '0:00';

    const trackRows = () => [...panel.querySelectorAll('.track')];

    function audioMessage(message = '') {
      const output = $('#audio-message');
      if (output) output.textContent = message;
    }

    function refreshPlayer() {
      trackRows().forEach((row, index) => {
        const selected = index === currentTrack;
        const playing = selected && !audio.paused && !audio.ended;

        row.classList.toggle('playing', playing);

        $('.pbtn', row).setAttribute(
          'aria-label',
          `${playing ? 'Pause' : 'Play'} ${MUSIC.tracks[index].title}`
        );

        $('.pbtn', row).setAttribute('aria-pressed', String(playing));

        const slider = $('.seek', row);
        const ready =
          selected &&
          Number.isFinite(audio.duration) &&
          audio.duration > 0;

        slider.disabled = !ready;
        slider.value = ready
          ? String(audio.currentTime / audio.duration * 100)
          : '0';

        slider.setAttribute(
          'aria-valuetext',
          ready
            ? `${formatTime(audio.currentTime)} of ${formatTime(audio.duration)}`
            : 'Not playing'
        );

        $('.time', row).textContent = selected
          ? `${formatTime(audio.currentTime)} / ${formatTime(audio.duration)}`
          : '0:00';
      });
    }

    async function toggleTrack(index) {
      const request = ++audioRequest;
      audioMessage();

      if (index === currentTrack && !audio.paused) {
        audio.pause();
        return;
      }

      if (index !== currentTrack) {
        audio.pause();
        currentTrack = index;
        audio.src = MUSIC.tracks[index].src;
      }

      if (audio.ended) {
        audio.currentTime = 0;
      }

      refreshPlayer();

      try {
        await audio.play();
        if (request === audioRequest) refreshPlayer();
      } catch (error) {
        if (
          request === audioRequest &&
          currentView === 'music' &&
          error.name !== 'AbortError'
        ) {
          audioMessage(
            'This track couldn’t be played. Please try again, or ask for a sample on Discord.'
          );
          refreshPlayer();
        }
      }
    }

    function stopAudio() {
      audioRequest++;
      audio.pause();
      audio.removeAttribute('src');
      audio.load();
      currentTrack = -1;
    }

    [
      'play',
      'pause',
      'loadedmetadata',
      'timeupdate',
      'durationchange'
    ].forEach(name => audio.addEventListener(name, refreshPlayer));

    audio.addEventListener('ended', () => {
      if (
        currentView === 'music' &&
        currentTrack < MUSIC.tracks.length - 1
      ) {
        toggleTrack(currentTrack + 1);
      } else {
        refreshPlayer();
      }
    });

    audio.addEventListener('error', () => {
      if (currentView === 'music' && currentTrack >= 0) {
        audioMessage(
          'This track is currently unavailable. You can request a sample on Discord.'
        );
        refreshPlayer();
      }
    });

    // Service page content
    function buildsHTML() {
      return BUILDS.map((project, groupIndex) => `
        <section
          class="project-group"
          id="project-${project.slug}"
          aria-labelledby="heading-${project.slug}"
        >
          <div class="group-head">
            <div class="group-title">
              <h2 id="heading-${project.slug}" tabindex="-1">
                ${esc(project.title)}
              </h2>
              ${project.tag
                ? `<span class="status">${esc(project.tag)}</span>`
                : ''}
            </div>
            <span class="group-count">
              ${String(project.imgs.length).padStart(2, '0')} IMAGES
            </span>
          </div>

          <div class="thumbs">
            ${project.imgs.map(([src, alt], imageIndex) => `
              <button
                class="thumb"
                data-gallery="${groupIndex}"
                data-image="${imageIndex}"
                aria-label="View ${esc(alt)} from ${esc(project.title)}"
              >
                <span class="thumb-image">
                  ${placeholder(alt)}
                  <img
                    src="${src}"
                    alt="${esc(alt)}"
                    loading="lazy"
                    data-fallback
                  >
                </span>
                <span class="thumb-caption">
                  ${esc(alt)}
                  ${arrow()}
                </span>
              </button>
            `).join('')}
          </div>
        </section>
      `).join('');
    }

    function musicHTML() {
      return `
        <div class="music-layout">
          <div class="album">
            <div class="album-cover">
              ${placeholder(MUSIC.title)}
              <img
                src="${MUSIC.cover}"
                alt="${esc(MUSIC.title)} album artwork"
                data-fallback
              >
            </div>
            <p class="album-note">
              Original music for Bloomville<br>
              Seasonal worlds. Different moods.
            </p>
          </div>

          <div class="player">
            <div class="player-title">
              <h2>${esc(MUSIC.title)}</h2>
              <span>04 original tracks</span>
            </div>

            ${MUSIC.tracks.map((track, index) => `
              <div class="track">
                <button
                  class="pbtn"
                  data-track="${index}"
                  aria-label="Play ${esc(track.title)}"
                  aria-pressed="false"
                >
                  ${playIcon}
                </button>

                <div class="track-info">
                  <strong>${esc(track.title)}</strong>
                  <small>${esc(track.type)}</small>
                  <input
                    class="seek"
                    type="range"
                    min="0"
                    max="100"
                    step="0.1"
                    value="0"
                    data-seek="${index}"
                    aria-label="Seek in ${esc(track.title)}"
                    aria-valuetext="Not playing"
                    disabled
                  >
                </div>

                <span class="time">0:00</span>
              </div>
            `).join('')}

            <p
              class="audio-message"
              id="audio-message"
              role="status"
              aria-live="polite"
            ></p>
          </div>
        </div>
      `;
    }

    function requestHTML(key) {
      const isSound = key === 'sfx';

      return `
        <div class="request-panel">
          <div class="request-copy">
            <h2>
              ${isSound
                ? 'Make every interaction<br>feel alive.'
                : 'Give your ideas<br>a little momentum.'}
            </h2>

            <p>
              ${isSound
                ? 'Looking for gameplay audio, environmental ambience or a distinctive UI sound? Tell me about your world and the feeling you want to create.'
                : 'Have a game system or a tool in mind? Share what it needs to do, how it fits into your project and the details that matter to you.'}
              Examples are available on request.
            </p>

            <a
              class="button primary"
              href="https://discord.gg/arvm99rawt"
              target="_blank"
              rel="noopener"
            >
              Ask for examples ${arrow()}
            </a>
          </div>

          <div class="request-art" aria-hidden="true">
            <span class="service-icon">${ICONS[key]}</span>
            <span class="mono">
              ${isSound
                ? 'THE DETAILS MAKE THE DIFFERENCE.'
                : 'FROM IDEA TO INTERACTION.'}
            </span>
          </div>
        </div>
      `;
    }

    function renderPanel(key) {
      const skill = SKILLS[key];
      const index = Object.keys(SKILLS).indexOf(key) + 1;

      panel.style.setProperty('--c', skill.color);

      panel.innerHTML = `
        <a class="back" href="#home">
          ${arrow(true)} Back to the studio
        </a>

        <div class="panel-heading">
          <div>
            <div class="section-label">
              <span>0${index} /</span> Rapture Studios
            </div>

            <h1 id="panel-title" tabindex="-1">
              ${esc(skill.name)}<span style="color:var(--c)">.</span>
            </h1>

            <p>${esc(skill.description)}</p>
          </div>

          <a
            class="quote"
            href="https://discord.gg/arvm99rawt"
            target="_blank"
            rel="noopener"
          >
            <small>
              ${skill.price ? 'Starting from' : 'Your project, your scope'}
            </small>
            <strong>
              ${skill.price ? esc(skill.price) : 'DM for a quote'}
              ${arrow()}
            </strong>
          </a>
        </div>

        <div class="styles">
          ${skill.styles.map(style => `<span>${esc(style)}</span>`).join('')}
        </div>

        ${key === 'builds'
          ? buildsHTML()
          : key === 'music'
            ? musicHTML()
            : requestHTML(key)}
      `;

      setupImageFallbacks(panel);
    }

    // Hash navigation
    function route(moveFocus = false) {
      const key = location.hash.slice(1);
      const isPanel = Object.hasOwn(SKILLS, key);
      const nextView = isPanel ? key : 'home';
      const changed = currentView !== nextView;

      if (changed) {
        stopAudio();
        if (lightbox.open) lightbox.close();
      }

      currentView = nextView;
      home.hidden = isPanel;
      panel.hidden = !isPanel;

      if (isPanel && changed) {
        renderPanel(key);
      }

      document.title = isPanel
        ? `${SKILLS[key].name} | Rapture Studios`
        : 'Rapture Studios | Worlds with feeling.';

      navigation.querySelectorAll('a').forEach(link => {
        if (link.hash === location.hash) {
          link.setAttribute('aria-current', 'page');
        } else {
          link.removeAttribute('aria-current');
        }
      });

      const target = isPanel
        ? (
          pendingProject && key === 'builds'
            ? document.getElementById('project-' + pendingProject)
            : $('#panel-title')
        )
        : (
          {
            work: $('#work'),
            services: $('#services'),
            contact: $('#contact'),
            main: $('#main')
          }[key] || $('#hero-title')
        );

      if (changed) {
        const visible = isPanel ? panel : home;
        visible.classList.remove('view-enter');
        void visible.offsetWidth;
        visible.classList.add('view-enter');
      }

      requestAnimationFrame(() => {
        if (target) {
          if (
            (isPanel && !pendingProject) ||
            (!isPanel && !['work', 'services', 'contact', 'main'].includes(key))
          ) {
            window.scrollTo({top: 0, behavior: 'instant'});
          } else {
            target.scrollIntoView({block: 'start', behavior: 'instant'});
          }

          if (moveFocus) {
            const heading = target.matches('h1,h2')
              ? target
              : target.querySelector('h1,h2') || target;

            const hadTabindex = heading.hasAttribute('tabindex');

            if (!hadTabindex) {
              heading.setAttribute('tabindex', '-1');
              heading.addEventListener('blur', () => {
                heading.removeAttribute('tabindex');
              }, {once: true});
            }

            heading.focus({preventScroll: true});
          }
        }

        pendingProject = null;
      });
    }

    panel.addEventListener('click', event => {
      const play = event.target.closest('[data-track]');

      if (play) {
        toggleTrack(Number(play.dataset.track));
        return;
      }

      const thumb = event.target.closest('[data-gallery]');

      if (thumb) {
        openGallery(
          Number(thumb.dataset.gallery),
          Number(thumb.dataset.image),
          thumb
        );
      }
    });

    panel.addEventListener('input', event => {
      const slider = event.target.closest('[data-seek]');

      if (
        slider &&
        Number(slider.dataset.seek) === currentTrack &&
        Number.isFinite(audio.duration)
      ) {
        audio.currentTime = Number(slider.value) / 100 * audio.duration;
        refreshPlayer();
      }
    });

    // Native image dialog
    const lightbox = $('#lightbox');
    const lightboxImage = $('#lightbox-image');

    let galleryIndex = 0;
    let imageIndex = 0;

    function updateGallery() {
      const project = BUILDS[galleryIndex];
      const [src, caption] = project.imgs[imageIndex];

      $('#lightbox-project').textContent = project.title;
      $('#lightbox-caption').textContent = caption;
      $('#lightbox-count').textContent =
        `${imageIndex + 1} / ${project.imgs.length}`;

      $('.lightbox-error').hidden = true;
      lightboxImage.hidden = false;
      lightboxImage.alt = caption;
      lightboxImage.src = src;

      $('#image-prev').disabled = imageIndex === 0;
      $('#image-next').disabled = imageIndex === project.imgs.length - 1;
    }

    function openGallery(group, index, trigger) {
      galleryIndex = group;
      imageIndex = index;
      lastGalleryTrigger = trigger;

      updateGallery();
      lightbox.showModal();
      document.body.classList.add('modal-open');
    }

    function stepGallery(direction) {
      const next = imageIndex + direction;

      if (next >= 0 && next < BUILDS[galleryIndex].imgs.length) {
        imageIndex = next;
        updateGallery();
      }
    }

    lightboxImage.addEventListener('error', () => {
      lightboxImage.hidden = true;
      $('.lightbox-error').hidden = false;
    });

    $('.close', lightbox).addEventListener('click', () => {
      lightbox.close();
    });

    $('#image-prev').addEventListener('click', () => stepGallery(-1));
    $('#image-next').addEventListener('click', () => stepGallery(1));

    lightbox.addEventListener('click', event => {
      if (event.target === lightbox) {
        const box = lightbox.getBoundingClientRect();

        if (
          event.clientX < box.left ||
          event.clientX > box.right ||
          event.clientY < box.top ||
          event.clientY > box.bottom
        ) {
          lightbox.close();
        }
      }
    });

    lightbox.addEventListener('close', () => {
      document.body.classList.remove('modal-open');

      if (lastGalleryTrigger?.isConnected) {
        lastGalleryTrigger.focus({preventScroll: true});
      }
    });

    lightbox.addEventListener('keydown', event => {
      if (event.key === 'ArrowRight') {
        event.preventDefault();
        stepGallery(1);
      }

      if (event.key === 'ArrowLeft') {
        event.preventDefault();
        stepGallery(-1);
      }
    });

    addEventListener('hashchange', () => route(true));
    addEventListener('pagehide', stopAudio);

    route();
  </script>
</body>
</html>