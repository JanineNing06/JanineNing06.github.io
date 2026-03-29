---
permalink: /
title:
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.about-hero {
  background: linear-gradient(135deg, #e8f0fb 0%, #f0f6fd 60%, #dceeff 100%);
  border-radius: 16px;
  padding: 32px 36px;
  margin-bottom: 36px;
}
.about-hero-title {
  font-size: 1.9em;
  font-weight: 800;
  color: #111;
  margin: 0 0 16px 0;
  line-height: 1.2;
}
.about-hero-title span {
  color: #2a6cc0;
}
.about-hero-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 22px;
}
.about-hero-tag {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  background: rgba(255,255,255,0.75);
  border: 1px solid rgba(42,108,192,0.2);
  border-radius: 999px;
  padding: 5px 14px;
  font-size: 0.83em;
  color: #444;
}
.about-hero-body {
  font-size: 0.97em;
  color: #222;
  line-height: 1.85;
}
.about-hero-body strong { color: #2a6cc0; }
.about-hero-keywords {
  margin-top: 14px;
  font-size: 0.83em;
  color: #666;
}
.about-hero-keywords span {
  display: inline-block;
  background: rgba(42,108,192,0.08);
  border: 1px solid rgba(42,108,192,0.2);
  border-radius: 6px;
  padding: 2px 10px;
  margin: 3px 3px 0 0;
  color: #2a6cc0;
  font-weight: 600;
}
</style>

<div class="about-hero">
  <div class="about-hero-title">Hi, I'm <span>Wanjun</span> 👋</div>
  <div class="about-hero-tags">
    <span class="about-hero-tag">🎓 Ph.D. Candidate</span>
    <span class="about-hero-tag">📐 Statistics &amp; Data Science</span>
    <span class="about-hero-tag">🏛 UT Arlington</span>
    <span class="about-hero-tag">📍 Dallas, TX</span>
  </div>
  <div class="about-hero-body">
    I am a Ph.D. candidate in Mathematics (Statistics and Data Science track) at the <strong>University of Texas at Arlington</strong>, co-advised by <strong>Prof. Li Wang</strong> and <strong>Prof. Rencang Li</strong> since 2023.
    <br><br>
    My research lies at the intersection of Machine Learning and Mathematics, with a focus on <strong>Dimensionality Reduction</strong>, <strong>Structure Learning</strong>, <strong>Multi-view Learning</strong>, and <strong>Optimization for Big Data</strong>.
    <br><br>
    Prior to my Ph.D. studies, I earned an M.Phil. in Probability and Mathematical Statistics from <strong>Hong Kong Baptist University</strong> (2023), supervised by <strong>Prof. Tiejun Tong</strong> and <strong>Prof. Jingjin Wu</strong>. I also hold a B.Sc. in Financial Mathematics from <strong>Hong Kong Baptist University</strong> (2020).
  </div>
</div>

## Research Interests

<style>
.ri-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
  margin: 16px 0 36px;
}
@media (max-width: 640px) {
  .ri-grid { grid-template-columns: 1fr 1fr; }
}
.ri-card {
  background: #fff;
  border: 1px solid #d8e8f8;
  border-radius: 12px;
  padding: 20px 18px;
  transition: box-shadow 0.15s, border-color 0.15s;
}
.ri-card:hover {
  border-color: #2a6cc0;
  box-shadow: 0 3px 14px rgba(42,108,192,0.12);
}
.ri-icon { font-size: 1.6em; margin-bottom: 10px; }
.ri-title {
  font-size: 0.95em;
  font-weight: 700;
  color: #2a6cc0;
  margin-bottom: 6px;
}
.ri-desc {
  font-size: 0.82em;
  color: #555;
  line-height: 1.6;
}
</style>

