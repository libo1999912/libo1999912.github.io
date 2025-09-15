{% if page.header.overlay_color or page.header.overlay_image or page.header.image %}
  {% include page__hero.html %}
{% elsif page.header.video.id and page.header.video.provider %}
  {% include page__hero_video.html %}
{% endif %}

<div id="main" role="main">
  <article class="splash" itemscope itemtype="https://schema.org/CreativeWork">
    {% if page.title %}<meta itemprop="headline" content="{{ page.title | markdownify | strip_html | strip_newlines | escape_once }}">{% endif %}
    {% if page.excerpt %}<meta itemprop="description" content="{{ page.excerpt | markdownify | strip_html | strip_newlines | escape_once }}">{% endif %}
    {% if page.date %}<meta itemprop="datePublished" content="{{ page.date | date_to_xmlschema }}">{% endif %}
    {% if page.last_modified_at %}<meta itemprop="dateModified" content="{{ page.last_modified_at | date_to_xmlschema }}">{% endif %}

    <section class="page__content" itemprop="text">
      <!-- 添加右侧项目展示区域 -->
      <div class="featured-projects">
        <h2 class="featured-projects__title">精选项目</h2>
        <div class="featured-projects__grid">
          {% for project in site.data.featured_projects %}
            <div class="featured-project-card">
              <div class="featured-project-card__header">
                <span class="featured-project-card__icon">
                  <i class="fas fa-bookmark"></i>
                </span>
                <h3 class="featured-project-card__title">
                  <a href="{{ project.url }}" target="_blank">{{ project.name }}</a>
                </h3>
              </div>
              <p class="featured-project-card__description">{{ project.description }}</p>
              <div class="featured-project-card__meta">
                <span class="featured-project-card__language">
                  <span class="featured-project-card__language-color" style="background-color: {{ project.language_color }};"></span>
                  {{ project.language }}
                </span>
                <span class="featured-project-card__stars">
                  <i class="fas fa-star"></i>
                  {{ project.stars }}
                </span>
              </div>
            </div>
          {% endfor %}
        </div>
      </div>
      
      <!-- 原有内容保持不变 -->
      {{ content }}
    </section>
  </article>
</div>



