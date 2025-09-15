---
layout: single
title: "欢迎访问李博的个人网站"
permalink: /
author_profile: true
---

{% include base_path %}

<div class="home-content">
  <div class="home-left">
    <!-- 左侧内容保持不变 -->
    {{ content }}
  </div>
  
  <div class="home-right">
    <!-- 添加项目展示区 -->
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
  </div>
</div>