<div class="ri-grid">
  <div class="ri-card">
    <div class="ri-icon">📉</div>
    <div class="ri-title">Dimensionality Reduction</div>
    <div class="ri-desc">Sparse PCA and graph-regularized projection methods for high-dimensional data analysis.</div>
  </div>
  <div class="ri-card">
    <div class="ri-icon">🕸️</div>
    <div class="ri-title">Structure Learning</div>
    <div class="ri-desc">Adaptive graph learning and data-driven similarity estimation for complex structured data.</div>
  </div>
  <div class="ri-card">
    <div class="ri-icon">🔀</div>
    <div class="ri-title">Multi-view Learning</div>
    <div class="ri-desc">Multimodal fusion across time series, spectra, images, and text for robust representation.</div>
  </div>
  <div class="ri-card">
    <div class="ri-icon">⚡</div>
    <div class="ri-title">Optimization for Big Data</div>
    <div class="ri-desc">Efficient alternating minimization and scalable algorithms with convergence guarantees.</div>
  </div>
  <div class="ri-card">
    <div class="ri-icon">🧠</div>
    <div class="ri-title">Feature Selection</div>
    <div class="ri-desc">Attention-based neural networks with unrolling strategies for unsupervised feature selection.</div>
  </div>
  <div class="ri-card">
    <div class="ri-icon">🏥</div>
    <div class="ri-title">Clinical Applications</div>
    <div class="ri-desc">Multimodal EEG–bbNIRS fusion for early Alzheimer's disease screening and classification.</div>
  </div>
</div>

## Latest News

<style>
.about-news-list { margin: 16px 0 10px; }
.about-news-list {
  background: #fff;
  border: 1px solid #d8e8f8;
  border-radius: 12px;
  padding: 6px 18px;
  box-shadow: 0 2px 10px rgba(42,108,192,0.07);
}
.about-news-item {
  display: flex; align-items: baseline; gap: 16px;
  padding: 10px 12px; border-bottom: 1px solid #eef2f8;
  border-radius: 8px;
  transition: background 0.15s, transform 0.15s, box-shadow 0.15s;
}
.about-news-item:last-child { border-bottom: none; }
.about-news-item:hover {
  background: #eef4fd;
  transform: scale(1.01);
  box-shadow: 0 2px 10px rgba(42,108,192,0.10);
}
.about-news-date {
  color: #2a6cc0; font-size: 0.82em; font-weight: 700;
  white-space: nowrap; flex-shrink: 0; width: 72px; text-align: right;
}
.about-news-text { font-size: 0.9em; color: #333; line-height: 1.55; }
.about-news-text strong { color: #111; }
.about-news-more {
  display: inline-block; margin-top: 10px;
  font-size: 0.88em; font-weight: 600; color: #2a6cc0; text-decoration: none;
}
.about-news-more:hover { text-decoration: underline; }
</style>

<div class="about-news-list">
  <div class="about-news-item">
    <span class="about-news-date">May 2026</span>
    <span class="about-news-text">Received <strong>Student Travel Award</strong> for NSF-CBMS 2026 (Ypsilanti, MI)</span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">Dec 2025</span>
    <span class="about-news-text">Received <strong>Student Travel Award</strong> for CBMS AMML 2025; Poster presentation at CBMS AMML, University of Houston</span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">Oct 2025</span>
    <span class="about-news-text">Poster presentation at <strong>AI for Biology &amp; Medicine Symposium</strong>, University of North Texas</span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">2025</span>
    <span class="about-news-text">Received <strong>Dr. Chien-Pai Han Memorial Scholarship</strong></span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">Jun 2025</span>
    <span class="about-news-text">Invited talk at Department of Mathematics, Hong Kong Baptist University</span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">Apr 2025</span>
    <span class="about-news-text">Poster presentation at <strong>Discover 2025 Student Research Symposium</strong></span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">2024</span>
    <span class="about-news-text">Received <strong>Benny M. McCarley Scholarship</strong></span>
  </div>
  <div class="about-news-item">
    <span class="about-news-date">Jun 2024</span>
    <span class="about-news-text">Invited paper presentation at <strong>International Chinese Statistical Association (ICSA)</strong></span>
  </div>
</div>

<a class="about-news-more" href="/year-archive/">See all news →</a>

