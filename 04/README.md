<!--
  README.md - Premium Cyberpunk GitHub Profile for
  Mahammad Aftab (mahammadaftab)
  Theme: Dark / Neon / Futuristic / Cyberpunk
  NOTE: This file uses advanced HTML + CSS inside Markdown for a premium look.
-->

<div align="center">

<!-- =========================
     Futuristic Neon Banner
     ========================= -->
<style>
  :root{
    --bg:#0b0f14;
    --panel:#071018;
    --neon-cyan:#00f0ff;
    --neon-pink:#ff2dcb;
    --neon-purple:#8a2be2;
    --muted:#9aa7b2;
    --glass: rgba(255,255,255,0.03);
    --accent: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink));
    --glass-border: rgba(255,255,255,0.04);
    --glass-glow: 0 6px 30px rgba(0,240,255,0.04), inset 0 1px 0 rgba(255,255,255,0.02);
    font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  }
  .readme-body{
    background: radial-gradient(1200px 600px at 10% 10%, rgba(138,43,226,0.06), transparent 6%),
                radial-gradient(1000px 500px at 90% 90%, rgba(0,240,255,0.03), transparent 6%),
                var(--bg);
    color: #cfeefb;
    padding: 36px 18px;
    border-radius: 14px;
    max-width: 1100px;
    margin: 28px auto;
    box-shadow: 0 10px 60px rgba(0,0,0,0.6);
    border: 1px solid rgba(255,255,255,0.02);
  }
  .banner{
    width:100%;
    border-radius:12px;
    padding:28px;
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border: 1px solid var(--glass-border);
    box-shadow: var(--glass-glow);
    display:flex;
    gap:20px;
    align-items:center;
    justify-content:space-between;
    flex-wrap:wrap;
  }
  .avatar-wrap{
    display:flex;
    gap:16px;
    align-items:center;
  }
  .avatar{
    width:120px;
    height:120px;
    border-radius:16px;
    background: linear-gradient(135deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border: 1px solid rgba(255,255,255,0.04);
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:700;
    color:var(--neon-cyan);
    font-size:28px;
    letter-spacing:1px;
    box-shadow: 0 8px 30px rgba(0,0,0,0.6), 0 0 18px rgba(0,240,255,0.03);
  }
  .title{
    text-align:left;
    max-width:720px;
  }
  .name{
    font-size:28px;
    font-weight:800;
    color: #e6faff;
    letter-spacing:0.6px;
    margin-bottom:6px;
    display:flex;
    gap:12px;
    align-items:center;
  }
  .neon-tag{
    padding:6px 10px;
    border-radius:999px;
    background: linear-gradient(90deg, rgba(0,240,255,0.06), rgba(255,45,203,0.04));
    color:var(--neon-cyan);
    font-weight:700;
    font-size:12px;
    border:1px solid rgba(0,240,255,0.06);
    box-shadow: 0 6px 30px rgba(0,240,255,0.02);
  }
  .role{
    color:var(--muted);
    font-size:14px;
    margin-bottom:8px;
  }
  .meta{
    display:flex;
    gap:12px;
    align-items:center;
    color:var(--muted);
    font-size:13px;
  }

  /* Typing animation */
  .type-wrap{
    display:flex;
    gap:12px;
    align-items:center;
    margin-top:10px;
  }
  .type {
    font-family: "Fira Code", monospace;
    color: #bfefff;
    font-weight:700;
    font-size:15px;
    letter-spacing:0.6px;
  }
  .cursor {
    width:10px;
    height:20px;
    background:var(--neon-cyan);
    margin-left:6px;
    border-radius:2px;
    animation: blink 1s steps(2, start) infinite;
    box-shadow: 0 0 12px rgba(0,240,255,0.6);
  }
  @keyframes blink { 50% { opacity:0 } }

  /* Section dividers */
  .divider{
    width:100%;
    height:1px;
    margin:20px 0;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.03), transparent);
  }

  /* Neon headings */
  h2.neon{
    font-size:18px;
    color:#e9faff;
    letter-spacing:1px;
    margin:8px 0 12px 0;
    display:inline-block;
    padding:8px 14px;
    border-radius:8px;
    background: linear-gradient(90deg, rgba(138,43,226,0.03), rgba(0,240,255,0.02));
    border:1px solid rgba(255,255,255,0.02);
    box-shadow: 0 6px 30px rgba(138,43,226,0.02);
  }

  /* Panels */
  .panel{
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    border:1px solid var(--glass-border);
    border-radius:12px;
    padding:18px;
    box-shadow: var(--glass-glow);
  }

  /* Grid */
  .grid{
    display:grid;
    grid-template-columns: 1fr 380px;
    gap:18px;
    align-items:start;
  }
  @media (max-width:980px){
    .grid{ grid-template-columns: 1fr; }
    .avatar{ width:96px; height:96px; font-size:22px; }
  }

  /* Social icons row */
  .socials{
    display:flex;
    gap:10px;
    align-items:center;
    margin-top:12px;
  }
  .socials a{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    width:44px;
    height:44px;
    border-radius:10px;
    color:var(--neon-cyan);
    text-decoration:none;
    border:1px solid rgba(255,255,255,0.02);
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    transition: transform .18s ease, box-shadow .18s ease;
  }
  .socials a:hover{ transform: translateY(-4px); box-shadow: 0 10px 30px rgba(0,0,0,0.6); }

  /* Tech stack animated chips */
  .tech-row{
    display:flex;
    gap:8px;
    flex-wrap:wrap;
    margin-top:12px;
  }
  .chip{
    padding:8px 12px;
    border-radius:999px;
    font-weight:700;
    font-size:13px;
    color:#e9fbff;
    background: linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border:1px solid rgba(255,255,255,0.02);
    box-shadow: 0 6px 20px rgba(0,0,0,0.5);
    transform: translateY(0);
    transition: transform .18s ease;
  }
  .chip:hover{ transform: translateY(-6px); }

  /* Skill bars */
  .skill{
    margin:10px 0;
  }
  .skill .label{
    display:flex;
    justify-content:space-between;
    font-size:13px;
    color:var(--muted);
    margin-bottom:6px;
  }
  .bar{
    height:12px;
    background: rgba(255,255,255,0.02);
    border-radius:999px;
    overflow:hidden;
    border:1px solid rgba(255,255,255,0.02);
  }
  .bar > i{
    display:block;
    height:100%;
    background: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink));
    box-shadow: 0 6px 30px rgba(0,240,255,0.04);
    border-radius:999px;
    transition: width 1.2s cubic-bezier(.2,.9,.2,1);
  }

  /* Projects grid */
  .projects{
    display:grid;
    grid-template-columns: repeat(2, 1fr);
    gap:12px;
  }
  @media (max-width:980px){ .projects{ grid-template-columns: 1fr; } }
  .project-card{
    padding:14px;
    border-radius:12px;
    border:1px solid rgba(255,255,255,0.02);
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    transition: transform .18s ease;
  }
  .project-card:hover{ transform: translateY(-6px); box-shadow: 0 20px 60px rgba(0,0,0,0.6); }

  /* Footer small */
  .muted-small{ color:var(--muted); font-size:13px; }

  /* Snake visitor animation */
  .snake-wrap{
    margin-top:18px;
    width:100%;
    height:80px;
    border-radius:10px;
    overflow:hidden;
    position:relative;
    border:1px solid rgba(255,255,255,0.02);
    background: linear-gradient(90deg, rgba(0,0,0,0.02), rgba(255,255,255,0.005));
  }
  .snake{
    position:absolute;
    top:50%;
    left:-20%;
    transform:translateY(-50%);
    width:20%;
    height:8px;
    background: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink));
    border-radius:999px;
    box-shadow: 0 8px 30px rgba(0,240,255,0.06);
    animation: snake 6s linear infinite;
  }
  @keyframes snake{
    0%{ left:-20%; width:20%; }
    25%{ left:20%; width:12%; }
    50%{ left:60%; width:28%; }
    75%{ left:90%; width:10%; }
    100%{ left:120%; width:20%; }
  }

  /* Quote */
  .quote{
    font-family: "Fira Code", monospace;
    color:#bfefff;
    font-size:14px;
    padding:12px;
    border-radius:8px;
    background: linear-gradient(90deg, rgba(0,240,255,0.02), rgba(138,43,226,0.02));
    border:1px solid rgba(255,255,255,0.02);
  }

  /* Roadmap list */
  .roadmap{
    display:flex;
    flex-direction:column;
    gap:10px;
  }
  .roadmap-item{
    display:flex;
    gap:12px;
    align-items:flex-start;
  }
  .dot{
    width:12px;
    height:12px;
    border-radius:999px;
    background:var(--neon-pink);
    box-shadow: 0 6px 20px rgba(255,45,203,0.06);
    margin-top:6px;
  }

  /* badges row (inline SVG badges) */
  .badges{
    display:flex;
    gap:8px;
    flex-wrap:wrap;
    margin-top:12px;
  }
  .badge{
    display:inline-flex;
    align-items:center;
    gap:8px;
    padding:6px 10px;
    border-radius:999px;
    background: rgba(255,255,255,0.01);
    border:1px solid rgba(255,255,255,0.02);
    color:#dff9ff;
    font-weight:700;
    font-size:12px;
  }

  /* trophies / stats placeholders */
  .stats-grid{
    display:grid;
    grid-template-columns: repeat(2, 1fr);
    gap:12px;
  }
  @media (max-width:980px){ .stats-grid{ grid-template-columns: 1fr; } }

  /* small link style */
  a.link{
    color:var(--neon-cyan);
    text-decoration:none;
    font-weight:700;
  }
  a.link:hover{ text-decoration:underline; }

