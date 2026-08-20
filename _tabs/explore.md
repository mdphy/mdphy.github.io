---
title: Explore
icon: fas fa-layer-group
order: 2
---

Explore the different areas of my scientific work, educational materials, and projects.

<style>
.explore-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
  margin: 2rem 0;
}

.explore-card {
  position: relative;
  display: flex;
  align-items: center;
  min-height: 110px;
  padding: 22px;

  border: 1px solid var(--main-border-color);
  border-radius: 18px;

  background: var(--card-bg);
  color: inherit !important;
  text-decoration: none !important;

  overflow: hidden;

  transition:
    transform .22s ease,
    box-shadow .22s ease,
    border-color .22s ease;
}

.explore-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 30px rgba(0,0,0,.12);
  border-color: var(--link-color);
}

.explore-icon {
  width: 58px;
  height: 58px;
  min-width: 58px;

  margin-right: 17px;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 16px;

  background: var(--main-bg);
  color: var(--link-color);

  font-size: 18px;
}

.explore-content {
  min-width: 0;
}

.explore-name {
  display: block;

  font-size: 1.05rem;
  font-weight: 700;
  line-height: 1.3;
}

.explore-description {
  display: block;

  margin-top: 6px;

  font-size: .82rem;
  line-height: 1.4;

  opacity: .65;
}

.explore-arrow {
  margin-left: auto;
  padding-left: 15px;

  font-size: 20px;
  opacity: .45;

  transition:
    transform .22s ease,
    opacity .22s ease;
}

.explore-card:hover .explore-arrow {
  transform: translate(4px,-4px);
  opacity: 1;
}


/* Individual icons */

.explore-lectures .explore-icon {
  color: #4285f4;
}

.explore-visual .explore-icon {
  color: #00a6a6;
}

.explore-research .explore-icon {
  color: #b31b1b;
}

.explore-notes .explore-icon {
  color: #7655a8;
}

.explore-projects .explore-icon {
  color: #d88900;
}


/* Mobile */

@media (max-width: 700px) {

  .explore-grid {
    grid-template-columns: 1fr;
    gap: 14px;
  }

  .explore-card {
    min-height: 92px;
    padding: 18px;
  }

  .explore-icon {
    width: 52px;
    height: 52px;
    min-width: 52px;
    margin-right: 14px;
  }

}
</style>


<div class="explore-grid">

  <a class="explore-card explore-lectures" href="#lectures">

    <div class="explore-icon">
      <i class="fas fa-chalkboard-user"></i>
    </div>

    <div class="explore-content">
      <span class="explore-name">Lectures</span>
      <span class="explore-description">
        Educational materials and lecture notes
      </span>
    </div>

    <span class="explore-arrow">↗</span>

  </a>


  <a class="explore-card explore-visual" href="#visual-science">

    <div class="explore-icon">
      <i class="fas fa-chart-line"></i>
    </div>

    <div class="explore-content">
      <span class="explore-name">Visual Science</span>
      <span class="explore-description">
        Scientific diagrams, visualizations and interactive content
      </span>
    </div>

    <span class="explore-arrow">↗</span>

  </a>


  <a class="explore-card explore-research" href="#research">

    <div class="explore-icon">
      <i class="fas fa-flask"></i>
    </div>

    <div class="explore-content">
      <span class="explore-name">Research</span>
      <span class="explore-description">
        Research ideas, results and ongoing work
      </span>
    </div>

    <span class="explore-arrow">↗</span>

  </a>


  <a class="explore-card explore-notes" href="#scientific-notes">

    <div class="explore-icon">
      <i class="fas fa-pen-to-square"></i>
    </div>

    <div class="explore-content">
      <span class="explore-name">Scientific Notes</span>
      <span class="explore-description">
        Short scientific notes and explanations
      </span>
    </div>

    <span class="explore-arrow">↗</span>

  </a>


  <a class="explore-card explore-projects" href="#projects">

    <div