---
layout: splash
permalink: /
hidden: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images2/eso_centaurus_a.jpg
  actions:
    - label: "<i class='fas fa-rocket'></i> Explore"
      url: "#about"
  caption: "Credit: ESO"
excerpt: "Astronomer & ML Engineer"

intro:
  - title: "About Me"
    excerpt: |
      I am a Research Software Engineer at LMU Munich, working at the
      intersection of astrophysics, machine learning, and scientific computing.

      I study how supermassive black holes grow across cosmic time. By combining
      large-scale astronomical surveys, gravitational lensing, and computational
      methods, I search for rare, short-lived accretion phases that conventional
      selection methods can miss, connecting individual episodes of black hole
      activity to their assembly over billions of years.

      My background spans academia and industry, integrating scientific research
      with experience developing data-driven solutions in fintech and e-commerce.
    url: "/about/"
    btn_label: "<i class='fas fa-satellite-dish'></i> Read My Bio"
    btn_class: "btn--info"

research:
  - image_path: /assets/images2/eso_galaxy_1.jpg
    alt: "Galaxy in the early Universe"
    image_caption: "Credit: ESO/Juan Carlos Muñoz"
    title: "Research Interest"
    excerpt: |
      - Supermassive black hole and galaxy evolution across cosmic time.
      - Time-domain astrophysics, including changing-state AGNs and transient accretion.
      - Strong gravitational lensing for probing faint and distant black holes.
      - Machine learning for rare-object discovery and physical inference in large-scale astronomical surveys.

publications:
  - image_path: /assets/images2/eso_galaxy_2.jpg
    alt: "Distant galaxy"
    image_caption: "Credit: ESO"
    title: "Publications"
    excerpt: |
      Selected projects and scientific results are highlighted on my Research
      page. I also write about astronomy for a broader audience on
      [XploreAstro](https://xploreastro.wordpress.com/). A complete list of my
      refereed publications is available on [ADS](https://ui.adsabs.harvard.edu/search/q=orcid%3A0000-0001-6102-9526&sort=date%20desc%2C%20bibcode%20desc&p_=0).
    url: "/research/"
    btn_label: "<i class='fas fa-laptop'></i> Research Page"
    btn_class: "btn--info"

images_set:
  - image_path: /assets/images2/nasa_galaxy_1.jpg
    alt: "Galaxy observed by NASA"
  - image_path: /assets/images2/nasa_galaxy_2.jpg
    alt: "Galaxy observed by NASA"
  - image_path: /assets/images2/nasa_galaxy_3.jpg
    alt: "Galaxy observed by NASA"
    image_caption: "Image courtesy of NASA"

codes:
  - title: "Scientific Codes"
    excerpt: |
      You can explore some of the scientific software and tools I have developed
      on my Codes page or [GitHub](https://github.com/irhamta/).
    url: "/codes/"
    btn_label: "<i class='fas fa-laptop-code'></i> Explore My Codes"
    btn_class: "btn--info"

contact:
  - title: "Want to Get in Touch?"
    excerpt: |
      Have a question about my research or scientific software, or interested in
      collaborating? Feel free to reach out by email.
    url: "mailto:irham.andika@lmu.de"
    btn_label: "<i class='fas fa-envelope'></i> irham.andika@lmu.de"
    btn_class: "btn--info"
---

<div id="about"></div>
{% include feature_row id="intro" type="center" %}

{% include feature_row id="research" type="left" %}

{% include feature_row id="publications" type="right" %}

{% include feature_row id="codes" type="center" %}

{% include feature_row id="images_set" %}

{% include feature_row id="contact" type="center" %}
