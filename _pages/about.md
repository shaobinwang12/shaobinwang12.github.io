---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<style>
  :root {
    --primary: #2e7d32;
    --primary-light: #81c784;
    --accent: #ff6b6b;
    --bg-card: #fafafa;
    --border: #e5e7eb;
    --text-muted: #6b7280;
  }
  .centered {
    text-align: center;
    margin-bottom: 1rem;
  }
  .centered h2 {
    font-size: 2rem;
    font-weight: 700;
    margin: 0;
    background: linear-gradient(to right, #81c784, #ff6b6b);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .hero-subtitle {
    color: var(--text-muted);
    font-size: 1rem;
    margin-top: 0.25rem;
  }
  .intro {
    margin-top: 1.5rem;
    line-height: 1.8;
  }
  .section-title {
    font-size: 1.4rem;
    margin-top: 2.2rem;
    padding-bottom: 0.4rem;
    border-bottom: 2px solid var(--primary-light);
  }
  .paper-card {
    display: block;
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-left: 4px solid var(--primary-light);
    border-radius: 8px;
    padding: 14px 18px;
    margin: 14px 0;
    transition: transform .15s ease, box-shadow .15s ease;
  }
  .paper-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  }
  .paper-title {
    font-weight: 700;
    font-size: 1.02rem;
    color: #111;
    margin-bottom: .35rem;
    line-height: 1.4;
  }
  .badge-row {
    display: block;
    margin: 8px 0 6px;
  }
  .badge {
    display: inline-flex;
    align-items: center;
    font-size: .75rem;
    line-height: 1.6;
    padding: 3px 10px;
    border-radius: 999px;
    background: #fff3e0;
    color: #b26a00;
    border: 1px solid #ffcc80;
    white-space: normal;
    word-break: break-word;
    max-width: 100%;
    box-sizing: border-box;
  }
  .paper-authors {
    color: #374151;
    font-size: .92rem;
    margin-bottom: .3rem;
  }
  .paper-venue {
    font-style: italic;
    color: var(--text-muted);
    font-size: .9rem;
  }
  .tag {
    display: inline-flex;
    align-items: center;
    font-size: .72rem;
    line-height: 1.6;
    padding: 2px 9px;
    border-radius: 999px;
    background: #e0f2f1;
    color: #00695c;
    margin-bottom: 6px;
  }
  .exp-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-left: 4px solid #ff8a65;
    border-radius: 8px;
    padding: 14px 18px;
    margin: 14px 0;
  }
  .exp-header {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    gap: 8px;
    margin-bottom: .5rem;
  }
  .exp-company {
    font-weight: 700;
    font-size: 1.05rem;
    color: #111;
  }
  .exp-role {
    color: #374151;
    font-size: .95rem;
  }
  .exp-meta {
    color: var(--text-muted);
    font-size: .88rem;
    white-space: nowrap;
  }
  .edu-card {
    display: flex;
    align-items: center;
    gap: 14px;
    margin: 14px 0;
    padding: 14px 18px;
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 8px;
  }
  .edu-card img {
    width: 72px;
    height: 72px;
    object-fit: contain;
    flex-shrink: 0;
  }
  .edu-card blockquote {
    border-left: 3px solid var(--primary-light);
    padding-left: 12px;
    margin: 0;
    color: #374151;
    line-height: 1.5;
  }
  .edu-card blockquote strong {
    color: #111;
  }
  .honor-list {
    padding-left: 1.2rem;
    line-height: 1.9;
  }
  .honor-list li {
    margin-bottom: 4px;
  }
  a { color: var(--primary); }
</style>

<div class="centered">
  <h2>Hi, I am Shaobin</h2>
  <div class="hero-subtitle">M.S. in Computer Science · Fudan University</div>
</div>

