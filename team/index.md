---
title: Team
nav:
  order: 1
  #tooltip: About our team
---

{% include section.html %}

# {% include icon.html icon="fa-solid fa-microscope" %} Principal Investigator

<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 1.5rem; align-items: center;">
  <div>
    {% include list.html data="members" component="portrait" filter="role == 'pi'" %}
  </div>
  <div>
    <p>
    I am an assistant professor in the 
      <a href="https://cmpe.bogazici.edu.tr/" target="_blank" rel="noopener noreferrer">Department of Computer Engineering at Boğaziçi University</a>.
      I received my Ph.D. degree from the Department of Computer Science & Engineering at Michigan State University. 
      I was a research assistant in the <a href="http://biometrics.cse.msu.edu/" target="_blank" rel="noopener noreferrer">Pattern Recognition and Image Processing Lab</a> under the supervision of 
      <a href="https://www.cse.msu.edu/~jain/" target="_blank" rel="noopener noreferrer">Anil Jain</a> and 
      <a href="https://jiayuzhou.github.io/" target="_blank" rel="noopener noreferrer">Jiayu Zhou</a>. 
      My research interests include machine learning, deep learning, adversarial machine learning, robust training, and temporal analysis, and their applications in biomedical informatics.

  </p>

<div style="display: flex; gap: 0.5rem; flex-wrap: wrap; margin-top: 0.5rem;">
  <a href="/files/resume_inci_baytas.pdf" target="_blank" rel="noopener noreferrer"
     style="display: inline-block; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #c2558d; color: white; border-radius: 4px; text-decoration: none;">
    📄 View My Resume
  </a>
      <a href="mailto:inci.baytas@bogazici.edu.tr" 
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #EA4335; color: white; border-radius: 4px; text-decoration: none;">
        📧 Email
      </a>
      <a href="https://scholar.google.com/citations?user=ELxSraIAAAAJ&hl=en" 
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #4285F4; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/googlescholar.svg" 
             alt="Google Scholar" width="18" style="vertical-align: middle; margin-right: 6px;">
        Google Scholar
      </a>

  <a href="https://www.linkedin.com/in/inci-m-baytas-00994a22/"
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #0A66C2; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg"
             alt="LinkedIn" width="18" style="vertical-align: middle; margin-right: 6px; filter: brightness(0) invert(1);">
        LinkedIn
      </a>
  </div>
    
  </div>
</div>






{% include section.html %}

# {% include icon.html icon="fa-solid fa-users" %}Team

## Graduate Students 

{% assign phd_members = site.members | where: "role", "phd-student" | where: "status", "active" %}
{% for member in phd_members %}
<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 1.5rem; align-items: center; margin-bottom: 3rem;">
  <div>
    {% include portrait.html lookup=member.name %}
  </div>
  <div>
    <h3 style="margin-top: 0;">{{ member.name }}</h3>
    <p>
      {{ member.bio }} 
    </p>
    <div style="display: flex; gap: 0.5rem; flex-wrap: wrap; margin-top: 0.5rem;">
      {% if member.links.resume %}
      <a href="{{ member.links.resume }}" target="_blank" rel="noopener noreferrer"
         style="display: inline-block; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #c2558d; color: white; border-radius: 4px; text-decoration: none;">
        📄 View My Resume
      </a>
      {% endif %}
      {% if member.links.email %}
      <a href="mailto:{{ member.links.email }}" 
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #EA4335; color: white; border-radius: 4px; text-decoration: none;">
        📧 Email
      </a>
      {% endif %}
      {% if member.links.google-scholar %}
      <a href="{{ member.links.google-scholar }}" 
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #4285F4; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/googlescholar.svg" 
             alt="Google Scholar" width="18" style="vertical-align: middle; margin-right: 6px;">
        Google Scholar
      </a>
      {% endif %}
      {% if member.links.linkedin %}
      <a href="{{ member.links.linkedin }}"
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #0A66C2; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg"
             alt="LinkedIn" width="18" style="vertical-align: middle; margin-right: 6px; filter: brightness(0) invert(1);">
        LinkedIn
      </a>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}


