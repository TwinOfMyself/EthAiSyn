# Mercedez Lopez — Personal Brand Site

Personal website for Mercedez Lopez: writer, strategist, and Human-AI Integration Architect.

Built around Eth•ai•Syn, an original framework for humane intelligence in applied praxis — at the intersection of mental health, AI psychology, and organizational design.

## Live Site
[mercedezlopez.com](https://twinofmyself.github.io/mercedez-lopez)

## What's Here
Single-page site (index.html) with four sections:
- Writing — topic areas and selected work
- About — background and credentials  
- Eth•ai•Syn — framework, principles, and operating philosophy
- Connect — contact form and professional links

## Stack
HTML · CSS · Vanilla JS
No frameworks. No dependencies. One file.

## To Update
Open index.html, find the section you want to edit, update the text, re-upload.      --slate: #5B7A96;
      --teal:  #5A8F8F;
      --gold:  #A88B58;
      --white: #F2EFE9;
      --ease:  cubic-bezier(0.16,1,0.3,1);
    }
    *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
    html{scroll-behavior:smooth}
    body{font-family:'DM Sans',sans-serif;background:var(--cream);color:var(--ink);-webkit-font-smoothing:antialiased}
    a{color:inherit;text-decoration:none}

    /* WORDMARK */
    .wm{font-family:'Cormorant Garamond',serif;font-style:italic;font-weight:400;letter-spacing:.01em;color:var(--ink);display:inline-flex;align-items:center}
    .dot{display:inline-block;border-radius:50%;flex-shrink:0}
    .dt{background:var(--teal)}
    .dg{background:var(--gold)}
    .wm-nav{font-size:18px;gap:3px}
    .wm-nav .dot{width:7px;height:7px;margin:0 1px;position:relative;top:1px}
    .wm-hero{font-size:clamp(52px,10vw,88px);line-height:1}
    .wm-hero .dot{width:14px;height:14px;margin:0 2px;position:relative;top:2px}
    .wm-sm{font-size:28px;gap:3px}
    .wm-sm .dot{width:9px;height:9px;margin:0 1px;position:relative;top:1px}

    /* NAV */
    nav{position:fixed;top:0;left:0;right:0;z-index:100;padding:20px 28px;display:flex;align-items:center;justify-content:space-between;background:rgba(232,229,223,.92);backdrop-filter:blur(10px)}
    .nav-menu{display:flex;flex-direction:column;gap:5px;cursor:pointer;padding:4px}
    .nav-menu span{display:block;width:22px;height:1.5px;background:var(--muted);border-radius:2px}
    .nav-drawer{position:fixed;top:0;right:-100%;width:min(300px,80vw);height:100vh;background:var(--white);z-index:200;padding:60px 36px;display:flex;flex-direction:column;gap:32px;transition:right .4s var(--ease);border-left:1px solid var(--border)}
    .nav-drawer.open{right:0}
    .nav-drawer a{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:300;font-style:italic;color:var(--ink);border-bottom:1px solid var(--border);padding-bottom:16px;transition:color .2s}
    .nav-drawer a:hover{color:var(--teal)}
    .nav-close{position:absolute;top:20px;right:24px;font-size:24px;color:var(--muted);cursor:pointer;background:none;border:none;font-family:'DM Sans',sans-serif}
    .nav-overlay{display:none;position:fixed;inset:0;background:rgba(42,40,37,.3);z-index:150}
    .nav-overlay.open{display:block}

    /* HERO */
    #hero{min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding:100px 32px 120px;position:relative}
    .hero-wm-wrap{opacity:0;animation:up 1s var(--ease) .2s forwards;margin-bottom:20px}
    .hero-rule{width:48px;height:1px;background:var(--border);margin:0 auto 22px;opacity:0;animation:up .8s var(--ease) .5s forwards}
    .hero-name{font-size:11px;font-weight:500;letter-spacing:.28em;text-transform:uppercase;color:var(--muted);margin-bottom:16px;opacity:0;animation:up .8s var(--ease) .65s forwards}
    .hero-tagline{font-family:'Cormorant Garamond',serif;font-size:clamp(18px,3vw,24px);font-weight:300;font-style:italic;color:var(--muted);line-height:1.55;max-width:560px;margin:0 auto 44px;opacity:0;animation:up .8s var(--ease) .8s forwards}
    .hero-btns{display:flex;flex-direction:column;align-items:center;gap:12px;opacity:0;animation:up .8s var(--ease) 1s forwards}
    .btn-filled{display:inline-flex;align-items:center;justify-content:center;min-width:220px;background:var(--slate);color:var(--white);font-family:'DM Sans',sans-serif;font-size:11px;font-weight:500;letter-spacing:.2em;text-transform:uppercase;padding:16px 32px;border-radius:2px;transition:background .2s,transform .15s}
    .btn-filled:hover{background:var(--teal);transform:translateY(-1px)}
    .btn-outline{display:inline-flex;align-items:center;justify-content:center;min-width:220px;background:transparent;color:var(--ink);font-family:'DM Sans',sans-serif;font-size:11px;font-weight:500;letter-spacing:.2em;text-transform:uppercase;padding:15px 32px;border-radius:2px;border:1px solid var(--border);transition:border-color .2s,color .2s,transform .15s}
    .btn-outline:hover{border-color:var(--ink);transform:translateY(-1px)}
    .hero-scroll{position:absolute;bottom:36px;left:50%;transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;gap:10px;opacity:0;animation:up .8s var(--ease) 1.4s forwards;cursor:pointer}
    .hero-scroll span{font-size:9px;font-weight:500;letter-spacing:.28em;text-transform:uppercase;color:var(--muted)}
    .scroll-line{width:1px;height:48px;background:var(--border);position:relative;overflow:hidden}
    .scroll-line::after{content:'';position:absolute;top:-100%;left:0;width:100%;height:50%;background:linear-gradient(to bottom,transparent,var(--gold),transparent);animation:drip 2.4s ease-in-out 2s infinite}
    @keyframes drip{0%{top:-80%;opacity:0}15%{opacity:1}100%{top:180%;opacity:0}}
    @keyframes up{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}

    /* SPINE + PANELS */
    #content{max-width:840px;margin:0 auto;padding:0 40px 120px;position:relative}
    .spine{position:absolute;left:calc(40px + 44px);top:0;bottom:60px;width:1px;background:var(--border);pointer-events:none}
    .spine-fill{position:absolute;top:0;left:0;width:100%;height:0%;background:linear-gradient(to bottom,var(--slate),var(--teal),var(--gold));transition:height .08s linear}
    .panel{position:relative;padding-left:calc(44px + 28px)}
    .spine-dot{position:absolute;left:calc(44px - 5px);top:38px;width:11px;height:11px;border-radius:50%;background:var(--cream);border:1.5px solid var(--border);z-index:2;transition:background .35s,border-color .35s,transform .35s var(--ease)}
    .spine-dot.lit{border-color:var(--teal)}
    .panel.open .spine-dot{background:var(--gold);border-color:var(--gold);transform:scale(1.35)}
    .panel-trigger{width:100%;background:none;border:none;border-top:1px solid var(--border);cursor:pointer;padding:32px 0;display:grid;grid-template-columns:1fr auto;align-items:start;gap:24px;text-align:left;color:var(--ink);transition:opacity .2s}
    .panel-trigger:hover{opacity:.6}
    .panel:last-child .panel-trigger{border-bottom:1px solid var(--border)}
    .panel.open:last-child .panel-trigger{border-bottom:none}
    .panel-label{font-size:10px;font-weight:500;letter-spacing:.22em;text-transform:uppercase;color:var(--muted);margin-bottom:10px}
    .panel-title{font-family:'Cormorant Garamond',serif;font-size:clamp(24px,3.5vw,34px);font-weight:300;line-height:1.2}
    .panel-title em{font-style:italic;color:var(--slate)}
    .panel-teaser{font-size:13px;font-weight:300;color:var(--muted);margin-top:9px;line-height:1.65;max-width:460px}
    .panel-icon{width:34px;height:34px;border-radius:50%;border:1px solid var(--border);flex-shrink:0;margin-top:4px;position:relative;transition:background .3s,border-color .3s}
    .panel-icon::before,.panel-icon::after{content:'';position:absolute;top:50%;left:50%;background:var(--muted);border-radius:2px;transition:transform .35s var(--ease),opacity .25s}
    .panel-icon::before{width:11px;height:1.5px;transform:translate(-50%,-50%)}
    .panel-icon::after{width:1.5px;height:11px;transform:translate(-50%,-50%)}
    .panel.open .panel-icon{background:var(--ink);border-color:var(--ink)}
    .panel.open .panel-icon::before,.panel.open .panel-icon::after{background:var(--cream)}
    .panel.open .panel-icon::after{transform:translate(-50%,-50%) rotate(90deg);opacity:0}
    .panel-body{display:grid;grid-template-rows:0fr;transition:grid-template-rows .55s var(--ease)}
    .panel.open .panel-body{grid-template-rows:1fr}
    .panel-body-inner{overflow:hidden}
    .panel-body-content{padding:32px 0 44px;border-top:1px solid var(--border)}
    .panel.open:last-child .panel-body-content{border-bottom:1px solid var(--border)}

    /* WRITING */
    .topics{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:var(--border);border:1px solid var(--border);border-radius:3px;overflow:hidden;margin-bottom:28px}
    .topic{background:var(--cream);padding:22px 18px;transition:background .2s}
    .topic:hover{background:var(--white)}
    .topic-num{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:300;color:var(--border);margin-bottom:8px}
    .topic-name{font-family:'Cormorant Garamond',serif;font-size:17px;font-weight:500;color:var(--ink);margin-bottom:6px}
    .topic-desc{font-size:12px;font-weight:300;color:var(--muted);line-height:1.65}
    .clips-label{font-size:10px;font-weight:500;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);margin:28px 0 12px}
    .clips{display:flex;flex-direction:column;gap:1px;background:var(--border);border:1px solid var(--border);border-radius:3px;overflow:hidden;margin-bottom:28px}
    .clip{display:flex;flex-direction:column;gap:4px;background:var(--cream);padding:16px 20px;transition:background .2s}
    .clip:hover{background:var(--white)}
    .clip-meta{font-size:10px;font-weight:500;letter-spacing:.16em;text-transform:uppercase;color:var(--teal)}
    .clip-title{font-family:'Cormorant Garamond',serif;font-size:17px;font-weight:400;color:var(--ink);line-height:1.3}
    .clip-pub{font-size:11px;font-weight:300;color:var(--muted)}
    .panel-cta{display:inline-flex;align-items:center;gap:7px;font-size:12px;font-weight:500;letter-spacing:.08em;border-bottom:1px solid var(--ink);padding-bottom:2px;transition:color .2s,border-color .2s}
    .panel-cta:hover{color:var(--teal);border-color:var(--teal)}

    /* ABOUT */
    .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px}
    .about-copy{font-size:14px;font-weight:300;line-height:1.9}
    .about-copy p{margin-bottom:16px}
    .about-copy strong{font-weight:500}
    .cred{padding:13px 0;border-bottom:1px solid var(--border)}
    .cred:first-child{border-top:1px solid var(--border)}
    .cred-title{font-size:13px;font-weight:500;display:flex;align-items:center;gap:8px;margin-bottom:3px}
    .cred-dot{width:6px;height:6px;border-radius:50%;flex-shrink:0}
    .cred-desc{font-size:12px;font-weight:300;color:var(--muted);line-height:1.55;padding-left:14px}

    /* EAS */
    .eas-grid{display:grid;grid-template-columns:auto 1fr;gap:48px;align-items:start}
    .eas-left{display:flex;flex-direction:column;gap:14px;min-width:160px}
    .eas-bars{display:flex;flex-direction:column;align-items:flex-start;gap:8px}
    .eas-bars span{display:block;border-radius:10px;height:5px}
    .eas-bars .b1{width:100px;background:var(--slate)}
    .eas-bars .b2{width:76px;background:var(--teal)}
    .eas-bars .b3{width:48px;background:var(--gold)}
    .eas-praxis{font-family:'DM Sans',sans-serif;font-size:10px;font-weight:400;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);line-height:1.7}
    .eas-praxis em{font-style:italic;font-family:'Cormorant Garamond',serif;font-size:13px;letter-spacing:.08em;text-transform:none;color:var(--teal)}
    .eas-quote{font-family:'Cormorant Garamond',serif;font-size:15px;font-weight:300;font-style:italic;line-height:1.75;padding:16px 0 16px 18px;border-left:2px solid var(--teal);margin-top:4px}
    .eas-quote cite{display:block;margin-top:10px;font-style:normal;font-size:9px;letter-spacing:.2em;text-transform:uppercase;color:var(--teal)}
    .eas-intro{font-size:13px;font-weight:300;color:var(--muted);line-height:1.8;margin-bottom:24px;padding-bottom:24px;border-bottom:1px solid var(--border)}
    .pillars{display:flex;flex-direction:column;gap:18px}
    .pillar-row{display:flex;gap:12px;align-items:flex-start}
    .pillar-badge{width:26px;height:26px;border-radius:3px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:600;flex-shrink:0}
    .pillar-badge.s{background:rgba(91,122,150,.12);color:var(--slate)}
    .pillar-badge.t{background:rgba(90,144,144,.12);color:var(--teal)}
    .pillar-badge.g{background:rgba(184,150,96,.12);color:var(--gold)}
    .pillar-text h4{font-size:13px;font-weight:500;margin-bottom:3px}
    .pillar-text p{font-size:12px;font-weight:300;color:var(--muted);line-height:1.6}

    /* CONNECT */
    .connect-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px}
    .connect-intro{font-size:14px;font-weight:300;color:var(--muted);line-height:1.85;margin-bottom:24px}
    .connect-links{display:flex;flex-direction:column;gap:10px}
    .connect-link{display:flex;align-items:center;gap:12px;padding:13px 14px;background:var(--fog);border:1px solid var(--border);border-radius:3px;transition:background .2s,border-color .2s}
    .connect-link:hover{background:var(--white);border-color:var(--muted)}
    .connect-icon{width:30px;height:30px;border-radius:3px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
    .connect-icon.li{background:rgba(91,122,150,.14)}
    .connect-icon.em{background:rgba(90,144,144,.14)}
    .connect-link strong{display:block;font-size:13px;font-weight:500}
    .connect-link span{font-size:11px;color:var(--muted)}
    .form-stack{display:flex;flex-direction:column;gap:12px}
    .form-stack label{display:flex;flex-direction:column;gap:5px;font-size:10px;font-weight:500;letter-spacing:.18em;text-transform:uppercase;color:var(--muted)}
    .form-stack input,.form-stack select,.form-stack textarea{background:var(--fog);border:1px solid var(--border);border-radius:2px;padding:10px 13px;color:var(--ink);font-family:'DM Sans',sans-serif;font-size:13px;font-weight:300;outline:none;transition:border-color .2s;width:100%}
    .form-stack input:focus,.form-stack textarea:focus{border-color:var(--teal)}
    .form-stack select option{background:var(--cream)}
    .form-stack textarea{resize:vertical;min-height:88px}
    .btn-send{background:var(--ink);color:var(--cream);border:none;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:11px;font-weight:500;letter-spacing:.14em;text-transform:uppercase;padding:13px 28px;border-radius:2px;align-self:flex-start;transition:background .2s,transform .15s}
    .btn-send:hover{background:var(--teal);transform:translateY(-1px)}

    footer{max-width:840px;margin:0 auto;padding:28px 40px;border-top:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px}
    .footer-wm{font-family:'Cormorant Garamond',serif;font-style:italic;font-weight:300;font-size:15px;color:var(--muted);display:inline-flex;align-items:center}
    .footer-wm .dot{width:6px;height:6px}
    .footer-note{font-size:10px;letter-spacing:.12em;color:var(--border)}

    @media(max-width:600px){
      #content{padding:0 20px 80px}
      .panel{padding-left:calc(44px + 16px)}
      .spine{left:calc(20px + 44px)}
      .topics,.about-grid,.eas-grid,.connect-grid{grid-template-columns:1fr;gap:24px}
      .hero-btns{width:100%;padding:0 20px}
      .btn-filled,.btn-outline{width:100%}
    }
  </style>
</head>
<body>

<nav>
  <a href="#hero" class="wm wm-nav">Eth<span class="dot dt"></span>ai<span class="dot dg"></span>Syn</a>
  <div class="nav-menu" onclick="openNav()"><span></span><span></span></div>
</nav>

<div class="nav-overlay" id="navOverlay" onclick="closeNav()"></div>
<div class="nav-drawer" id="navDrawer">
  <button class="nav-close" onclick="closeNav()">x</button>
  <a href="#p-writing"  onclick="closeNav();setTimeout(()=>toggle('p-writing'),300)">Writing</a>
  <a href="#p-about"    onclick="closeNav();setTimeout(()=>toggle('p-about'),300)">About</a>
  <a href="#p-ethaisyn" onclick="closeNav();setTimeout(()=>toggle('p-ethaisyn'),300)">Eth-ai-Syn</a>
  <a href="#p-connect"  onclick="closeNav();setTimeout(()=>toggle('p-connect'),300)">Connect</a>
</div>

<section id="hero">
  <div class="hero-wm-wrap"><span class="wm wm-hero">Eth<span class="dot dt"></span>ai<span class="dot dg"></span>Syn</span></div>
  <div class="hero-rule"></div>
  <p class="hero-name">Mercedez Lopez</p>
  <p class="hero-tagline">Writer. Researcher. Framework-builder at the intersection<br>of mental health, AI, and human dignity.</p>
  <div class="hero-btns">
    <a href="#p-writing" class="btn-filled" onclick="setTimeout(()=>toggle('p-writing'),200)">Read My Work</a>
    <a href="#p-connect" class="btn-outline" onclick="setTimeout(()=>toggle('p-connect'),200)">Get In Touch</a>
  </div>
  <div class="hero-scroll" onclick="document.getElementById('content').scrollIntoView({behavior:'smooth'})">
    <span>Scroll</span>
    <div class="scroll-line"></div>
  </div>
</section>

<div id="content">
  <div class="spine"><div class="spine-fill" id="spineFill"></div></div>

  <div class="panel" id="p-writing">
    <div class="spine-dot" id="dot-writing"></div>
    <button class="panel-trigger" onclick="toggle('p-writing')" aria-expanded="false">
      <div>
        <div class="panel-label">01 - Writing</div>
        <div class="panel-title">Words that <em>hold</em> their weight.</div>
        <div class="panel-teaser">Mental health, AI psychology, workplace wellbeing - written with clinical grounding and genuine care. Applied knowledge, not observation from a distance.</div>
      </div>
      <div class="panel-icon"></div>
    </button>
    <div class="panel-body"><div class="panel-body-inner"><div class="panel-body-content">
      <div class="topics">
        <div class="topic"><div class="topic-num">01</div><div class="topic-name">Mental Health</div><p class="topic-desc">Trauma-informed, clinically grounded, genuinely readable. For healthcare, advocacy, and wellness brands that want content with integrity.</p></div>
        <div class="topic"><div class="topic-num">02</div><div class="topic-name">AI Psychology</div><p class="topic-desc">The human side of machine systems - cognitive debt, moral development, and what it means to stay whole inside technology that thinks.</p></div>
        <div class="topic"><div class="topic-num">03</div><div class="topic-name">Workplace Wellbeing</div><p class="topic-desc">Psychological safety as infrastructure. Burnout, leadership, and the conditions humans need to do their best work.</p></div>
      </div>
      <div class="clips-label">Selected work</div>
      <div class="clips">
        <a href="#" class="clip"><div class="clip-meta">Mental Health - Essay</div><div class="clip-title">Add your first writing sample title here</div><div class="clip-pub">Publication or platform name</div></a>
        <a href="#" class="clip"><div class="clip-meta">AI Psychology - Article</div><div class="clip-title">Add your second writing sample title here</div><div class="clip-pub">Publication or platform name</div></a>
        <a href="#" class="clip"><div class="clip-meta">Workplace Wellbeing - LinkedIn</div><div class="clip-title">Add your third writing sample title here</div><div class="clip-pub">LinkedIn - your strongest post</div></a>
      </div>
      <a href="#p-connect" class="panel-cta" onclick="setTimeout(()=>toggle('p-connect'),120)">Hire me to write</a>
    </div></div></div>
  </div>

  <div class="panel" id="p-about">
    <div class="spine-dot" id="dot-about"></div>
    <button class="panel-trigger" onclick="toggle('p-about')" aria-expanded="false">
      <div>
        <div class="panel-label">02 - About</div>
        <div class="panel-title">Systems thinker.<br><em>Human first.</em></div>
        <div class="panel-teaser">A background spanning clinical psychology, healthcare operations, and organizational design - each field studied, then operationalized. Pattern recognition across disciplines is the methodology.</div>
      </div>
      <div class="panel-icon"></div>
    </button>
    <div class="panel-body"><div class="panel-body-inner"><div class="panel-body-content">
      <div class="about-grid">
        <div class="about-copy">
          <p>I grew up in a Navy IT household where <strong>systems were the native language.</strong> What I learned early - and have spent a career proving - is that every system, no matter how technical, is ultimately a human one.</p>
          <p>My background spans clinical psychology, healthcare administration, HR and organizational development, and revenue cycle operations. I have built training programs, led teams, designed workflows, and spent years watching what happens when the humans inside systems are not designed for.</p>
          <p>The through-line across every role is applied practice - not observation, not theory-building in isolation, but direct intervention inside systems while documenting what breaks and why. In clinical and organizational literature, this is defined as <strong>praxis</strong>: the iterative cycle of evidence, action, and reflection that produces knowledge you cannot generate any other way.</p>
        </div>
        <div>
          <div class="cred"><div class="cred-title"><span class="cred-dot" style="background:var(--slate)"></span>BA Clinical Psychology</div><div class="cred-desc">Mental Health concentration - the foundation for everything that followed.</div></div>
          <div class="cred"><div class="cred-title"><span class="cred-dot" style="background:var(--teal)"></span>Healthcare Operations</div><div class="cred-desc">Benefits verification, prior authorization, revenue cycle - the systems that touch patients most.</div></div>
          <div class="cred" style="border-bottom:none"><div class="cred-title"><span class="cred-dot" style="background:var(--gold)"></span>HR / Organizational Development</div><div class="cred-desc">People analytics, workforce strategy, designing orgs where humans actually thrive.</div></div>
        </div>
      </div>
    </div></div></div>
  </div>

  <div class="panel" id="p-ethaisyn">
    <div class="spine-dot" id="dot-ethaisyn"></div>
    <button class="panel-trigger" onclick="toggle('p-ethaisyn')" aria-expanded="false">
      <div>
        <div class="panel-label">03 - Eth-ai-Syn</div>
        <div class="panel-title">A framework for<br><em>humane intelligence in praxis.</em></div>
        <div class="panel-teaser">Research consistently shows that AI systems alter human cognition, judgment, and moral reasoning - whether or not they are designed to. Eth-ai-Syn is a framework for designing them with that data in view.</div>
      </div>
      <div class="panel-icon"></div>
    </button>
    <div class="panel-body"><div class="panel-body-inner"><div class="panel-body-content">
      <div class="eas-grid">
        <div class="eas-left">
          <div class="eas-bars"><span class="b1"></span><span class="b2"></span><span class="b3"></span></div>
          <span class="wm wm-sm">Eth<span class="dot dt"></span>ai<span class="dot dg"></span>Syn</span>
          <div class="eas-praxis">Ethics - AI - Synthesis<br><em>applied praxis</em></div>
          <div class="eas-quote">Clarity is an act of care. Structure is never neutral - it either holds the people inside it, or it does not.<cite>Eth-ai-Syn, core operating principle</cite></div>
        </div>
        <div>
          <p class="eas-intro">In clinical and organizational development literature, praxis is defined as the evidence-action-reflection cycle - the only methodology that produces knowledge you cannot derive from theory alone. Eth-ai-Syn applies that cycle specifically to human-AI integration: observe the behavioral and cognitive effects of AI systems on the humans using them, act on that data in design, reflect on outcomes, repeat. Each principle below is an operational protocol, not a position statement.</p>
          <div class="pillars">
            <div class="pillar-row"><div class="pillar-badge s">E</div><div class="pillar-text"><h4>Ethics-First Design</h4><p>Evaluate AI not just for what it produces, but for what it does to the person using it - to their cognition, their agency, their moral development. Then design accordingly.</p></div></div>
            <div class="pillar-row"><div class="pillar-badge t">A</div><div class="pillar-text"><h4>AI as Augmentation</h4><p>Augmentation is a practice, not a promise. It requires actively protecting human judgment, resisting dependency, and building toward amplification - not replacement.</p></div></div>
            <div class="pillar-row"><div class="pillar-badge g">S</div><div class="pillar-text"><h4>Synthesis Over Speed</h4><p>Cognitive load research demonstrates that systems optimized for speed at the expense of comprehension degrade reasoning over time. Systems designed for synthesis produce measurably more capable human collaborators.</p></div></div>
          </div>
        </div>
      </div>
    </div></div></div>
  </div>

  <div class="panel" id="p-connect">
    <div class="spine-dot" id="dot-connect"></div>
    <button class="panel-trigger" onclick="toggle('p-connect')" aria-expanded="false">
      <div>
        <div class="panel-label">04 - Connect</div>
        <div class="panel-title">Let's build something<br><em>worth preserving.</em></div>
        <div class="panel-teaser">Whether you need a writer, a strategic mind, or a professional connection - I would like to hear from you.</div>
      </div>
      <div class="panel-icon"></div>
    </button>
    <div class="panel-body"><div class="panel-body-inner"><div class="panel-body-content">
      <div class="connect-grid">
        <div>
          <p class="connect-intro">I write for brands, publications, and people who believe how we treat humans inside our systems is never a footnote. Open to professional connections and job leads.</p>
          <div class="connect-links">
            <a href="https://linkedin.com" target="_blank" class="connect-link">
              <div class="connect-icon li"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="var(--slate)" stroke-width="2"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></div>
              <div><strong>LinkedIn</strong><span>Connect professionally</span></div>
            </a>
            <a href="mailto:hello@mercedezlopez.com" class="connect-link">
              <div class="connect-icon em"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="var(--teal)" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg></div>
              <div><strong>Email</strong><span>hello@mercedezlopez.com</span></div>
            </a>
          </div>
        </div>
        <div class="form-stack">
          <label>Your Name<input type="text" placeholder="First and last"/></label>
          <label>Email<input type="email" placeholder="you@company.com"/></label>
          <label>Reaching out about
            <select><option value="" disabled selected>Select one</option><option>Hiring you as a writer</option><option>Professional connection / job lead</option><option>Eth-ai-Syn / speaking / collaboration</option><option>Something else</option></select>
          </label>
          <label>Message<textarea placeholder="Tell me what you are working on"></textarea></label>
          <button class="btn-send" type="button">Send</button>
        </div>
      </div>
    </div></div></div>
  </div>

</div>

<footer>
  <span class="footer-wm">Eth<span class="dot dt" style="width:6px;height:6px;margin:0 2px"></span>ai<span class="dot dg" style="width:6px;height:6px;margin:0 2px"></span>Syn</span>
  <span class="footer-note">Healthcare - People Strategy - Ethical AI</span>
</footer>

<script>
  function openNav(){document.getElementById('navDrawer').classList.add('open');document.getElementById('navOverlay').classList.add('open')}
  function closeNav(){document.getElementById('navDrawer').classList.remove('open');document.getElementById('navOverlay').classList.remove('open')}
  function toggle(id){
    const panel=document.getElementById(id);
    const isOpen=panel.classList.contains('open');
    document.querySelectorAll('.panel').forEach(p=>{p.classList.remove('open');p.querySelector('.panel-trigger').setAttribute('aria-expanded','false')});
    if(!isOpen){panel.classList.add('open');panel.querySelector('.panel-trigger').setAttribute('aria-expanded','true');setTimeout(()=>panel.scrollIntoView({behavior:'smooth',block:'start'}),60)}
  }
  const spineFill=document.getElementById('spineFill');
  const spine=document.querySelector('.spine');
  const dots=[
    {el:document.getElementById('dot-writing'),panel:document.getElementById('p-writing')},
    {el:document.getElementById('dot-about'),panel:document.getElementById('p-about')},
    {el:document.getElementById('dot-ethaisyn'),panel:document.getElementById('p-ethaisyn')},
    {el:document.getElementById('dot-connect'),panel:document.getElementById('p-connect')},
  ];
  function updateSpine(){
    const spineTop=spine.getBoundingClientRect().top+window.scrollY;
    const spineH=spine.offsetHeight;
    const pct=Math.min(Math.max((window.scrollY+window.innerHeight*.65-spineTop)/spineH,0),1);
    spineFill.style.height=(pct*100)+'%';
    const fillBottom=spineTop+spineH*pct;
    dots.forEach(({el,panel})=>{
      const dotTop=el.getBoundingClientRect().top+window.scrollY;
      if(!panel.classList.contains('open'))el.classList.toggle('lit',dotTop<=fillBottom+6);
    });
  }
  window.addEventListener('scroll',updateSpine,{passive:true});
  updateSpine();
</script>

</body>
</html>
