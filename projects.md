---
title: Projects

projects:
  - title: Ba-Turing
    text: Ba-Turing is a better Turing editor, built on Electron.js and node.js.
    img:
      src: /ba-turing/screenshot.png
      alt: Screenshot of ba-turing Editor
    links:
    - href: https://github.com/balaji-venkatesh/ba-turing
      text: Source
      icon: github
    - href: /ba-turing
      text: Site
      icon: box-arrow-up-right
  - title: Skule™ Website
    text: Skule.ca is the website for the University of Toronto Engineering Society and the engineering student body, Skule™.
    img:
      src: /assets/skule.jpeg
      alt: Screenshot of skule.ca
    links:
    - href: https://github.com/skule/skule.ca
      text: Source
      icon: github
    - href: https://skule.ca/
      text: Site
      icon: box-arrow-up-right
  - title: ECE532 FPGA Robot
    text: Our ECE532 project was an autonomous search and rescue robot using FPGA-based audio localization.
    img:
      src: /ece532-project/selfie.png
      alt: Image of robot and video stream.
    links:
    - href: https://github.com/balaji-venkatesh/ece532-project
      text: Source
      icon: github
    - href: /ece532-project/doc/Final Presentation.pdf
      text: Slides
      icon: file-earmark-pdf-fill
  - title: ECE352 Vector Extension
    text: Our ECE352 project was a SIMD (vector) extension for a multicycle processor.
    img:
      src: /ece352-project/datra.PNG
      alt: Diagram of processor.
    links:
    - href: https://github.com/balaji-venkatesh/ece352-project
      text: Source
      icon: github
  - title: Snek
    text: Snek is a pixel graphics game built in Java 8. It's Snake, but with 2 Snakes! It includes an underlying from-scratch game engine with sprites, fonts, timers, and customizable keyboard controls.
    img:
      src: /snek/screenshot.png
      alt: Screenshot of snek game.
    links:
    - href: https://github.com/balaji-venkatesh/snek
      text: Source
      icon: github
---

<div class="row row-cols-1 row-cols-sm-1 row-cols-md-2 row-cols-lg-3 row-cols-xl-4 g-4">
  {% for project in page.projects %}
  <div class="col">
    <div class="card h-100">
      <img src="{{project.img.src}}" height="200px" class="placeholder card-img-top" alt="{{project.img.alt}}">
      <div class="card-body">
        <h5 class="card-title">{{project.title}}</h5>
        <p class="card-text">{{project.text}}</p>
      </div>
      <div class="card-footer">
        {% for link in project.links %}
        <a href="{{link.href}}" class="btn btn-primary">
          {{link.text}}
          {% if link.icon %}<i class="bi bi-{{link.icon}}"></i>{% endif %}
        </a>
        {% endfor %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>

<hr>
<a href="https://github.com/balaji-venkatesh/" class="mb-1 btn btn-lg btn-primary"><i class="bi bi-github"></i> balaji-venkatesh </a>