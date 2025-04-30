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
        <h1>About Me</h1>
        <div class="container">
    <h1>Professional Journey</h1>

    <p>I'm a seasoned software developer and product professional with a career spanning full-stack development, systems integration, and agile product ownership. I began my journey at Online Information Services, where I led ETL development and integrated complex data sets to support debt collection operations. I also collaborated on internal tools, vendor communications, and reporting applications.</p>

    <p>From there, I joined flyExclusive as a full-stack developer. My work included building an aircraft maintenance system from the ground up, contributing to shared class libraries, developing microservices, and supporting mobile and web platforms across a wide range of technologies. It was an incredibly fulfilling role that expanded both my technical and architectural knowledge.</p>

    <p>I then worked solo at OSSID, developing WPF applications and SDKs to support industrial packaging machines—an interesting and deeply technical challenge, but one that left me craving more team collaboration. At Listrak, I encountered the complexities of joining a large, fast-scaling organization. Despite my efforts, the role wasn’t the right fit, but it taught me valuable lessons about communication, onboarding, and tech debt in high-growth environments.</p>

    <p>At Segra, I dove into ERP and CRM systems, tackled legacy SQL and PowerShell scripts, and learned the importance of clarity and documentation. Despite the challenges, I found satisfaction in bringing order to chaos and exploring the power of automation.</p>

    <p>These experiences inspired me to shift into a Certified Scrum Product Owner (CSPO) role, aiming to help teams avoid the very pitfalls I’d encountered. At Thirdwave Business Systems, I co-led the development of an SAP e-commerce integration platform. It was a highlight of my career until the company was acquired and my role dissolved.</p>

    <p>I then joined NetApp as a contractor through Webb Design. I built a full-stack internal reporting application for C-level executives using Sails.js, Vue, and PostgreSQL, and contributed broadly to automation and integration efforts using tools like Tray.io and Microsoft Power Automate. It was a rewarding role—cut short only by widespread budget cuts.</p>

    <p>Most recently, I joined iPaaS.com in a challenging integration role. Although it was short-lived due to unmet expectations, I believe my time there helped pave the way for others by identifying and addressing foundational obstacles within their platform.</p>

    <p>Each role, whether smooth or turbulent, has deepened my empathy, sharpened my skills, and reinforced my belief in continuous improvement, collaboration, and building things that matter.</p>

</div>

        <h2>Philosophy & Expertise</h2>
        <p>Throughout my career, I’ve embraced continuous learning, adaptability, and collaboration—whether optimizing code, designing intuitive products, or mentoring teams to navigate technical complexity. I thrive in environments that demand strategic problem-solving and innovative solutions, always aiming to build technology that truly matters.</p>
      </div>
  
      <div class="footer-banner">
        <p class="footer-text">Thanks for stopping by — let’s connect soon!</p>
      </div>
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
