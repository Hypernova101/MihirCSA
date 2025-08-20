---
layout: base
title: I'm Mihir Bapat
permalink: /about/
comments: true
toc: true
image: /images/mario_animation.png
---

{% raw %}
<div align="center">
  <h1>Hi, I'm <span class="auto-type">Mihir</span></h1>
</div>
{% endraw %}

<br>

<div align="center">
<img align="center" style="border-radius: 4px; box-shadow: 0px 0px 30px #35bde7;" src="{{site.baseurl}}/images/Freeform.png" height="300px" alt="about"/>
<br>
<br>
<em>My about me picture</em>
</div>

<p align="center" style="color:white;">
Hello! My name is Mihir Bapat. I am a Junior at Del Norte High School with heritage from India.  
The above picture is my Freeform picture. It covers the very things I find to be a part of myself.  
To start off, I am a massive sports fan. I like to watch and play Soccer and Cricket.  
I support Liverpool FC in Soccer, and the Mumbai Indians and team India in cricket.  
Finally, in my free time, I like to code, play the piano, and play Fortnite while listening to Spotify.  
</p>

---

### Development Environment

> Coding starts with tools, explore these tools and procedures with a click.

<div style="display: flex; flex-wrap: wrap; gap: 10px;">
    <a href="https://github.com/Open-Coding-Society/student">
        <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
    </a>
    <a href="https://open-coding-society.github.io/student">
        <img src="https://img.shields.io/badge/GitHub%20Pages-327FC7?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Pages">
    </a>
    <a href="https://kasm.nighthawkcodingsociety.com/">
        <img src="https://img.shields.io/badge/KASM-0078D4?style=for-the-badge&logo=kasm&logoColor=white" alt="KASM">
    </a>
    <a href="https://vscode.dev/">
        <img src="https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VSCode">
    </a>
</div>

---

### Class Progress

> Here is my progress through coding, click to see these online

<div style="display: flex; flex-wrap: wrap; gap: 10px;">
    <a href="{{site.baseurl}}/snake" style="text-decoration: none;">
        <div style="background-color: #00FF00; color: black; padding: 10px 20px; border-radius: 5px; font-weight: bold;">
            Snake Game
        </div>
    </a>
    <a href="{{site.baseurl}}/turtle" style="text-decoration: none;">
        <div style="background-color: #FF0000; color: white; padding: 10px 20px; border-radius: 5px; font-weight: bold;">
            Turtle
        </div>
    </a>
</div>

---

### Fun Section 🎮  

<p id="mario" class="sprite"></p>

<div align="center">
  <button id="factButton" style="background:red;">Get a Random Liverpool FC Fact</button>
</div>
<p id="factDisplay" align="center" style="color:white; font-weight:bold;"></p>

---

### Get in Touch  

> Feel free to reach out if you'd like to collaborate or learn more about our work.  

<p style="color: #2A7DB1;">Open Coding Society: <a href="https://opencodingsociety.com" style="color: #2A7DB1; text-decoration: underline;">Socials</a></p>

---

<!-- Scripts -->
<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
<script>
  var typed = new Typed(".auto-type", {
        strings: ["Mihir", "a Coder", "a Gamer", "a Kopite"],
        typeSpeed: 200,
        backSpeed: 200,
        loop: true
   })
</script>

<script>
  const liverpoolFacts = [
    "Liverpool FC was founded in 1892 and is one of England’s most successful football clubs.",
    "Anfield, Liverpool's home stadium, was originally the home of Everton FC.",
    "Liverpool has won six European Cups, more than any other English team.",
    "Bill Shankly, one of the most iconic managers in football history, led Liverpool from 1959 to 1974.",
    "The famous 'You'll Never Walk Alone' anthem has been sung at Anfield since the early 1960s.",
    "Liverpool's rivalry with Manchester United is one of the most intense in world football.",
    "In 2020, Liverpool won their first Premier League title after a 30-year wait."
  ];

  function getRandomFact() {
    const randomIndex = Math.floor(Math.random() * liverpoolFacts.length);
    return liverpoolFacts[randomIndex];
  }

  document.getElementById('factButton').addEventListener('click', () => {
    const fact = getRandomFact();
    document.getElementById('factDisplay').textContent = fact;
  });
</script>
