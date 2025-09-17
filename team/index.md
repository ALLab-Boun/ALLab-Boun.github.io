---
title: Team
nav:
  order: 3
  tooltip: About our team
---

{% include section.html %}

# {% include icon.html icon="fa-solid fa-microscope" %} Principal Investigator

<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 1.5rem; align-items: center;">
  <div>
    {% include list.html data="members" component="portrait" filter="role == 'pi'" %}
  </div>
  <div>
    <p>
    More detailed text; background and research focus of the Principal Investigator.
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



