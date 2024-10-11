---
layout: archive
title:
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    body {
      margin: 0;
      padding: 20px;
    }
    .container {
      margin: 0 auto;
      padding: 20px;
    }
    h2.section-title {
      border-bottom: 2px solid;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }
    h2 {
        color: #007bff;
    }
    h3 i {
      margin-right: 10px;
    }
    p {
      margin: 5px 0;
    }
    p strong {

    }
    ul {
      list-style-type: none;
      padding-left: 20px;
    }
    ul li {
      margin-bottom: 10px;
      position: relative;
    }
    hr {
      margin: 20px 0;
      border: 1px solid #ddd;
    }
    .experience-item, .education-item {
      margin-bottom: 20px;
    }
    .languages {
      display: flex;
      gap: 20px;
    }
  </style>
</head>
<div class="container">
  <h2 class="section-title"><i class="fas fa-user icon"></i> Summary</h2>
  <p>
    I am a PhD Candidate in Computer Engineering with a strong background in machine learning, deep learning, and medical image analysis. I specialize in AI-driven solutions for the healthcare industry, focusing on medical image analysis, drug discovery, and bioinformatics. With over five years of experience in the field, I am dedicated to applying advanced technologies to solve complex healthcare challenges.
  </p>
  <hr>
  <h2 class="section-title"><i class="fas fa-briefcase icon"></i> Professional Experience</h2>
  <div class="experience-item">
    <h3><i class="fas fa-laptop-code icon"></i> Computer Engineer - Bakircay University Training and Research Hospital</h3>
    <p><em>2023 - Present</em></p>
    <ul>
      <li><i class="fas fa-flask icon"></i> Conducted research on deep learning models for drug discovery.</li>
      <li><i class="fas fa-vial icon"></i> Contributed to ongoing cancer research projects.</li>
    </ul>
  </div>
  <div class="experience-item">
    <h3><i class="fas fa-cogs icon"></i> IT Specialist - Various Health Organizations</h3>
    <p><em>2017 - 2022</em></p>
    <ul>
      <li><i class="fas fa-project-diagram icon"></i> Designed and implemented AI-driven solutions for healthcare systems.</li>
      <li><i class="fas fa-industry icon"></i> Focused on improving industrial processes through IoT and automation.</li>
    </ul>
  </div>
  <hr>
  <h2 class="section-title"><i class="fas fa-code icon"></i> Technical Skills</h2>
  <ul>
    <li><i class="fas fa-laptop-code icon"></i> <strong>Programming:</strong> Python, PyTorch, TensorFlow</li>
    <li><i class="fas fa-robot icon"></i> <strong>Machine Learning:</strong> Deep Learning, Computer Vision, Federated Learning</li>
    <li><i class="fas fa-tools icon"></i> <strong>Tools:</strong> Git, Docker, MLFlow, Scikit-Learn, Neptune.ai</li>
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-graduation-cap icon"></i> Education</h2>
  <ul>
      <h3><i class="fas fa-university icon"></i> PhD in Computer Engineering [ <em>Bakircay University - Ongoing</em> ]</h3>
      <p><strong>Focus:</strong> Deep Learning for Drug Discovery</p>
      <h3><i class="fas fa-university icon"></i> Master's Degree in Computer Engineering [<em>Bakircay University - 2023</em>]</h3>
      <p><strong>Focus:</strong> Federated Learning for Medical Image Domain</p>
      <h3><i class="fas fa-university icon"></i> Bachelor's Degree in Computer Engineering [<em>S.Demirel University - 2015</em>]</h3>
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-book icon"></i> Publications</h2>
  <ul>
    {% for post in site.publications %}
      <li>
        <i class="fas fa-file-alt icon"></i> <!-- Yayın için bir ikon ekliyoruz -->
        <strong><a href="{{ post.url }}">{{ post.title }}</a></strong> <!-- Yayın başlığına link -->
        <p>{{ post.excerpt }}</p> <!-- Yayının kısa özeti -->
      </li>
    {% endfor %}
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-certificate icon"></i> Certifications</h2>
  <ul>
    <li><i class="fas fa-check icon"></i> NVIDIA Certified AI Practitioner</li>
    <li><i class="fas fa-check icon"></i> Microsoft AI Engineer Certification</li>
    <li><i class="fas fa-check icon"></i> Coursera Machine Learning and Deep Learning Specializations</li>
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-language icon"></i> Languages</h2>
  <div class="languages">
    <span><i class="fas fa-globe icon"></i> <strong>Turkish:</strong> Native</span>
    <span><i class="fas fa-globe icon"></i> <strong>English:</strong> B2 (Improving)</span>
    <span><i class="fas fa-globe icon"></i> <strong>German:</strong> A1 (Improving)</span>
  </div>
  <hr>
  <h2 class="section-title"><i class="fas fa-users icon"></i> Volunteering & Memberships</h2>
  <div class="languages">
  <ul>
    <li><i class="fas fa-hands-helping icon"></i> Founding Board Member, Aegean Health Managers Association</li>
    <li><i class="fas fa-user-md icon"></i> Member, Medical Informatics Association</li>
  </ul>
    </div>
</div>
