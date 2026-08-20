---
title: Explore
icon: fas fa-layer-group
order: 2
---

Explore the different areas of my scientific work, educational materials, and projects.

<style>

/* ================================
   EXPLORE DASHBOARD
   ================================ */

.explore-dashboard {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 20px;
  margin: 32px 0;
}


/* ================================
   CARD
   ================================ */

.explore-item {
  --accent: #4285f4;

  position: relative;
  display: flex;
  align-items: center;

  min-height: 118px;
  padding: 22px 23px;

  overflow: hidden;

  border: 1px solid rgba(0, 0, 0, 0.08);
  border-radius: 20px;

  background: rgba(255, 255, 255, 0.92);

  box-sizing: border-box;

  box-shadow:
    0 2px 8px rgba(0, 0, 0, 0.025),
    0 8px 24px rgba(0, 0, 0, 0.035);

  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease,
    border-color 0.25s ease;
}


/* subtle top accent */

.explore-item::before {
  content: "";

  position: absolute;

  top: 0;
  left: 0;

  width: 100%;
  height: 3px;

  background: var(--accent);

  opacity: 0;

  transition: opacity 0.25s ease;
}


/* hover */

.explore-item:hover {
  transform: translateY(-5px);

  border-color: color-mix(
    in srgb,
    var(--accent) 35%,
    transparent
  );

  box-shadow:
    0 8px 18px rgba(0, 0, 0, 0.06),
    0 18px 38px rgba(0, 0, 0, 0.08);
}

.explore-item:hover::before {
  opacity: 1;
}


/* ================================
   ICON
   ================================ */

.explore-symbol {
  position: relative;

  flex: 0 0 58px;

  width: 58px;
  height: 58px;

  display: flex;
  align-items: center;
  justify-content: center;

  margin-right: 18px;

  border-radius: 17px;

  background: color-mix(
    in srgb,
    var(--accent) 11%,
    transparent
  );

  color: var(--accent);

  font-size: 19px;

  transition:
    transform 0.25s ease,
    background 0.25s ease;
}

.explore-item:hover .explore-symbol {
  transform: scale(1.06);

  background: color-mix(
    in srgb,
    var(--accent) 16%,
    transparent
  );
}


/* ================================
   TEXT
   ================================ */

.explore-text {
  flex: 1;
  min-width: 0;
}

.explore-title {
  font-size: 1.06rem;
  font-weight: 700;
  line-height: 1.35;

  letter-spacing: -0.01em;
}

.explore-description {
  margin-top: 6px;

  font-size: 0.82rem;
  line-height: 1.5;

  opacity: 0.62;
}


/* ================================
   NUMBER
   ================================ */

.explore-number {
  align-self: flex-start;

  margin-right: 16px;
  margin-top: 2px;

  font-size: 0.68rem;
  font-weight: 700;

  letter-spacing: 0.08em;

  color: var(--accent);

  opacity: 0.55;
}


/* ================================
   ARROW
   ================================ */

.explore-link {
  margin-left: 16px;

  font-size: 0.76rem;
  font-weight: 600;

  color: var(--accent);

  opacity: 0.35;

  white-space: nowrap;

  transition:
    opacity 0.25s ease,
    transform 0.25s ease;
}

.explore-item:hover .explore-link {
  opacity: 0.95;

  transform: translate(3px, -2px);
}


/* ================================
   INDIVIDUAL COLORS
   ================================ */

.explore-item-01 {
  --accent: #4285f4;
}

.explore-item-02 {
  --accent: #00a99d;
}

.explore-item-03 {
  --accent: #c0392b;
}

.explore-item-04 {
  --accent: #e39a28;
}

.explore-item-05 {
  --accent: #7957b5;
}


/* ================================
   LAST CARD
   ================================ */

.explore-item-05 {
  grid-column: 1 / -1;
}


/* ================================
   DARK MODE
   ================================ */


/* ================================
   DARK MODE
   ================================ */

