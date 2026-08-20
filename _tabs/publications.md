---
title: Publications
icon: fas fa-book-open
order: 3
---

Welcome to my publications page. Here you can find my academic profiles.

# Academic Profiles

<style>

/* =========================================
   PUBLICATIONS — ACADEMIC PROFILE CARDS
   ========================================= */

.academic-profiles {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 20px;
  margin: 30px 0;
}


/* =========================================
   CARD
   ========================================= */

.academic-profile-card {
  --accent: #4285f4;

  position: relative;

  display: flex;
  align-items: center;

  min-height: 118px;
  padding: 22px 23px;

  box-sizing: border-box;
  overflow: hidden;

  border: 1px solid rgba(0, 0, 0, 0.08);
  border-radius: 20px;

  background: rgba(255, 255, 255, 0.92);

  color: inherit !important;
  text-decoration: none !important;

  box-shadow:
    0 2px 8px rgba(0, 0, 0, 0.025),
    0 8px 24px rgba(0, 0, 0, 0.035);

  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease,
    border-color 0.25s ease;
}


/* Top accent */

.academic-profile-card::before {
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


/* Hover */

.academic-profile-card:hover {
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

.academic-profile-card:hover::before {
  opacity: 1;
}


/* =========================================
   ICON
   ========================================= */

.academic-profile-icon {
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

  font-size: 16px;
  font-weight: 800;

  letter-spacing: -0.4px;

  transition:
    transform 0.25s ease,
    background 0.25s ease;
}

.academic-profile-card:hover .academic-profile-icon {
  transform: scale(1.06);

  background: color-mix(
    in srgb,
    var(--accent) 16%,
    transparent
  );
}


/* =========================================
   CONTENT
   ========================================= */

.academic-profile-content {
  flex: 1;

  min-width: 0;
}

.academic-profile-name {
  display: block;

  font-size: 1.06rem;
  font-weight: 700;

  line-height: 1.35;

  letter-spacing: -0.01em;
}

.academic-profile-description {
  display: block;

  margin-top: 6px;

  font-size: 0.82rem;
  line-height: 1.5;

  opacity: 0.62;
}


/* =========================================
   ARROW
   ========================================= */

.academic-profile-arrow {
  margin-left: 16px;

  padding-left: 4px;

  font-size: 20px;

  color: var(--accent);

  opacity: 0.35;

  transition:
    transform 0.25s ease,
    opacity 0.25s ease;
}

.academic-profile-card:hover .academic-profile-arrow {
  transform: translate(3px, -3px);

  opacity: 0.95;
}


/* =========================================
   PLATFORM COLORS
   ========================================= */

.academic-scholar {
  --accent: #4285f4;
}

.academic-orcid {
  --accent: #79b82a;
}

.academic-arxiv {
  --accent: #c0392b;
}

.academic-researchgate {
  --accent: #00a99d;
}

.academic-inspire {
  --accent: #7957b5;
}


/* =========================================
   LAST CARD
   ========================================= */

.academic-profile-card:last-child {
  grid-column: 1 / -1;
}


/* =========================================
   INTRODUCTION
   ========================================= */

.academic-profile-intro {
  margin-bottom: 1.8rem;

  opacity: 0.72;
}


/* =========================================
   DARK MODE
   ========================================= */

[data-mode="dark"] .academic-profile-card {
  background: rgba(28, 28, 30, 0.92);

  border-color: rgba(255, 255, 255, 0.09);

  box-shadow:
    0 3px 12px rgba(0, 0, 0, 0.18),
    0 10px 28px rgba(0, 0, 0, 0.22);
}

[data-mode="dark"] .academic-profile-card:hover {
  border-color: color-mix(
    in srgb,
    var(--accent) 35%,
    transparent
  );

  box-shadow:
    0 8px 20px rgba(0, 0, 0, 0.25),
    0 18px 40px rgba(0, 0, 0, 0.32);
}


/* =========================================
   TABLET / MOBILE
   ========================================= */

@media (max-width: 800px) {

  .academic-profiles {
    grid-template-columns: 1fr;

    gap: 15px;

    margin: 26px 0;
  }

  .academic-profile-card:last-child {
    grid-column: auto;
  }

  .academic-profile-card {
    min-height: 105px;

    padding: 19px 20px;

    border-radius: 18px;
  }

  .academic-profile-icon {
    flex-basis: 53px;

    width: 53px;
    height: 53px;

    margin-right: 15px;

    border-radius: 15px;
  }
}


/* =========================================
   SMALL MOBILE
   ========================================= */

@media (max-width: 520px) {

  .academic-profile-card {
    min-height: 96px;

    padding: 17px 16px;

    border-radius: 16px;
  }

  .academic-profile-icon {
    flex-basis: 48px;

    width: 48px;
    height: 48px;

    margin-right: 13px;

    border-radius: 14px;

    font-size: 15px;
  }

  .academic-profile-name {
    font-size: 0.98rem;
  }

  .academic-profile-description {
    font-size: 0.78rem;
  }

  .academic-profile-arrow {
    display: none;
  }
}

</style>


<p class="academic-profile-intro">
Explore my research profiles and publications across major academic platforms.
</p>


<div class="academic-profiles">


  <!-- Google Scholar -->

  <a
    class="academic-profile-card academic-scholar"
    href="https://scholar.google.com/citations?user=c5z8m20AAAAJ&hl=en"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="academic-profile-icon">
      GS
    </div>

    <div class="academic-profile-content">

      <span class="academic-profile-name">
        Google Scholar
      </span>

      <span class="academic-profile-description">
        Publications · Citations · Research impact
      </span>

    </div>

    <span class="academic-profile-arrow">
      ↗
    </span>

  </a>


  <!-- ORCID -->

  <a
    class="academic-profile-card academic-orcid"
    href="https://orcid.org/0009-0001-8380-9328"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="academic-profile-icon">
      iD
    </div>

    <div class="academic-profile-content">

      <span class="academic-profile-name">
        ORCID
      </span>

      <span class="academic-profile-description">
        Persistent researcher identifier
      </span>

    </div>

    <span class="academic-profile-arrow">
      ↗
    </span>

  </a>


  <!-- arXiv -->

  <a
    class="academic-profile-card academic-arxiv"
    href="https://arxiv.org/search/gr-qc?searchtype=author&query=Davari%2C+M"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="academic-profile-icon">
      arXiv
    </div>

    <div class="academic-profile-content">

      <span class="academic-profile-name">
        arXiv
      </span>

      <span class="academic-profile-description">
        Preprints · Gravitational physics · Cosmology
      </span>

    </div>

    <span class="academic-profile-arrow">
      ↗
    </span>

  </a>


  <!-- ResearchGate -->

  <a
    class="academic-profile-card academic-researchgate"
    href="https://www.researchgate.net/profile/Mohammadreza-Davari-3"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="academic-profile-icon">
      RG
    </div>

    <div class="academic-profile-content">

      <span class="academic-profile-name">
        ResearchGate
      </span>

      <span class="academic-profile-description">
        Research · Publications · Collaboration
      </span>

    </div>

    <span class="academic-profile-arrow">
      ↗
    </span>

  </a>


  <!-- INSPIRE-HEP -->

  <a
    class="academic-profile-card academic-inspire"
    href="https://inspirehep.net/authors/2826968"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="academic-profile-icon">
      HEP
    </div>

    <div class="academic-profile-content">

      <span class="academic-profile-name">
        INSPIRE-HEP
      </span>

      <span class="academic-profile-description">
        High-energy physics literature database
      </span>

    </div>

    <span class="academic-profile-arrow">
      ↗
    </span>

  </a>


</div>