---
layout: page
title: Categories
icon: fas fa-layer-group
order: 1
---

<div class="category-dashboard">

  <a class="category-card" href="{{ '/lectures/' | relative_url }}">
    <div class="category-icon">
      <i class="fas fa-chalkboard-user"></i>
    </div>
    <div class="category-content">
      <h2>Lectures</h2>
      <p>Educational materials and lecture notes</p>
    </div>
    <div class="category-arrow">↗</div>
  </a>

  <a class="category-card" href="{{ '/visual-science/' | relative_url }}">
    <div class="category-icon">
      <i class="fas fa-chart-line"></i>
    </div>
    <div class="category-content">
      <h2>Visual Science</h2>
      <p>Scientific diagrams, visualizations and interactive content</p>
    </div>
    <div class="category-arrow">↗</div>
  </a>

  <a class="category-card" href="{{ '/research/' | relative_url }}">
    <div class="category-icon">
      <i class="fas fa-flask"></i>
    </div>
    <div class="category-content">
      <h2>Research</h2>
      <p>Research ideas, results and ongoing work</p>
    </div>
    <div class="category-arrow">↗</div>
  </a>

  <a class="category-card" href="{{ '/scientific-notes/' | relative_url }}">
    <div class="category-icon">
      <i class="fas fa-pen-to-square"></i>
    </div>
    <div class="category-content">
      <h2>Scientific Notes</h2>
      <p>Short scientific notes and explanations</p>
    </div>
    <div class="category-arrow">↗</div>
  </a>

  <a class="category-card" href="{{ '/projects/' | relative_url }}">
    <div class="category-icon">
      <i class="fas fa-code"></i>
    </div>
    <div class="category-content">
      <h2>Projects</h2>
      <p>Scientific software, code and research projects</p>
    </div>
    <div class="category-arrow">↗</div>
  </a>

</div>

<style>

.category-dashboard {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin: 2rem 0;
}

.category-card {
  display: flex;
  align-items: center;
  min-height: 105px;
  padding: 18px;

  border: 1px solid var(--main-border-color);
  border-radius: 16px;

  background: var(--card-bg);
  color: inherit !important;
  text-decoration: none !important;

  transition:
    transform .18s ease,
    border-color .18s ease,
    box-shadow .18s ease;
}

.category-card:hover {
  transform: translateY(-3px);
  border-color: var(--link-color);
  box-shadow: 0 8px 22px rgba(0, 0, 0, .08);
}

.category-icon {
  width: 52px;
  height: 52px;
  min-width: 52px;

  display: flex;
  align-items: center;
  justify-content: center;

  margin-right: 15px;
  border-radius: 14px;

  background: var(--main-bg);
  color: var(--link-color);

  font-size: 18px;
}

.category-content {
  min-width: 0;
}

.category-content h2 {
  margin: 0;
  font-size: 1rem;
  font-weight: 700;
}

.category-content p {
  margin: 5px 0 0;
  font-size: .76rem;
  line-height: 1.4;
  opacity: .58;
}

.category-arrow {
  margin-left: auto;
  padding-left: 12px;
  font-size: 18px;
  opacity: .35;

  transition:
    transform .18s ease,
    opacity .18s ease;
}

.category-card:hover .category-arrow {
  transform: translate(2px, -2px);
  opacity: .85;
}

@media (max-width: 700px) {

  .category-dashboard {
    grid-template-columns: 1fr;
    gap: 11px;
  }

  .category-card {
    min-height: 90px;
    padding: 15px;
  }

  .category-icon {
    width: 48px;
    height: 48px;
    min-width: 48px;
    margin-right: 13px;
  }
}

@media (prefers-reduced-motion: reduce) {

  .category-card,
  .category-arrow {
    transition: none;
  }

  .category-card:hover {
    transform: none;
  }

}

</style>