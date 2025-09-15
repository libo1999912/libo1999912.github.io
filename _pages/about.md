---
title: "李博的个人网站"
author_profile: true
permalink: /
---

<style>
  .home-container {
    display: grid;
    grid-template-columns: 1fr;
    gap: 8px;
    margin-top: 5px;
  }
  
  .welcome-section {
    margin-bottom: 5px;
  }
  
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 10px;
    margin-bottom: 0; /* 减少项目网格底部外边距 */
  }
  
  .project-card {
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 8px;
    background-color: #fff;
    transition: all 0.3s ease;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .project-card:hover {
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transform: translateY(-3px);
  }
  
  @media (min-width: 992px) {
    .projects-grid {
      grid-template-columns: repeat(2, 1fr);
      margin-bottom: 0; /* 大屏幕下也减少底部外边距 */
    }
    
    .project-card {
      max-width: 100%;
    }
  }
</style>

{% include base_path %}

<div class="welcome-section">
  <p>欢迎来到我的个人网站！这里展示我的学术研究和个人项目。</p>
</div>

<div class="home-container">
  <div>
    <h2 style="font-size: 1.4rem; border-bottom: 1px solid #eee; padding-bottom: 10px; margin-bottom: 10px;">精选项目</h2>
    
    <div class="projects-grid">
      <!-- 项目1 -->
      <div class="project-card">
        <div style="display: flex; align-items: center; margin-bottom: 10px;">
          <i class="fas fa-bookmark" style="color: #6a737d; margin-right: 8px; font-size: 1.1rem;"></i>
          <h3 style="margin: 0; font-size: 1.1rem;">
            <a href="https://github.com/libo1999912/Social-Robot-Detection-Project" 
               style="color: #0366d6; text-decoration: none; font-weight: 600;">
              Social-Robot-Detection-Project
            </a>
          </h3>
        </div>
        <p style="font-size: 0.95rem; color: #586069; margin-bottom: 12px; line-height: 1.4;">
          Social Robot Detection on Short Video Platform Based on Random Forest and LDA Model
        </p>
        <div style="display: flex; font-size: 0.85rem; color: #586069;">
          <span style="display: flex; align-items: center; margin-right: 15px;">
            <span style="width: 10px; height: 10px; border-radius: 50%; background-color: #3572A5; margin-right: 5px;"></span>
            Python
          </span>
          <span style="display: flex; align-items: center;">
            <i class="fas fa-star" style="color: #f1c40f; margin-right: 4px;"></i>
            1
          </span>
        </div>
      </div>
      
      <!-- 项目2 -->
      <div class="project-card">
        <div style="display: flex; align-items: center; margin-bottom: 10px;">
          <i class="fas fa-bookmark" style="color: #6a737d; margin-right: 8px; font-size: 1.1rem;"></i>
          <h3 style="margin: 0; font-size: 1.1rem;">
            <a href="https://github.com/libo1999912/A-lightweight-compression-model-based-on-transform" 
               style="color: #0366d6; text-decoration: none; font-weight: 600;">
              A-lightweight-compression-model-based-on-transform
            </a>
          </h3>
        </div>
        <p style="font-size: 0.95rem; color: #586069; margin-bottom: 12px; line-height: 1.4;">
          A-lightweight-compression-model-based-on-transform
        </p>
        <div style="display: flex; font-size: 0.85rem; color: #586069;">
          <span style="display: flex; align-items: center; margin-right: 15px;">
            <span style="width: 10px; height: 10px; border-radius: 50%; background-color: #e34c26; margin-right: 5px;"></span>
            HTML
          </span>
          <span style="display: flex; align-items: center;">
            <i class="fas fa-star" style="color: #f1c40f; margin-right: 4px;"></i>
            3
          </span>
        </div>
      </div>
    </div>
  </div>
</div>
