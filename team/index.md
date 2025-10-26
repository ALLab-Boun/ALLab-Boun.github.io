---
title: Team
nav:
  order: 4
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

<p>
  <a href="/files/resume.pdf" target="_blank" rel="noopener noreferrer"
     style="display: inline-block; padding: 0.5rem 1rem; background-color: #2a1a36; color: white; border-radius: 4px; text-decoration: none;">
    📄 View My Resume
  </a>
</p>
    
  </div>
</div>






{% include section.html %}

# {% include icon.html icon="fa-solid fa-users" %}Team



{% include list.html data="members" component="portrait" filter="role == 'phd-candidate'and status=='active'"%}
{% include list.html data="members" component="portrait" filter="role == 'msc-student' and status=='active'" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}

# {% include icon.html icon="fa-solid fa-graduation-cap" %} Alumni 
{% include list.html data="members" component="portrait" filter="role == 'phd-candidate'and status=='alumni'"%}
{% include list.html data="members" component="portrait" filter="role == 'msc-student' and status=='alumni'" %}



