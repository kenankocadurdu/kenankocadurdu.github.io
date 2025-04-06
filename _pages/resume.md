---
layout: archive
title: Kenan Kocadurdu
permalink: /resume/
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
    body { margin: 0; }
    .section-title { border-bottom: 2px solid #ccc; padding-bottom: 10px; margin: 30px 0 20px; }
    .icon { margin-right: 10px; }
    p, li { margin: 5px 0; }
    ul { list-style-type: none; padding-left: 0; }
    .experience-item, .education-item { margin-bottom: 25px; }
    .languages span { display: inline-block; margin-right: 20px; }
  </style>
</head>

<div class="container">
  <h2 class="section-title"><i class="fas fa-user icon"></i> Summary</h2>
  <p>
    PhD candidate in Computer Engineering with expertise in AI-based systems for healthcare. Skilled in deep learning, computer vision, and bioinformatics, with a focus on medical imaging, drug discovery, and intelligent automation. Passionate about developing scalable, data-driven solutions to address real-world challenges in clinical and industrial domains.
  </p>

  <h2 class="section-title"><i class="fas fa-briefcase icon"></i> Professional Experience</h2>
  
  <div class="experience-item">
    <h3><i class="fas fa-hospital icon"></i> Computer Engineer – Bakircay University Hospital</h3>
    <p><em>2019 – Present</em></p>
    <ul>
      <li>Conduct research in AI for medical imaging and personalized healthcare.</li>
      <li>Develop platforms for intelligent diagnosis and clinical decision support.</li>
      <li>Design and deploy custom software for operational analysis and automation.</li>
    </ul>
  </div>

  <div class="experience-item">
    <h3><i class="fas fa-network-wired icon"></i> IT Specialist – Aydin Health Directorate</h3>
    <p><em>2017 – 2019</em></p>
    <ul>
      <li>Managed IT systems across more than 10 hospitals.</li>
      <li>Designed and deployed HR and data management solutions.</li>
      <li>Led training sessions to enhance system usage and efficiency.</li>
    </ul>
  </div>

  <div class="experience-item">
    <h3><i class="fas fa-industry icon"></i> Software Engineer – Maroli Food Industry</h3>
    <p><em>2017 – 2018</em></p>
    <ul>
      <li>Developed an ERP system for production and procurement workflows.</li>
      <li>Achieved measurable gains in resource planning and process optimization.</li>
    </ul>
  </div>

  <div class="experience-item">
    <h3><i class="fas fa-clinic-medical icon"></i> Computer Engineer – Aydin Cancer Early Diagnosis Center</h3>
    <p><em>2014 – 2017</em></p>
    <ul>
      <li>Maintained the data infrastructure ensuring reliability and integrity.</li>
      <li>Developed a Java-based system for patient tracking and reporting.</li>
    </ul>
  </div>

  <h2 class="section-title"><i class="fas fa-laptop-code icon"></i> Technical Skills</h2>
  <ul>
    <li><strong>Programming:</strong> Python, Java, MATLAB</li>
    <li><strong>AI & ML:</strong> Deep Learning, Computer Vision, Federated Learning</li>
    <li><strong>Frameworks & Tools:</strong> PyTorch, Scikit-Learn, MLFlow, FastAPI, Docker, Git</li>
    <li><strong>Cloud & DevOps:</strong> Azure DevOps, Kubernetes</li>
    <li><strong>Databases:</strong> Neo4j, Graph Databases</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-graduation-cap icon"></i> Education</h2>
  <ul>
    <li><strong>PhD in Computer Engineering</strong> – Bakircay University (2024 – ongoing)</li>
    <li><strong>MSc in Computer Engineering</strong> – Bakircay University (2021 – 2023)</li>
    <li><strong>BSc in Computer Engineering</strong> – Suleyman Demirel University (2011 – 2015)</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-book icon"></i> Publications</h2>
  <ul>
    {% for post in site.publications %}
      <li><a href="{{ post.url }}"><i class="fas fa-file-alt icon"></i> {{ post.title }}</a><p>{{ post.excerpt }}</p></li>
    {% endfor %}
  </ul>

  <h2 class="section-title"><i class="fas fa-certificate icon"></i> Certifications</h2>
  <ul>
    <li>Microsoft Azure AI Fundamentals</li>
    <li>Deep Learning Specialization – Coursera</li>
    <li>AI for Medical Diagnosis – deeplearning.ai</li>
    <li>NVIDIA Jetson Nano – NVIDIA DLI</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-hands-helping icon"></i> Volunteering</h2>
  <ul>
    <li>Member – Medical Informatics Association, Türkiye</li>
    <li>Founding Member – Aegean Health Managers Association</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-language icon"></i> Languages</h2>
  <div class="languages">
    <span><strong>Turkish:</strong> Native</span>
    <span><strong>English:</strong> B2 (Improving)</span>
    <span><strong>German:</strong> A1 (Improving)</span>
  </div>
</div>
