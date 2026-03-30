---
layout: default
permalink: /
---

<style>
.home-bg {
  position: relative;
  padding: 2rem 0.5rem 3rem;
  border-radius: 24px;
  overflow: hidden;
}

.home-bg::before {
  content: "";
  position: absolute;
  inset: 0;
  background:
    linear-gradient(rgba(255,255,255,0.38), rgba(255,255,255,0.48)),
    url('{{ "/assets/red-panda-home-bg.png" | relative_url }}') center center / cover no-repeat;
  z-index: 0;
}

.home-bg > * {
  position: relative;
  z-index: 1;
}

.home-bg h1,
.home-bg h2,
.home-bg h3,
.home-bg h4,
.home-bg p,
.home-bg li {
  text-shadow: 0 1px 2px rgba(255,255,255,0.18);
}

.glass-panel {
  background: rgba(255,255,255,0.48);
  backdrop-filter: blur(6px);
  border-radius: 18px;
  box-shadow: 0 8px 22px rgba(0,0,0,0.08);
}

.hero-row {
  margin-top: 0.5rem;
}

.hero-panel {
  padding: 1.5rem;
  height: 100%;
}

.hero-main {
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

.hero-avatar {
  flex: 0 0 170px;
}

.hero-avatar img {
  width: 170px;
  height: 170px;
  object-fit: cover;
  border-radius: 50%;
  box-shadow: 0 8px 22px rgba(0,0,0,0.16);
}

.hero-text h1 {
  margin-bottom: 0.5rem;
}

.hero-subtitle {
  font-size: 1.05rem;
  line-height: 1.7;
  margin-bottom: 0.5rem;
}

.hero-note {
  margin-bottom: 0;
  line-height: 1.75;
}

.quick-links-panel {
  padding: 1.4rem 1.35rem;
  height: 100%;
}

.quick-links-panel h4 {
  margin-bottom: 1rem;
}

.quick-links-panel p {
  margin-bottom: 0.7rem;
}

.research-map-section {
  margin-top: 9rem;
  background: transparent !important;
  backdrop-filter: none !important;
  border-radius: 0 !important;
  box-shadow: none !important;
}

.research-map-layout {
  display: grid;
  grid-template-columns: 1fr 1.5fr 1fr;
  gap: 1.25rem;
  align-items: center;
}

.research-side {
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
}

.research-box {
  position: relative;
  background: rgba(255,255,255,0.40);
  backdrop-filter: blur(6px);
  border-radius: 18px;
  padding: 1rem 1.1rem;
  box-shadow: 0 6px 18px rgba(0,0,0,0.08);
}

.research-box h4 {
  margin-bottom: 0.55rem;
  font-size: 1.05rem;
}

.research-box p {
  margin-bottom: 0;
  font-size: 0.95rem;
  line-height: 1.65;
}

.research-center {
  display: flex;
  justify-content: center;
}

.research-center img {
  width: 100%;
  max-width: 900px;
  border-radius: 22px;
  box-shadow: 0 10px 28px rgba(0,0,0,0.14);
}

.publications-note {
  margin-top: 1.5rem;
  margin-bottom: 0;
}

.page-visitor-map-wrap {
  margin: 1rem auto 0.8rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.page-visitor-map-shell {
  position: relative;
  width: 300px;
  height: 95px;
  overflow: hidden;
  border-radius: 10px;
  line-height: 0;
}

.page-visitor-map-inner {
  position: absolute;
  left: 50%;
  top: 0;
  width: 1000px;
  transform: translateX(-50%) scale(0.22);
  transform-origin: top center;
  line-height: 0;
}

@media (min-width: 1200px) {
  .research-side:first-child .research-box::after {
    content: "";
    position: absolute;
    right: -22px;
    top: 50%;
    width: 22px;
    height: 2px;
    background: rgba(255,255,255,0.85);
    transform: translateY(-50%);
  }

  .research-side:last-child .research-box::before {
    content: "";
    position: absolute;
    left: -22px;
    top: 50%;
    width: 22px;
    height: 2px;
    background: rgba(255,255,255,0.85);
    transform: translateY(-50%);
  }
}

@media (max-width: 991.98px) {
  .hero-main {
    flex-direction: column;
    align-items: flex-start;
  }

  .hero-avatar {
    flex: none;
  }

  .hero-avatar img {
    width: 150px;
    height: 150px;
  }
}

@media (max-width: 1199.98px) {
  .research-map-layout {
    grid-template-columns: 1fr;
  }

  .research-center {
    order: -1;
  }

  .research-side {
    gap: 1rem;
  }
}

@media (max-width: 768px) {
  .page-visitor-map-wrap {
    margin-top: 0.8rem;
    margin-bottom: 0.6rem;
  }

  .page-visitor-map-shell {
    width: 240px;
    height: 64px;
  }

  .page-visitor-map-inner {
    width: 1000px;
    transform: translateX(-50%) scale(0.19);
    transform-origin: top center;
  }
}
</style>

<div class="home-bg">

  <div class="row hero-row align-items-stretch">
    <div class="col-lg-8">
      <div class="glass-panel hero-panel">
        <div class="hero-main">
          <div class="hero-avatar">
            <img src="{{ site.author.image }}" alt="{{ site.title }}">
          </div>
          <div class="hero-text">
            <h1>{{ site.title }}</h1>
            <p class="hero-subtitle">
              <strong>Associate Research Scientist</strong><br>
              MoE Key Lab of Artificial Intelligence, AI Institute, Shanghai Jiao Tong University
            </p>
            <p class="hero-note">
              Research on perceptual quality evaluation and enhancement for visual content,
              spanning PGC, UGC, and AIGC scenarios.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="col-lg-4 mt-4 mt-lg-0">
      <div class="glass-panel quick-links-panel">
        <h4>Quick Links</h4>
        <p><a href="{{ '/publications/' | relative_url }}"><strong>Publications</strong></a></p>
        <p><a href="{{ '/about/' | relative_url }}"><strong>About</strong></a></p>
        <hr>
        <p><a href="mailto:zwx8981@sjtu.edu.cn">Email</a></p>
        <p><a href="https://scholar.google.com/citations?user=KK2nLnQAAAAJ">Google Scholar</a></p>
        <p class="mb-0"><a href="https://github.com/zwx8981">GitHub</a></p>
      </div>
    </div>
  </div>

  <div class="research-map-section">
    <div class="research-map-layout">
      <div class="research-side">
        <div class="research-box">
          <h4><strong>Multimedia Quality Assessment</strong></h4>
          <p>
            Focusing on accurate and fair evaluation of multimedia quality, while also serving as loss functions,
            reward models, or real-time feedback signal in shaping various vision systems.
          </p>
        </div>

        <div class="research-box">
          <h4><strong>Perceptual Optimization</strong></h4>
          <p>
            Working on existing visual content, seeking to enhance, restore, or edit images/videos to improve
            their perceived quality.
          </p>
        </div>
      </div>

      <div class="research-center">
        <img src="{{ '/assets/research_overview.png' | relative_url }}" alt="Research overview illustration">
      </div>

      <div class="research-side">
        <div class="research-box">
          <h4><strong>Computational Photography</strong></h4>
          <p>
            Targeting the visual capture stage, aiming to produce high-quality images/videos directly at the
            moment of acquisition.
          </p>
        </div>

        <div class="research-box">
          <h4><strong>Industrial Vision Analysis</strong></h4>
          <p>
            Extending quality assessment from alignment with human visual perception to alignment with task-specific
            goals, such as object defect detection and safety monitoring of workers.
          </p>
        </div>
      </div>
    </div>
  </div>

  <p class="publications-note">
    See the <a href="{{ '/publications/' | relative_url }}"><strong>full publications list</strong></a> for more details.
  </p>

</div>

<div class="page-visitor-map-wrap">
  <div class="page-visitor-map-shell">
    <div class="page-visitor-map-inner">
      <script
        type="text/javascript"
        id="mapmyvisitors"
        src="https://mapmyvisitors.com/map.js?cl=ffffff&w=a&t=tt&d=UWJZsT5Cd6QONPhxbnNfgB6bFHglPXnxwrMUVUWsIkc&co=09304c">
      </script>
    </div>
  </div>
</div>
