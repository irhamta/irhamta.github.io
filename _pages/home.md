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
excerpt: "Astronomer and Data Scientist"

intro: 
  - title: "About Me"
    excerpt: "<p>
		Hi there! I am a Postdoctoral Fellow at the <a href='https://www.tum.de/en/' style='text-decoration:none'>Technical University of Munich</a> and <a href='https://www.mpa-garching.mpg.de/' style='text-decoration:none'>Max Planck Institute for Astrophysics</a> in Garching.
  		<br><br>
		My research focuses on understanding how the first <b>black holes</b> and <b>galaxies</b> assembled across cosmic time by studying <b>high-redshift quasars</b>.
		Assisted by <b>gravitational lensing</b>, we can probe their star formation and accretion processes in high fidelity.
		I am also interested in modeling lens systems to constrain the nature of <b>dark matter</b> and the processes that govern <b>cosmological structure formation</b>.
  		<br><br>
  		I completed my Ph.D. at the <a href='http://www.mpia.de/en' style='text-decoration:none'>Max Planck Institute for Astronomy</a> and <a href='https://www.ugent.be/en' style='text-decoration:none'>Ghent University</a> in 2022.
                Before then, I worked as a Data Scientist with experience in delivering insights via data analytics and advanced machine learning for the fintech/e-commerce business, products, and market.
	     </p>"
    url: "/about/"
    btn_label: "<i class='fas fa-satellite-dish'></i> Read My Bio"
    btn_class: "btn--info"

research:
  - image_path: /assets/images2/eso_galaxy_1.jpg
    image_caption: "Credit: ESO/Juan Carlos Muñoz"
    title: "Research Interest"
    excerpt: "<ul>
                  <li>Formation and evolution of active galaxies in the early Universe.</li>
                  <li>Cosmic reionization and properties of the intergalactic medium at high redshifts.</li>
                  <li>Extragalactic astrophysics with gravitational lensing.</li>
                  <li>Photometric redshifts estimation and applications.</li>
                  <li>Predictive analytics with the machine and deep learning.</li>
              </ul>"

publications:
  - image_path: /assets/images2/eso_galaxy_2.jpg
    image_caption: "Credit: ESO"
    title: "Publications"
    excerpt: "Most of my publications can be found on my research page.
    I usually store my scientific results in ResearchGate, while popular articles about astronomy are posted in XploreAstro.
    You can also find my refereed journal articles via the <a href='https://ui.adsabs.harvard.edu/search/q=orcid%3A0000-0001-6102-9526&sort=date%20desc%2C%20bibcode%20desc&p_=0' style='text-decoration:none'>SAO/NASA ADS</a>."
    url: "/research/"
    btn_label: "<i class='fas fa-laptop'></i> Research Page"
    btn_class: "btn--info"

images_set:
  - image_path: /assets/images2/nasa_galaxy_1.jpg
  - image_path: /assets/images2/nasa_galaxy_2.jpg
  - image_path: /assets/images2/nasa_galaxy_3.jpg
    image_caption: "Image courtesy of NASA"

code: 
  - title: "Scientific Codes"
    excerpt: "Some of the scientific codes that I have developed can be found on my <a href='/codes/' style='text-decoration:none'>codes</a> page, or you can also go directly to my <a href='https://github.com/irhamta/' style='text-decoration:none'>GitHub</a> webpage."

contact:
  - title: "Want to reach me?"
    excerpt: "If you have any questions about my research, articles, or codes, feel free to contact me via this email. I can also be contacted informally through my social media below."
    url: "mailto:irham.andika@tum.de"
    btn_label: "<i class='fas fa-envelope'></i> irham.andika@tum.de"
    btn_class: "btn--info"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="research" type="left" %}

{% include feature_row id="publications" type="right" %}

{% include feature_row id="code" type="center" %}

{% include feature_row id="images_set" %}

{% include feature_row id="contact" type="center" %}