I received my master's degree from [Fudan University](https://www.fudan.edu.cn/en/) in 2026, where I was advised by Professor [Yang Chen](https://chenyang03.wordpress.com/). Prior to that, I earned my Bachelor's degree from the School of Cyber Science and Engineering at [Zhengzhou University](https://english.zzu.edu.cn/) in 2023. During my graduate studies at the School of Computer Science at Fudan University, I focused my research on network systems and social networks.
{: .intro }

# 📄 Publications

<div class="paper-card">
  <div class="paper-title">When Deepfake Text Detectors Leave the Lab: Robust Detection Under Unsupervised Transductive Deployment Across Online Social Networks</div>
  <div class="badge-row">
    <span class="badge">🎖️ Artifact Badges: Available, Functional, Reproduced</span>
  </div>
  <div class="paper-authors">Shaojie Min, Jiayin Xue, <strong>Shaobin Wang</strong>, Yaxiao Luo, Roy Ka-Wei Lee, Yupeng Li, Xinlei He, Qingyuan Gong*, Yang Chen*</div>
  <div class="paper-venue">To appear: 48th IEEE Symposium on Security and Privacy (S&amp;P'27)</div>
</div>

<div class="paper-card">
  <div class="paper-title">Energy-Aware Collaborative Perception in HetVNETs: Balancing Accuracy and Sustainability</div>
  <div class="paper-authors">Mengying Zhou, <strong>Shaobin Wang</strong>, Qiang Duan, Aaron Yi Ding, Xin Wang*, Yang Chen*</div>
  <div class="paper-venue">To appear: IEEE Communications Magazine</div>
</div>

<div class="paper-card">
  <div class="paper-title">Understanding Cross-Platform Links in User Profiles: A Data-Driven Analysis on Mastodon</div>
  <div class="tag">🏅 Most Welcomed Paper Award</div>
  <div class="paper-authors">Shaojie Min, <strong>Shaobin Wang</strong>, Yaxiao Luo, Qingyuan Gong*, Yang Chen*</div>
  <div class="paper-venue">Proc. of the 10th China National Conference on Big Data and Social Computing (BDSC'25), Kunming, China, Aug. 2025</div>
</div>

<div class="paper-card">
  <div class="paper-title">FediLive: A Framework for Collecting and Preprocessing Snapshots of Decentralized Online Social Networks</div>
  <div class="paper-authors">Shaojie Min<sup>#</sup>, <strong>Shaobin Wang</strong><sup>#</sup>, Yaxiao Luo, Min Gao, Qingyuan Gong*, Yu Xiao, Yang Chen*</div>
  <div class="paper-venue">Proc. of the Web Conference (WWW'25), Resource Track, Sydney, Australia, Apr.–May 2025</div>
</div>

<div class="paper-card">
  <div class="paper-title">Towards the Predictability of IPFS Nodes' Session Time Using Machine Learning</div>
  <div class="paper-authors">Dan Zhuo, Jiawei Tang, Yang Chen*, <strong>Shaobin Wang</strong>, Xin Wang</div>
  <div class="paper-venue">Proc. of Turing Award Celebration Conference (TURC'23), Poster, Wuhan, China, July 2023</div>
  <div class="paper-venue">[<a href="https://dl.acm.org/doi/10.1145/3603165.3607397" target="_blank">Detail</a>]</div>
</div>

---

# 💼 Internship Experience

<div class="exp-card">
  <div class="exp-header">
    <div>
      <span class="exp-company">Meituan</span>
      <span class="exp-role">— Backend Development Engineer Intern</span>
    </div>
    <span class="exp-meta">May 2025 – Aug. 2025</span>
  </div>
  <ul>
    <li>Participated in the design and development of backend services, writing maintainable and tested code in a large-scale distributed system.</li>
    <li>Collaborated with cross-functional teams to deliver features end-to-end, from requirement analysis and API design to online deployment.</li>
    <li>Optimized service performance and reliability, including database query tuning and cache usage.</li>
  </ul>
  <p><strong>Tech Stack:</strong> Java / Go, Spring Boot, MySQL, Redis, Kafka, Git</p>
</div>

---

# 🎓 Education

<div class="edu-card">
  <img src="../images/Fudan_University_Logo.svg.png" alt="Fudan University">
  <blockquote>
    <strong>Fudan University</strong><br>
    M.S. in Computer Science, School of Computer Science<br>
    Sep. 2023 – Jun. 2026
  </blockquote>
</div>

<div class="edu-card">
  <img src="../images/zzulogo.png" alt="Zhengzhou University">
  <blockquote>
    <strong>Zhengzhou University</strong><br>
    B.Eng. in Internet of Things Engineering, School of Cyber Science and Engineering<br>
    Sep. 2019 – Jun. 2023
  </blockquote>
</div>

---

# 🏆 Honors and Awards

<ul class="honor-list">
  <li>Outstanding Graduates of Fudan University, Fudan University, 2026</li>
  <li>Outstanding Cadre of the Communist Youth League, Zhengzhou University, 2020</li>
</ul>
