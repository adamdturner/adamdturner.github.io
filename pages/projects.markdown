---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects-content">
  <h1 class="text-center mb-4">My Projects</h1>
  <p class="text-center mb-4">A collection of projects showcasing my skills in software development, machine learning, and full-stack engineering.</p>

  <div class="projects-grid">
    {% for project in site.projects %}
      <div class="project-card">
        {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
        {% else %}
        <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 1.5rem; font-weight: 600;">
          {{ project.title | slice: 0 }}
        </div>
        {% endif %}
        <div class="project-content">
          <h3 class="project-title">{{ project.title }}</h3>
          <p class="project-description">{{ project.description }}</p>
          
          {% if project.technologies %}
          <div class="project-tech">
            {% for tech in project.technologies limit: 5 %}
              <span class="tech-tag">{{ tech }}</span>
            {% endfor %}
            {% if project.technologies.size > 5 %}
              <span class="tech-tag">+{{ project.technologies.size | minus: 5 }} more</span>
            {% endif %}
          </div>
          {% endif %}

          <div class="project-meta">
            {% if project.duration %}
            <span class="meta-item">{{ project.duration }}</span>
            {% endif %}
            {% if project.status %}
            <span class="meta-item">{{ project.status }}</span>
            {% endif %}
          </div>

          <div class="project-links">
            <a href="{{ project.url | relative_url }}" class="project-link">View Details</a>
            {% if project.github_url %}
            <a href="{{ project.github_url }}" class="project-link" target="_blank">GitHub</a>
            {% endif %}
            {% if project.live_url %}
            <a href="{{ project.live_url }}" class="project-link" target="_blank">Live Demo</a>
            {% endif %}
            {% if project.demo_url %}
            <a href="{{ project.demo_url }}" class="project-link" target="_blank">Demo</a>
            {% endif %}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>

  <!-- Featured Projects Section -->
  <div class="featured-section mt-4">
    <h2 class="text-center mb-4">Featured Projects</h2>
    <div class="projects-grid">
      {% assign featured_projects = site.projects | where: "featured", true %}
      {% for project in featured_projects %}
        <div class="project-card featured-card">
          {% if project.image %}
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
          {% else %}
          <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 1.5rem; font-weight: 600;">
            {{ project.title | slice: 0 }}
          </div>
          {% endif %}
          <div class="project-content">
            <div class="featured-badge">Featured</div>
            <h3 class="project-title">{{ project.title }}</h3>
            <p class="project-description">{{ project.description }}</p>
            
            {% if project.technologies %}
            <div class="project-tech">
              {% for tech in project.technologies limit: 6 %}
                <span class="tech-tag">{{ tech }}</span>
              {% endfor %}
            </div>
            {% endif %}

            <div class="project-links">
              <a href="{{ project.url | relative_url }}" class="project-link">View Details</a>
              {% if project.github_url %}
              <a href="{{ project.github_url }}" class="project-link" target="_blank">GitHub</a>
              {% endif %}
              {% if project.live_url %}
              <a href="{{ project.live_url }}" class="project-link" target="_blank">Live Demo</a>
              {% endif %}
            </div>
          </div>
        </div>
      {% endfor %}
    </div>
  </div>

  <!-- Project Categories -->
  <div class="project-categories mt-4">
    <h2 class="text-center mb-4">Project Categories</h2>
    <div class="categories-grid">
      <div class="category-card">
        <h3>Web Development</h3>
        <p>Full-stack web applications with modern frameworks and technologies</p>
        <div class="category-stats">
          <span>1 Project</span>
        </div>
      </div>
      <div class="category-card">
        <h3>Mobile Development</h3>
        <p>Cross-platform mobile applications and responsive web apps</p>
        <div class="category-stats">
          <span>2 Projects</span>
        </div>
      </div>
      <div class="category-card">
        <h3>Hardware & IoT</h3>
        <p>Embedded systems, robotics, and Internet of Things projects</p>
        <div class="category-stats">
          <span>5 Projects</span>
        </div>
      </div>
    </div>
  </div>
</div>
