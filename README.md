<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>James — Portfolio</title>
<style>
  :root{
    --ink:#0f1822;
    --bg:#0b1016;
    --panel:#121b26;
    --paper:#f4f6f8;
    --accent:#4ea3ff;
    --accent-deep:#1e6fd0;
    --muted:#8a99ab;
    --muted-dark:#5d6b7d;
    --line:#1e2a38;
    --line-light:#e0e4ea;
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html{scroll-behavior:smooth;}
  body{
    font-family:'Inter','Helvetica Neue',Arial,sans-serif;
    color:var(--ink);
    background:var(--paper);
    line-height:1.65;
    -webkit-font-smoothing:antialiased;
  }
  .wrap{max-width:760px;margin:0 auto;padding:0 26px;}
  .display{font-family:'Georgia',serif;}

  /* ---------- HERO ---------- */
  .hero{
    background:radial-gradient(1200px 600px at 70% -10%, #16314e 0%, var(--bg) 55%);
    color:var(--paper);
    padding:120px 0 96px;
    position:relative;
    overflow:hidden;
  }
  .hero::after{
    content:"";
    position:absolute;inset:0;
    background:linear-gradient(transparent 60%, rgba(78,163,255,.05));
    pointer-events:none;
  }
  .hero .eyebrow{
    letter-spacing:.22em;text-transform:uppercase;
    font-size:.7rem;font-weight:700;color:var(--accent);
    margin-bottom:26px;
  }
  .hero h1{
    font-family:'Georgia',serif;
    font-size:clamp(2.6rem,7.5vw,4.4rem);
    line-height:1.04;font-weight:700;letter-spacing:-.02em;
    margin-bottom:24px;
  }
  .hero h1 .glow{color:var(--accent);}
  .lede{
    font-size:clamp(1.15rem,2.8vw,1.5rem);
    color:#c4d2e2;max-width:580px;font-weight:300;
  }
  .scroll-cue{
    margin-top:54px;font-size:.78rem;letter-spacing:.14em;
    text-transform:uppercase;color:var(--muted);font-weight:600;
  }

  /* ---------- NARRATIVE BLOCKS ---------- */
  section{padding:84px 0;}
  .chapter{
    letter-spacing:.18em;text-transform:uppercase;
    font-size:.72rem;font-weight:700;color:var(--accent-deep);
    margin-bottom:22px;display:flex;align-items:center;gap:12px;
  }
  .chapter::before{
    content:"";width:30px;height:2px;background:var(--accent-deep);display:inline-block;
  }
  h2{
    font-family:'Georgia',serif;
    font-size:clamp(1.7rem,4vw,2.4rem);
    line-height:1.15;font-weight:700;letter-spacing:-.01em;
    margin-bottom:20px;max-width:600px;
  }
  .prose p{font-size:1.12rem;color:#33414f;margin-bottom:18px;max-width:620px;}
  .prose p.note{color:var(--muted-dark);font-style:italic;font-size:.98rem;}

  .pull{
    border-left:3px solid var(--accent);
    padding:6px 0 6px 24px;margin:34px 0;
    font-family:'Georgia',serif;font-size:1.45rem;line-height:1.4;
    color:var(--ink);max-width:600px;
  }

  /* ---------- TIMELINE ---------- */
  .alt{background:var(--ink);color:var(--paper);}
  .alt .chapter{color:var(--accent);}
  .alt .chapter::before{background:var(--accent);}
  .alt h2{color:#fff;}
  .timeline{margin-top:36px;border-left:2px solid var(--line);}
  .moment{position:relative;padding:0 0 38px 30px;}
  .moment:last-child{padding-bottom:0;}
  .moment::before{
    content:"";position:absolute;left:-7px;top:6px;
    width:12px;height:12px;border-radius:50%;
    background:var(--accent);box-shadow:0 0 0 4px var(--ink);
  }
  .moment .when{
    font-size:.74rem;letter-spacing:.1em;text-transform:uppercase;
    color:var(--accent);font-weight:700;margin-bottom:6px;
  }
  .moment h3{font-family:'Georgia',serif;font-size:1.3rem;margin-bottom:6px;}
  .moment p{color:#aebccd;font-size:1.02rem;max-width:560px;}

  /* ---------- CLOSING ---------- */
  .close{text-align:center;padding:96px 0;}
  .close h2{margin:0 auto 18px;}
  .close p{margin:0 auto 30px;color:#33414f;font-size:1.12rem;max-width:520px;}
  .links{display:flex;flex-wrap:wrap;gap:13px;justify-content:center;}
  .links a{
    font-size:.92rem;font-weight:600;text-decoration:none;color:var(--ink);
    border:1px solid var(--line-light);padding:12px 22px;border-radius:999px;
    transition:.16s ease;
  }
  .links a:hover{background:var(--ink);color:#fff;border-color:var(--ink);}

  footer{padding:34px 0;text-align:center;color:var(--muted-dark);font-size:.82rem;}

  @media (max-width:560px){
    .hero{padding:88px 0 68px;}
    section{padding:60px 0;}
    .close{padding:70px 0;}
  }
</style>
</head>
<body>

<!-- ===== HERO ===== -->
<header class="hero">
  <div class="wrap">
    <div class="eyebrow">Engineering · Applicant Portfolio</div>
    <h1>I build things to<br>understand <span class="glow">how they work.</span></h1>
    <p class="lede">My name is James. This page is the story of how a kid who took apart the family toaster became someone who wants to engineer what comes next.</p>
    <div class="scroll-cue">Scroll to read ↓</div>
  </div>
</header>

<!-- ===== WHERE IT STARTED ===== -->
<section class="prose">
  <div class="wrap">
    <div class="chapter">Where it started</div>
    <h2>The first thing I ever fixed, I had broken myself.</h2>
    <p>[Open with a real, specific moment. The lamp you rewired, the code that finally compiled at 2am, the bike you rebuilt from parts. One concrete scene that shows the spark — not "I've always loved engineering."]</p>
    <p>[Then connect it: what did that moment teach you about how you think? Admissions readers remember images, not adjectives.]</p>
    <p class="note">↑ Replace this whole block with your own origin story.</p>

    <div class="pull">"[A single line that captures your mindset. Make it sound like you.]"</div>
  </div>
</section>

<!-- ===== THE WORK (timeline) ===== -->
<section class="alt">
  <div class="wrap">
    <div class="chapter">The work</div>
    <h2>A few moments I'm proud of.</h2>
    <div class="timeline">

      <div class="moment">
        <div class="when">2025 · Grade 11</div>
        <h3>[Robotics / project name]</h3>
        <p>[What you built or led, and the result. Numbers help: hours, teammates, ranking, what it actually did.]</p>
      </div>

      <div class="moment">
        <div class="when">2024 · Grade 10</div>
        <h3>[Award or competition]</h3>
        <p>[Don't just name it — say what was hard about it and what you learned getting there.]</p>
      </div>

      <div class="moment">
        <div class="when">2024 · Grade 10</div>
        <h3>[Leadership / club / initiative]</h3>
        <p>[Show impact on other people, not just yourself. Who did your work help?]</p>
      </div>

      <div class="moment">
        <div class="when">2023 · Grade 9</div>
        <h3>[Where it began at school]</h3>
        <p>[The early thing that set the rest in motion.]</p>
      </div>

    </div>
  </div>
</section>

<!-- ===== WHAT'S NEXT ===== -->
<section class="prose">
  <div class="wrap">
    <div class="chapter">What's next</div>
    <h2>Why I'm applying.</h2>
    <p>[The forward-looking part. What problem do you actually want to work on — clean energy, accessible hardware, AI safety, something local to you? Be specific enough that it could only be your answer.]</p>
    <p>[Tie it back to the origin story. The toaster kid grew up and now wants to ___. That loop is what makes a page feel whole.]</p>
  </div>
</section>

<!-- ===== CLOSING ===== -->
<section class="close">
  <div class="wrap">
    <h2 class="display">Let's talk.</h2>
    <p>I'd love to tell you the rest in person.</p>
    <div class="links">
      <a href="mailto:you@example.com">Email</a>
      <a href="https://github.com/yourusername" target="_blank" rel="noopener">GitHub</a>
      <a href="#" target="_blank" rel="noopener">LinkedIn</a>
    </div>
  </div>
</section>

<footer>© 2026 James</footer>

</body>
</html>
