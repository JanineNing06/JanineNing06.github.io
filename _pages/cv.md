---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<style>
.cv-download-bar {
  background: #f0f6fd;
  border: 1px solid #d0e4f0;
  border-radius: 12px;
  padding: 20px 28px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 32px;
}
.cv-download-bar h2 { margin: 0; font-size: 1.3em; }
.cv-download-btn {
  display: inline-block;
  padding: 8px 20px;
  background: #2a6cc0;
  color: #fff !important;
  border-radius: 8px;
  font-size: 0.9em;
  font-weight: 600;
  text-decoration: none !important;
  transition: background 0.15s;
}
.cv-download-btn:hover { background: #1a4e99; }

.cv-section { margin-bottom: 36px; }
.cv-section-title {
  font-size: 1.1em;
  font-weight: 700;
  color: #333;
  margin-bottom: 14px;
  padding-bottom: 6px;
  border-bottom: 2px solid #2a6cc0;
}

/* Card base */
.cv-card {
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 10px;
  padding: 18px 22px;
  margin-bottom: 12px;
  transition: box-shadow 0.15s;
}
.cv-card:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.08); }

/* Education card */
.cv-edu-header { display: flex; justify-content: space-between; align-items: flex-start; }
.cv-edu-degree { font-weight: 700; font-size: 0.97em; color: #222; }
.cv-edu-date { font-size: 0.83em; color: #888; white-space: nowrap; margin-left: 12px; }
.cv-edu-school { font-size: 0.88em; color: #2a6cc0; margin-top: 3px; }
.cv-edu-detail { font-size: 0.83em; color: #666; margin-top: 6px; line-height: 1.6; }

/* Experience card — collapsible */
.cv-exp-summary {
  display: flex; justify-content: space-between; align-items: flex-start;
  cursor: pointer; list-style: none; user-select: none;
}
.cv-exp-summary::-webkit-details-marker { display: none; }
.cv-exp-summary::after {
  content: '▸'; font-size: 0.85em; color: #aaa;
  margin-left: 10px; flex-shrink: 0; margin-top: 2px; transition: transform 0.2s;
}
details[open] > .cv-exp-summary::after { transform: rotate(90deg); }
.cv-exp-summary-left { flex: 1; }
.cv-exp-role { font-weight: 700; font-size: 0.97em; color: #222; }
.cv-exp-date { font-size: 0.83em; color: #888; white-space: nowrap; margin-left: 12px; flex-shrink: 0; }
.cv-exp-org { font-size: 0.88em; color: #2a6cc0; margin-top: 3px; }
.cv-exp-items { font-size: 0.83em; color: #555; margin-top: 10px; line-height: 1.7; padding-left: 16px; }
.cv-exp-items li { margin-bottom: 6px; }
.cv-exp-project { font-style: italic; font-weight: 600; color: #444; }
.cv-exp-sub { padding-left: 14px; margin-top: 4px; }
.cv-exp-sub li { margin-bottom: 3px; color: #666; }

/* Publication card */
.cv-pub-card {
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 10px;
  padding: 14px 18px;
  margin-bottom: 10px;
  display: flex;
  gap: 14px;
  align-items: flex-start;
  transition: box-shadow 0.15s;
}
.cv-pub-card:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.08); }
.cv-pub-year {
  background: #eef4fd; color: #2a6cc0; border: 1px solid #c0d8f0;
  border-radius: 6px; padding: 3px 10px; font-size: 0.78em; font-weight: 600;
  white-space: nowrap; flex-shrink: 0; margin-top: 2px;
}
.cv-pub-body { flex: 1; }
.cv-pub-title { font-weight: 600; font-size: 0.93em; color: #222; line-height: 1.4; }
.cv-pub-authors { font-size: 0.82em; color: #888; margin-top: 4px; }
.cv-pub-venue { font-size: 0.82em; color: #666; font-style: italic; margin-top: 2px; }
.cv-pub-badge span {
  border-radius: 6px; padding: 3px 10px; font-size: 0.75em; font-weight: 600;
  border: 1.5px solid; flex-shrink: 0; white-space: nowrap;
}
.badge-conf   { color: #2a7ac0; border-color: #2a7ac0 !important; }
.badge-review { color: #888; border-color: #bbb !important; }

/* Award row */
.cv-award-card {
  display: flex; align-items: center; gap: 14px;
  background: #fff; border: 1px solid #e8e8e8; border-radius: 10px;
  padding: 12px 18px; margin-bottom: 10px; transition: box-shadow 0.15s;
}
.cv-award-card:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.08); }
.cv-award-year {
  background: #fffbe8; color: #b07a00; border: 1px solid #e8d080;
  border-radius: 6px; padding: 3px 10px; font-size: 0.78em; font-weight: 600;
  white-space: nowrap; flex-shrink: 0;
}
.cv-award-name { font-size: 0.9em; font-weight: 600; color: #222; flex: 1; }

/* Skills */
.cv-skills-grid { display: flex; gap: 12px; flex-wrap: wrap; }
.cv-skill-group {
  background: #f7f9fc; border: 1px solid #e0e8f0;
  border-radius: 10px; padding: 14px 18px; flex: 1; min-width: 200px;
}
.cv-skill-group-title { font-weight: 700; font-size: 0.85em; color: #2a6cc0; margin-bottom: 8px; }
.cv-skill-tags { display: flex; flex-wrap: wrap; gap: 6px; }
.cv-skill-tag {
  background: #fff; border: 1px solid #d0dff0; border-radius: 6px;
  padding: 3px 10px; font-size: 0.8em; color: #444;
}
</style>

<!-- Header -->
<div class="cv-download-bar">
  <h2>📄 Curriculum Vitae</h2>
  <a class="cv-download-btn" href="/files/WanjunNing_CV.pdf" download>⬇ Download PDF</a>
</div>

<!-- Education -->
<div class="cv-section">
  <div class="cv-section-title">Education</div>

  <div class="cv-card">
    <div class="cv-edu-header">
      <div class="cv-edu-degree">Ph.D. in Mathematics — Statistics and Data Science Track</div>
      <div class="cv-edu-date">2023 – 2027 (expected)</div>
    </div>
    <div class="cv-edu-school">University of Texas at Arlington, Texas, USA</div>
    <div class="cv-edu-detail">
      Principal supervisor: Prof. Li Wang &nbsp;·&nbsp; Co-supervisor: Prof. Rencang Li
    </div>
  </div>

  <div class="cv-card">
    <div class="cv-edu-header">
      <div class="cv-edu-degree">M.Phil. in Probability and Mathematical Statistics</div>
      <div class="cv-edu-date">2021 – 2023</div>
    </div>
    <div class="cv-edu-school">Hong Kong Baptist University, Hong Kong, China</div>
    <div class="cv-edu-detail">
      Principal supervisor: Prof. Tiejun Tong &nbsp;·&nbsp; Co-supervisor: Prof. Jingjin Wu<br>
      Thesis: <em>Analysis and Optimization of User Association in Wireless Networks</em>
    </div>
  </div>

  <div class="cv-card">
    <div class="cv-edu-header">
      <div class="cv-edu-degree">B.Sc. (Honours) in Financial Mathematics</div>
      <div class="cv-edu-date">2016 – 2020</div>
    </div>
    <div class="cv-edu-school">Hong Kong Baptist University, Hong Kong, China</div>
  </div>
</div>

<!-- Research Experience -->
<div class="cv-section">
  <div class="cv-section-title">Research and Work Experience</div>

  <div class="cv-card">
    <details>
      <summary class="cv-exp-summary">
        <div class="cv-exp-summary-left">
          <div class="cv-exp-role">Research Assistant</div>
          <div class="cv-exp-org">University of Texas at Arlington, Texas, USA</div>
        </div>
        <div class="cv-exp-date">Feb 2024 – present</div>
      </summary>
      <ul class="cv-exp-items">
        <li>
          <span class="cv-exp-project">Adaptive Multimodal Fusion Network for Hybrid EEG–bbNIRS Alzheimer's Screening</span>
          <ul class="cv-exp-sub">
            <li>Built a multimodal fusion framework integrating EEG and bbNIRS signals for early Alzheimer's screening.</li>
            <li>Stabilized training with targeted augmentations, adaptive regularization, and learning-rate scheduling.</li>
            <li>Analyzed modality contributions, highlighting complementary temporal and metabolic information.</li>
            <li><strong>Performance:</strong> Achieved 7–12% improvement in AUC over unimodal baselines with robust cross-validation.</li>
          </ul>
        </li>
        <li>
          <span class="cv-exp-project">Graph-Regularized Sparse Principal Component Analysis</span>
          <ul class="cv-exp-sub">
            <li>Proposed a unified framework for unsupervised dimensionality reduction, feature selection, and adaptive graph structure learning.</li>
            <li>Formulated a joint optimization with ℓ₂,₁-norm sparsity and data-driven graph similarity.</li>
            <li>Introduced graph ensembles to capture heterogeneous structures.</li>
            <li>Designed efficient alternating minimization with closed-form updates and convergence guarantees.</li>
            <li><strong>Performance:</strong> 3× faster runtime with stronger clustering/classification accuracy on high-dimensional datasets.</li>
          </ul>
        </li>
        <li>
          <span class="cv-exp-project">Unrolled Attention-Based Neural Network for Efficient Unsupervised Feature Selection</span>
          <ul class="cv-exp-sub">
            <li>Modified attention-based neural networks with unrolling and new regularization strategies for high-dimensional feature selection.</li>
            <li>Integrated feature selection with dimensionality reduction across imaging and tabular biomarkers, validated by clinical experts.</li>
            <li>Improved stability and calibration via task-specific objectives and hyperparameter tuning.</li>
            <li><strong>Performance:</strong> 2.5× faster convergence with reduced computation cost while preserving interpretability.</li>
          </ul>
        </li>
      </ul>
    </details>
  </div>

  <div class="cv-card">
    <details>
      <summary class="cv-exp-summary">
        <div class="cv-exp-summary-left">
          <div class="cv-exp-role">Research Assistant</div>
          <div class="cv-exp-org">Beijing Normal-Hong Kong Baptist University, Zhuhai, China</div>
        </div>
        <div class="cv-exp-date">Jun 2020 – Dec 2020</div>
      </summary>
      <ul class="cv-exp-items">
        <li>Investigated energy efficiency and Quality of Service (QoS) trade-offs in cellular networks by modeling Base Stations (BSs) as processor-sharing queues with vacations.</li>
        <li>Developed and analyzed three BS sleep schemes: isolated, cooperative, and hybrid.</li>
        <li>Proposed a scalable analytical method to evaluate QoS metrics and power consumption.</li>
        <li>Validated results through simulations and conducted experiments to compare scheme performance under different network conditions.</li>
        <li><strong>Skills:</strong> MATLAB, Queueing Theory, Network Optimization, Power Efficiency, Simulation.</li>
      </ul>
    </details>
  </div>

  <div class="cv-card">
    <details>
      <summary class="cv-exp-summary">
        <div class="cv-exp-summary-left">
          <div class="cv-exp-role">Business Analysis Intern</div>
          <div class="cv-exp-org">China Capital Management Company, Beijing, China</div>
        </div>
        <div class="cv-exp-date">Jun 2019 – Aug 2019</div>
      </summary>
      <ul class="cv-exp-items">
        <li>Analyzed a biotech's Phase III oncology asset, synthesizing trial outcomes, market potential, competitive landscape, and strategic implications to inform go-to-market and investment decisions.</li>
        <li>Assessed drug efficacy and safety through clinical data, regulatory submissions, and scientific literature.</li>
        <li>Modeled market share and revenue projections based on disease prevalence and competitor analysis.</li>
        <li>Assisted project manager in presenting key findings and strategic recommendations to senior management.</li>
        <li><strong>Skills:</strong> R Programming, Data Analysis, Market Research, Financial Modeling, Pharmaceutical Industry.</li>
      </ul>
    </details>
  </div>
</div>

<!-- Publications -->
<div class="cv-section">
  <div class="cv-section-title">Publications</div>

  <div class="cv-pub-card">
    <div class="cv-pub-year">2026</div>
    <div class="cv-pub-body">
      <div class="cv-pub-title">Bridging Neural and Hemodynamic Pathways through EEG–bbNIRS Fusion for Early Alzheimer's Disease Classification</div>
      <div class="cv-pub-authors">W. Ning, F. Saeed, H. Tang, H. Liu, and L. Wang</div>
      <div class="cv-pub-venue">Under review, 2026</div>
    </div>
    <div class="cv-pub-badge"><span class="badge-review">Under Review</span></div>
  </div>

  <div class="cv-pub-card">
    <div class="cv-pub-year">2023</div>
    <div class="cv-pub-body">
      <div class="cv-pub-title"><a href="https://ieeexplore.ieee.org/document/10437288" target="_blank" style="color:#222;text-decoration:none;">A Ring Topology-Based Communication-Efficient Scheme for D2D Wireless Federated Learning</a></div>
      <div class="cv-pub-authors">Z. Xu, W. Tian, Y. Liu, W. Ning and J. Wu</div>
      <div class="cv-pub-venue">IEEE Global Communications Conference (GLOBECOM), 2023, pp. 2820–2825</div>
    </div>
    <div class="cv-pub-badge"><span class="badge-conf">Conference</span></div>
  </div>

  <div class="cv-pub-card">
    <div class="cv-pub-year">2022</div>
    <div class="cv-pub-body">
      <div class="cv-pub-title"><a href="https://ieeexplore.ieee.org/document/9839128" target="_blank" style="color:#222;text-decoration:none;">Sequence Q-Learning Algorithm for Optimal Mobility-Aware User Association</a></div>
      <div class="cv-pub-authors">W. Ning, Z. Xu, J. Wu and T. Tong</div>
      <div class="cv-pub-venue">IEEE International Conference on Communications (ICC), 2022, pp. 726–732</div>
    </div>
    <div class="cv-pub-badge"><span class="badge-conf">Conference</span></div>
  </div>
</div>

<!-- Awards -->
<div class="cv-section">
  <div class="cv-section-title">Awards & Honors</div>

  <div class="cv-award-card">
    <div class="cv-award-year">2026</div>
    <div class="cv-award-name">Math Academic Excellence Scholarship</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2026</div>
    <div class="cv-award-name">Student Travel Award — NSF-CBMS 2026 (Ypsilanti, MI)</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2025</div>
    <div class="cv-award-name">Student Travel Award — CBMS AMML 2025 (Houston, TX)</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2025</div>
    <div class="cv-award-name">Dr. Chien-Pai Han Memorial Scholarship</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2024</div>
    <div class="cv-award-name">Benny M. McCarley Scholarship</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2023 - now</div>
    <div class="cv-award-name">Graduate Research Assistantship / Graduate Teaching Assistantship, UT Arlington</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2021–22</div>
    <div class="cv-award-name">Graduate Full Scholarship, Hong Kong Baptist University</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2020</div>
    <div class="cv-award-name">University Merit Scholarship</div>
  </div>
  <div class="cv-award-card">
    <div class="cv-award-year">2018</div>
    <div class="cv-award-name">American Mathematical Contest in Modelling — Honourable Mention</div>
  </div>
</div>

<!-- Skills -->
<div class="cv-section">
  <div class="cv-section-title">Skills</div>
  <div class="cv-skills-grid">
    <div class="cv-skill-group">
      <div class="cv-skill-group-title">Programming</div>
      <div class="cv-skill-tags">
        <span class="cv-skill-tag">Python</span>
        <span class="cv-skill-tag">MATLAB</span>
        <span class="cv-skill-tag">C++</span>
        <span class="cv-skill-tag">R</span>
        <span class="cv-skill-tag">EViews</span>
      </div>
    </div>
    <div class="cv-skill-group">
      <div class="cv-skill-group-title">Tools</div>
      <div class="cv-skill-tags">
        <span class="cv-skill-tag">LaTeX</span>
        <span class="cv-skill-tag">Markdown</span>
        <span class="cv-skill-tag">Word</span>
        <span class="cv-skill-tag">Excel</span>
        <span class="cv-skill-tag">PowerPoint</span>
      </div>
    </div>
  </div>
</div>
