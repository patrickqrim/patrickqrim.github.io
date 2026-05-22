---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.exp-block {
  display: flex;
  gap: 1.25rem;
  margin-bottom: 1.4rem;
  align-items: flex-start;
}
.exp-logo {
  flex: 0 0 17%;
  max-width: 17%;
  text-align: center;
  padding-top: 0.15rem;
}
.exp-logo img {
  width: 100%;
  height: auto;
  max-height: 38px;
  object-fit: contain;
}
.exp-dates {
  font-size: 0.72rem;
  color: #777;
  margin-top: 0.3rem;
  line-height: 1.3;
}
.exp-text {
  flex: 1 1 0;
  font-size: 0.95rem;
  line-height: 1.5;
}
.home-section {
  position: relative;
  padding-top: 0.35rem;
}
.home-section__flare {
  position: relative;
  height: 3px;
  margin: 0.45rem 0 1.1rem;
  overflow: hidden;
  background: linear-gradient(90deg, #d9dfe3, #e9edf0, #d9dfe3);
  background-size: 220% 100%;
  border-radius: 999px;
  animation: section-line-breathe 7s ease-in-out infinite;
}
.home-section__flare::before {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(90deg, transparent 0%, rgba(111,143,168,0.2) 18%, rgba(214,168,79,0.55) 50%, rgba(122,168,134,0.22) 82%, transparent 100%);
  background-size: 240% 100%;
  opacity: 0.75;
  animation: section-flare-dance 5.5s ease-in-out infinite;
}
.home-section__flare::after {
  content: none;
}
.home-section.is-sparked .home-section__flare {
  animation: section-line-breathe 7s ease-in-out infinite, section-line-intensify 1500ms ease-out;
}
.home-section.is-sparked .home-section__flare::before {
  animation: section-flare-dance 5.5s ease-in-out infinite, section-stream-intensify 1500ms ease-out;
}
.home-section h2 {
  font-family: "Avenir Next", "Avenir", "Century Gothic", sans-serif;
}
.home-pubs p > a:first-child {
  font-family: "Avenir Next Medium", "Avenir Next", "Avenir", "Century Gothic", sans-serif;
  font-weight: 500;
}
.home-pubs .venue {
  font-family: inherit;
  font-style: normal;
  background: linear-gradient(90deg, #557d9b 0%, #b28a3e 42%, #6d987b 68%, #557d9b 100%);
  background-size: 240% 100%;
  -webkit-background-clip: text;
  background-clip: text;
  color: #557d9b;
  -webkit-text-fill-color: transparent;
  animation: venue-color-wave 5.5s ease-in-out infinite;
}
.equal-contribution {
  display: inline-block;
  margin-top: 0.2rem;
  text-align: left;
  font-size: 0.875em;
  color: #777;
}
.equal-contribution__line {
  border-top: 1px solid #d6d6d6;
  width: 100%;
  margin-bottom: 3px;
}
@keyframes section-line-breathe {
  0%, 100% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
}
@keyframes section-flare-dance {
  0%, 100% { background-position: 0% 50%; opacity: 0.45; }
  45% { background-position: 100% 50%; opacity: 0.82; }
  70% { background-position: 55% 50%; opacity: 0.62; }
}
@keyframes section-line-intensify {
  0%, 100% { box-shadow: none; filter: saturate(1); }
  28%, 62% {
    box-shadow: 0 0 14px rgba(85,125,155,0.34), 0 0 30px rgba(214,168,79,0.32);
    filter: saturate(1.9) brightness(1.08);
  }
}
@keyframes section-stream-intensify {
  0%, 100% { opacity: 0.75; }
  28%, 62% { opacity: 1; }
}
@keyframes venue-color-wave {
  0%, 100% { background-position: 0% 50%; }
  45% { background-position: 100% 50%; }
  70% { background-position: 55% 50%; }
}
@media (prefers-reduced-motion: reduce) {
  .home-section__flare,
  .home-section__flare::before,
  .home-section.is-sparked .home-section__flare::before {
    animation: none;
  }
  .home-pubs .venue {
    animation: none;
  }
}
@media (max-width: 640px) {
  .home-section:first-of-type { margin-top: 1.1rem; }
  .exp-block { gap: 0.9rem; }
  .exp-logo { flex: 0 0 26%; max-width: 26%; }
  .exp-text { font-size: 0.9rem; }
}
</style>

<section class="home-section" data-section-flare>

<div class="exp-block">
  <div class="exp-logo">
    <img src="/images/logo-yale.svg" alt="Yale University">
    <div class="exp-dates">2024 – 2028</div>
  </div>
  <div class="exp-text">
    <strong>Yale University</strong> · Ph.D., Computer Science
    <p style="margin:0.2rem 0 0 0;">Researching 3D computer vision and multimodal AI systems at Yale Vision Lab.</p>
  </div>
</div>

<div class="exp-block">
  <div class="exp-logo">
    <img src="/images/logo-caltech.svg" alt="Caltech" style="max-height:30px;">
    <div class="exp-dates">2020 – 2024</div>
  </div>
  <div class="exp-text">
    <strong>Caltech</strong> · B.S., Computer Science &amp; Applied Mathematics (minor)
    <p style="margin:0.2rem 0 0 0;">Awarded in recognition of the Best Academic Record in Computer Science.</p>
  </div>
</div>

<hr style="border:none;border-top:1px solid #e1e1e1;margin:0.5rem 0 1.1rem;">

<div class="exp-block">
  <div class="exp-logo">
    <img src="/images/logo-google.svg" alt="Google">
    <div class="exp-dates">May 2026 – Present</div>
  </div>
  <div class="exp-text">
    <strong>Google</strong> · Research Intern
    <p style="margin:0.2rem 0 0 0;">Building real-time streaming 3D reconstruction and end-to-end transformer-based SLAM, integrating open-vocabulary semantic distillation from Gemini to power robotic manipulation, navigation, and AR/VR applications.</p>
  </div>
</div>

<div class="exp-block">
  <div class="exp-logo">
    <img src="/images/logo-nvidia.svg" alt="NVIDIA">
    <div class="exp-dates">Feb 2026 – May 2026</div>
  </div>
  <div class="exp-text">
    <strong>NVIDIA Research</strong> · Research Scientist Intern
    <p style="margin:0.2rem 0 0 0;">Led the creation of Spatial-IQ, a novel hierarchical framework that deconstructs spatial reasoning in multimodal LLMs. Post-training on Spatial-IQ via chained SFT-CoT and RLVR improves spatial intelligence.</p>
  </div>
</div>

<div class="exp-block">
  <div class="exp-logo">
    <img src="/images/logo-meta.svg" alt="Meta Reality Labs">
    <div class="exp-dates">May 2025 – Jan 2026</div>
  </div>
  <div class="exp-text">
    <strong>Meta Reality Labs</strong> · Research Scientist Intern
    <p style="margin:0.2rem 0 0 0;">Led the creation of SHOW3D, the first ever hand-object interaction dataset captured in the wild. The most valuable 4.6 million frames of egocentric data ever captured, open-sourced for the community!</p>
  </div>
</div>

</section>

<section class="home-section" data-section-flare markdown="1">
<div class="home-section__flare" aria-hidden="true"></div>

## What I Research and Why

My work is centered on building embodied AI agents capable of adaptive, efficient, and robust physical perception. My research bridges the gap between digital reasoning and the physical world by integrating multimodal capabilities across vision, language, and range sensing.

What coding agents did for white-collar workflows, physical AI will do for all of humankind.

</section>

<section class="home-section" data-section-flare markdown="1">
<div class="home-section__flare" aria-hidden="true"></div>

## Recent Publications

<div class="home-pubs" markdown="1">

[SHOW3D: Capturing Scenes of 3D Hands and Objects in the Wild](https://protodepth.github.io/)  
**Patrick Rim**, Kevin Harris, Braden Copple, Shangchen Han, Xu Xie, Ivan Shugurov, Sizhe An, He Wen, Alex Wong, Tomas Hodan, Kun He  
<span class="venue">CVPR 2026</span>

[Radar-Guided Polynomial Fitting for Metric Depth Estimation](https://arxiv.org/abs/2503.17182)  
**Patrick Rim**, Hyoungseob Park, Vadim Ezhov, Jeffrey Moon, Alex Wong  
<span class="venue">CVPR 2026</span>

[Iris: Integrating Language into Diffusion-based Monocular Depth Estimation](https://arxiv.org/abs/2411.16750)  
Ziyao Zeng, Jingcheng Ni, Daniel Wang, **Patrick Rim**, Younjoon Chung, Fengyu Yang, Byung-Woo Hong, Alex Wong  
<span class="venue">CVPR 2026</span>

[ODE-GS: Latent ODEs for Dynamic Scene Extrapolation with 3D Gaussian Splatting](https://arxiv.org/abs/2506.05480)  
Daniel Wang, **Patrick Rim**, Tian Tian, Alex Wong, Ganesh Sundaramoorthi  
<span class="venue">ICLR 2026</span>

[Unsupervised Depth Completion via Occluded Region Completion as Supervision](https://arxiv.org/abs/2506.05480)  
Hyoungseob Park, Runjian Chen, **Patrick Rim**, Dong Lao, Alex Wong  
<span class="venue">ICLR 2026</span>

[ProtoDepth: Unsupervised Continual Depth Completion with Prototypes](https://protodepth.github.io/)  
**Patrick Rim**, Hyoungseob Park, S. Gangopadhyay, Ziyao Zeng, Younjoon Chung, Alex Wong  
<span class="venue">CVPR 2025</span>

[ETA: Energy-based Test-time Adaptation for Depth Completion](https://arxiv.org/abs/2508.05989)  
Younjoon Chung\*, Hyoungseob Park\*, **Patrick Rim\***, Xiaoran Zhang, Jihe He, Ziyao Zeng, Safa Cicek, Byung-Woo Hong, James S. Duncan, Alex Wong  
<span class="venue">ICCV 2025</span>

[Extending Foundational Monocular Depth Estimators to Fisheye Cameras with Calibration Tokens](https://www.arxiv.org/abs/2508.04928)  
S. Gangopadhyay\*, Jung-Hee Kim\*, Xien Chen\*, **Patrick Rim**, Hyoungseob Park, Alex Wong  
<span class="venue">ICCV 2025</span>

[SparseFusion: Fusing Multi-Modal Sparse Representations for Multi-Sensor 3D Object Detection](https://github.com/yichen928/SparseFusion)  
Yichen Xie, Chenfeng Xu, MJ Rakotosaona, **Patrick Rim**, Federico Tombari, Kurt Keutzer, Masayoshi Tomizuka, Wei Zhan  
<span class="venue">ICCV 2023</span>

[Quadric Representations for LiDAR Odometry, Mapping and Localization](https://ieeexplore.ieee.org/document/10167749)  
Chao Xia\*, Chenfeng Xu\*, **Patrick Rim**, Mingyu Ding, Nanning Zheng, Kurt Keutzer, Masayoshi Tomizuka, Wei Zhan  
<span class="venue">RA-L 2023</span>

</div>

<div class="equal-contribution">
  <div class="equal-contribution__line"></div>
  * denotes Equal Contribution
</div>

</section>

<script>
document.addEventListener("DOMContentLoaded", function() {
  var sections = document.querySelectorAll("[data-section-flare]");
  if (!sections.length || !("IntersectionObserver" in window)) return;

  var flare = function(section) {
    section.classList.remove("is-sparked");
    void section.offsetWidth;
    section.classList.add("is-sparked");
  };

  var observer = new IntersectionObserver(function(entries) {
    entries.forEach(function(entry) {
      var wasVisible = entry.target.getAttribute("data-flare-visible") === "true";
      var isVisible = entry.intersectionRatio > 0.35;
      var isLeaving = wasVisible && entry.intersectionRatio < 0.08;

      if (isVisible && !wasVisible) {
        entry.target.setAttribute("data-flare-visible", "true");
        flare(entry.target);
      } else if (isLeaving) {
        entry.target.setAttribute("data-flare-visible", "false");
        flare(entry.target);
      }
    });
  }, { threshold: [0, 0.08, 0.35], rootMargin: "-8% 0px -20% 0px" });

  sections.forEach(function(section) {
    observer.observe(section);
  });
});
</script>
