---
name: mfs16
languages: Rust, MFS-16 Assembly
blurb: "A from-scratch virtual computer."
date: 24-11-21
---

The MFS-16 is a virtual computer, designed from scratch, with an original CPU instruction set and assembly language. The project aims to be an accurate virtual representation of a theoretical computing system that could be implemented as real hardware.

Comprehensive MFS-16 documentation can be found <a href="../book/index.html" target="_blank">here</a>.

<div class="figures">
  {% 
    include figure.html 
        img="bouncing_logo" 
        type="gif" 
        alt="A colourful MFS-16 logo bouncing around the screen." 
        caption="The MFS-16 logo bouncing around the screen."
        class="fig-img"
        use-href="true"
        href="../assets/images/bouncing_logo.gif"
    %}
</div>


The MFS-16 project consists of three main components:

## 1. mfs16core

The core is responsible for all the basic system functionality. The CPU itself has registers, an x86-inspired instruction set, and interrupt logic. The MMU is responsible for all functionality related to the system memory, and also serves as a middleman for communication with I/O devices and VRAM access. Functionality for the keyboard, GPU, and hard drives is also located here.

## 2. mfs16desktop

The desktop program is a frontend for the core which allows emulation of the MFS-16 system directly on your PC! It uses SDL2 to display a screen and has a built-in debugger, keyboard input, and user configuration.

## 3. mfs16assembler

This standalone program, accessible as a CLI utility, is responsible for lexing, parsing, and assembling the original MFS-16 Assembly dialect into binaries executable by the MFS-16 itself! This allows one to write their own programs for the MFS-16.

<div class="figures">
  {% 
    include figure.html 
        img="scribe_demo" 
        type="gif" 
        alt="Some MFS-16 text." 
        caption="Typing some text using the 'Scribe' typing program." 
        class="fig-img" 
        use-href="true" 
        href="../assets/images/scribe_demo.gif"
    %}
</div>
