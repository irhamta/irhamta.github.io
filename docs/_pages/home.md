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
      url: "#contact"
  caption: "Credit: ESO"
excerpt: "Observational Astronomer and Experienced Data Scientist"

intro: 
  - title: "About Me"
    excerpt: "<p>
                    Hi there! I am a PhD student at the Max Planck Institute for Astronomy and Heidelberg University, Germany. As part of the Euclid Dark Energy Mission group, my research is focused on the discovery and characterization of the quasars in the early universe (redshift > 6). These objects are indispensable tracers to decipher the build-up of the first supermassive black holes and their host galaxies, the early structure formation, and the history of cosmic reionization.
			        <br><br>
			        Outside astronomy, I am a Data Scientist with experience in delivering insights via data analytics and advanced machine learning for the fintech/e-commerce business, products, and market.
		       </p>
             "
    url: "/about/"
    btn_label: "Read More"
    btn_class: "btn--info"

research:
  - image_path: /assets/images2/eso_galaxy_1.jpg
    image_caption: "Credit: ESO/Juan Carlos Muñoz"
    title: "Research Interest"
    excerpt: "<ul>
                  <li>Formation and evolution of active galaxies at the early universe.</li>
                  <li>Cosmic reionization and properties of the intergalactic medium at high redshifts.</li>
                  <li>Photometric redshifts estimation and applications.</li>
                  <li>Predictive analytics with machine and deep learning.</li>
              </ul>
             "

publications:
  - image_path: /assets/images2/eso_galaxy_2.jpg
    image_caption: "Credit: ESO"
    title: "Publications"
    excerpt: " Most of my publications can be found through my [research page](/research/). I usually store my scientific results in ResearchGate while popular articles about astronomy were posted in XploreAstro. You can also find my refereed journal articles via the SAO/NASA Astrophysics Data System ([ADS](https://ui.adsabs.harvard.edu/search/q=orcid%3A0000-0001-6102-9526&sort=date%20desc%2C%20bibcode%20desc&p_=0))."

feature_row:
  - image_path: /assets/images2/nasa_galaxy_1.jpg
  - image_path: /assets/images2/nasa_galaxy_2.jpg
  - image_path: /assets/images2/nasa_galaxy_3.jpg
    image_caption: "Image courtesy of NASA"

code: 
  - title: "Scientific Codes"
    excerpt: "Some of the scientific codes that I’ve developed can be found in my [code page](/codes/)."

contact:
  - title: "Want to reach me?"
    excerpt: 'If you have any question about my research, articles, or codes, feel free to contact me via this email. I can also be contacted informally through my social media below.'
    url: "mailto:andika@mpia.de"
    btn_label: "andika@mpia.de"
    btn_class: "btn--info"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="research" type="left" %}

{% include feature_row id="publications" type="right" %}

{% include feature_row id="code" type="center" %}

{% include feature_row %}

{% include feature_row id="contact" type="center" %}
