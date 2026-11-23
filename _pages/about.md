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
  .page__content .home {
    --ink: #1b1f23;
    --text: #3f464c;
    --muted: #70777d;
    --rule: #e6e3de;
    --accent: #1f4e79;
    --award: #9a5b21;
  }

  .page__content .home p {
    margin-bottom: 0.8em;
    color: var(--text);
    line-height: 1.8;
  }

  .page__content .home a {
    color: var(--accent);
    text-decoration: none;
    border-bottom: 1px solid rgba(31, 78, 121, 0.25);
    transition: border-color 0.15s ease;
  }

  .page__content .home a:hover {
    border-bottom-color: var(--accent);
  }

  /* 简介 */
  .home-intro {
    max-width: 46em;
    scroll-margin-top: 5em;
  }

  .home-intro p {
    font-size: 1.02rem;
  }

  /* 小节标题 */
  .home > h1.sec:first-child {
    margin-top: 0.6em;
  }

  .page__content h1.sec {
    margin: 3em 0 1.2em;
    padding: 0 0 0.55em;
    border-bottom: 1px solid var(--rule);
    color: var(--ink);
    font-size: 0.84rem;
    font-weight: 600;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    scroll-margin-top: 5em;
  }

  .page__content .home p.footnote {
    margin: -0.5em 0 1.6em;
    color: var(--muted);
    font-size: 0.82rem;
    line-height: 1.6;
  }

  /* 论文列表 */
  .pubs {
    counter-reset: pub;
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .pubs > li {
    position: relative;
    margin-bottom: 1.6em;
    padding-left: 2.1em;
  }

  .pubs > li::before {
    position: absolute;
    left: 0;
    top: 0.1em;
    content: counter(pub) ".";
    counter-increment: pub;
    color: #b3b8bd;
    font-size: 0.85em;
    font-variant-numeric: tabular-nums;
  }

  .pubs .t {
    display: block;
    margin-bottom: 0.3em;
    color: var(--ink);
    font-size: 1rem;
    font-weight: 600;
    line-height: 1.5;
  }

  .pubs .a {
    display: block;
    margin-bottom: 0.15em;
    color: #5e666c;
    font-size: 0.9rem;
    line-height: 1.65;
  }

  .pubs .a strong {
    color: var(--ink);
    font-weight: 600;
  }

  .pubs .a sup {
    color: var(--muted);
  }

  .pubs .v {
    display: block;
    color: var(--muted);
    font-size: 0.88rem;
    line-height: 1.6;
  }

  .pubs .n {
    display: block;
    margin-top: 0.2em;
    color: var(--muted);
    font-size: 0.84rem;
    line-height: 1.6;
  }

  .award {
    color: var(--award);
    letter-spacing: 0.03em;
  }

  /* 经历条目 */
  .entry {
    display: grid;
    grid-template-columns: 8.6em 1fr;
    column-gap: 1.2em;
    margin-bottom: 1.6em;
  }

  .entry .when {
    color: var(--muted);
    font-size: 0.82rem;
    line-height: 1.9;
    white-space: nowrap;
    font-variant-numeric: tabular-nums;
  }

  .entry .head {
    display: flex;
    align-items: center;
    gap: 0.55em;
    color: var(--ink);
    font-size: 1rem;
    font-weight: 600;
    line-height: 1.6;
  }

  .entry .head img {
    flex: 0 0 auto;
    width: 24px;
    height: 24px;
    object-fit: contain;
  }

  .entry .sub {
    color: var(--text);
    font-size: 0.92rem;
    line-height: 1.65;
  }

  /* 荣誉 */
  .awards {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .awards li {
    display: grid;
    grid-template-columns: 3.4em 1fr;
    column-gap: 1.2em;
    margin-bottom: 0.5em;
    color: var(--text);
    font-size: 0.95rem;
    line-height: 1.7;
  }

  .awards .yr {
    color: var(--muted);
    font-size: 0.84rem;
    font-variant-numeric: tabular-nums;
  }

  .page__content .home p.updated {
    margin-top: 3em;
    color: #90979d;
    font-size: 0.8rem;
  }

  @media (max-width: 40em) {
    .entry {
      grid-template-columns: 1fr;
      row-gap: 0.15em;
    }

    .entry .when {
      line-height: 1.6;
    }
  }
</style>

<div class="home">
  <h1 class="sec" id="about-me">About Me</h1>
  <div class="home-intro">
    <p>I received my master's degree from <a href="https://www.fudan.edu.cn/en/">Fudan University</a> in 2026, where I worked with Prof. <a href="https://chenyang03.wordpress.com/">Yang Chen</a> at the School of Computer Science. Before that I studied Internet of Things Engineering at <a href="https://english.zzu.edu.cn/">Zhengzhou University</a> and graduated in 2023.</p>
    <p>Most of my current work involves collecting and preprocessing snapshots of decentralized social platforms such as Mastodon, understanding how people link their identities across them, and figuring out whether deepfake text detectors still hold up once they leave the lab. On the side I work on network systems, most recently on energy-aware collaborative perception in vehicular networks.</p>
  </div>

  <h1 class="sec" id="publications">Publications</h1>
  <p class="footnote"><sup>#</sup> equal contribution &nbsp;·&nbsp; <sup>*</sup> corresponding author</p>

  <ol class="pubs">
    <li>
      <span class="t">When Deepfake Text Detectors Leave the Lab: Robust Detection Under Unsupervised Transductive Deployment Across Online Social Networks</span>
      <span class="a">Shaojie Min, Jiayin Xue, <strong>Shaobin Wang</strong>, Yaxiao Luo, Roy Ka-Wei Lee, Yupeng Li, Xinlei He, Qingyuan Gong<sup>*</sup>, Yang Chen<sup>*</sup></span>
      <span class="v">To appear at the 48th IEEE Symposium on Security and Privacy (S&amp;P&rsquo;27)</span>
      <span class="n">Artifact badges: Available, Functional, Reproduced</span>
    </li>
    <li>
      <span class="t">Energy-Aware Collaborative Perception in HetVNETs: Balancing Accuracy and Sustainability</span>
      <span class="a">Mengying Zhou, <strong>Shaobin Wang</strong>, Qiang Duan, Aaron Yi Ding, Xin Wang<sup>*</sup>, Yang Chen<sup>*</sup></span>
      <span class="v">To appear in IEEE Communications Magazine</span>
    </li>
    <li>
      <span class="t">Understanding Cross-Platform Links in User Profiles: A Data-Driven Analysis on Mastodon</span>
      <span class="a">Shaojie Min, <strong>Shaobin Wang</strong>, Yaxiao Luo, Qingyuan Gong<sup>*</sup>, Yang Chen<sup>*</sup></span>
      <span class="v">Proc. of the 10th China National Conference on Big Data and Social Computing (BDSC&rsquo;25), Kunming, China, Aug. 2025</span>
      <span class="n"><span class="award">Most Welcomed Paper Award</span></span>
    </li>
    <li>
      <span class="t">FediLive: A Framework for Collecting and Preprocessing Snapshots of Decentralized Online Social Networks</span>
      <span class="a">Shaojie Min<sup>#</sup>, <strong>Shaobin Wang</strong><sup>#</sup>, Yaxiao Luo, Min Gao, Qingyuan Gong<sup>*</sup>, Yu Xiao, Yang Chen<sup>*</sup></span>
      <span class="v">Proc. of the Web Conference (WWW&rsquo;25), Resource Track, Sydney, Australia, Apr.&ndash;May 2025</span>
    </li>
    <li>
      <span class="t">Towards the Predictability of IPFS Nodes' Session Time Using Machine Learning</span>
      <span class="a">Dan Zhuo, Jiawei Tang, Yang Chen<sup>*</sup>, <strong>Shaobin Wang</strong>, Xin Wang</span>
      <span class="v">Proc. of Turing Award Celebration Conference (TURC&rsquo;23), Poster, Wuhan, China, Jul. 2023 &nbsp;·&nbsp; <a href="https://dl.acm.org/doi/10.1145/3603165.3607397" target="_blank" rel="noopener">paper</a></span>
    </li>
  </ol>

  <h1 class="sec" id="internship">Internship Experience</h1>

  <div class="entry">
    <div class="when">May 2025 &ndash; Aug 2025</div>
    <div>
      <div class="head">Meituan</div>
      <div class="sub">Software Engineering Intern</div>
      <!-- 这里可以再补一到两句实习期间做的事情，例如所属团队与方向 -->
    </div>
  </div>

  <h1 class="sec" id="education">Education</h1>

  <div class="entry">
    <div class="when">Sep 2023 &ndash; Jun 2026</div>
    <div>
      <div class="head"><img src="{{ '/images/Fudan_University_Logo.svg.png' | relative_url }}" alt="Fudan University">Fudan University</div>
      <div class="sub">M.S. in Computer Science, School of Computer Science</div>
    </div>
  </div>

  <div class="entry">
    <div class="when">Sep 2019 &ndash; Jun 2023</div>
    <div>
      <div class="head"><img src="{{ '/images/zzulogo.png' | relative_url }}" alt="Zhengzhou University">Zhengzhou University</div>
      <div class="sub">B.Eng. in Internet of Things Engineering, School of Cyber Science and Engineering</div>
    </div>
  </div>

  <h1 class="sec" id="honors">Honors &amp; Awards</h1>

  <ul class="awards">
    <li><span class="yr">2026</span><span>Outstanding Graduates of Fudan University</span></li>
    <li><span class="yr">2020</span><span>Outstanding Cadre of the Communist Youth League, Zhengzhou University</span></li>
  </ul>

  <p class="updated">Last updated: November 2026</p>
</div>
