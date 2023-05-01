---
layout: default
---

<section class="hero">
  <div class="hero-background"></div>
  <div class="hero-content">
    <h1>Aiomin Studios</h1>
    <p class="tagline">Innovative technology creators and explorers</p>
    <a href="#projects" class="cta-button">View Our Projects</a>
  </div>
</section>

<section id="about">
  <h2>About Us</h2>
  <p>Aiomin Studios is a company of engineers, designers, and business analysts who are passionate about using technology to solve real-world problems. We're committed to quality over quantity, and we're dedicated to bringing novel approaches to every project we undertake.</p>
  <a href="/about" class="read-more-link">Learn More About Us</a>
</section>

<section id="projects">
  <h2>Our Latest Projects</h2>
  <ul class="project-grid">
    {% for project in site.projects limit:3 %}
    <li>
      <a href="{{ project.url }}">
        <img src="{{ project.image }}" alt="{{ project.title }}" />
        <h3>{{ project.title }}</h3>
        <p>{{ project.short_description }}</p>
      </a>
    </li>
    {% endfor %}
  </ul>
  <a href="/projects" class="read-more-link">View All Projects</a>
</section>

<section id="team">
  <h2>Meet Our Team</h2>
  <ul class="team-grid">
    {% for member in site.team %}
    <li>
      <img src="{{ member.image }}" alt="{{ member.name }}" />
      <h3>{{ member.name }}</h3>
      <p>{{ member.title }}</p>
    </li>
    {% endfor %}
  </ul>
  <a href="/team" class="read-more-link">Learn More About Our Team</a>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <p>Interested in working with us or have a question? Get in touch!</p>
  <a href="/contact" class="cta-button">Contact Us</a>
</section>
