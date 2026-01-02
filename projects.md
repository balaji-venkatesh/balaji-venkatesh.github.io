---
title: Projects
permalink: projects
layout: page

projects:
  - title: Ba-Turing IDE
    text: Ba-Turing is an IDE for the Turing programming language. I built it with Electron.js and node.js.
    img:
      src: https://balajiv.ca/ba-turing/screenshot.png
      alt: Screenshot of ba-turing Editor.
    links:
    - href: https://github.com/balaji-venkatesh/ba-turing
      text: View source code on GitHub
    - href: https://balajiv.ca/ba-turing
      text: View site
  - title: Skule™ Website
    text: Skule.ca is the website for the University of Toronto Engineering Society and the engineering student body, Skule™. During my term as their Webmaster, I migrated the site to Github Pages, using the Jekyll static site generator to compile a static website from HTML, Markdown, and Liquid. Additionally, I wrote a responsive custom theme using the Bootstrap frontend toolkit.
    img:
      src: /assets/skule.jpeg
      alt: Screenshot of https://skule.ca.
    links:
    - href: https://github.com/skule/skule.ca
      text: View source code on GitHub
    - href: https://skule.ca
      text: View site
  - title: FPGA Audio-Localised Search & Rescue Robot
    text: Digital Systems Design (ECE532) is a course at the University of Toronto where teams of four students build complex FPGA-based systems. Our project was an autonomous search and rescue robot with audio localisation. My main contribution to the project was the camera stream from the robot to the base station, in which I created my own hardware implementation of an Ethernet stack and H.262 MPEG compression algorithm. 
    img:
      src: assets/ece532.png
      alt: Image of robot and video stream.
    links:
    - href: https://github.com/balaji-venkatesh/ece532-project
      text: View source code on GitHub
    - href: https://balajiv.ca/ece532-project/doc/Final Presentation.pdf
      text: Download presentation slides PDF
  - title: Vector Processor Extension
    text: Computer Organisation (ECE352) is a course at the University of Toronto. Our final project was a single instruction multiple data (SIMD/vector) extension for a multicycle processor.
    img:
      src: https://balajiv.ca/ece352-project/datra.PNG
      alt: Diagram of vector processor.
    links:
    - href: https://github.com/balaji-venkatesh/ece352-project
      text: View source code on GitHub
  - title: Snek
    text: Snek is a pixel graphics game built in Java 8. It's Snake, but with 2 Snakes! I wrote my own underlying pixel graphics game engine with sprites, fonts, timers, and customizable keyboard controls.
    img:
      src: https://balajiv.ca/snek/screenshot.png
      alt: Screenshot of snek game.
    links:
    - href: https://github.com/balaji-venkatesh/snek
      text: View source code on GitHub
---

{% for project in page.projects %}

## {{project.title}}

{{project.text}}

{% for link in project.links %}
[{{link.text}}]({{link.href}})
{% endfor %}

<img src="{{project.img.src}}" style="max-height:15rem; border-radius:8px; margin:auto; display:block;" alt="{{project.img.alt}}">

{% endfor %}