</style>

<div class="readme-body">

  <div class="banner">
    <div class="avatar-wrap">
      <div class="avatar" aria-hidden="true">MA</div>
      <div class="title">
        <div class="name">
          <span>Mahammad Aftab</span>
          <span class="neon-tag">AI Engineer • Full Stack</span>
        </div>
        <div class="role">AI Engineer | Full Stack Developer | Generative AI Enthusiast</div>
        <div class="meta">
          <div>📍 India</div>
          <div>💼 Senior • MERN • Python • ML</div>
          <div>🔗 <a class="link" href="https://mahammadaftab.github.io" target="_blank">Portfolio</a></div>
        </div>

        <div class="type-wrap" style="margin-top:10px;">
          <div class="type" id="type-text">Building intelligent systems • Shipping production-grade ML & full-stack apps</div>
          <div class="cursor" aria-hidden="true"></div>
        </div>

        <div class="socials" style="margin-top:12px;">
          <!-- Inline SVG icons for socials -->
          <a href="https://github.com/mahammadaftab" target="_blank" title="GitHub" aria-label="GitHub">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" style="color:var(--neon-cyan)">
              <path d="M12 .5C5.73.5.75 5.48.75 11.75c0 4.96 3.22 9.16 7.69 10.64.56.1.76-.24.76-.53 0-.26-.01-1.12-.02-2.03-3.13.68-3.79-1.51-3.79-1.51-.51-1.3-1.25-1.65-1.25-1.65-1.02-.7.08-.69.08-.69 1.13.08 1.73 1.16 1.73 1.16 1 .17 1.56-.76 1.56-.76.98-1.67 2.57-1.19 3.2-.91.1-.71.39-1.19.71-1.46-2.5-.28-5.13-1.25-5.13-5.56 0-1.23.44-2.24 1.16-3.03-.12-.28-.5-1.4.11-2.92 0 0 .95-.3 3.12 1.16.9-.25 1.86-.38 2.82-.38.96 0 1.92.13 2.82.38 2.17-1.46 3.12-1.16 3.12-1.16.61 1.52.23 2.64.11 2.92.72.79 1.16 1.8 1.16 3.03 0 4.32-2.64 5.28-5.15 5.55.4.35.76 1.05.76 2.12 0 1.53-.01 2.76-.01 3.14 0 .29.2.64.77.53C19.03 20.9 22.25 16.7 22.25 11.75 22.25 5.48 17.27.5 11 .5z" fill="currentColor"/>
            </svg>
          </a>

          <a href="https://www.linkedin.com/in/mahammadaftab" target="_blank" title="LinkedIn" aria-label="LinkedIn">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" style="color:var(--neon-pink)">
              <path d="M4.98 3.5C4.98 4.88 3.86 6 2.48 6S0 4.88 0 3.5 1.12 1 2.5 1 4.98 2.12 4.98 3.5zM.24 8.5h4.48V24H.24zM8.5 8.5h4.3v2.12h.06c.6-1.14 2.06-2.34 4.24-2.34 4.54 0 5.38 2.98 5.38 6.86V24h-4.48v-7.5c0-1.79-.03-4.1-2.5-4.1-2.5 0-2.88 1.95-2.88 3.98V24H8.5z" fill="currentColor"/>
            </svg>
          </a>

          <a href="https://twitter.com/mahammadaftab" target="_blank" title="Twitter" aria-label="Twitter">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" style="color:var(--neon-cyan)">
              <path d="M22.46 6c-.77.35-1.6.58-2.46.69a4.3 4.3 0 0 0 1.88-2.37 8.59 8.59 0 0 1-2.72 1.04 4.28 4.28 0 0 0-7.3 3.9A12.14 12.14 0 0 1 3.16 4.6a4.28 4.28 0 0 0 1.33 5.72 4.24 4.24 0 0 1-1.94-.54v.05a4.28 4.28 0 0 0 3.43 4.2 4.3 4.3 0 0 1-1.93.07 4.28 4.28 0 0 0 4 2.97A8.6 8.6 0 0 1 2 19.54a12.13 12.13 0 0 0 6.56 1.92c7.88 0 12.2-6.53 12.2-12.2 0-.19 0-.39-.01-.58A8.7 8.7 0 0 0 22.46 6z" fill="currentColor"/>
            </svg>
          </a>

          <a href="mailto:mahammad@aftab.dev" target="_blank" title="Email" aria-label="Email">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" style="color:var(--neon-purple)">
              <path d="M12 13.065L.75 5.25V18a2 2 0 0 0 2 2h18.5a2 2 0 0 0 2-2V5.25L12 13.065zM12 11L23.25 3H.75L12 11z" fill="currentColor"/>
            </svg>
          </a>

          <a href="https://discord.gg/yourserver" target="_blank" title="Discord" aria-label="Discord">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" style="color:var(--neon-cyan)">
              <path d="M20.317 4.369A19.791 19.791 0 0 0 16.5 3.2a13.4 13.4 0 0 0-.7 1.5 17.9 17.9 0 0 0-5.6 0 13.4 13.4 0 0 0-.7-1.5 19.8 19.8 0 0 0-3.817 1.169C3.5 9.2 2.5 14.2 3.2 19.1a19.9 19.9 0 0 0 6.1 3.1c.5-.7.9-1.4 1.3-2.1-2.1-.6-3.6-1.6-4.1-2.1.3-.2.6-.4.9-.6 1.8 1 4.1 1.6 6.6 1.6 2.5 0 4.8-.6 6.6-1.6.3.2.6.4.9.6-.5.5-2 1.5-4.1 2.1.4.7.8 1.4 1.3 2.1a19.9 19.9 0 0 0 6.1-3.1c.7-4.9-.3-9.9-3.683-14.731z" fill="currentColor"/>
            </svg>
          </a>
        </div>

      </div>
    </div>

    <!-- Right column: quick badges & counters -->
    <div style="display:flex;flex-direction:column;align-items:flex-end;gap:12px;">
      <div class="badges">
        <div class="badge">⭐ Senior • AI Engineer</div>
        <div class="badge">⚡ Generative AI • ML</div>
        <div class="badge">☁️ Cloud • AWS • K8s</div>
      </div>

      <!-- Profile views counter (link to dynamic badge) -->
      <div class="panel" style="padding:10px 14px;border-radius:10px;">
        <div style="font-size:12px;color:var(--muted);">Profile Views</div>
        <div style="font-weight:800;font-size:20px;color:var(--neon-cyan);margin-top:6px;"><!-- dynamic placeholder -->
          <!-- Link to dynamic counter (click to open) -->
          <a class="link" href="https://komarev.com/ghpvc/?username=mahammadaftab" target="_blank">View live counter</a>
        </div>
      </div>

      <!-- GitHub quick links -->
      <div style="display:flex;gap:8px;">
        <a class="link" href="https://github.com/mahammadaftab?tab=repositories" target="_blank">Repositories</a>
        <span style="color:var(--muted)">•</span>
        <a class="link" href="https://github.com/mahammadaftab?tab=projects" target="_blank">Projects</a>
      </div>
    </div>
  </div>

  <div class="divider"></div>

  <!-- =========================
       Main Grid: Left (About, Tech, Projects)
       Right (Stats, Trophies, Activity)
       ========================= -->
  <div class="grid">

    <!-- LEFT COLUMN -->
    <div>

      <!-- About Me -->
      <h2 class="neon">About Me</h2>
      <div class="panel">
        <p style="margin:0;color:#dff9ff;font-size:15px;">
          I'm <strong>Mahammad Aftab</strong>, an AI Engineer and Full Stack Developer focused on building production-grade
          generative AI systems, scalable MERN applications, and secure cloud-native platforms. I design ML pipelines,
          deploy models to Kubernetes on AWS, and integrate blockchain primitives where decentralization adds value.
        </p>

        <div style="display:flex;gap:18px;margin-top:14px;flex-wrap:wrap;">
          <div style="min-width:220px;">
            <div class="muted-small">Primary Focus</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">Generative AI • LLMs • Full-stack systems</div>
          </div>
          <div style="min-width:220px;">
            <div class="muted-small">Experience</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">5+ years building ML & web platforms</div>
          </div>
          <div style="min-width:220px;">
            <div class="muted-small">Open to</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">Senior roles, AI research engineering, contractor work</div>
          </div>
        </div>

        <div style="margin-top:14px;">
          <div class="muted-small">Core strengths</div>
          <div class="tech-row" style="margin-top:8px;">
            <div class="chip">MERN</div>
            <div class="chip">Generative AI</div>
            <div class="chip">Python • PyTorch</div>
            <div class="chip">Docker • Kubernetes</div>
            <div class="chip">AWS • Terraform</div>
            <div class="chip">Blockchain • Smart Contracts</div>
            <div class="chip">CI/CD • Observability</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Tech Stack (animated icons via CSS chips) -->
      <h2 class="neon">Tech Stack</h2>
      <div class="panel">
        <div style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap;">
          <div style="flex:1;min-width:260px;">
            <div class="muted-small">Primary</div>
            <div class="tech-row" style="margin-top:8px;">
              <div class="chip">React</div>
              <div class="chip">Node.js</div>
              <div class="chip">Express</div>
              <div class="chip">MongoDB</div>
              <div class="chip">Python</div>
              <div class="chip">PyTorch</div>
            </div>
          </div>
          <div style="flex:1;min-width:260px;">
            <div class="muted-small">Infrastructure</div>
            <div class="tech-row" style="margin-top:8px;">
              <div class="chip">Docker</div>
              <div class="chip">Kubernetes</div>
              <div class="chip">AWS</div>
              <div class="chip">Terraform</div>
              <div class="chip">CI/CD</div>
            </div>
          </div>
        </div>

        <div style="margin-top:14px;">
          <div class="muted-small">Emerging / Research</div>
          <div class="tech-row" style="margin-top:8px;">
            <div class="chip">LLMs • Fine-tuning</div>
            <div class="chip">Diffusion Models</div>
            <div class="chip">Blockchain Integrations</div>
            <div class="chip">Federated Learning</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Skills with progress bars -->
      <h2 class="neon">Skills</h2>
      <div class="panel">
        <div class="skill">
          <div class="label"><span>Machine Learning & Deep Learning</span><span>92%</span></div>
          <div class="bar"><i style="width:92%"></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Generative AI / LLMs</span><span>90%</span></div>
          <div class="bar"><i style="width:90%"></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Full Stack (MERN)</span><span>88%</span></div>
          <div class="bar"><i style="width:88%"></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Cloud & DevOps (AWS / K8s)</span><span>85%</span></div>
          <div class="bar"><i style="width:85%"></i></div>
        </div>
        <div class="skill">
          <div class="label"><span>Blockchain & Smart Contracts</span><span>72%</span></div>
          <div class="bar"><i style="width:72%"></i></div>
        </div>
        <div style="margin-top:12px;" class="muted-small">I focus on production-readiness: observability, testing, CI/CD, and secure deployments.</div>
      </div>

      <div style="height:12px"></div>

      <!-- Featured Projects -->
      <h2 class="neon">Featured Projects</h2>
      <div class="projects">
        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:800;font-size:15px;color:#e9fbff;">AstraAI • Generative Platform</div>
              <div class="muted-small" style="margin-top:6px;">End-to-end generative AI platform: fine-tuning, inference, and deployment on K8s.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted-small">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">PyTorch • FastAPI • K8s</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/astraai" target="_blank">Repository</a>
            <span style="color:var(--muted)">•</span>
            <a class="link" href="https://astraai.example.com" target="_blank">Live Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:800;font-size:15px;color:#e9fbff;">NeonShop • Scalable MERN E‑commerce</div>
              <div class="muted-small" style="margin-top:6px;">High-throughput storefront with server-side rendering and microservices.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted-small">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">React • Node • MongoDB • Docker</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/neonshop" target="_blank">Repository</a>
            <span style="color:var(--muted)">•</span>
            <a class="link" href="https://neonshop.example.com" target="_blank">Live Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:800;font-size:15px;color:#e9fbff;">ChainGuard • Smart Contract Auditor</div>
              <div class="muted-small" style="margin-top:6px;">Automated security checks and fuzzing for Solidity contracts.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted-small">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">Solidity • Python • Docker</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/chainguard" target="_blank">Repository</a>
            <span style="color:var(--muted)">•</span>
            <a class="link" href="https://chainguard.example.com" target="_blank">Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:800;font-size:15px;color:#e9fbff;">Realtime-ML • Streaming Inference</div>
              <div class="muted-small" style="margin-top:6px;">Low-latency model serving with autoscaling and A/B experiments.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted-small">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">Kafka • FastAPI • K8s</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/realtime-ml" target="_blank">Repository</a>
            <span style="color:var(--muted)">•</span>
            <a class="link" href="https://realtime-ml.example.com" target="_blank">Demo</a>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Achievements & Certifications -->
      <h2 class="neon">Achievements & Certifications</h2>
      <div class="panel">
        <ul style="margin:0 0 0 18px;padding:0;color:#dff9ff;">
          <li>Certified AWS Solutions Architect – Professional (2024)</li>
          <li>Deep Learning Specialization – Coursera (TensorFlow / PyTorch)</li>
          <li>Winner • HackAI 2023 – Best Generative Model</li>
          <li>Certified Kubernetes Application Developer (CKAD)</li>
          <li>Multiple open-source contributions to ML infra & tooling</li>
        </ul>
      </div>

      <div style="height:12px"></div>

      <!-- Roadmap -->
      <h2 class="neon">Roadmap</h2>
      <div class="panel roadmap">
        <div class="roadmap-item">
          <div class="dot" style="background:var(--neon-cyan)"></div>
          <div>
            <div style="font-weight:800;color:#e9fbff;">Q3 2026 — Productionize AstraAI</div>
            <div class="muted-small">Scale inference, add multi-tenant orchestration, and enterprise integrations.</div>
          </div>
        </div>

        <div class="roadmap-item">
          <div class="dot" style="background:var(--neon-pink)"></div>
          <div>
            <div style="font-weight:800;color:#e9fbff;">Q4 2026 — Decentralized ML Marketplace</div>
            <div class="muted-small">Integrate blockchain for model provenance and micropayments.</div>
          </div>
        </div>

        <div class="roadmap-item">
          <div class="dot" style="background:var(--neon-purple)"></div>
          <div>
            <div style="font-weight:800;color:#e9fbff;">2027 — Research: Federated & Privacy-preserving LLMs</div>
            <div class="muted-small">Focus on privacy-first model training and deployment.</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Support / Contact -->
      <h2 class="neon">Support / Contact</h2>
      <div class="panel" style="display:flex;gap:12px;flex-wrap:wrap;align-items:center;">
        <div style="flex:1;min-width:260px;">
          <div style="font-weight:800;color:#e9fbff;">Hire / Collaborate / Contract</div>
          <div class="muted-small" style="margin-top:6px;">Open to senior engineering roles, AI research engineering, and consulting.</div>
        </div>
        <div style="min-width:220px;">
          <div style="font-weight:700;color:var(--neon-cyan);">Email</div>
          <div class="muted-small" style="margin-top:6px;">mahammad@aftab.dev</div>
        </div>
      </div>

      <div style="height:18px"></div>

      <!-- Coding Quote -->
      <h2 class="neon">Coding Quote</h2>
      <div class="panel quote">
        "Ship small, iterate fast, and let the data decide. Build systems that are observable, testable, and kind to users."
      </div>

    </div>

    <!-- RIGHT COLUMN -->
    <div>

      <!-- GitHub Stats (links to dynamic APIs; click to view live images) -->
      <h2 class="neon">GitHub Stats & Activity</h2>
      <div class="panel">
        <div class="stats-grid">
          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.02);">
            <div style="font-weight:800;color:#e9fbff;">GitHub Stats</div>
            <div class="muted-small" style="margin-top:8px;">Click to view live, dynamic cards</div>
            <div style="margin-top:10px;display:flex;flex-direction:column;gap:8px;">
              <a class="link" href="https://github-readme-stats.vercel.app/api?username=mahammadaftab&show_icons=true&theme=dark" target="_blank">View dynamic stats card</a>
              <a class="link" href="https://github-readme-streak-stats.herokuapp.com/?user=mahammadaftab&theme=dark" target="_blank">View streak stats</a>
              <a class="link" href="https://github-readme-stats.vercel.app/api/top-langs/?username=mahammadaftab&layout=compact&theme=dark" target="_blank">Top languages</a>
            </div>
          </div>

          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.02);">
            <div style="font-weight:800;color:#e9fbff;">Contribution Graph</div>
            <div class="muted-small" style="margin-top:8px;">Live contributions & activity</div>
            <div style="margin-top:10px;">
              <a class="link" href="https://github.com/mahammadaftab" target="_blank">Open GitHub profile</a>
            </div>
          </div>
        </div>

        <div style="margin-top:12px;" class="muted-small">
          Note: For live, embeddable images use the GitHub Readme Stats APIs (links above). They provide dynamic SVGs for stats, streaks, and top languages.
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Trophies & Activity -->
      <h2 class="neon">Trophies & Activity</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:10px;">
          <div style="font-weight:800;color:#e9fbff;">Trophies</div>
          <div class="muted-small">Open-source contributions, challenge wins, and community recognition.</div>

          <div style="margin-top:8px;display:flex;gap:8px;flex-wrap:wrap;">
            <div class="badge">🏆 Open Source Contributor</div>
            <div class="badge">🏅 HackAI Winner</div>
            <div class="badge">🔒 Security Advocate</div>
            <div class="badge">☁️ Cloud Certified</div>
          </div>

          <div style="margin-top:12px;">
            <div style="font-weight:800;color:#e9fbff;">Activity Graph</div>
            <div class="muted-small" style="margin-top:6px;">For a live activity graph, click below</div>
            <div style="margin-top:8px;">
              <a class="link" href="https://github.com/mahammadaftab" target="_blank">View activity & contributions</a>
            </div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- AI / ML / Blockchain / Cloud Sections -->
      <h2 class="neon">AI • ML • Blockchain • Cloud</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:12px;">
          <div>
            <div style="font-weight:800;color:#e9fbff;">Generative AI & ML</div>
            <div class="muted-small" style="margin-top:6px;">
              Architected LLM fine-tuning pipelines, built multimodal models, and deployed inference services with autoscaling.
            </div>
          </div>

          <div>
            <div style="font-weight:800;color:#e9fbff;">Blockchain</div>
            <div class="muted-small" style="margin-top:6px;">
              Smart contract development, security audits, and integrating on-chain provenance for ML models and datasets.
            </div>
          </div>

          <div>
            <div style="font-weight:800;color:#e9fbff;">Cloud & DevOps</div>
            <div class="muted-small" style="margin-top:6px;">
              Production deployments on AWS, Kubernetes orchestration, infra-as-code, and observability with Prometheus & Grafana.
            </div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Spotify / Discord / Portfolio -->
      <h2 class="neon">Now Playing • Community • Portfolio</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:10px;">
          <div>
            <div style="font-weight:800;color:#e9fbff;">Spotify</div>
            <div class="muted-small" style="margin-top:6px;">Curated playlists for deep work and ML research.</div>
            <div style="margin-top:8px;"><a class="link" href="https://open.spotify.com/user/yourprofile" target="_blank">Open Spotify</a></div>
          </div>

          <div>
            <div style="font-weight:800;color:#e9fbff;">Discord</div>
            <div class="muted-small" style="margin-top:6px;">Active in AI & DevOps communities — join the server for discussions.</div>
            <div style="margin-top:8px;"><a class="link" href="https://discord.gg/yourserver" target="_blank">Join Discord</a></div>
          </div>

          <div>
            <div style="font-weight:800;color:#e9fbff;">Portfolio</div>
            <div class="muted-small" style="margin-top:6px;">Detailed case studies, architecture diagrams, and research notes.</div>
            <div style="margin-top:8px;"><a class="link" href="https://mahammadaftab.github.io" target="_blank">Visit Portfolio</a></div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Visitor snake animation -->
      <div class="snake-wrap panel">
        <div style="position:absolute;left:12px;top:12px;color:var(--muted);font-size:12px;">Visitor trail</div>
        <div class="snake" aria-hidden="true"></div>
      </div>

    </div>
  </div>

  <div style="height:18px"></div>

  <!-- =========================
       Footer: Contact, Links, Legal
       ========================= -->
  <div style="display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap;align-items:center;">
    <div class="muted-small">© <strong>Mahammad Aftab</strong> • AI Engineer • Full Stack Developer • India</div>
    <div style="display:flex;gap:12px;align-items:center;">
      <a class="link" href="https://github.com/mahammadaftab" target="_blank">GitHub</a>
      <a class="link" href="https://www.linkedin.com/in/mahammadaftab" target="_blank">LinkedIn</a>
      <a class="link" href="mailto:mahammad@aftab.dev">Email</a>
    </div>
  </div>

  <div style="height:12px"></div>

  <!-- =========================
       Extra: Dynamic badges (SVG-like inline badges)
       ========================= -->
  <div style="display:flex;gap:8px;flex-wrap:wrap;align-items:center;">
    <div class="badge">👨‍💻 Open to work</div>
    <div class="badge">🧠 LLMs • Generative</div>
    <div class="badge">☁️ AWS • K8s</div>
    <div class="badge">🛡️ Security-minded</div>
  </div>

