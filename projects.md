---
title: Projects

projects:
  - title: Ba-Turing
    text: Ba-Turing is a better Turing editor, built on Electron.js and node.js.
    img:
      src: /ba-turing/screenshot.png
      alt: Screenshot of ba-turing Editor.
    links:
    - href: https://github.com/balaji-venkatesh/ba-turing
      text: Source
      icon: github
    - href: /ba-turing
      text: Site
      icon: link
  - title: Skule™ Website
    text: Skule.ca is the website for the University of Toronto Engineering Society and the engineering student body, Skule™.
    img:
      src: /assets/skule.jpeg
      alt: Screenshot of https://skule.ca.
    links:
    - href: https://github.com/skule/skule.ca
      text: Source
      icon: github
    - href: https://skule.ca
      text: Site
      icon: link
  - title: FPGA Search & Rescue Robot
    text: Digital Systems Design (ECE532) is a course at the University of Toronto where teams of four students build complex FPGA-based systems. Our project was an autonomous search and rescue robot with audio localisation.
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
  - title: Vector Processor
    text: Computer Organisation (ECE352) is a course at the University of Toronto. Our final project was a single instruction multiple data (SIMD/vector) extension for a multicycle processor.
    img:
      src: /ece352-project/datra.PNG
      alt: Diagram of vector processor.
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
  - title: balajiv.ca
    text: balajiv.ca is my personal website, which is what you're looking at right now! It's hosted on Github Pages, and uses the Jekyll static site generator to compile a static website from the source HTML, Markdown, and Liquid. I wrote a custom, responsive theme using the Bootstrap frontend toolkit.
    img: 
      src: /assets/balajiv.ca.jpeg
      alt: Screenshot of https://balajiv.ca.
    links:
    - href: https://github.com/balaji-venkatesh/balaji-venkatesh.github.io
      text: Source
      icon: github
    - href: https://balajiv.ca
      text: Site
      icon: link
---

<div class=" row row-cols-1 row-cols-sm-1 row-cols-md-2 row-cols-lg-3 row-cols-xxl-4 g-3 justify-content-center">
  {% for project in page.projects %}
  <div class="col" style="max-width:300px !important">
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