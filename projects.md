---
title: Projects
permalink: projects

projects:
  - title: Ba-Turing IDE
    text: Ba-Turing is an IDE for the Turing programming language. I built it with Electron.js and node.js.
    img:
      src: https://balajiv.ca/ba-turing/screenshot.png
      alt: Screenshot of ba-turing Editor.
    links:
    - href: https://github.com/balaji-venkatesh/ba-turing
      text: Source
      icon: github
    - href: https://balajiv.ca/ba-turing
      text: Site
      icon: link
  - title: Skule™ Website
    text: Skule.ca is the website for the University of Toronto Engineering Society and the engineering student body, Skule™. It's hosted on Github Pages, and uses the Jekyll static site generator to compile a static website from the source HTML, Markdown, and Liquid. I wrote a responsive custom theme using the Bootstrap frontend toolkit.
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
  - title: FPGA Audio-Localised Search & Rescue Robot
    text: Digital Systems Design (ECE532) is a course at the University of Toronto where teams of four students build complex FPGA-based systems. Our project was an autonomous search and rescue robot with audio localisation. My main contribution to the project was the camera stream from the robot to the base station, in which I created my own hardware implementation of an Ethernet stack and H.262 MPEG compression algorithm. 
    img:
      src: assets/ece532.png
      alt: Image of robot and video stream.
    links:
    - href: https://github.com/balaji-venkatesh/ece532-project
      text: Source
      icon: github
    - href: https://balajiv.ca/ece532-project/doc/Final Presentation.pdf
      text: Slides
      icon: file-earmark-pdf-fill
  - title: Vector Processor Extension
    text: Computer Organisation (ECE352) is a course at the University of Toronto. Our final project was a single instruction multiple data (SIMD/vector) extension for a multicycle processor.
    img:
      src: https://balajiv.ca/ece352-project/datra.PNG
      alt: Diagram of vector processor.
    links:
    - href: https://github.com/balaji-venkatesh/ece352-project
      text: Source
      icon: github
  - title: Snek
    text: Snek is a pixel graphics game built in Java 8. It's Snake, but with 2 Snakes! I wrote my own underlying pixel graphics game engine with sprites, fonts, timers, and customizable keyboard controls.
    img:
      src: https://balajiv.ca/snek/screenshot.png
      alt: Screenshot of snek game.
    links:
    - href: https://github.com/balaji-venkatesh/snek
      text: Source
      icon: github
  - title: My Website
    text: balajiv.ca is my personal website. You're looking at it right now! It's hosted on Github Pages, and uses the Jekyll static site generator to compile a static website from the source HTML, Markdown, and Liquid. I wrote a responsive custom theme using the Bootstrap frontend toolkit.
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

# Projects

{% for project in page.projects %}

#### {{project.title}}
{{project.text}}

<img src="{{project.img.src}}" class="rounded border h-100" style="max-height:15rem; max-width:80vw" alt="{{project.img.alt}}">

<div class="mb-4">
{% for link in project.links %}
  <a href="{{link.href}}" class="btn btn-primary">
    {% if link.icon %} <i class="bi bi-{{link.icon}}"></i> {% endif %}
    {{link.text}}
  </a>
{% endfor %}
</div>

{% unless forloop.last %} 
---
{% endunless %}

{% endfor %}
