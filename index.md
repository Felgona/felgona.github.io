---
layout: home
title: Home
---
<link rel="stylesheet" href="/assets/css/style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<!-- 🌙 DARK MODE BUTTON -->
<button onclick="toggleDarkMode()" style="
  position:fixed;
  top:20px;
  right:20px;
  padding:8px 12px;
  border:none;
  background:#333;
  color:white;
  border-radius:5px;
  cursor:pointer;
">
🌙 Dark Mode
</button>

<!-- 🔥 HERO SECTION -->
<div style="
  text-align:center;
  padding:80px 20px;

  background: linear-gradient(to right, #336699, #99ccff);

  color:white;
  border-radius:16px;

  /* Glass effect */
  backdrop-filter: blur(10px);

  /* Soft border */
  border: 1px solid rgba(255,255,255,0.3);

  /* Premium shadow */
  box-shadow: 0 10px 30px rgba(0,0,0,0.15);
">

<img src="/assets/images/profile.png" 
style="
  width:150px;
  height:150px;
  border-radius:50%;
  object-fit:cover;
  border:4px solid white;
  margin-bottom:15px;

">
<h1 style="font-size:45px;">Felgona Awuor Owuor</h1>

<p style="font-size:20px;">
Data Analyst | Economics & Statistics | MEL & Impact Analytics
</p>

<a href="/projects" style="
  margin-top:20px;
  display:inline-block;
  padding:12px 20px;
  background:white;
  color:#007acc;
  text-decoration:none;
  border-radius:6px;
  font-weight:bold;
">
View My Work
</a>

<div style="
  margin-top:25px;
  display:flex;
  justify-content:center;
  gap:30px;
  flex-wrap:wrap;
  font-size:16px;
">

  <a href="mailto:awuorowuorfelgona@gmail.com" style="color:white; text-decoration:none;">
    <i class="fas fa-envelope"></i> Email
  </a>

  <a href="https://www.linkedin.com/in/owuorfelgona" target="_blank" style="color:white; text-decoration:none;">
    <i class="fab fa-linkedin"></i> LinkedIn
  </a>

  <a href="https://github.com/Felgona" target="_blank" style="color:white; text-decoration:none;">
    <i class="fab fa-github"></i> GitHub
  </a>

</div>

<!-- 👩‍💻 ABOUT -->
<div class="section fade-in">

<h2>👩‍💻 About Me</h2>

<div class="card">

<p style="font-size:17px; line-height:1.7;">
I am a <strong>Data Analyst</strong> specializing in 
<strong>data-driven decision making, statistical analysis, and impact evaluation</strong>.
</p>

<p style="font-size:17px; line-height:1.7;">
My work bridges <strong>quantitative analytics</strong> with 
<strong>program monitoring and strategic learning systems</strong>, 
enabling organizations to make informed, evidence-based decisions.
</p>

</div>

</div>

<!-- 🚀 WHAT I DO -->
<div class="section fade-in">

<h2>🚀 What I Do</h2>

<div style="display:grid; grid-template-columns:1fr 1fr; gap:20px;">

<div class="card">
<h4>📊 Data Analysis</h4>
<p>Cleaning and transforming data to extract insights.</p>
</div>

<div class="card">
<h4>📈 Visualization</h4>
<p>Building dashboards and storytelling visuals.</p>
</div>

<div class="card">
<h4>📉 Statistical Analysis</h4>
<p>Applying statistical methods for validation.</p>
</div>

<div class="card">
<h4>📋 MEL Analytics</h4>
<p>Designing impact measurement systems.</p>
</div>

</div>

</div>

<!-- 📂 CTA -->
<div class="section fade-in">

<div class="card" style="text-align:center;">

<h2>📂 Explore My Work</h2>

<p>
Discover projects in data analytics, dashboards, and impact evaluation.
</p>

<a href="/projects" style="
  display:inline-block;
  margin-top:15px;
  padding:12px 20px;
  background:#007acc;
  color:white;
  text-decoration:none;
  border-radius:6px;
  font-weight:bold;
">
View Projects
</a>

</div>

</div>

<!-- SCRIPT -->
<script>
function toggleDarkMode() {
  document.body.classList.toggle("dark-mode");
}

const faders = document.querySelectorAll('.fade-in');

window.addEventListener('scroll', () => {
  faders.forEach(el => {
    const rect = el.getBoundingClientRect();
    if (rect.top < window.innerHeight - 100) {
      el.classList.add('visible');
    }
  });
});
</script>
