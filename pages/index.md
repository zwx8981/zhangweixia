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
.home-bg .list-group-item,
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
</style>

<div class="home-bg">

{% include landing.html %}

<div class="row mt-5">
  <div class="col-lg-8">
    <h2 class="mb-3">Research Overview</h2>
    <p>
      I am an <strong>Associate Research Scientist</strong> at the <strong>MoE Key Lab of Artificial Intelligence, AI Institute, Shanghai Jiao Tong University</strong>.
      My research focuses on <strong>perceptual quality evaluation and enhancement</strong> for visual content, spanning
      <strong>PGC</strong>, <strong>UGC</strong>, and <strong>AIGC</strong> settings.
    </p>
    <p>
      Recent work centers on <strong>blind / no-reference image quality assessment</strong>,
      <strong>cross-dataset generalization</strong>, <strong>continual learning for BIQA</strong>,
      <strong>vision-language quality understanding</strong>, and <strong>human-aligned perceptual modeling</strong>.
    </p>
    <p class="mb-0">
      I am interested in building accurate and robust perceptual models that can better align machine decisions with human visual experience.
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

## Selected Publications

<div class="list-group list-group-flush mb-4">
  <div class="list-group-item px-0">
    <div class="d-flex flex-wrap align-items-center mb-2">
      <span class="badge badge-primary mr-2">TIP 2024</span>
      <strong>Task-Specific Normalization for Continual Learning of Blind Image Quality Models</strong>
    </div>
    <div class="text-muted small">Weixia Zhang, Kede Ma, Guangtao Zhai, Xiaokang Yang</div>
    <div class="mt-2">
      <a class="btn btn-sm btn-outline-primary mr-2 mb-2" href="https://arxiv.org/abs/2107.13429">Paper</a>
      <a class="btn btn-sm btn-outline-dark mr-2 mb-2" href="https://github.com/zwx8981/TSN-IQA">Code</a>
    </div>
  </div>

  <div class="list-group-item px-0">
    <div class="d-flex flex-wrap align-items-center mb-2">
      <span class="badge badge-primary mr-2">TPAMI 2023</span>
      <strong>Continual Learning for Blind Image Quality Assessment</strong>
    </div>
    <div class="text-muted small">Weixia Zhang, Dingquan Li, Chao Ma, Guangtao Zhai, Xiaokang Yang, Kede Ma</div>
    <div class="mt-2">
      <a class="btn btn-sm btn-outline-primary mr-2 mb-2" href="https://arxiv.org/abs/2102.09717">Paper</a>
      <a class="btn btn-sm btn-outline-dark mr-2 mb-2" href="https://github.com/zwx8981/BIQA_CL">Code</a>
    </div>
  </div>

  <div class="list-group-item px-0">
    <div class="d-flex flex-wrap align-items-center mb-2">
      <span class="badge badge-primary mr-2">CVPR 2023</span>
      <strong>Blind Image Quality Assessment via Vision-Language Correspondence: A Multitask Learning Perspective</strong>
    </div>
    <div class="text-muted small">Weixia Zhang, Guangtao Zhai, Wei Ying, Xiaokang Yang, Kede Ma</div>
    <div class="mt-2">
      <a class="btn btn-sm btn-outline-primary mr-2 mb-2" href="https://arxiv.org/abs/2303.14968">Paper</a>
      <a class="btn btn-sm btn-outline-dark mr-2 mb-2" href="https://github.com/zwx8981/LIQE">Code</a>
    </div>
  </div>

  <div class="list-group-item px-0">
    <div class="d-flex flex-wrap align-items-center mb-2">
      <span class="badge badge-primary mr-2">NeurIPS 2022</span>
      <strong>Perceptual Attacks of No-Reference Image Quality Models with Human-in-the-Loop</strong>
    </div>
    <div class="text-muted small">Weixia Zhang, Dingquan Li, Xiongkuo Min, Guangtao Zhai, Guodong Guo, Xiaokang Yang, Kede Ma</div>
    <div class="mt-2">
      <a class="btn btn-sm btn-outline-primary mr-2 mb-2" href="https://arxiv.org/abs/2210.00933">Paper</a>
      <a class="btn btn-sm btn-outline-dark mr-2 mb-2" href="https://github.com/zwx8981/PerceptualAttack_BIQA">Code</a>
    </div>
  </div>

  <div class="list-group-item px-0">
    <div class="d-flex flex-wrap align-items-center mb-2">
      <span class="badge badge-primary mr-2">TIP 2021</span>
      <strong>Uncertainty-aware Blind Image Quality Assessment in the Laboratory and Wild</strong>
    </div>
    <div class="text-muted small">Weixia Zhang, Kede Ma, Guangtao Zhai, Xiaokang Yang</div>
    <div class="mt-2">
      <a class="btn btn-sm btn-outline-primary mr-2 mb-2" href="https://arxiv.org/abs/2005.13983">Paper</a>
      <a class="btn btn-sm btn-outline-dark mr-2 mb-2" href="https://github.com/zwx8981/UNIQUE">Code</a>
    </div>
  </div>
</div>

<p>
  See the <a href="{{ '/publications/' | relative_url }}"><strong>full publications list</strong></a> for journal articles, conference papers, preprints, and thesis information.
</p>

</div>