{% assign msc_members = site.members | where: "role", "msc-student" | where: "status", "active" %}
{% for member in msc_members %}
<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 1.5rem; align-items: center; margin-bottom: 3rem;">
  <div>
    {% include portrait.html lookup=member.name %}
  </div>
  <div>
    <h3 style="margin-top: 0;">{{ member.name }}</h3>
    <p>
      {{ member.bio }} 
    </p>
    <div style="display: flex; gap: 0.5rem; flex-wrap: wrap; margin-top: 0.5rem;">
      {% if member.links.resume %}
      <a href="{{ member.links.resume }}" target="_blank" rel="noopener noreferrer"
         style="display: inline-block; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #c2558d; color: white; border-radius: 4px; text-decoration: none;">
        📄 View My Resume
      </a>
      {% endif %}
      {% if member.links.email %}
      <a href="mailto:{{ member.links.email }}" 
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #EA4335; color: white; border-radius: 4px; text-decoration: none;">
        📧 Email
      </a>
      {% endif %}
      {% if member.links.google-scholar %}
      <a href="{{ member.links.google-scholar }}" 
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #4285F4; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/googlescholar.svg" 
             alt="Google Scholar" width="18" style="vertical-align: middle; margin-right: 6px;">
        Google Scholar
      </a>
      {% endif %}
      {% if member.links.linkedin %}
      <a href="{{ member.links.linkedin }}"
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #0A66C2; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg"
             alt="LinkedIn" width="18" style="vertical-align: middle; margin-right: 6px; filter: brightness(0) invert(1);">
        LinkedIn
      </a>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}

## Undergraduate Students

{% assign undergrad_members = site.members | where: "role", "undergrad-student" | where: "status", "active" %}
{% for member in undergrad_members %}
<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 1.5rem; align-items: center; margin-bottom: 3rem;">
  <div>
    {% include portrait.html lookup=member.name %}
  </div>
  <div>
    <h3 style="margin-top: 0;">{{ member.name }}</h3>
    <p>
      {{ member.bio }} 
    </p>
    <div style="display: flex; gap: 0.5rem; flex-wrap: wrap; margin-top: 0.5rem;">
      {% if member.links.resume %}
      <a href="{{ member.links.resume }}" target="_blank" rel="noopener noreferrer"
         style="display: inline-block; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #c2558d; color: white; border-radius: 4px; text-decoration: none;">
        📄 View My Resume
      </a>
      {% endif %}
      {% if member.links.email %}
      <a href="mailto:{{ member.links.email }}" 
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #EA4335; color: white; border-radius: 4px; text-decoration: none;">
        📧 Email
      </a>
      {% endif %}
      {% if member.links.google-scholar %}
      <a href="{{ member.links.google-scholar }}" 
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #4285F4; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/googlescholar.svg" 
             alt="Google Scholar" width="18" style="vertical-align: middle; margin-right: 6px;">
        Google Scholar
      </a>
      {% endif %}
      {% if member.links.linkedin %}
      <a href="{{ member.links.linkedin }}"
         target="_blank" rel="noopener noreferrer"
         style="display: inline-flex; align-items: center; padding: 0.25rem 0.6rem; font-size: 0.9rem; background-color: #0A66C2; color: white; border-radius: 4px; text-decoration: none;">
        <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/linkedin.svg"
             alt="LinkedIn" width="18" style="vertical-align: middle; margin-right: 6px; filter: brightness(0) invert(1);">
        LinkedIn
      </a>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}
{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

# {% include icon.html icon="fa-solid fa-graduation-cap" %} Alumni 
{% include list.html data="members" component="portrait" filter="role == 'phd-student' and status == 'alumni'" sort="year" order="descending" %}
{% include list.html data="members" component="portrait" filter="role == 'msc-student' and status == 'alumni'" sort="year" order="descending" %}




