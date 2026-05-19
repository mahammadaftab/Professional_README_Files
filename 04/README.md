<!--
  README.md - Premium Cyberpunk GitHub Profile for
  Mahammad Aftab (mahammadaftab)
  Theme: Dark / Neon / Futuristic / Cyberpunk
  NOTE: Paste this entire file into your GitHub profile README.
-->

<div align="center">

<!-- =========================
     Styles: Dark Cyberpunk Theme
     ========================= -->
<style>
  :root{
    --bg:#05060a;
    --panel:#071018;
    --neon-cyan:#00f0ff;
    --neon-pink:#ff2dcb;
    --neon-purple:#8a2be2;
    --muted:#8fa6b3;
    --glass: rgba(255,255,255,0.02);
    --accent: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink));
    font-family: Inter, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Fira Code", monospace;
  }
  .readme {
    background: radial-gradient(800px 300px at 10% 10%, rgba(138,43,226,0.04), transparent 6%),
                radial-gradient(700px 250px at 90% 90%, rgba(0,240,255,0.03), transparent 6%),
                var(--bg);
    color: #dff9ff;
    padding: 28px;
    border-radius: 14px;
    max-width: 1100px;
    margin: 28px auto;
    box-shadow: 0 18px 80px rgba(0,0,0,0.7);
    border: 1px solid rgba(255,255,255,0.02);
  }
  .banner {
    display:flex;
    gap:18px;
    align-items:center;
    justify-content:space-between;
    padding:20px;
    border-radius:12px;
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    border: 1px solid rgba(255,255,255,0.02);
    box-shadow: 0 10px 40px rgba(0,0,0,0.6);
    flex-wrap:wrap;
  }
  .left {
    display:flex;
    gap:16px;
    align-items:center;
  }
  .avatar {
    width:120px;
    height:120px;
    border-radius:16px;
    background: linear-gradient(135deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border: 1px solid rgba(255,255,255,0.04);
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:800;
    color:var(--neon-cyan);
    font-size:34px;
    letter-spacing:1px;
    box-shadow: 0 8px 30px rgba(0,0,0,0.6), 0 0 18px rgba(0,240,255,0.03);
  }
  .title {
    text-align:left;
    min-width:320px;
  }
  .name {
    font-size:28px;
    font-weight:900;
    color:#e9fbff;
    display:flex;
    gap:12px;
    align-items:center;
  }
  .role {
    color:var(--muted);
    font-size:13px;
    margin-top:6px;
  }
  .meta {
    display:flex;
    gap:10px;
    margin-top:10px;
    color:var(--muted);
    font-size:13px;
    flex-wrap:wrap;
  }

  /* Typing animation */
  .type {
    font-family: "Fira Code", monospace;
    color:#bfefff;
    font-weight:700;
    font-size:14px;
    letter-spacing:0.4px;
  }
  .cursor {
    display:inline-block;
    width:10px;
    height:18px;
    background:var(--neon-cyan);
    margin-left:8px;
    border-radius:2px;
    animation: blink 1s steps(2, start) infinite;
    box-shadow: 0 0 12px rgba(0,240,255,0.6);
    vertical-align:middle;
  }
  @keyframes blink { 50% { opacity:0 } }

  .badges { display:flex; gap:8px; flex-wrap:wrap; align-items:center; }
  .badge {
    padding:6px 10px;
    border-radius:999px;
    background: linear-gradient(90deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    border:1px solid rgba(255,255,255,0.02);
    color:#dff9ff;
    font-weight:700;
    font-size:12px;
  }

  .divider { height:1px; background: linear-gradient(90deg, transparent, rgba(255,255,255,0.03), transparent); margin:18px 0; }

  .grid { display:grid; grid-template-columns: 1fr 380px; gap:18px; align-items:start; }
  @media (max-width:980px){ .grid{ grid-template-columns: 1fr; } .avatar{ width:96px; height:96px; font-size:26px; } }

  .panel {
    background: linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    border-radius:12px;
    padding:16px;
    border:1px solid rgba(255,255,255,0.02);
    box-shadow: 0 10px 40px rgba(0,0,0,0.6);
  }

  h2.neon {
    font-size:16px;
    color:#e9faff;
    letter-spacing:1px;
    margin:6px 0 12px 0;
    display:inline-block;
    padding:8px 12px;
    border-radius:8px;
    background: linear-gradient(90deg, rgba(138,43,226,0.03), rgba(0,240,255,0.02));
    border:1px solid rgba(255,255,255,0.02);
  }

  .tech-row { display:flex; gap:8px; flex-wrap:wrap; margin-top:8px; }
  .chip {
    padding:8px 12px;
    border-radius:999px;
    font-weight:800;
    font-size:13px;
    color:#e9fbff;
    background: linear-gradient(90deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));
    border:1px solid rgba(255,255,255,0.02);
    box-shadow: 0 8px 30px rgba(0,0,0,0.6);
    transition: transform .18s ease;
  }
  .chip:hover{ transform: translateY(-6px); }

  .skill { margin:10px 0; }
  .skill .label { display:flex; justify-content:space-between; font-size:13px; color:var(--muted); margin-bottom:6px; }
  .bar { height:12px; background: rgba(255,255,255,0.02); border-radius:999px; overflow:hidden; border:1px solid rgba(255,255,255,0.02); }
  .bar > i { display:block; height:100%; background: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink)); border-radius:999px; transition: width 1.2s cubic-bezier(.2,.9,.2,1); }

  .projects { display:grid; grid-template-columns: repeat(2, 1fr); gap:12px; }
  @media (max-width:980px){ .projects{ grid-template-columns: 1fr; } }
  .project-card { padding:12px; border-radius:12px; transition: transform .18s ease; }
  .project-card:hover{ transform: translateY(-6px); box-shadow: 0 20px 60px rgba(0,0,0,0.6); }

  .stats-grid { display:grid; grid-template-columns: 1fr 1fr; gap:12px; }
  @media (max-width:980px){ .stats-grid{ grid-template-columns: 1fr; } }

  .snake-wrap { margin-top:12px; width:100%; height:70px; border-radius:10px; overflow:hidden; position:relative; border:1px solid rgba(255,255,255,0.02); background: linear-gradient(90deg, rgba(0,0,0,0.02), rgba(255,255,255,0.005)); }
  .snake { position:absolute; top:50%; left:-20%; transform:translateY(-50%); width:20%; height:8px; background: linear-gradient(90deg,var(--neon-cyan),var(--neon-pink)); border-radius:999px; box-shadow: 0 8px 30px rgba(0,240,255,0.06); animation: snake 6s linear infinite; }
  @keyframes snake{ 0%{ left:-20%; width:20%; } 25%{ left:20%; width:12%; } 50%{ left:60%; width:28%; } 75%{ left:90%; width:10%; } 100%{ left:120%; width:20%; } }

  .quote { font-family: "Fira Code", monospace; color:#bfefff; font-size:14px; padding:12px; border-radius:8px; background: linear-gradient(90deg, rgba(0,240,255,0.02), rgba(138,43,226,0.02)); border:1px solid rgba(255,255,255,0.02); }

  .muted { color:var(--muted); font-size:13px; }
  a.link { color:var(--neon-cyan); text-decoration:none; font-weight:800; }
  a.link:hover { text-decoration:underline; }

  /* Responsive small tweaks */
  @media (max-width:640px){
    .name{ font-size:20px; }
    .role{ font-size:12px; }
  }
</style>

<div class="readme">

  <!-- =========================
       Header / Banner
       ========================= -->
  <div class="banner">
    <div class="left">
      <div class="avatar">MA</div>
      <div class="title">
        <div class="name">Mahammad Aftab <span style="font-size:12px;color:var(--neon-pink);padding:6px 10px;border-radius:999px;background:rgba(255,45,203,0.04);font-weight:800;">AI Engineer • Full Stack</span></div>
        <div class="role">AI Engineer | Full Stack Developer | Generative AI Enthusiast — India</div>

        <div style="margin-top:10px;display:flex;align-items:center;gap:12px;flex-wrap:wrap;">
          <div class="type" id="type-text">Designing production-grade AI systems • MERN • Cloud-native</div>
          <div class="cursor" aria-hidden="true"></div>
        </div>

        <div class="meta">
          <div>📍 India</div>
          <div>💼 Senior • MERN • Python • ML</div>
          <div>🔗 <a class="link" href="https://mahammadaftab.github.io" target="_blank">Portfolio</a></div>
        </div>

        <div style="margin-top:12px;" class="badges">
          <!-- Shields.io badges -->
          <img src="https://img.shields.io/badge/Status-Open%20to%20Work-00f0ff?style=for-the-badge&logo=github" alt="Open to work" />
          <img src="https://img.shields.io/badge/Top%20Tech-MERN-%2300f0ff?style=for-the-badge&logo=react" alt="MERN" />
          <img src="https://img.shields.io/badge/AI-Generative-%23ff2dcb?style=for-the-badge&logo=python" alt="Generative AI" />
          <img src="https://img.shields.io/badge/Cloud-AWS-%238a2be2?style=for-the-badge&logo=amazon-aws" alt="AWS" />
        </div>
      </div>
    </div>

    <div style="display:flex;flex-direction:column;align-items:flex-end;gap:12px;">
      <!-- Profile views counter -->
      <div style="display:flex;gap:8px;align-items:center;">
        <img src="https://komarev.com/ghpvc/?username=mahammadaftab&color=00f0ff" alt="Profile views" />
      </div>

      <!-- Dynamic GitHub cards (click to view live) -->
      <div style="display:flex;gap:8px;flex-direction:column;align-items:flex-end;">
        <a class="link" href="https://github-readme-stats.vercel.app/api?username=mahammadaftab&show_icons=true&theme=dark" target="_blank">Live GitHub Stats</a>
        <a class="link" href="https://github-readme-streak-stats.herokuapp.com/?user=mahammadaftab&theme=dark" target="_blank">Streak Stats</a>
        <a class="link" href="https://github-readme-stats.vercel.app/api/top-langs/?username=mahammadaftab&layout=compact&theme=dark" target="_blank">Top Languages</a>
      </div>

      <!-- Social icons -->
      <div style="display:flex;gap:8px;margin-top:6px;">
        <a href="https://github.com/mahammadaftab" target="_blank" title="GitHub"><img src="https://img.shields.io/badge/GitHub-@mahammadaftab-00f0ff?style=for-the-badge&logo=github" alt="GitHub" /></a>
        <a href="https://www.linkedin.com/in/mahammadaftab" target="_blank" title="LinkedIn"><img src="https://img.shields.io/badge/LinkedIn-Connect-8a2be2?style=for-the-badge&logo=linkedin" alt="LinkedIn" /></a>
        <a href="https://twitter.com/mahammadaftab" target="_blank" title="Twitter"><img src="https://img.shields.io/badge/Twitter-@mahammadaftab-00f0ff?style=for-the-badge&logo=twitter" alt="Twitter" /></a>
        <a href="mailto:mahammad@aftab.dev" title="Email"><img src="https://img.shields.io/badge/Email-Contact-ff2dcb?style=for-the-badge&logo=gmail" alt="Email" /></a>
      </div>
    </div>
  </div>

  <div class="divider"></div>

  <!-- =========================
       Main Grid
       ========================= -->
  <div class="grid">

    <!-- LEFT: About, Tech, Projects -->
    <div>

      <!-- About Me -->
      <h2 class="neon">About Me</h2>
      <div class="panel">
        <p style="margin:0;color:#dff9ff;font-size:15px;">
          I'm <strong>Mahammad Aftab</strong>, an AI Engineer and Full Stack Developer building production-grade generative AI systems,
          scalable MERN applications, and secure cloud-native platforms. I design ML pipelines, deploy models to Kubernetes on AWS,
          and integrate blockchain primitives where decentralization adds value.
        </p>

        <div style="display:flex;gap:18px;margin-top:14px;flex-wrap:wrap;">
          <div style="min-width:220px;">
            <div class="muted">Primary Focus</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">Generative AI • LLMs • Full-stack systems</div>
          </div>
          <div style="min-width:220px;">
            <div class="muted">Experience</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">5+ years building ML & web platforms</div>
          </div>
          <div style="min-width:220px;">
            <div class="muted">Open to</div>
            <div style="font-weight:800;color:#e9fbff;margin-top:6px;">Senior roles, AI research engineering, contractor work</div>
          </div>
        </div>

        <div style="margin-top:14px;">
          <div class="muted">Core strengths</div>
          <div class="tech-row" style="margin-top:8px;">
            <div class="chip">MERN</div>
            <div class="chip">Generative AI</div>
            <div class="chip">Python • PyTorch</div>
            <div class="chip">Docker • Kubernetes</div>
            <div class="chip">AWS • Terraform</div>
            <div class="chip">Blockchain</div>
            <div class="chip">CI/CD • Observability</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Tech Stack -->
      <h2 class="neon">Tech Stack</h2>
      <div class="panel">
        <div style="display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap;">
          <div style="flex:1;min-width:260px;">
            <div class="muted">Primary</div>
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
            <div class="muted">Infrastructure</div>
            <div class="tech-row" style="margin-top:8px;">
              <div class="chip">Docker</div>
              <div class="chip">Kubernetes</div>
              <div class="chip">AWS</div>
              <div class="chip">Terraform</div>
              <div class="chip">CI/CD</div>
            </div>
          </div>
        </div>

        <div style="margin-top:12px;">
          <div class="muted">Emerging / Research</div>
          <div class="tech-row" style="margin-top:8px;">
            <div class="chip">LLMs • Fine-tuning</div>
            <div class="chip">Diffusion Models</div>
            <div class="chip">Federated Learning</div>
            <div class="chip">On-chain Model Provenance</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Skills -->
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

        <div style="margin-top:12px;" class="muted">I focus on production-readiness: observability, testing, CI/CD, and secure deployments.</div>
      </div>

      <div style="height:12px"></div>

      <!-- Featured Projects -->
      <h2 class="neon">Featured Projects</h2>
      <div class="projects">
        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:900;font-size:15px;color:#e9fbff;">AstraAI • Generative Platform</div>
              <div class="muted" style="margin-top:6px;">End-to-end generative AI platform: fine-tuning, inference, and deployment on Kubernetes with autoscaling.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">PyTorch • FastAPI • K8s</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/astraai" target="_blank">Repository</a>
            <span class="muted">•</span>
            <a class="link" href="https://astraai.example.com" target="_blank">Live Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:900;font-size:15px;color:#e9fbff;">NeonShop • Scalable MERN E‑commerce</div>
              <div class="muted" style="margin-top:6px;">High-throughput storefront with SSR, microservices, and observability.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">React • Node • MongoDB • Docker</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/neonshop" target="_blank">Repository</a>
            <span class="muted">•</span>
            <a class="link" href="https://neonshop.example.com" target="_blank">Live Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:900;font-size:15px;color:#e9fbff;">ChainGuard • Smart Contract Auditor</div>
              <div class="muted" style="margin-top:6px;">Automated security checks and fuzzing for Solidity contracts with CI integration.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">Solidity • Python • Docker</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/chainguard" target="_blank">Repository</a>
            <span class="muted">•</span>
            <a class="link" href="https://chainguard.example.com" target="_blank">Demo</a>
          </div>
        </div>

        <div class="project-card panel">
          <div style="display:flex;justify-content:space-between;align-items:start;">
            <div>
              <div style="font-weight:900;font-size:15px;color:#e9fbff;">Realtime-ML • Streaming Inference</div>
              <div class="muted" style="margin-top:6px;">Low-latency model serving with autoscaling, A/B experiments, and observability.</div>
            </div>
            <div style="text-align:right;">
              <div class="muted">Tech</div>
              <div style="font-weight:800;color:var(--neon-cyan);margin-top:6px;">Kafka • FastAPI • K8s</div>
            </div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px;">
            <a class="link" href="https://github.com/mahammadaftab/realtime-ml" target="_blank">Repository</a>
            <span class="muted">•</span>
            <a class="link" href="https://realtime-ml.example.com" target="_blank">Demo</a>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Achievements -->
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
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:10px;">
          <div style="display:flex;gap:12px;align-items:flex-start;">
            <div style="width:12px;height:12px;border-radius:999px;background:var(--neon-cyan);margin-top:6px;"></div>
            <div>
              <div style="font-weight:900;color:#e9fbff;">Q3 2026 — Productionize AstraAI</div>
              <div class="muted">Scale inference, add multi-tenant orchestration, enterprise integrations.</div>
            </div>
          </div>

          <div style="display:flex;gap:12px;align-items:flex-start;">
            <div style="width:12px;height:12px;border-radius:999px;background:var(--neon-pink);margin-top:6px;"></div>
            <div>
              <div style="font-weight:900;color:#e9fbff;">Q4 2026 — Decentralized ML Marketplace</div>
              <div class="muted">Integrate blockchain for model provenance and micropayments.</div>
            </div>
          </div>

          <div style="display:flex;gap:12px;align-items:flex-start;">
            <div style="width:12px;height:12px;border-radius:999px;background:var(--neon-purple);margin-top:6px;"></div>
            <div>
              <div style="font-weight:900;color:#e9fbff;">2027 — Research: Federated & Privacy-preserving LLMs</div>
              <div class="muted">Privacy-first model training and deployment strategies.</div>
            </div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Contact / Support -->
      <h2 class="neon">Support • Contact</h2>
      <div class="panel" style="display:flex;gap:12px;flex-wrap:wrap;align-items:center;">
        <div style="flex:1;min-width:220px;">
          <div style="font-weight:900;color:#e9fbff;">Hire • Collaborate • Contract</div>
          <div class="muted" style="margin-top:6px;">Open to senior engineering roles, AI research engineering, and consulting.</div>
        </div>
        <div style="min-width:220px;">
          <div style="font-weight:800;color:var(--neon-cyan);">Email</div>
          <div class="muted" style="margin-top:6px;">mahammad@aftab.dev</div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Quote -->
      <h2 class="neon">Coding Quote</h2>
      <div class="panel quote">
        "Ship small, iterate fast, and let the data decide. Build systems that are observable, testable, and kind to users."
      </div>

    </div>

    <!-- RIGHT: Stats, Trophies, Activity -->
    <div>

      <!-- GitHub Stats -->
      <h2 class="neon">GitHub Stats</h2>
      <div class="panel">
        <div class="stats-grid">
          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.02);">
            <div style="font-weight:900;color:#e9fbff;">Dynamic Stats</div>
            <div class="muted" style="margin-top:8px;">Live, embeddable SVGs (click to open)</div>
            <div style="margin-top:10px;display:flex;flex-direction:column;gap:8px;">
              <a class="link" href="https://github-readme-stats.vercel.app/api?username=mahammadaftab&show_icons=true&theme=dark" target="_blank">View stats card</a>
              <a class="link" href="https://github-readme-streak-stats.herokuapp.com/?user=mahammadaftab&theme=dark" target="_blank">View streak stats</a>
              <a class="link" href="https://github-readme-stats.vercel.app/api/top-langs/?username=mahammadaftab&layout=compact&theme=dark" target="_blank">Top languages</a>
            </div>
          </div>

          <div style="padding:12px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.02);">
            <div style="font-weight:900;color:#e9fbff;">Contribution Graph</div>
            <div class="muted" style="margin-top:8px;">Click to view live contributions</div>
            <div style="margin-top:10px;">
              <a class="link" href="https://github.com/mahammadaftab" target="_blank">Open GitHub profile</a>
            </div>
          </div>
        </div>

        <div style="margin-top:12px;" class="muted">Tip: Add the dynamic SVGs directly into this README using the GitHub Readme Stats endpoints for live visuals.</div>
      </div>

      <div style="height:12px"></div>

      <!-- Trophies & Activity -->
      <h2 class="neon">Trophies • Activity</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:10px;">
          <div style="font-weight:900;color:#e9fbff;">Trophies</div>
          <div class="muted">Open-source contributions, challenge wins, and community recognition.</div>

          <div style="margin-top:8px;display:flex;gap:8px;flex-wrap:wrap;">
            <div class="badge">🏆 Open Source Contributor</div>
            <div class="badge">🏅 HackAI Winner</div>
            <div class="badge">🔒 Security Advocate</div>
            <div class="badge">☁️ Cloud Certified</div>
          </div>

          <div style="margin-top:12px;">
            <div style="font-weight:900;color:#e9fbff;">Activity Graph</div>
            <div class="muted" style="margin-top:6px;">For live activity, view the GitHub profile or embed contribution SVGs.</div>
            <div style="margin-top:8px;">
              <a class="link" href="https://github.com/mahammadaftab" target="_blank">View activity</a>
            </div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- AI / ML / Blockchain / Cloud -->
      <h2 class="neon">AI • ML • Blockchain • Cloud</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:12px;">
          <div>
            <div style="font-weight:900;color:#e9fbff;">Generative AI & ML</div>
            <div class="muted" style="margin-top:6px;">Architected LLM fine-tuning pipelines, built multimodal models, and deployed inference services with autoscaling.</div>
          </div>

          <div>
            <div style="font-weight:900;color:#e9fbff;">Blockchain</div>
            <div class="muted" style="margin-top:6px;">Smart contract development, security audits, and integrating on-chain provenance for ML models and datasets.</div>
          </div>

          <div>
            <div style="font-weight:900;color:#e9fbff;">Cloud & DevOps</div>
            <div class="muted" style="margin-top:6px;">Production deployments on AWS, Kubernetes orchestration, infra-as-code, and observability with Prometheus & Grafana.</div>
          </div>
        </div>
      </div>

      <div style="height:12px"></div>

      <!-- Spotify / Discord / Portfolio -->
      <h2 class="neon">Now Playing • Community • Portfolio</h2>
      <div class="panel">
        <div style="display:flex;flex-direction:column;gap:10px;">
          <div>
            <div style="font-weight:900;color:#e9fbff;">Spotify</div>
            <div class="muted" style="margin-top:6px;">Curated playlists for deep work and ML research.</div>
            <div style="margin-top:8px;"><a class="link" href="https://open.spotify.com/user/yourprofile" target="_blank">Open Spotify</a></div>
          </div>

          <div>
            <div style="font-weight:900;color:#e9fbff;">Discord</div>
            <div class="muted" style="margin-top:6px;">Active in AI & DevOps communities — join the server for discussions.</div>
            <div style="margin-top:8px;"><a class="link" href="https://discord.gg/yourserver" target="_blank">Join Discord</a></div>
          </div>

          <div>
            <div style="font-weight:900;color:#e9fbff;">Portfolio</div>
            <div class="muted" style="margin-top:6px;">Detailed case studies, architecture diagrams, and research notes.</div>
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

  <!-- Footer -->
  <div style="display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap;align-items:center;">
    <div class="muted">© <strong>Mahammad Aftab</strong> • AI Engineer • Full Stack Developer • India</div>
    <div style="display:flex;gap:12px;align-items:center;">
      <a class="link" href="https://github.com/mahammadaftab" target="_blank">GitHub</a>
      <a class="link" href="https://www.linkedin.com/in/mahammadaftab" target="_blank">LinkedIn</a>
      <a class="link" href="mailto:mahammad@aftab.dev">Email</a>
    </div>
  </div>

  <div style="height:12px"></div>

  <!-- Inline dynamic badges -->
  <div style="display:flex;gap:8px;flex-wrap:wrap;align-items:center;">
    <img src="https://img.shields.io/badge/Stack-MERN%20%7C%20Python-00f0ff?style=flat-square&logo=react" alt="Stack" />
    <img src="https://img.shields.io/badge/AI-Generative-ff2dcb?style=flat-square&logo=python" alt="AI" />
    <img src="https://img.shields.io/badge/Cloud-AWS-8a2be2?style=flat-square&logo=amazon-aws" alt="AWS" />
    <img src="https://img.shields.io/badge/Infra-Docker%20%7C%20K8s-00f0ff?style=flat-square&logo=docker" alt="Docker K8s" />
  </div>

