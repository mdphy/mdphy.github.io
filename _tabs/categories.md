---
layout: page
title: Categories
icon: fas fa-layer-group
order: 3
---

<div class="category-dashboard">

  {% assign category_names = "Lectures|Visual Science|Research|Scientific Notes|Projects" | split: "|" %}

  {% for category_name in category_names %}

    {% assign category_slug = category_name | slugify %}
    {% assign category_posts = site.categories[category_name] %}
    {% assign category_count = category_posts | size %}

    <a
      class="category-card"
      href="{{ '/categories/' | append: category_slug | append: '/' | relative_url }}"
    >

      <div class="category-icon">

        {% if category_name == "Lectures" %}
          <i class="fas fa-chalkboard-user"></i>

        {% elsif category_name == "Visual Science" %}
          <i class="fas fa-chart-line"></i>

        {% elsif category_name == "Research" %}
          <i class="fas fa-flask"></i>

        {% elsif category_name == "Scientific Notes" %}
          <i class="fas fa-pen-to-square"></i>

        {% elsif category_name == "Projects" %}
          <i class="fas fa-code"></i>
        {% endif %}

      </div>

      <div class="category-content">

        <h2>{{ category_name }}</h2>

        <p>

          {% if category_name == "Lectures" %}
            Educational materials and lecture notes

          {% elsif category_name == "Visual Science" %}
            Scientific diagrams, visualizations and interactive content

          {% elsif category_name == "Research" %}
            Research ideas, results and ongoing work

          {% elsif category_name == "Scientific Notes" %}
            Short scientific notes and explanations

          {% elsif category_name == "Projects" %}
            Scientific software, code and research projects
          {% endif %}

        </p>

        <span class="category-count">
          {{ category_count }}
          {% if category_count == 1 %}
            post
          {% else %}
            posts
          {% endif %}
        </span>

      </div>

      <div class="category-arrow">↗</div>

    </a>

  {% endfor %}

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

  min-height: 112px;
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

  line-height: 1.3;
}

.category-content p {
  margin: 5px 0 0;

  font-size: .76rem;
  line-height: 1.4;

  opacity: .58;
}

.category-count {
  display: block;

  margin-top: 7px;

  font-size: .68rem;
  font-weight: 600;

  opacity: .42;
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
    min-height: 92px;
    padding: 15px;

    border-radius: 14px;
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