html[data-mode="dark"] .explore-item {
  background: #1c1c1e;
  border-color: rgba(255, 255, 255, 0.10);

  box-shadow:
    0 3px 12px rgba(0, 0, 0, 0.25),
    0 10px 28px rgba(0, 0, 0, 0.30);
}

html[data-mode="dark"] .explore-item:hover {
  border-color: color-mix(
    in srgb,
    var(--accent) 35%,
    transparent
  );

  box-shadow:
    0 8px 20px rgba(0, 0, 0, 0.30),
    0 18px 40px rgba(0, 0, 0, 0.38);
}

html[data-mode="dark"] .explore-title {
  color: inherit;
}

html[data-mode="dark"] .explore-description {
  color: inherit;
}

html[data-mode="dark"] .explore-number,
html[data-mode="dark"] .explore-link,
html[data-mode="dark"] .explore-symbol {
  color: var(--accent);
}

/* ================================
   TABLET
   ================================ */

@media (max-width: 800px) {

  .explore-dashboard {
    grid-template-columns: 1fr;

    gap: 15px;

    margin: 26px 0;
  }

  .explore-item {
    min-height: 105px;

    padding: 19px 20px;

    border-radius: 18px;
  }

  .explore-symbol {
    flex-basis: 53px;

    width: 53px;
    height: 53px;

    margin-right: 15px;

    border-radius: 15px;
  }

  .explore-item-05 {
    grid-column: auto;
  }
}


/* ================================
   SMALL MOBILE
   ================================ */

@media (max-width: 520px) {

  .explore-item {
    min-height: 96px;

    padding: 17px 16px;

    border-radius: 16px;
  }

  .explore-symbol {
    flex-basis: 48px;

    width: 48px;
    height: 48px;

    margin-right: 13px;

    border-radius: 14px;

    font-size: 17px;
  }

  .explore-title {
    font-size: 0.98rem;
  }

  .explore-description {
    font-size: 0.78rem;
  }

  .explore-number,
  .explore-link {
    display: none;
  }
}

</style>


<div class="explore-dashboard">


  <!-- 01 -->

  <div class="explore-item explore-item-01">

    <div class="explore-number">
      01
    </div>

    <div class="explore-symbol">
      <i class="fas fa-chalkboard-user"></i>
    </div>

    <div class="explore-text">

      <div class="explore-title">
        Lectures
      </div>

      <div class="explore-description">
        Educational materials, lecture notes, and learning resources.
      </div>

    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <!-- 02 -->

  <div class="explore-item explore-item-02">

    <div class="explore-number">
      02
    </div>

    <div class="explore-symbol">
      <i class="fas fa-chart-line"></i>
    </div>

    <div class="explore-text">

      <div class="explore-title">
        Visual Science
      </div>

      <div class="explore-description">
        Scientific diagrams, visualizations, simulations, and interactive content.
      </div>

    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <!-- 03 -->

  <div class="explore-item explore-item-03">

    <div class="explore-number">
      03
    </div>

    <div class="explore-symbol">
      <i class="fas fa-flask"></i>
    </div>

    <div class="explore-text">

      <div class="explore-title">
        Research
      </div>

      <div class="explore-description">
        Research ideas, scientific results, questions, and ongoing work.
      </div>

    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <!-- 04 -->

  <div class="explore-item explore-item-04">

    <div class="explore-number">
      04
    </div>

    <div class="explore-symbol">
      <i class="fas fa-pen-to-square"></i>
    </div>

    <div class="explore-text">

      <div class="explore-title">
        Scientific Notes
      </div>

      <div class="explore-description">
        Short scientific explanations, ideas, derivations, and notes.
      </div>

    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


  <!-- 05 -->

  <div class="explore-item explore-item-05">

    <div class="explore-number">
      05
    </div>

    <div class="explore-symbol">
      <i class="fas fa-code"></i>
    </div>

    <div class="explore-text">

      <div class="explore-title">
        Projects
      </div>

      <div class="explore-description">
        Scientific software, computational tools, and research projects.
      </div>

    </div>

    <div class="explore-link">
      Explore ↗
    </div>

  </div>


</div>