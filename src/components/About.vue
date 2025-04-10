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
        <p>I'm a seasoned software engineer and Certified Scrum Product Owner (CSPO) with a passion for building scalable systems, integrating complex technologies, and driving product innovation. My career has spanned full-stack development, API architecture, and agile product leadership—each role shaping my ability to transform business challenges into technical solutions.</p>
  
        <h2>Career Journey</h2>
        <p>I started at Online Information Services, where I led ETL development, streamlining data integration for reporting and operational efficiency. Moving to flyExclusive, I designed an aircraft maintenance system from the ground up, built microservices, and contributed to shared class libraries, further honing my expertise in backend architecture.</p>
  
        <p>At OSSID, I tackled WPF application development and SDKs for industrial packaging machines, but my passion for team collaboration led me to Listrak, where I navigated the intricacies of a fast-scaling tech organization. This experience strengthened my understanding of onboarding, tech debt, and large-scale software ecosystems.</p>
  
        <p>At Segra, I worked extensively with ERP and CRM systems, refining legacy SQL and PowerShell scripts while emphasizing automation. These experiences inspired my transition into product ownership, where at Thirdwave Business Systems, I co-led the development of an SAP e-commerce integration platform until the company’s acquisition.</p>
  
        <p>Later, as a contractor for NetApp via Webb Design, I built a full-stack internal reporting application using Sails.js, Vue, and PostgreSQL, alongside broader automation and integration efforts leveraging Tray.io and Power Automate. Most recently, at iPaaS.com, I stepped into a challenging integration role, identifying foundational obstacles to strengthen future platform development.</p>
  
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
