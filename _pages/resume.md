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
    body {
      margin: 0;
      font-family: sans-serif;
      font-size: 15px;
      line-height: 1.6;
    }
    .container {
      max-width: 950px;
      margin: auto;
      padding: 15px 20px;
    }
    .section-title {
      font-size: 18px;
      font-weight: 600;
      border-bottom: 1px solid #ccc;
      margin: 20px 0 10px;
      padding-bottom: 5px;
    }
    .experience-item, .education-item {
      margin-bottom: 15px;
    }
    .experience-header, .education-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      font-weight: 600;
      margin-top: 10px;
    }
    ul {
      list-style-type: disc;
      padding-left: 25px;
      margin: 5px 0 0;
    }
    li {
      margin: 3px 0;
    }
    .languages span {
      margin-right: 15px;
    }
    .icon {
      margin-right: 8px;
    }
  </style>
</head>

<div class="container">

  <h2 class="section-title"><i class="fas fa-user icon"></i> Summary</h2>
  <p>
    PhD candidate in Computer Engineering with expertise in AI-driven systems for healthcare and industrial domains. Skilled in machine learning, deep learning, computer vision, and bioinformatics. Passionate about scalable, data-centric technologies for real-world impact.
  </p>

  <h2 class="section-title"><i class="fas fa-briefcase icon"></i> Experience</h2>

  <div class="experience-item">
    <div class="experience-header">
      <span><i class="fas fa-hospital icon"></i> Bakircay University Hospital – Computer Engineer</span>
      <span><em>2019 – Present</em></span>
    </div>
    <ul>
      <li>Conduct research in AI for medical imaging, drug discovery, and bioinformatics.</li>
      <li>Developed <strong>EchoMotion</strong>, an AI tool for analyzing echocardiography videos.</li>
      <li>Designed <strong>PLAff</strong>, an explainable protein-ligand interaction model using LLM-based knowledge graphs.</li>
      <li>Built <strong>FlowSphere</strong>, an MLOps platform for streamlined model training, deployment, and monitoring.</li>
      <li>Created <strong>AutoMicro</strong>, a system for automated analysis of microscopic images.</li>
      <li>Engineered a Java-based hospital cost analysis tool for financial decision-making.</li>
      <li>Developed a QR-based patrol tracking system using FastAPI and Node.js.</li>
    </ul>
  </div>

  <div class="experience-item">
    <div class="experience-header">
      <span><i class="fas fa-network-wired icon"></i> Aydin Health Directorate – IT Specialist</span>
      <span><em>2017 – 2019</em></span>
    </div>
    <ul>
      <li>Managed IT infrastructure across more than 10 hospitals, ensuring stability and performance.</li>
      <li>Designed and implemented a human resources information system (HRIS).</li>
      <li>Led technical training programs for IT staff.</li>
    </ul>
  </div>

  <div class="experience-item">
    <div class="experience-header">
      <span><i class="fas fa-industry icon"></i> Maroli Food Industry – Software Engineer</span>
      <span><em>2017 – 2018</em></span>
    </div>
    <ul>
      <li>Built a custom ERP system for procurement and production operations in an olive factory.</li>
      <li>Achieved 10% improvement in purchasing and 5% in production efficiency through automation.</li>
    </ul>
  </div>

  <div class="experience-item">
    <div class="experience-header">
      <span><i class="fas fa-clinic-medical icon"></i> Aydin Cancer Early Diagnosis Center – Computer Engineer</span>
      <span><em>2014 – 2017</em></span>
    </div>
    <ul>
      <li>Maintained data storage infrastructure with high availability and integrity.</li>
      <li>Developed a Java-based web application for patient tracking and reporting.</li>
    </ul>
  </div>

  <h2 class="section-title"><i class="fas fa-code icon"></i> Technical Skills</h2>
  <ul>
    <li><strong>Languages:</strong> Python, Java, MATLAB</li>
    <li><strong>AI:</strong> Deep Learning, Computer Vision, Federated Learning</li>
    <li><strong>Frameworks:</strong> PyTorch, Scikit-Learn, MLFlow, FastAPI</li>
    <li><strong>DevOps:</strong> Docker, Kubernetes, Azure DevOps, Git</li>
    <li><strong>Data:</strong> Neo4j, Graph Databases</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-graduation-cap icon"></i> Education</h2>

  <div class="education-item">
    <div class="education-header">
      <span><i class="fas fa-university icon"></i> PhD in Computer Engineering – Bakircay University</span>
      <span><em>2024 – ongoing</em></span>
    </div>
    <p><em>Focus:</em> Medical Image Analysis, Drug Discovery, and LLMs</p>
  </div>

  <div class="education-item">
    <div class="education-header">
      <span><i class="fas fa-university icon"></i> MSc in Computer Engineering – Bakircay University</span>
      <span><em>2021 – 2023</em></span>
    </div>
    <p><em>Thesis:</em> Comparison of Federated Learning Frameworks for Medical Image Domain</p>
  </div>

  <div class="education-item">
    <div class="education-header">
      <span><i class="fas fa-university icon"></i> BSc in Computer Engineering – Suleyman Demirel University</span>
      <span><em>2011 – 2015</em></span>
    </div>
    <p><em>Capstone:</em> IoT-based patient monitoring system</p>
  </div>

  <h2 class="section-title"><i class="fas fa-book icon"></i> Publications</h2>
  <ul>
    {% for post in site.publications %}
      <li><a href="{{ post.url }}"><i class="fas fa-file-alt icon"></i> {{ post.title }}</a> — {{ post.excerpt }}</li>
    {% endfor %}
  </ul>

  <h2 class="section-title"><i class="fas fa-certificate icon"></i> Certifications</h2>
  <ul>
    <li>Microsoft Azure AI Fundamentals</li>
    <li>Deep Learning Specialization – Coursera</li>
    <li>AI for Medical Diagnosis – deeplearning.ai</li>
    <li>Getting Started with AI on Jetson Nano – NVIDIA DLI</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-hands-helping icon"></i> Volunteering</h2>
  <ul>
    <li>Member – Medical Informatics Association, Türkiye</li>
    <li>Founding Member – Aegean Health Managers Association</li>
  </ul>

  <h2 class="section-title"><i class="fas fa-language icon"></i> Languages</h2>
  <div class="languages">
    <span><strong>Turkish:</strong> Native</span>
    <span><strong>English:</strong> B2</span>
    <span><strong>German:</strong> A1</span>
  </div>
</div>
