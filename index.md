---
layout: homepage
---

<style>
.research-grid {
  display: grid;
  gap: 10px;
  grid-template-columns: repeat(auto-fit, minmax(185px, 1fr));
  margin: -4px 0 22px;
}

.research-card {
  background: #f8fafc;
  border-left: 3px solid #043361;
  border-radius: 6px;
  padding: 10px 12px;
}

.research-card strong {
  display: block;
  margin-bottom: 4px;
}

.experience-list {
  list-style: none;
  padding-left: 0;
}

.experience-list li {
  margin-bottom: 14px;
}

.experience-title {
  color: #222;
  font-weight: 600;
}

.experience-note {
  display: block;
  margin-top: 4px;
}

@media (prefers-color-scheme: dark) {
  .research-card {
    background: #282936;
    border-left-color: rgb(62, 183, 240);
  }

  .experience-title {
    color: #f0f1f4;
  }
}
</style>

## About Me 👋

I am currently at ByteDance BandAI, working on AIGC, efficient video generation, and agent-oriented AI systems.
Before joining ByteDance full-time, I received my master's degree from the Department of Automation at the University of Science and Technology of China (USTC) in 2026, after completing my bachelor's degree at USTC in June 2023.

My recent work has appeared in ECCV, CVPR, and ACM Multimedia.
I am interested in building efficient, controllable AI systems that connect high-quality generation, multimodal reasoning, and practical tool use.

## Research Interests 🔭

<div class="research-grid">
  <div class="research-card">
    <strong>AIGC ✨</strong>
    <span>Efficient generation, controllable visual generation, and multimodal creation.</span>
  </div>
  <div class="research-card">
    <strong>Efficient AI ⚡</strong>
    <span>Feature caching, single-step generation, and inference efficiency for practical generation systems.</span>
  </div>
  <div class="research-card">
    <strong>Agent 🧭</strong>
    <span>Tool use, multimodal reasoning, and agent workflows for effect generation, evaluation, and iterative refinement.</span>
  </div>
</div>

## News 🗞️

- **[Jul. 2026]** Drift-AR was accepted by ECCV 2026.
- **[Jun. 2026]** I graduated from USTC with a master's degree and joined ByteDance.
- **[Jul. 2025]** AB-Cache was accepted by ACM Multimedia 2025.
- **[Feb. 2025]** Adaptive Dropout was accepted by CVPR 2025.
- **[Jul. 2024]** FreqMamba was accepted by ACM Multimedia 2024.

## Experience 💼

<ul class="experience-list">
  <li>
    <strong>[Jun. 2026 - Present]</strong> <span class="experience-title">ByteDance BandAI</span>
    <span class="experience-note">Full-time position after graduating from USTC.</span>
  </li>
  <li>
    <strong>[Apr. 2025 - Jun. 2026]</strong> <span class="experience-title">ByteDance, Intern</span>
    <span class="experience-note">Worked on inference acceleration for video generation models and agent-related systems.</span>
  </li>
  <li>
    <strong>[Dec. 2024 - Apr. 2025]</strong> <span class="experience-title">TeleAI, Intern</span>
    <span class="experience-note">Participated in training and inference acceleration for VAST, a video generation model.</span>
  </li>
</ul>

{% include_relative _includes/publications.md %}

## Education 🎓

- **[2023 - 2026]** M.S., Department of Automation, University of Science and Technology of China.
- **[2019 - 2023]** B.E., University of Science and Technology of China.
