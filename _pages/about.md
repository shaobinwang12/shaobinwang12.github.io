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
    --paper: #fbfaf7;
    --ink: #16181b;
    --body: #3e444a;
    --muted: #7d838a;
    --rule: #e1ddd5;
    --rule-soft: #ece9e2;
    --accent: #8a3324;
    --serif: Georgia, "Times New Roman", "Songti SC", "SimSun", serif;
  }

  html,
  body {
    background: var(--paper);
  }

  /* ---------- 顶栏 ---------- */
  .masthead {
    border-bottom: 1px solid var(--rule);
    background: var(--paper);
  }

  .masthead__inner-wrap {
    padding: 0.9em 1em;
  }

  .masthead .visible-links a {
    margin: 0 0.95rem;
    padding: 0.4rem 0;
    color: var(--muted);
    font-size: 0.74rem;
    font-weight: 400;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .masthead .visible-links a::before {
    bottom: -0.5em;
    height: 1.5px;
    background: var(--accent);
  }

  .masthead .visible-links a:hover {
    color: var(--ink);
  }

  .masthead .greedy-nav button {
    background: var(--ink);
  }

  .masthead .hidden-links {
    border-color: var(--rule);
    background: var(--paper);
    box-shadow: 0 8px 20px rgba(22, 24, 27, 0.08);
  }

  .masthead .hidden-links a {
    font-size: 0.74rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  /* ---------- 侧栏 ---------- */
  .sidebar .author__content {
    display: none;
  }

  .sidebar .author__avatar img {
    padding: 0;
    border: 1px solid var(--rule);
    border-radius: 2px;
  }

  .sidebar .author__urls {
    margin-top: 2em;
  }

  .sidebar .author__label {
    margin: 0 0 0.9em;
    color: var(--muted);
    font-size: 0.68rem;
    letter-spacing: 0.18em;
    text-transform: uppercase;
  }

  .sidebar .author__urls a {
    font-size: 0.85rem;
    text-decoration: none;
  }

  .sidebar .author__urls a:hover {
    color: var(--accent);
    text-decoration: none;
  }

  /* ---------- 正文 ---------- */
  .home p {
    margin: 0 0 0.8em;
    color: var(--body);
    font-size: 1rem;
    line-height: 1.78;
  }

  .page__content .home a {
    color: var(--ink);
    text-decoration: none;
    border-bottom: 1px solid rgba(22, 24, 27, 0.3);
    transition: color 0.15s ease, border-color 0.15s ease;
  }

  .page__content .home a:hover {
    color: var(--accent);
    border-bottom-color: var(--accent);
  }

  /* 头部 */
  .hero {
    padding-top: 0.2em;
    scroll-margin-top: 5.5em;
  }

  .hero::before {
    display: block;
    width: 2.6em;
    height: 2px;
    margin-bottom: 1.5em;
    background: var(--ink);
    content: "";
  }

  .home .hero .kicker {
    margin: 0 0 1.1em;
    color: var(--accent);
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 0.2em;
    text-transform: uppercase;
  }

  .page__content .home .display {
    margin: 0;
    padding: 0;
    border: 0;
    color: var(--ink);
    font-family: var(--serif);
    font-size: 2.6rem;
    font-weight: 400;
    letter-spacing: -0.015em;
    line-height: 1.06;
  }

  .home .hero .sub {
    margin: 0.95em 0 0;
    color: var(--muted);
    font-size: 0.87rem;
    letter-spacing: 0.01em;
  }

  .prose {
    max-width: 44em;
    margin-top: 1.9em;
  }

  .home .prose p {
    font-size: 1.01rem;
  }

  /* 小节标题 */
  .home .sec {
    display: flex;
    align-items: baseline;
    gap: 0.9em;
    margin: 3.6em 0 1.7em;
    padding: 0;
    border: 0;
    scroll-margin-top: 5.5em;
  }

  .home .sec .num {
    color: var(--accent);
    font-family: var(--serif);
    font-size: 1rem;
    font-style: italic;
    line-height: 1;
  }

  .home .sec .label {
    color: var(--ink);
    font-size: 0.78rem;
    font-weight: 600;
    letter-spacing: 0.18em;
    white-space: nowrap;
    text-transform: uppercase;
  }

  .home .sec::after {
    flex: 1 1 auto;
    border-top: 1px solid var(--rule);
    content: "";
  }

  .home .legend {
    margin: -0.6em 0 1.7em;
    color: var(--muted);
    font-size: 0.78rem;
    line-height: 1.6;
  }

  /* 论文 */
  .pubs {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .pubs > li {
    margin-bottom: 1.5em;
    padding-bottom: 1.5em;
    border-bottom: 1px solid var(--rule-soft);
  }

  .pubs > li:last-child {
    margin-bottom: 0;
    padding-bottom: 0;
    border-bottom: 0;
  }

  .home .pubs .meta {
    margin: 0 0 0.45em;
    color: var(--muted);
    font-size: 0.79rem;
    line-height: 1.6;
  }

  .pubs .meta .venue {
    color: #4d555b;
    font-weight: 600;
  }

  .page__content .home .pubs .pt {
    margin: 0 0 0.4em;
    padding: 0;
    border: 0;
    color: var(--ink);
    font-family: var(--serif);
    font-size: 1.1rem;
    font-weight: 400;
    line-height: 1.45;
  }

  .home .pubs .authors {
    margin: 0;
    color: #5f676d;
    font-size: 0.86rem;
    line-height: 1.65;
  }

  .home .pubs .note {
    margin: 0.45em 0 0;
    color: var(--muted);
    font-size: 0.8rem;
  }

  .home .pubs .award {
    color: var(--accent);
    letter-spacing: 0.02em;
  }

  /* 分栏条目 */
  .entry {
    display: grid;
    grid-template-columns: 8.4em 1fr;
    column-gap: 1.4em;
    margin-bottom: 1.5em;
    padding-bottom: 1.5em;
    border-bottom: 1px solid var(--rule-soft);
  }

  .entry:last-of-type {
    margin-bottom: 0;
    padding-bottom: 0;
    border-bottom: 0;
  }

  .entry .when {
    padding-top: 0.2em;
    color: var(--muted);
    font-size: 0.72rem;
    font-variant-numeric: tabular-nums;
    letter-spacing: 0.1em;
    line-height: 1.75;
    text-transform: uppercase;
  }

  .entry .org {
    display: flex;
    align-items: center;
    gap: 0.6em;
    color: var(--ink);
    font-family: var(--serif);
    font-size: 1.08rem;
    line-height: 1.4;
  }

  .entry .org img {
    flex: 0 0 auto;
    width: 32px;
    height: 32px;
    object-fit: contain;
  }

  .home .entry .role {
    margin: 0.3em 0 0;
    color: var(--body);
    font-size: 0.89rem;
  }

  /* 荣誉 */
  .awards {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .awards li {
    display: grid;
    grid-template-columns: 8.4em 1fr;
    column-gap: 1.4em;
    margin-bottom: 0.9em;
    padding-bottom: 0.9em;
    border-bottom: 1px solid var(--rule-soft);
    color: var(--body);
    font-size: 0.94rem;
    line-height: 1.65;
  }

  .awards li:last-child {
    margin-bottom: 0;
    padding-bottom: 0;
    border-bottom: 0;
  }

  .awards .yr {
    padding-top: 0.15em;
    color: var(--muted);
    font-size: 0.72rem;
    font-variant-numeric: tabular-nums;
    letter-spacing: 0.1em;
  }

  /* 页脚 */
  .foot {
    margin-top: 4.5em;
    padding-top: 1.3em;
    border-top: 1px solid var(--rule);
  }

  .home .foot p {
    margin: 0;
    color: var(--muted);
    font-size: 0.78rem;
    letter-spacing: 0.02em;
  }

  @media (max-width: 40em) {
    .page__content .home .display {
      font-size: 2.05rem;
    }

    .entry,
    .awards li {
      grid-template-columns: 1fr;
      row-gap: 0.35em;
    }

    .entry .when,
    .awards .yr {
      padding-top: 0;
    }
  }
</style>

<div class="home">
  <header class="hero" id="about-me">
    <p class="kicker">Network systems &amp; social computing</p>
    <h1 class="display">Shaobin Wang</h1>
    <p class="sub">M.S. in Computer Science · Fudan University · Shanghai, China</p>
  </header>

  <div class="prose">
    <p>I received my master's degree from <a href="https://www.fudan.edu.cn/en/">Fudan University</a> in 2026, where I worked with Prof. <a href="https://chenyang03.wordpress.com/">Yang Chen</a> at the School of Computer Science. Before that I studied Internet of Things Engineering at <a href="https://english.zzu.edu.cn/">Zhengzhou University</a> and graduated in 2023.</p>
    <p>Most of my current work involves collecting and preprocessing snapshots of decentralized social platforms such as Mastodon, understanding how people link their identities across them, and figuring out whether deepfake text detectors still hold up once they leave the lab. On the side I work on network systems, most recently on energy-aware collaborative perception in vehicular networks.</p>
  </div>

  <h2 class="sec" id="publications"><span class="num">01</span><span class="label">Publications</span></h2>

  <p class="legend"><sup>#</sup> equal contribution &nbsp;·&nbsp; <sup>*</sup> corresponding author</p>

  <ol class="pubs">
    <li>
      <p class="meta"><span class="venue">48th IEEE Symposium on Security and Privacy (S&amp;P '27)</span> · to appear</p>
      <h3 class="pt">When Deepfake Text Detectors Leave the Lab: Robust Detection Under Unsupervised Transductive Deployment Across Online Social Networks</h3>
      <p class="authors">Shaojie Min, Jiayin Xue, <strong>Shaobin Wang</strong>, Yaxiao Luo, Roy Ka-Wei Lee, Yupeng Li, Xinlei He, Qingyuan Gong<sup>*</sup>, Yang Chen<sup>*</sup></p>
      <p class="note">Artifact badges: Available, Functional, Reproduced</p>
    </li>
    <li>
      <p class="meta"><span class="venue">IEEE Communications Magazine</span> · to appear</p>
      <h3 class="pt">Energy-Aware Collaborative Perception in HetVNETs: Balancing Accuracy and Sustainability</h3>
      <p class="authors">Mengying Zhou, <strong>Shaobin Wang</strong>, Qiang Duan, Aaron Yi Ding, Xin Wang<sup>*</sup>, Yang Chen<sup>*</sup></p>
    </li>
    <li>
      <p class="meta"><span class="venue">10th China National Conference on Big Data and Social Computing (BDSC '25)</span> · Kunming, China · Aug 2025</p>
      <h3 class="pt">Understanding Cross-Platform Links in User Profiles: A Data-Driven Analysis on Mastodon</h3>
      <p class="authors">Shaojie Min, <strong>Shaobin Wang</strong>, Yaxiao Luo, Qingyuan Gong<sup>*</sup>, Yang Chen<sup>*</sup></p>
      <p class="note"><span class="award">Most Welcomed Paper Award</span></p>
    </li>
    <li>
      <p class="meta"><span class="venue">The Web Conference (WWW '25)</span> · Resource Track · Sydney, Australia · Apr&ndash;May 2025</p>
      <h3 class="pt">FediLive: A Framework for Collecting and Preprocessing Snapshots of Decentralized Online Social Networks</h3>
      <p class="authors">Shaojie Min<sup>#</sup>, <strong>Shaobin Wang</strong><sup>#</sup>, Yaxiao Luo, Min Gao, Qingyuan Gong<sup>*</sup>, Yu Xiao, Yang Chen<sup>*</sup></p>
    </li>
    <li>
      <p class="meta"><span class="venue">Turing Award Celebration Conference (TURC '23)</span> · Poster · Wuhan, China · Jul 2023</p>
      <h3 class="pt">Towards the Predictability of IPFS Nodes' Session Time Using Machine Learning</h3>
      <p class="authors">Dan Zhuo, Jiawei Tang, Yang Chen<sup>*</sup>, <strong>Shaobin Wang</strong>, Xin Wang</p>
      <p class="note"><a href="https://dl.acm.org/doi/10.1145/3603165.3607397" target="_blank" rel="noopener">Paper</a></p>
    </li>
  </ol>

  <h2 class="sec" id="internship"><span class="num">02</span><span class="label">Internship Experience</span></h2>

  <div class="entry">
    <div class="when">May 2025 &ndash;<br>Aug 2025</div>
    <div>
      <div class="org">Meituan</div>
      <p class="role">Software Engineering Intern</p>
      <!-- 可在此补一句实习期间的团队与工作方向 -->
    </div>
  </div>

  <h2 class="sec" id="education"><span class="num">03</span><span class="label">Education</span></h2>

  <div class="entry">
    <div class="when">Sep 2023 &ndash;<br>Jun 2026</div>
    <div>
      <div class="org"><img src="{{ '/images/Fudan_University_Logo.svg.png' | relative_url }}" alt="Fudan University">Fudan University</div>
      <p class="role">M.S. in Computer Science, School of Computer Science</p>
    </div>
  </div>

  <div class="entry">
    <div class="when">Sep 2019 &ndash;<br>Jun 2023</div>
    <div>
      <div class="org"><img src="{{ '/images/zzulogo.png' | relative_url }}" alt="Zhengzhou University">Zhengzhou University</div>
      <p class="role">B.Eng. in Internet of Things Engineering, School of Cyber Science and Engineering</p>
    </div>
  </div>

  <h2 class="sec" id="honors"><span class="num">04</span><span class="label">Honors &amp; Awards</span></h2>

  <ul class="awards">
    <li><span class="yr">2026</span><span>Outstanding Graduates of Fudan University</span></li>
    <li><span class="yr">2020</span><span>Outstanding Cadre of the Communist Youth League, Zhengzhou University</span></li>
  </ul>

  <footer class="foot">
    <p>Last updated November 2026 · <a href="mailto:sbwang23@m.fudan.edu.cn">sbwang23@m.fudan.edu.cn</a></p>
  </footer>
</div>
