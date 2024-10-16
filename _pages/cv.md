---
layout: archive
title: Kenan Kocadurdu
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
    }
    h2.section-title {
      border-bottom: 2px solid;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }
    h2 {
      margin-right: 10px;
    }
    h3 i {
      margin-right: 10px;
    }
    p {
      margin: 5px 0;
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
  <h2 class="section-title"><i class="fas fa-user icon"></i> Summary </h2>
  <p>
    I am a PhD Candidate in Computer Engineering with a strong background in machine learning, deep learning, and medical image analysis. I specialize in AI-driven solutions for the healthcare industry, focusing on medical image analysis, drug discovery, and bioinformatics. With over five years of experience in the field, I am dedicated to applying advanced technologies to solve complex healthcare challenges.
  </p>
  <hr>
  <h2 class="section-title"><i class="fas fa-briefcase icon"></i> Professional Experience</h2>
  <div class="experience-item">
    <h3><i class="fas fa-laptop-code icon"></i> Computer Engineer - Bakircay University Training and Research Hospital</h3>
    <p><em>2023 - Present</em></p>
    <ul>
      <li><i class="fas fa-flask icon"></i> Actively engaged in academic research, with a particular focus on medical image analysis and recent work on protein-ligand interaction studies.</li>
      <li><i class="fas fa-microchip icon"></i> Led the conception and execution of an innovative Internet of Things (IoT) project derived from academic research, focusing on the automated analysis of blood culture gram stains.</li>
      <li><i class="fas fa-calculator icon"></i> Contributed to hospital cost analysis studies, culminating in the development of a Java-based web application as the final output.</li>
    </ul>
  </div>
  <div class="experience-item">
    <h3><i class="fas fa-desktop icon"></i> IT Specialist - Aydin Health Directorate</h3>
    <p><em>2017 - 2019</em></p>
    <ul>
      <li><i class="fas fa-server icon"></i> Led the installation and maintenance of IT systems across a portfolio of over 10 hospitals, ensuring seamless operations and optimal performance.</li>
      <li><i class="fas fa-users-cog icon"></i> Designed, developed, and deployed an information management system tailored for the Human Resources department, streamlining processes and enhancing data efficiency.</li>
    </ul>
  </div>
  <div class="experience-item">
    <h3><i class="fas fa-code icon"></i> Software Engineer - Maroli Food Industry and Foreign Trade. Inc.</h3>
    <p><em>2017 - 2018</em></p>
    <ul>
      <li><i class="fas fa-industry icon"></i> Engineered an Enterprise Resource Planning (ERP) application specifically for an Olive Factory, orchestrating a significant optimization of business operations.</li>
      <li><i class="fas fa-chart-line icon"></i> Efficiency improvements of 10% in the raw material purchasing process and 5% in the production process have been realized.</li>
    </ul>
  </div>
  <div class="experience-item">
    <h3><i class="fas fa-laptop-code icon"></i> Computer Engineer - Aydin Cancer Early Diagnosis Center</h3>
    <p><em>2014 - 2017</em></p>
    <ul>
      <li><i class="fas fa-database icon"></i> Oversaw the maintenance of the data storage infrastructure at the center, ensuring data integrity and system reliability.</li>
      <li><i class="fas fa-stethoscope icon"></i> Developed and deployed a Java-based web application for a patient tracking system, effectively optimizing transactions and resulting in significant time and material savings.</li>
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
        <i class="fas fa-file-alt icon"></i>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-certificate icon"></i> Certifications</h2>
  <ul>
    <li><i class="fas fa-certificate icon"></i> NVIDIA Certified AI Practitioner</li>
    <li><i class="fas fa-certificate icon"></i> Microsoft AI Engineer Certification</li>
    <li><i class="fas fa-certificate icon"></i> Coursera Machine Learning and Deep Learning Specializations</li>
  </ul>
  <hr>
  <h2 class="section-title"><i class="fas fa-language icon"></i> Languages</h2>
    <span><i class="fas fa-globe icon"></i> <strong>Turkish:</strong> Native</span>
    <span><i class="fas fa-globe icon"></i> <strong>English:</strong> B2 (Improving)</span>
    <span><i class="fas fa-globe icon"></i> <strong>German:</strong> A1 (Improving)</span>
  <hr>
</div>
