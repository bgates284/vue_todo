<template>
  <div>
    <div class="image-banner">
      <div class="banner-text">
        <h1>Software Engineer</h1>
        <h2>&</h2>
        <h2>Certified Scrum Product Owner</h2>
      </div>
      <img class="pic" src="/Images/ProfileImage.jpg" alt="Profile image" />
    </div>

<div class="bio-section">
  <p>
    I’m a results-driven Software Engineer and Certified Scrum Product Owner (CSPO) with over a decade of experience building scalable software, integrating complex systems, and solving problems with code. I specialize in full-stack development, API integrations, and product lifecycle management, with a strong foundation in C#, .NET Core, JavaScript, and SQL.
  </p>
  <p>
    Over the years, I’ve led projects across a range of industries — from telecom and aviation to marketing tech and SaaS — consistently turning technical challenges into streamlined, user-focused solutions.
  </p>
  <p>
    Recently, I worked as an Integration Developer at iPaaS.com, where I developed integrations for their new Marketplace platform. The environment was fast-moving and experimental, with early-stage SDKs and evolving documentation. It was a hands-on, behind-the-scenes look at what developers face when building on emerging platforms — and I gained a lot of insight into designing with resilience, debugging under pressure, and communicating clearly in ambiguous scenarios. That experience deepened my appreciation for thoughtful architecture, clean documentation, and developer-first design.
  </p>
  <p>
    Whether I’m writing backend services, crafting intuitive UIs, or architecting systems that just make sense, I’m driven by one goal: building technology that helps people work smarter and move faster.
  </p>
  <p>
    When I’m not coding, I enjoy mentoring newer devs, contributing to open-source tools, and experimenting with automation workflows. I’m always open to new opportunities, cool ideas, and the occasional code puzzle.
  </p>
  <p>Let’s build something useful.</p>
</div>
  </div>
  <div class="footer-banner">
  <p class="footer-text">Thanks for stopping by — let’s connect soon!</p>
</div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap');

.image-banner {
  margin: 0 auto; /* Center it horizontally */
  max-width: 800px; /* Match bio-section width */
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(to right, #007bff, #ffffff),
              linear-gradient(to bottom, #007bff, white);
  background-blend-mode: overlay;
  padding: 2rem;
  width: 100%; /* Ensures it stretches within the max-width */
  border-radius: 20px 20px 0 0;
  overflow: hidden;
}

.footer-banner {
  margin: 0 auto;
  max-width: 800px;
  padding: 2rem;
  background: linear-gradient(to right, #007bff, #ffffff),
              linear-gradient(to top, #007bff, white);
  background-blend-mode: overlay;
  border-radius: 0 0 20px 20px;
  text-align: center;
  color: rgb(4, 0, 0);
  font-family: 'Playfair Display', serif;
  box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.05);
}

.footer-text {
  margin: 0;
  font-size: 1.25rem;
  font-weight: 600;
}

.banner-text {
  flex: 1;
  color: rgb(4, 0, 0);
  font-family: 'Playfair Display', serif;
}

.banner-text h1 {
  font-size: 2rem;
  margin: 0;
  line-height: 1.3;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.banner-text h2 {
  font-size: 1.5rem;
  margin: 0;
  line-height: 1.3;
}

.pic {
  border-radius: 50%;
  width: 100px;
  height: 100px;
  object-fit: cover;
  margin-left: 1rem;
}

.bio-section {
  margin: 2rem auto;
  padding: 2rem;
  max-width: 800px;
  /* border: 2px solid #007bff; */
  border-radius: 15px;
  background-color: #f9f9f9;
  font-family: sans-serif;
  font-size: 1rem;
  line-height: 1.6;
  color: #333;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
}

@media (max-width: 768px) {
  .image-banner {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .banner-text {
    padding-bottom: 1rem;
  }

  .pic {
    width: 120px;
    height: 120px;
    margin: 1rem 0 0;
  }

  .bio-section {
    margin: 1rem;
    padding: 1.5rem;
  }
}

html, body {
  overflow-x: hidden;
  scrollbar-width: auto; /* Keep vertical scroll visible */
}

/* Hide horizontal scrollbar on WebKit */
html::-webkit-scrollbar:horizontal {
  display: none;
}
</style>