</div>

<!-- =========================
     Typing animation script
     (Works on GitHub when JS is allowed in preview; GitHub strips scripts in README,
     but this remains for local preview or other renderers that allow scripts.)
     ========================= -->
<script>
  (function(){
    const phrases = [
      "Designing production-grade AI systems • MERN • Cloud-native",
      "Fine-tuning LLMs • Deploying scalable inference",
      "Building secure, observable, and testable platforms",
      "Integrating blockchain for model provenance"
    ];
    let idx = 0;
    const el = document.getElementById('type-text');
    function typePhrase(phrase, cb){
      el.textContent = '';
      let i=0;
      const t = setInterval(()=>{
        el.textContent += phrase[i++] || '';
        if(i>phrase.length){ clearInterval(t); setTimeout(cb,900); }
      }, 28);
    }
    function loop(){
      typePhrase(phrases[idx%phrases.length], ()=>{ idx++; loop(); });
    }
    if(el){ loop(); }
  })();
</script>

</div>

<!--
  Quick embed examples (copy into README where you want live images):

  GitHub Readme Stats:
  ![Mahammad's GitHub stats](https://github-readme-stats.vercel.app/api?username=mahammadaftab&show_icons=true&theme=dark)

  Streak Stats:
  ![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=mahammadaftab&theme=dark)

  Top Languages:
  ![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=mahammadaftab&layout=compact&theme=dark)

  Contribution Graph (example service):
  ![Contribution Graph](https://activity-graph.herokuapp.com/graph?username=mahammadaftab&theme=react-dark&area=true)

  Profile Views:
  ![Profile Views](https://komarev.com/ghpvc/?username=mahammadaftab&color=00f0ff)

  Notes:
  - Replace example demo links with your real deployments.
  - GitHub strips <script> tags and some inline styles in profile READMEs; the HTML/CSS here is optimized for renderers that allow it and for local preview. For pure GitHub compatibility, embed the dynamic SVG images (GitHub Readme Stats) and keep the HTML minimal.
  - To maximize recruiter impact: include live stats images (above), polished project READMEs, and links to case studies in your portfolio.
-->
