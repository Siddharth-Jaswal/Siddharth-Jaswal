<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Siddharth Jaswal — GitHub Bio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#94a3b8;
      --accent-1:#7c3aed;
      --accent-2:#06b6d4;
      --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
      --max-width:1000px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      background: radial-gradient(1200px 600px at 10% 10%, rgba(124,58,237,0.12), transparent 8%),
                  radial-gradient(800px 400px at 90% 90%, rgba(6,182,212,0.06), transparent 8%),
                  var(--bg);
      color:#e6eef8;
      font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:48px 20px;
    }

    .card{
      width:100%;
      max-width:var(--max-width);
      background:linear-gradient(180deg,var(--card), rgba(255,255,255,0.01));
      border-radius:18px;
      padding:28px;
      box-shadow: 0 10px 30px rgba(2,6,23,0.6), inset 0 1px 0 rgba(255,255,255,0.02);
      border: 1px solid rgba(255,255,255,0.03);
      display:grid;
      grid-template-columns: 260px 1fr;
      gap:28px;
      align-items:start;
    }

    /* Sidebar */
    .sidebar{
      padding:18px;
      border-radius:12px;
      background: linear-gradient(180deg,var(--glass),transparent);
      backdrop-filter: blur(6px) saturate(120%);
      min-height:220px;
      display:flex;
      flex-direction:column;
      gap:14px;
    }

    .avatar{
      width:100%;
      aspect-ratio: 1/1;
      border-radius:12px;
      background: linear-gradient(135deg,var(--accent-1),var(--accent-2));
      display:flex;align-items:center;justify-content:center;
      font-weight:800;font-size:36px;color:rgba(255,255,255,0.95);
      box-shadow: 0 6px 18px rgba(12,18,40,0.6);
    }

    .name{font-size:20px;font-weight:700;margin:0}
    .role{color:var(--muted);font-size:13px;margin-top:4px}

    .meta{display:flex;flex-direction:column;gap:6px;margin-top:8px}
    .meta .line{display:flex;justify-content:space-between;color:var(--muted);font-size:13px}

    .badges{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
    .badge{padding:6px 10px;border-radius:999px;font-size:12px;background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.02)}

    /* main */
    .main{
      padding:18px;
      border-radius:12px;
      background: linear-gradient(180deg,var(--glass-2),transparent);
      backdrop-filter: blur(6px) saturate(120%);
      min-height:220px;
      display:flex;flex-direction:column;gap:16px;
    }

    .headline{display:flex;align-items:center;gap:14px}
    .headline h1{margin:0;font-size:18px}
    .headline p{margin:0;color:var(--muted);font-size:13px}

    .summary{
      font-size:14px;line-height:1.5;color:#dbeafe;padding:12px;border-radius:10px;background:linear-gradient(90deg, rgba(124,58,237,0.04), rgba(6,182,212,0.02));
      border:1px solid rgba(255,255,255,0.02);
    }

    .skills-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:10px}
    .skill{
      padding:10px;border-radius:10px;background:rgba(255,255,255,0.02);font-size:13px;display:flex;align-items:center;gap:8px;
      border:1px solid rgba(255,255,255,0.02);
    }

    .skill .dot{width:10px;height:10px;border-radius:50%;background:linear-gradient(135deg,var(--accent-1),var(--accent-2))}

    .pro-level{margin-left:auto;font-size:12px;color:var(--muted)}

    pre{background:rgba(2,6,23,0.6);padding:12px;border-radius:10px;font-size:12px;color:#d1f0ff;overflow:auto}

    .footer{display:flex;gap:12px;align-items:center}
    .btn{
      padding:10px 14px;border-radius:10px;font-weight:600;background:linear-gradient(90deg,var(--accent-1),var(--accent-2));
      border:none;color:white;cursor:pointer;display:inline-flex;align-items:center;gap:10px;text-decoration:none
    }
    .ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}

    /* small screens */
    @media (max-width:880px){
      .card{grid-template-columns:1fr;}
      .skills-grid{grid-template-columns:repeat(1,1fr)}
    }

    /* subtle animation */
    @keyframes floaty{0%{transform:translateY(0)}50%{transform:translateY(-6px)}100%{transform:translateY(0)}}
    .avatar{animation:floaty 6s ease-in-out infinite}

    /* little code-like tags */
    .tagline{font-family:monospace;background:rgba(255,255,255,0.02);border-radius:8px;padding:8px;font-size:12px;color:#a5f3fc}

    /* social icons */
    .socials{display:flex;gap:8px}
    .socials a{display:inline-flex;align-items:center;justify-content:center;width:38px;height:38px;border-radius:8px;background:rgba(255,255,255,0.02);text-decoration:none;color:inherit;border:1px solid rgba(255,255,255,0.02)}

  </style>
</head>
<body>
  <div class="card" role="region" aria-label="GitHub bio card">
    <aside class="sidebar">
      <div class="avatar">SJ</div>
      <div>
        <p class="name">Siddharth Jaswal</p>
        <p class="role">Coder • Web Dev • ML Enthusiast • Problem Solver</p>
      </div>

      <div class="meta">
        <div class="line"><span>Location</span><span>India</span></div>
        <div class="line"><span>Contact</span><span>github.com/siddharth</span></div>
        <div class="line"><span>Focus</span><span>Full-stack & ML</span></div>
      </div>

      <div class="badges">
        <div class="badge">Algorithms</div>
        <div class="badge">C++</div>
        <div class="badge">Python</div>
        <div class="badge">JavaScript</div>
        <div class="badge">MongoDB</div>
        <div class="badge">Express</div>
        <div class="badge">Bootstrap</div>
        <div class="badge">Pandas</div>
        <div class="badge">NumPy</div>
      </div>

      <div style="margin-top:auto;display:flex;flex-direction:column;gap:10px">
        <div class="socials">
          <a href="#" title="GitHub"> <!-- github svg -->
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 .5C5.648.5.5 5.648.5 12c0 5.086 3.292 9.402 7.865 10.93.575.106.785-.25.785-.556 0-.274-.01-1-.016-1.96-3.2.696-3.876-1.544-3.876-1.544-.524-1.33-1.28-1.684-1.28-1.684-1.047-.716.08-.702.08-.702 1.158.082 1.767 1.19 1.767 1.19 1.03 1.764 2.703 1.255 3.36.96.104-.747.403-1.255.732-1.544-2.554-.29-5.24-1.277-5.24-5.68 0-1.255.448-2.28 1.182-3.084-.118-.29-.512-1.46.112-3.043 0 0 .963-.308 3.156 1.177A10.94 10.94 0 0112 6.844c.976.004 1.96.132 2.876.387 2.192-1.485 3.153-1.177 3.153-1.177.627 1.584.233 2.753.115 3.043.736.804 1.18 1.83 1.18 3.084 0 4.414-2.692 5.386-5.257 5.674.414.356.783 1.058.783 2.134 0 1.54-.014 2.78-.014 3.16 0 .31.207.67.79.556C20.21 21.397 23.5 17.083 23.5 12 23.5 5.648 18.352.5 12 .5z" fill="currentColor"/></svg>
          </a>
          <a href="#" title="LinkedIn"> <!-- linkedin svg -->
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.88 6 2.5 6S0 4.88 0 3.5 1.1 1 2.5 1 4.98 2.12 4.98 3.5zM.24 8h4.5V24h-4.5zM8.5 8h4.32v2.16h.06c.6-1.14 2.06-2.34 4.24-2.34C22.66 7.82 24 9.98 24 14.24V24h-4.5v-8.06c0-1.92-.04-4.39-2.68-4.39-2.68 0-3.09 2.1-3.09 4.26V24H8.5z" fill="currentColor"/></svg>
          </a>
        </div>
        <div style="display:flex;gap:8px">
          <a class="btn" href="#">Follow</a>
          <a class="btn ghost" href="#">Contact</a>
        </div>
      </div>
    </aside>

    <main class="main">
      <div class="headline">
        <div style="flex:1">
          <h1>Hi — I'm Siddharth. I write scalable web apps & train ML models.</h1>
          <p style="margin-top:6px;color:var(--muted)">A curious coder who loves algorithms, data, and clean UIs.</p>
        </div>
        <div class="tagline">&lt;Coder • Problem Solver • Engineer /&gt;</div>
      </div>

      <div class="summary">
        I build full-stack web applications with a focus on backend APIs (MongoDB + Express) and polished frontends using Bootstrap and modern JavaScript. On the other side, I prototype ML models using Python, NumPy, and Pandas — then productionize them into APIs. I enjoy algorithmic challenges and competitive programming: efficient, correct, and clean solutions are my jam.
      </div>

      <section>
        <h3 style="margin:0 0 8px 0">What I do</h3>
        <div class="skills-grid">
          <div class="skill"><div class="dot"></div><div>Algorithms & Problem Solving</div><div class="pro-level">Expert</div></div>
          <div class="skill"><div class="dot"></div><div>Web Dev — JS, Express, MongoDB</div><div class="pro-level">Advanced</div></div>
          <div class="skill"><div class="dot"></div><div>Languages — C++, Python, JS</div><div class="pro-level">Advanced</div></div>
          <div class="skill"><div class="dot"></div><div>Data / ML — NumPy, Pandas, prototyping</div><div class="pro-level">Intermediate</div></div>
        </div>
      </section>

      <section aria-label="sample-snippet">
        <h3 style="margin:10px 0 8px 0">Code snapshots</h3>
        <pre><code>// algorithms — clean & concise
int binary_search(vector<int>&A, int x){
  int l=0,r=A.size()-1;
  while(l<=r){
    int m=(l+r)/2;
    if(A[m]==x) return m;
    if(A[m]<x) l=m+1; else r=m-1;
  }
  return -1;
}

# python — data prototyping
import pandas as pd
import numpy as np

# quick model pipeline (toy)
</code></pre>
      </section>

      <div class="footer">
        <a class="btn" href="#">⭐ Star my projects</a>
        <a class="btn ghost" href="#">📄 Resume</a>
      </div>

    </main>
  </div>

</body>
</html>
