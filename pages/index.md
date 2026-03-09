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
    linear-gradient(rgba(255,255,255,0.72), rgba(255,255,255,0.84)),
    url('{{ "/assets/red-panda-home-bg.png" | relative_url }}') center center / cover no-repeat;
  z-index: 0;
}

.home-bg > * {
  position: relative;
  z-index: 1;
}

.home-bg .card,
.home-bg .jumbotron,
.home-bg section {
  background: rgba(255,255,255,0.80);
  backdrop-filter: blur(6px);
  border-radius: 16px;
}

.home-bg h1,
.home-bg h2,
.home-bg h3,
.home-bg h4,
.home-bg p,
.home-bg li {
  text-shadow: 0 1px 2px rgba(255,255,255,0.18);
}

.research-map-section {
  margin-top: 3rem;
}

.research-map-title {
  margin-bottom: 1.5rem;
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
  background: rgba(255,255,255,0.84);
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
</style>

<div class="home-bg">

{% include landing.html %}

<div class="row mt-5">
  <div class="col-lg-8">
    <h2 class="mb-3">Research Overview</h2>
    <p>
      I am an <strong>Associate Research Scientist</strong> at the <strong>MoE Key Lab of Artificial Intelligence, AI Institute, Shanghai Jiao Tong University</strong>.
      My research focuses on <strong>perceptual quality evaluation and enhancement</strong> for visual content, spanning
      <strong>PGC</strong>, <strong>UGC</strong>, and <strong>AIGC</strong> scenarios. I am interested in building accurate and robust perceptual models that can better align machine intelligence with human value.
    </p>
  </div>
  <div class="col-lg-4">
    <div class="card border-0 shadow-sm mt-4 mt-lg-0">
      <div class="card-body">
        <h4 class="mb-3">Quick Links</h4>
        <p class="mb-2"><a href="{{ '/publications/' | relative_url }}"><strong>Publications</strong></a></p>
        <p class="mb-2"><a href="{{ '/about/' | relative_url }}"><strong>About</strong></a></p>
        <hr>
        <p class="mb-2"><a href="mailto:zwx8981@sjtu.edu.cn">Email</a></p>
        <p class="mb-2"><a href="https://scholar.google.com/citations?user=KK2nLnQAAAAJ">Google Scholar</a></p>
        <p class="mb-0"><a href="https://github.com/zwx8981">GitHub</a></p>
      </div>
    </div>
  </div>
</div>

<section class="research-map-section">
  <h2 class="research-map-title">Research Directions</h2>

  <div class="research-map-layout">
    <div class="research-side">
      <div class="research-box">
        <h4>Multimedia Quality Assessment</h4>
        <p>
          Focusing on accurate and fair evaluation of multimedia quality, while also serving as a loss function, reward model, or real-time feedback signal in shaping various vision systems.
        </p>
      </div>

      <div class="research-box">
        <h4>Perceptual Optimization</h4>
        <p>
          Working on existing visual content, seeking to enhance, restore, or edit images/videos to improve their perceived quality.
        </p>
      </div>
    </div>

    <div class="research-center">
      <img src="{{ '/assets/research_overview.png' | relative_url }}" alt="Research overview illustration">
    </div>

    <div class="research-side">
      <div class="research-box">
        <h4>Computational Photography</h4>
        <p>
           Targeting the visual capture stage, aiming to produce high-quality images/videos directly at the moment of acquisition.
        </p>
      </div>

      <div class="research-box">
        <h4>Industrial Vision Analysis</h4>
        <p>
          Extending quality assessment from alignment with human visual perception to alignment with task-specific goals, such as object defect detection, safety monitoring of workers, etc.
        </p>
      </div>
    </div>
  </div>
</section>

<p class="mt-4">
  See the <a href="{{ '/publications/' | relative_url }}"><strong>full publications list</strong></a> for more details.
</p>

</div>
