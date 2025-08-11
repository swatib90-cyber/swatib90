<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Swati B — Research Assistant Professor & Data Scientist</title>

<style>
  :root{
    --bg1:#071027;
    --bg2:#082338;
    --card:#081427;
    --accent1:#60e0b0;
    --accent2:#6fc9ff;
    --muted:#9fb0bf;
    --glass: rgba(255,255,255,0.025);
    --radius:14px;
    --mono: "Courier New", monospace;
  }

  *{box-sizing:border-box}
  html,body{height:100%}
  body{
    margin:0;
    font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    background: radial-gradient(1000px 500px at 10% 15%, rgba(96,224,176,0.04), transparent 10%),
                linear-gradient(135deg,var(--bg1),var(--bg2));
    color:#eaf6ff;
    display:flex;
    align-items:center;
    justify-content:center;
    padding:36px;
  }

  .card{
    width: min(980px, 96%);
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border-radius: var(--radius);
    padding:26px;
    display:flex;
    gap:22px;
    align-items:center;
    box-shadow: 0 12px 40px rgba(4,10,30,0.6), inset 0 1px 0 rgba(255,255,255,0.02);
    backdrop-filter: blur(6px);
    transform: translateY(18px);
    opacity:0;
    animation: pop 520ms cubic-bezier(.2,.9,.3,1) forwards 120ms;
  }

  @keyframes pop{ to{transform:none; opacity:1} }

  .avatar{
    flex: 0 0 140px;
    width:140px; height:140px;
    border-radius:18px;
    overflow:hidden;
    background:linear-gradient(120deg,var(--accent1),var(--accent2));
    padding:4px;
    display:grid; place-items:center;
  }
  .avatar img{
    width:100%; height:100%; object-fit:cover; border-radius:12px; display:block;
  }

  .meta{ flex:1; min-width:0; }
  .title-row{ display:flex; align-items:center; gap:12px; flex-wrap:wrap; }

  h1{ margin:0; font-size:1.25rem; letter-spacing:-0.3px; }
  .role{ font-weight:600; color:var(--accent1); font-size:0.95rem; margin-left:6px; }

  .years {
    font-weight:700;
    color:var(--accent1);
    background:var(--glass);
    padding:6px 10px;
    border-radius:10px;
    font-size:0.95rem;
  }

  .typing {
    margin-top:8px;
    font-family: var(--mono);
    color:var(--accent2);
    font-weight:700;
    display:inline-block;
    white-space:nowrap;
    overflow:hidden;
    border-right:2px solid rgba(255,255,255,0.12);
    padding-right:6px;
    max-width:0ch;
  }

  p.lead{
    margin:12px 0 14px 0;
    color:var(--muted);
    line-height:1.45;
    font-size:0.95rem;
    max-width:70ch;
  }

  .skills-wrap{ --h:36px; height:var(--h); overflow:hidden; position:relative; width:100%; }
  .skills{ display:flex; flex-direction:column; gap:10px; transform: translateY(0); animation: slideSkills 10s linear infinite; }
  @keyframes slideSkills{
    0%{transform:translateY(0)}
    25%{transform:translateY(-36px)}
    50%{transform:translateY(-72px)}
    75%{transform:translateY(-108px)}
    100%{transform:translateY(0)}
  }

  .chip{
    display:inline-flex; gap:10px; align-items:center; padding:6px 10px;
    border-radius:999px; background: linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    color:var(--muted); font-weight:700; width:max-content; font-size:0.88rem;
    box-shadow: 0 6px 16px rgba(4,10,30,0.35);
  }

  .links{ margin-top:14px; display:flex; gap:10px; flex-wrap:wrap; align-items:center; }
  .btn{
    text-decoration:none; color:var(--accent2); border:1px solid rgba(127,211,255,0.12);
    padding:8px 12px; border-radius:10px; font-weight:700; font-size:0.9rem; transition: all 160ms ease; background:transparent;
  }
  .btn:hover{ transform:translateY(-3px); box-shadow: 0 10px 30px rgba(7,18,39,0.45); }

  .meta-right{ flex:0 0 190px; display:flex; flex-direction:column; gap:12px; align-items:flex-end; }
  .stat{
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    padding:10px 12px; border-radius:12px; text-align:center; min-width:120px;
  }
  .stat .big{ font-size:1.15rem; font-weight:800; color:var(--accent1); }
  .stat .small{ font-size:0.78rem; color:var(--muted); margin-top:4px }

  @media (max-width:760px){
    .card{ flex-direction:column; align-items:center; padding:18px }
    .meta-right{ align-items:center; width:100% }
    .avatar{ width:120px; height:120px }
  }
