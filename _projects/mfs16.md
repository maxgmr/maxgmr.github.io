---
name: mfs16
languages: Rust, MFS-16 Assembly
blurb: "A from-scratch virtual computer."
date: 24-11-21
---

The MFS-16 is a virtual computer, designed from scratch, with an original CPU instruction set and assembly language. The project attempts to be an accurate virtual representation of a theoretical computing system that could be implemented as real hardware.

MFS-16 documentation can be found <a href="../book/index.html" target="_blank">here</a>.

<div class="figures">
  {% 
    include figure.html 
        img="hello_world" 
        type="png" 
        alt="Text and colour test." 
        caption="Hello, world! A test program showing the computer font and colour palette."
        class="fig-img"
        use-href="true"
        href="../assets/images/hello_world.png"
    %}
  {% 
    include figure.html 
        img="scribe" 
        type="png" 
        alt="Some MFS-16 text." 
        caption="Typing some text using the `scribe` typing program." 
        class="fig-img" 
        use-href="true" 
        href="../assets/images/scribe.png"
    %}
</div>
