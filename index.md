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
  <p>I am {{ site.author.employer | default: "a Professor of Finance" }} at {{ site.author.location | default: "[University Name] Business School" }}, where I conduct research on corporate finance, ESG, and political economy. </p>
  
  <p>I also work as a research associate at Institute of International M&As and Investment, Renmin University of China. I received my Ph.D. in Financial Engineering from Renmin University of China.</p>

  <p>My current research focuses on understanding how technological innovation, regulatory changes, and behavioral factors shape financial markets and corporate decision-making. I am particularly interested in the intersection of finance and technology, exploring how FinTech innovations are transforming traditional financial services.</p>

  {% if site.author.bio %}
  <p><strong>Bio:</strong> {{ site.author.bio }}</p>
  {% endif %}
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

<div class="section" id="contact-info">
  <h2>Contact Information</h2>
  <div class="contact-grid">
    {% if site.author.email %}
    <div class="contact-item">
      <strong>📧 Email:</strong> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>
    </div>
    {% endif %}
    
    {% if site.author.phone %}
    <div class="contact-item">
      <strong>📞 Phone:</strong> {{ site.author.phone }}
    </div>
    {% endif %}
    
    {% if site.author.office %}
    <div class="contact-item">
      <strong>🏢 Office:</strong> {{ site.author.office }}
    </div>
    {% endif %}
    
    <div class="contact-item">
      <strong>🎓 Academic Profiles:</strong><br>
      {% if site.author.googlescholar %}<a href="{{ site.author.googlescholar }}" target="_blank">Google Scholar</a>{% endif %}
      {% if site.author.orcid %} | <a href="{{ site.author.orcid }}" target="_blank">ORCID</a>{% endif %}
      {% if site.author.researchgate %} | <a href="{{ site.author.researchgate }}" target="_blank">ResearchGate</a>{% endif %}
      {% if site.author.ssrn %} | <a href="{{ site.author.ssrn }}" target="_blank">SSRN</a>{% endif %}
    </div>
  </div>
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
  border-left: 4px solid #a71a3d;
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
  background: linear-gradient(135deg, rgba(167, 26, 61, 0.02), rgba(220, 47, 90, 0.02));
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
  color: #a71a3d;
  margin-bottom: 1rem;
  font-size: 1.2rem;
  font-weight: 600;
}

.research-card p {
  color: #64748b;
  font-size: 1rem;
  line-height: 1.6;
}

/* 联系信息网格 */
.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.contact-item {
  background: #f8fafc;
  padding: 1.5rem;
  border-radius: 12px;
  border-left: 4px solid #dc2f5a;
}

.contact-item strong {
  color: #a71a3d;
}

.contact-item a {
  color: #dc2f5a;
  text-decoration: none;
  font-weight: 500;
}

.contact-item a:hover {
  text-decoration: underline;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .research-grid,
  .contact-grid {
    grid-template-columns: 1fr;
  }
}
</style>