</style>
</head>

<body>
  <main class="card" role="main" aria-label="Profile card">
    <div class="avatar">
      <!-- Replace profile.jpg with your photo -->
      <img src="profile.jpg" alt="Profile photo">
    </div>

    <section class="meta">
      <div class="title-row">
        <div>
          <h1>Swati B <span class="role">• Research Assistant Professor</span></h1>
          <div style="margin-top:6px">
            <span class="years" aria-hidden="true">16 years</span>
            <span style="margin-left:10px;color:var(--muted);font-size:0.92rem">Academia • Industry • Data Science</span>
          </div>
        </div>
      </div>

      <div class="typing" id="typing"></div>

      <p class="lead">I combine 16 years of academic leadership with hands-on data science and AI engineering — building reproducible research, production-ready ML systems, and scalable analytics pipelines.</p>

      <div class="skills-wrap" aria-hidden="true">
        <div class="skills" id="skills">
          <div class="chip">📊 Data Science • ML • Deep Learning</div>
          <div class="chip">🤖 Production ML • Model Ops • Real-time Analytics</div>
          <div class="chip">📡 Networks • MANETs • Energy-efficient Routing</div>
          <div class="chip">☁️ Kafka • Docker • Distributed Systems</div>
          <div class="chip">📚 Research • Supervision • Publications</div>
        </div>
      </div>

      <div class="links">
        <a class="btn" href="#" onclick="alert('Replace with link to your CV or publications');return false">View CV</a>
        <a class="btn" href="#" onclick="alert('Replace with link to your GitHub repos');return false">Projects</a>
        <a class="btn" href="#" onclick="alert('Replace with contact link');return false">Contact</a>
      </div>
    </section>

    <aside class="meta-right" aria-hidden="true">
      <div class="stat">
        <div class="big" id="papers">0</div>
        <div class="small">Publications</div>
      </div>
      <div class="stat">
        <div class="big" id="projects">0</div>
        <div class="small">Projects / Repos</div>
      </div>
      <div class="stat">
        <div class="big" id="students">0</div>
        <div class="small">Students Mentored</div>
      </div>
    </aside>
  </main>

<script>
  // Personalise the lines below
  const texts = [
    "Research-led data science with production delivery.",
    "16 years — academia & industry, mentoring teams.",
    "Building reproducible ML, real-time analytics, and scalable systems."
  ];
  const el = document.getElementById('typing');
  let ti = 0, pos = 0, forward = true;

  function typeStep(){
    const txt = texts[ti];
    if(forward){
      pos++;
      el.style.maxWidth = pos + 'ch';
      el.textContent = txt.slice(0,pos);
      if(pos >= txt.length){ forward=false; setTimeout(typeStep,1200); return; }
    } else {
      pos--;
      el.style.maxWidth = pos + 'ch';
      el.textContent = txt.slice(0,pos);
      if(pos <= 0){ forward=true; ti = (ti+1)%texts.length; setTimeout(typeStep,300); return; }
    }
    setTimeout(typeStep, 48);
  }
  setTimeout(typeStep, 300);

  // Animated counters (edit numbers to real values)
  function animateCount(id, end, duration=900){
    const el = document.getElementById(id);
    if(!el) return;
    let start = 0;
    const stepTime = Math.max(12, Math.floor(duration / Math.max(1,end)));
    const ticker = setInterval(()=>{
      start += 1;
      el.textContent = start;
      if(start >= end) clearInterval(ticker);
    }, stepTime);
  }
  // TODO: replace counts with your real numbers
  animateCount('papers', 28, 1000);     // publications
  animateCount('projects', 42, 1000);   // repos / projects
  animateCount('students', 68, 1000);   // students mentored
</script>
</body>
</html>
