---
layout: page
title: Resume
permalink: /resume/
---

<div class="resume-content">
  <h1 class="text-center mb-4">Resume & CV</h1>
  <p class="text-center mb-4">Download my resume or view my professional experience and qualifications below.</p>

  <!-- Resume Download Section -->
  <div class="resume-section">
    <h2>Download Resume</h2>
    <p>Get a PDF copy of my resume with complete details about my experience, skills, and achievements.</p>
    <div class="cta-buttons">
      <a href="{{ site.resume_url | relative_url }}" class="btn btn-primary" target="_blank">
        📄 Download PDF Resume
      </a>
      <a href="mailto:{{ site.email }}" class="btn btn-secondary">
        📧 Contact Me
      </a>
    </div>
  </div>

  <!-- Professional Summary -->
  <div class="about-section">
    <h2>Professional Summary</h2>
    <p>Passionate software developer with 3+ years of experience in full-stack development, machine learning, and system design. Proven track record of delivering high-quality solutions and leading technical projects from conception to deployment.</p>
    
    <div class="summary-highlights">
      <div class="highlight-item">
        <strong>3+ Years</strong> of professional development experience
      </div>
      <div class="highlight-item">
        <strong>15+ Projects</strong> completed across various technologies
      </div>
      <div class="highlight-item">
        <strong>5+ Languages</strong> proficient in programming
      </div>
      <div class="highlight-item">
        <strong>100%</strong> project delivery success rate
      </div>
    </div>
  </div>

  <!-- Technical Skills Summary -->
  <div class="about-section">
    <h2>Core Technical Skills</h2>
    <div class="skills-summary">
      <div class="skill-group">
        <h3>Programming Languages</h3>
        <p>Python, JavaScript, TypeScript, Java, C++, Go</p>
      </div>
      <div class="skill-group">
        <h3>Web Technologies</h3>
        <p>React, Vue.js, Node.js, Express, Django, Flask</p>
      </div>
      <div class="skill-group">
        <h3>Databases</h3>
        <p>PostgreSQL, MongoDB, Redis, MySQL</p>
      </div>
      <div class="skill-group">
        <h3>Cloud & DevOps</h3>
        <p>AWS, Docker, Kubernetes, CI/CD, Linux</p>
      </div>
      <div class="skill-group">
        <h3>Machine Learning</h3>
        <p>TensorFlow, PyTorch, Scikit-learn, Pandas, NumPy</p>
      </div>
    </div>
  </div>

  <!-- Professional Experience -->
  <div class="about-section">
    <h2>Professional Experience</h2>
    
    <div class="experience-item">
      <div class="experience-header">
        <h3>Senior Software Developer</h3>
        <span class="company">Tech Solutions Inc.</span>
        <span class="duration">2022 - Present</span>
      </div>
      <ul>
        <li>Led development of microservices architecture serving 100K+ users</li>
        <li>Implemented CI/CD pipelines reducing deployment time by 60%</li>
        <li>Mentored junior developers and conducted code reviews</li>
        <li>Designed and developed RESTful APIs with 99.9% uptime</li>
        <li>Collaborated with cross-functional teams on product roadmap</li>
      </ul>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Full-Stack Developer</h3>
        <span class="company">Digital Innovations LLC</span>
        <span class="duration">2021 - 2022</span>
      </div>
      <ul>
        <li>Developed responsive web applications using React and Node.js</li>
        <li>Integrated third-party APIs and payment processing systems</li>
        <li>Optimized database queries improving performance by 40%</li>
        <li>Implemented automated testing reducing bugs by 50%</li>
        <li>Worked with Agile development methodology</li>
      </ul>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Software Developer Intern</h3>
        <span class="company">StartupXYZ</span>
        <span class="duration">2020 - 2021</span>
      </div>
      <ul>
        <li>Assisted in developing mobile applications using React Native</li>
        <li>Participated in code reviews and team meetings</li>
        <li>Contributed to documentation and testing procedures</li>
        <li>Gained experience with version control and collaborative development</li>
      </ul>
    </div>
  </div>

  <!-- Education -->
  <div class="about-section">
    <h2>Education</h2>
    
    <div class="education-item">
      <div class="education-header">
        <h3>Bachelor of Science in Computer Science</h3>
        <span class="institution">University of Technology</span>
        <span class="duration">2018 - 2022</span>
      </div>
      <p>Graduated Magna Cum Laude with focus on Software Engineering and Machine Learning</p>
      <ul>
        <li>Relevant Coursework: Data Structures, Algorithms, Database Systems, Machine Learning</li>
        <li>Senior Project: Developed AI-powered recommendation system</li>
        <li>GPA: 3.8/4.0</li>
      </ul>
    </div>
  </div>

  <!-- Certifications -->
  <div class="about-section">
    <h2>Certifications & Achievements</h2>
    
    <div class="certifications-grid">
      <div class="cert-item">
        <h3>AWS Certified Developer Associate</h3>
        <p>Amazon Web Services</p>
        <span class="cert-date">2023</span>
      </div>
      <div class="cert-item">
        <h3>Google Cloud Professional Developer</h3>
        <p>Google Cloud Platform</p>
        <span class="cert-date">2023</span>
      </div>
      <div class="cert-item">
        <h3>Certified Kubernetes Application Developer</h3>
        <p>Cloud Native Computing Foundation</p>
        <span class="cert-date">2022</span>
      </div>
      <div class="cert-item">
        <h3>Meta Frontend Developer Certificate</h3>
        <p>Meta (Facebook)</p>
        <span class="cert-date">2022</span>
      </div>
    </div>
  </div>

  <!-- Contact Information -->
  <div class="about-section">
    <h2>Contact Information</h2>
    
    <div class="contact-info">
      <div class="contact-card">
        <h3>📧 Email</h3>
        <a href="mailto:{{ site.email }}">{{ site.email }}</a>
      </div>
      <div class="contact-card">
        <h3>💼 LinkedIn</h3>
        <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank">linkedin.com/in/{{ site.linkedin_username }}</a>
      </div>
      <div class="contact-card">
        <h3>🐙 GitHub</h3>
        <a href="https://github.com/{{ site.github_username }}" target="_blank">github.com/{{ site.github_username }}</a>
      </div>
      <div class="contact-card">
        <h3>📍 Location</h3>
        <span>{{ site.location }}</span>
      </div>
    </div>
  </div>
</div>
