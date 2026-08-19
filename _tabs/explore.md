---
layout: page
title: Explore
icon: fas fa-layer-group
order: 3
---

<div class="explore-grid">

  <a class="explore-card" href="#lectures">
    <div class="explore-icon">
      <i class="fas fa-chalkboard-user"></i>
    </div>

    <div class="explore-content">
      <h2>Lectures</h2>
      <p>Educational materials and lecture notes</p>
    </div>

    <span class="explore-arrow">↗</span>
  </a>


  <a class="explore-card" href="#visual-science">
    <div class="explore-icon">
      <i class="fas fa-chart-line"></i>
    </div>

    <div class="explore-content">
      <h2>Visual Science</h2>
      <p>Scientific diagrams and visualizations</p>
    </div>

    <span class="explore-arrow">↗</span>
  </a>


  <a class="explore-card" href="#research">
    <div class="explore-icon">
      <i class="fas fa-flask"></i>
    </div>

    <div class="explore-content">
      <h2>Research</h2>
      <p>Research ideas, results and ongoing work</p>
    </div>

    <span class="explore-arrow">↗</span>
  </a>


  <a class="explore-card" href="#scientific-notes">
    <div class="explore-icon">
      <i class="fas fa-pen-to-square"></i>
    </div>

    <div class="explore-content">
      <h2>Scientific Notes</h2>
      <p>Short scientific notes and explanations</p>
    </div>

    <span class="explore-arrow">↗</span>
  </a>


  <a class="explore-card" href="#projects">
    <div class="explore-icon">
      <i class="fas fa-code"></i>
    </div>

    <div class="explore-content">
      <h2>Projects</h2>
      <p>Scientific software and research projects</p>
    </div>

    <span class="explore-arrow">↗</span>
  </a>

</div>

<style>

.explore-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin: 2rem 0;
}

.explore-card {
  display: flex;
  align-items: center;
  gap: 15px;

  min-height: 105px;
  padding: 17px;

  border: 1px solid var(--main-border-color);
  border-radius: 16px;

  color: inherit !important;
  text-decoration: none !important;

  transition:
    transform .18s ease,
    border-color .18s ease,
    box-shadow .18s ease;
}

.explore-card:hover {
  transform: translateY(-3px);
  border-color: var(--link-color);
  box-shadow: 0 8px 24px rgba(0, 0, 0, .08);
}

.explore-icon {
  width: 50px;
  height: 50px;
  min-width: 50px;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 13px;

  background: var(--main-bg);
  color: var(--link-color);

  font-size: 18px;
}

.explore-content {
  min-width: 0;
}

.explore-content h2 {
  margin: 0;

  font-size: 1rem;
  font-weight: 700;
}

.explore-content p {
  margin: 5px 0 0;

  font-size: .74rem;
  line-height: 1.45;

  opacity: .55;
}

.explore-arrow {
  margin-left: auto;
  font-size: 18px;
  opacity: .35;
}

.explore-card:hover .explore-arrow {
  transform: translate(2px, -2px);
  opacity: .85;
}

@media (max-width: 700px) {

  .explore-grid {
    grid-template-columns: 1fr;
    gap: 11px;
  }

  .explore-card {
    min-height: 92px;
    padding: 15px;
  }

  .explore-icon {
    width: 47px;
    height: 47px;
    min-width: 47px;
  }

}

@media (prefers-reduced-motion: reduce) {

  .explore-card,
  .explore-arrow {
    transition: none;
  }

  .explore-card:hover {
    transform: none;
  }

}

</style>