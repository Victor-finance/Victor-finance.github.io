---
permalink: /
title: "Welcome"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="section" id="about">
  <h2>About</h2>
  <p>I am a Professor of Finance at [University Name] Business School, where I conduct research on corporate finance, financial markets, and behavioral finance. My work has been published in leading academic journals and has influenced both academic discourse and industry practice.</p>
  
  <p>Prior to joining [University Name], I held positions at [Previous Institution] and worked as a consultant for several financial institutions. I received my Ph.D. in Finance from [University] and hold professional certifications including the CFA designation.</p>

  <p>My current research focuses on understanding how technological innovation, regulatory changes, and behavioral factors shape financial markets and corporate decision-making. I am particularly interested in the intersection of finance and technology, exploring how FinTech innovations are transforming traditional financial services.</p>
</div>

<div class="section" id="research">
  <h2>Research Interests</h2>
  <div class="research-grid">
    <div class="research-card">
      <h4>Corporate Finance</h4>
      <p>Capital structure optimization, dividend policy analysis, mergers and acquisitions strategy, and corporate governance mechanisms in modern markets.</p>
    </div>
    <div class="research-card">
      <h4>Financial Markets</h4>
      <p>Market microstructure dynamics, asset pricing models, market efficiency testing, and the impact of algorithmic trading on market quality.</p>
    </div>
    <div class="research-card">
      <h4>Behavioral Finance</h4>
      <p>Investor psychology and decision-making biases, market anomalies, sentiment analysis, and the role of emotions in financial markets.</p>
    </div>
    <div class="research-card">
      <h4>Financial Technology</h4>
      <p>FinTech innovation impact, digital banking transformation, cryptocurrency markets, and blockchain applications in traditional finance.</p>
    </div>
    <div class="research-card">
      <h4>Sustainable Finance</h4>
      <p>ESG investing strategies, climate risk assessment in financial markets, and the economics of sustainable business models.</p>
    </div>
    <div class="research-card">
      <h4>International Finance</h4>
      <p>Cross-border capital flows, exchange rate dynamics, international portfolio diversification, and emerging market finance.</p>
    </div>
  </div>
</div>

<div class="section" id="recent-news">
  <h2>Recent News</h2>
  <ul style="color: var(--text-light); line-height: 1.8;">
    <li><strong>June 2025:</strong> New paper accepted at Journal of Finance</li>
    <li><strong>May 2025:</strong> Invited speaker at AFA Annual Meeting</li>
    <li><strong>April 2025:</strong> Received Teaching Excellence Award</li>
    <li><strong>March 2025:</strong> Research featured in Financial Times</li>
  </ul>
</div>

<style>
/* 研究兴趣网格 */
.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.research-card {
  background: linear-gradient(135deg, #f8fafc, #ffffff);
  padding: 2rem;
  border-radius: 16px;
  border-left: 4px solid #1e3a8a;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.research-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(135deg, rgba(30, 58, 138, 0.02), rgba(59, 130, 246, 0.02));
  opacity: 0;
  transition: opacity 0.3s ease;
}

.research-card:hover::before {
  opacity: 1;
}

.research-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}

.research-card h4 {
  color: #1e3a8a;
  margin-bottom: 1rem;
  font-size: 1.2rem;
  font-weight: 600;
}

.research-card p {
  color: #64748b;
  font-size: 1rem;
  line-height: 1.6;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .research-grid {
    grid-template-columns: 1fr;
  }
}
</style>
