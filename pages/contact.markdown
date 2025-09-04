---
layout: page
title: Contact
permalink: /contact/
---

<div class="contact-content">
  <h1 class="text-center mb-4">Get In Touch</h1>
  <p class="text-center mb-4">I'm always interested in new opportunities, collaborations, and interesting projects. Let's connect!</p>

  <!-- Contact Information Cards -->
  <div class="contact-info">
    <div class="contact-card">
      <h3>📧 Email</h3>
      <a href="mailto:{{ site.email }}">{{ site.email }}</a>
      <p>Send me an email and I'll get back to you within 24 hours.</p>
    </div>
    
    <div class="contact-card">
      <h3>💼 LinkedIn</h3>
      <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank">linkedin.com/in/{{ site.linkedin_username }}</a>
      <p>Connect with me professionally and see my career updates.</p>
    </div>
    
    <div class="contact-card">
      <h3>🐙 GitHub</h3>
      <a href="https://github.com/{{ site.github_username }}" target="_blank">github.com/{{ site.github_username }}</a>
      <p>Check out my code repositories and contributions.</p>
    </div>
    
    <div class="contact-card">
      <h3>📍 Location</h3>
      <span>{{ site.location }}</span>
      <p>Available for remote work and local opportunities.</p>
    </div>
  </div>

  <!-- Resume Download Section -->
  <div class="resume-section">
    <h2>Download Resume</h2>
    <p>Get a PDF copy of my resume with complete details about my experience, skills, and achievements.</p>
    <div class="cta-buttons">
      <a href="{{ site.resume_url | relative_url }}" class="btn btn-primary" target="_blank">
        📄 Download PDF Resume
      </a>
    </div>
  </div>

  <!-- Contact Form Section -->
  <div class="contact-form-section">
    <h2>Send Me a Message</h2>
    <p>Have a project in mind or want to discuss an opportunity? Fill out the form below and I'll get back to you as soon as possible.</p>
    
    <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
      <div class="form-group">
        <label for="name">Name *</label>
        <input type="text" id="name" name="name" required>
      </div>
      
      <div class="form-group">
        <label for="email">Email *</label>
        <input type="email" id="email" name="email" required>
      </div>
      
      <div class="form-group">
        <label for="subject">Subject *</label>
        <input type="text" id="subject" name="subject" required>
      </div>
      
      <div class="form-group">
        <label for="message">Message *</label>
        <textarea id="message" name="message" rows="6" required></textarea>
      </div>
      
      <button type="submit" class="btn btn-primary">Send Message</button>
    </form>
  </div>

  <!-- Social Media Links -->
  <div class="social-section">
    <h2>Follow Me</h2>
    <p>Stay updated with my latest projects and thoughts on technology.</p>
    
    <div class="social-links">
      <a href="https://github.com/{{ site.github_username }}" class="social-link" target="_blank">
        <span>🐙</span> GitHub
      </a>
      <a href="https://linkedin.com/in/{{ site.linkedin_username }}" class="social-link" target="_blank">
        <span>💼</span> LinkedIn
      </a>
      {% if site.instagram_username %}
      <a href="https://instagram.com/{{ site.instagram_username }}" class="social-link" target="_blank">
        <span>📷</span> Instagram
      </a>
      {% endif %}
    </div>
  </div>

  <!-- Response Time Information -->
  <div class="response-info">
    <h3>Response Time</h3>
    <p>I typically respond to messages within 24 hours during business days. For urgent matters, please mention it in your message subject line.</p>
  </div>
</div>