</div>

<!-- =========================
     Animated typing JS (pure CSS-like simulation)
     ========================= -->
<script>
  // Simple typing rotation (no external libs)
  (function(){
    const phrases = [
      "Building intelligent systems • Shipping production-grade ML & full-stack apps",
      "MERN • Python • Generative AI • Cloud-native",
      "Deploying models to Kubernetes • Observability-first",
      "Blockchain integrations for model provenance"
    ];
    let idx = 0;
    const el = document.getElementById('type-text');
    const cursor = document.querySelector('.cursor');
    function typePhrase(phrase, cb){
      el.textContent = '';
      let i=0;
      const t = setInterval(()=>{
        el.textContent += phrase[i++] || '';
        if(i>phrase.length){ clearInterval(t); setTimeout(cb,1200); }
      }, 28);
    }
    function loop(){
      typePhrase(phrases[idx%phrases.length], ()=>{ idx++; loop(); });
    }
    if(el){ loop(); }
  })();
</script>

</div>

</div>

<!-- =========================
     Notes for recruiters (hidden in HTML comment)
     =========================
     - GitHub username: mahammadaftab
     - Name: Mahammad Aftab
     - Role: AI Engineer | Full Stack Developer | Generative AI Enthusiast
     - Location: India
     - Tech: MERN, Python, React, Node.js, MongoDB, Express, Docker, Kubernetes, AWS, Blockchain, ML
     - For live dynamic cards (stats, streaks, top langs) use:
       https://github-readme-stats.vercel.app/api?username=mahammadaftab&show_icons=true&theme=dark
       https://github-readme-streak-stats.herokuapp.com/?user=mahammadaftab&theme=dark
       https://github-readme-stats.vercel.app/api/top-langs/?username=mahammadaftab&layout=compact&theme=dark
     ========================= -->

