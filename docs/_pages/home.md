---
layout: splash
permalink: /
hidden: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images2/ESO_Centaurus_A.jpg
  actions:
    - label: "Explore"
      url: "#contact"
excerpt: "Hello! I am an astronomer who works on deciphering the build-up of the first active galaxies, the early structure formation, and the history of cosmic reionization."
intro: 
  - image_path: /assets/images2/gal1.jpg
    title: "About Me"
    excerpt: "<p>
                    Currently, I am a PhD student at the Max Planck Institute for Astronomy and Heidelberg University, Germany. As part of the Euclid Dark Energy Mission group, my research is focused on the discovery and characterization of the quasars in the early universe (redshift > 6). These objects are indispensable tracers to understand the growth of the supermassive black holes, their role in cosmic reionization, and the environments where they live in, when the universe was still very young.
			        <br><br>
			        Outside astronomy, I am a Data Scientist with experience in delivering insights via data analytics and advanced machine learning for the fintech/e-commerce business, products, and market.
			        <br>
		        </p>
             "
publications:
  - image_path: /assets/images2/gal2.jpg
    title: "Publications"
    excerpt: " Most of my publications can be found through the links below. I usually store my scientific results in [ResearchGate](https://www.researchgate.net/profile/Irham_Andika/publications) while popular articles about astronomy were posted in [XploreAstro](https://xploreastro.wordpress.com/category/astrophysics/). You can also find my refereed journal articles via NASA/ADS."
    url: "https://ui.adsabs.harvard.edu/search/q=orcid%3A0000-0001-6102-9526&sort=date%20desc%2C%20bibcode%20desc&p_=0"
    btn_label: "NASA/ADS"
    btn_class: "btn--info"

feature_row:
  - image_path: /assets/images2/galaxy_1.jpg
  - image_path: /assets/images2/galaxy_2.jpg
  - image_path: /assets/images2/galaxy_3.jpg
contact:
  - title: "Want to reach me?"
    excerpt: 'If you have any question about my research, articles, or codes, feel free to contact me via this email. I can also be contacted informally through my social media below.'
    url: "mailto:andika@mpia.de"
    btn_label: "andika@mpia.de"
    btn_class: "btn--info"
---

{% include feature_row id="intro" type="left" %}

{% include feature_row id="publications" type="right" %}

{% include feature_row %}

{% include feature_row id="contact" type="center" %}
