---
title: Explore
icon: fas fa-layer-group
order: 2
---

Explore the different areas of my scientific work, educational materials, and projects.

<style>

.explore-dashboard {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
  margin: 30px 0;
}

.explore-item {
  position: relative;
  display: flex;
  align-items: center;

  min-height: 110px;
  padding: 20px 22px;

  border: 1px solid #d9d9d9;
  border-radius: 18px;

  background: #ffffff;

  box-sizing: border-box;

  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease,
    border-color 0.25s ease;
}

.explore-item:hover {
  transform: translateY(-5px);
  border-color: #b5b5b5;
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.10);
}


/* Icon */

.explore-symbol {
  flex: 0 0 58px;

  width: 58px;
  height: 58px;

  display: flex;
  align-items: center;
  justify-content: center;

  margin-right: 17px;

  border-radius: 15px;

  background: #f0f0f0;

  font-size: 18px;
}


/* Text */

.explore-text {
  flex: 1;
  min-width: 0;
}

.explore-title {
  font-size: 1.05rem;
  font-weight: 700;
  line-height: 1.35;
}

.explore-description {
  margin-top: 5px;

  font-size: 0.82rem;
  line-height: 1.4;

  opacity: 0.65;
}


/* Number */

.explore-number {
  margin-right: 15px;

  font-size: 0.70rem;
  font-weight: 700;

  opacity: 0.35;
}


/* Arrow */

.explore-link {
  margin-left: 15px;

  font-size: 0.78rem;

  opacity: 0.45;

  white-space: nowrap;

  transition:
    opacity 0.25s ease,
    transform 0.25s ease;
}

.explore-item:hover .explore-link {
  opacity: 1;
  transform: translate(2px, -2px);
}


/* Individual icons */

.explore-item-01 .explore-symbol {
  background: rgba(66, 133, 244, 0.12);
}

.explore-item-02 .explore-symbol {
  background: rgba(0, 170, 160, 0.12);
}

.explore-item-03 .explore-symbol {
  background: rgba(180, 40, 40, 0.12);
}

.explore-item-04 .explore-symbol {
  background: rgba(230, 150, 40, 0.13);
}

.explore-item-05 .explore-symbol {
  background: rgba(120, 90, 190, 0.12);
}


/* Last card */

.explore-item-05 {
  grid-column: 1 / -1;
}


/* Dark mode */

[data-mode="dark"] .explore-item {
  background: #1b1b1b;
  border-color: #3a3a3a;
}

[data-mode="dark"] .explore-item:hover {
  border-color: #555555;
  box-shadow: 0 14px 35px rgba(0, 0, 0, 0.35);
}


/* Mobile */

@media (max-width: 800px) {

  .explore-dashboard {
    grid-template-columns: 1fr;
    gap: 14px;
  }

  .explore-item {
    min-height: 95px;
    padding: 17px 18px;
  }

  .explore-symbol {
    flex-basis: 52px;
    width: 52px;
    height: 52px;

    margin-right: 14px;
  }

  .explore-item-05 {
    grid-column: auto;
  }

}


@media (max-width: 520px) {

  .explore-number {
    display: none;
  }

  .explore-link {
    display: none;
  }

}

</style>


<div class="explore-dashboard">

  <div class="explore-item explore-item-01">

    <div class="explore-number">01</div>

    <div class="explore-symbol">
      <i class="fas fa-chalkboard-user"></i>
    </div>

    <div class="explore-text">
      <div class="explore-title">Lectures</div>
      <div class="explore-description">
        Educational materials, lecture notes, and learning resources.
      </div>
    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <div class="explore-item explore-item-02">

    <div class="explore-number">02</div>

    <div class="explore-symbol">
      <i class="fas fa-chart-line"></i>
    </div>

    <div class="explore-text">
      <div class="explore-title">Visual Science</div>
      <div class="explore-description">
        Scientific diagrams, visualizations, simulations, and interactive content.
      </div>
    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <div class="explore-item explore-item-03">

    <div class="explore-number">03</div>

    <div class="explore-symbol">
      <i class="fas fa-flask"></i>
    </div>

    <div class="explore-text">
      <div class="explore-title">Research</div>
      <div class="explore-description">
        Research ideas, scientific results, questions, and ongoing work.
      </div>
    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <div class="explore-item explore-item-04">

    <div class="explore-number">04</div>

    <div class="explore-symbol">
      <i class="fas fa-pen-to-square"></i>
    </div>

    <div class="explore-text">
      <div class="explore-title">Scientific Notes</div>
      <div class="explore-description">
        Short scientific explanations, ideas, derivations, and notes.
      </div>
    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <div class="explore-item explore-item-05">

    <div class="explore-number">05</div>

    <div class="explore-symbol">
      <i class="fas fa-code"></i>
    </div>

    <div class="explore-text">
      <div class="explore-title">Projects</div>
      <div class="explore-description">
        Scientific software, computational tools, and research projects.
      </div>
    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>

</div>