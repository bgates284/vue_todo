<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="container">
    <h1>William Gates</h1>
    <div class="contact">
      North Carolina | (252) 417-3824 | <a href="mailto:wjg284@gmail.com">wjg284@gmail.com</a>
    </div>

    <div class="section">
      <h2>Professional Summary</h2>
      <p>
        Results-driven Software Engineer & Certified Scrum Product Owner (CSPO) with 10+ years of experience in full-stack development, API integrations, and product lifecycle management. Skilled in developing scalable software solutions, leading cross-functional teams, and streamlining business processes. Adept at translating technical requirements into actionable outcomes with expertise in C#, .Net, SQL, jQuery, and Agile methodologies.
      </p>
    </div>

    <div class="section">
      <h2>Technical Skills</h2>
      <p><span class="subheading">Programming:</span> C#, .NET Core, Entity Framework, JavaScript, Python, PHP, Java, C++</p>
      <p><span class="subheading">Databases:</span> Microsoft SQL Server, Oracle SQL, SAP Hana, PostgreSQL</p>
      <p><span class="subheading">Cloud & DevOps:</span> Azure, AWS, Docker, Jenkins, Kubernetes, SDLC, Unit Testing</p>
      <p><span class="subheading">Web Technologies:</span> HTML, CSS, Bootstrap, Vue.js, jQuery, Sails.js</p>
      <p><span class="subheading">API Development:</span> RESTful APIs, Microservices, Integration Services</p>
      <p><span class="subheading">Agile & Scrum:</span> Product Ownership, Backlog Management, Roadmap Planning, Jira</p>
      <p><span class="subheading">ETL & Data Processing:</span> SQL, Tray.io, CloverDX, Reporting & Analytics</p>
    </div>

    <div class="section">
      <h2>Professional Experience</h2>

      <p><span class="job-title">iPaaS.com | Integration Developer</span> <span class="job-date">Dec 2024 – Mar 2025</span></p>
      <ul>
        <li>Developed C# integrations for the iPaaS.com Marketplace to enhance automation.</li>
        <li>Assisted integration team, testing the integration SDK and software functionality.</li>
      </ul>

      <p><span class="job-title">Webb Design (NetApp) | Integration Specialist</span> <span class="job-date">Mar 2023 – Dec 2024</span></p>
      <ul>
        <li>Led marketing tech integration strategy, automating workflows and connections.</li>
        <li>Developed integrations for business goals using Sails.js & PostgreSQL.</li>
      </ul>

      <p><span class="job-title">Third Wave Business Systems | Product Owner</span> <span class="job-date">Mar 2022 – Jan 2023</span></p>
      <ul>
        <li>Defined and executed product roadmaps with third-party integrations.</li>
        <li>Optimized eCommerce performance using SQL, iPaaS, and Agile methodologies.</li>
      </ul>

      <p><span class="job-title">Segra | Software Engineer</span> <span class="job-date">Feb 2021 – Mar 2022</span></p>
      <ul>
        <li>Designed and implemented backend solutions to improve system automation.</li>
        <li>Developed integrations with C#, .NET Core, JavaScript, and PowerShell.</li>
      </ul>

      <p><span class="job-title">OSSID ProMach | Software Engineer</span> <span class="job-date">Oct 2019 – Apr 2021</span></p>
      <ul>
        <li>Built full-stack product management system, guiding API architecture and scalability.</li>
        <li>Developed class libraries to enhance functionality.</li>
      </ul>

      <p><span class="job-title">FlyExclusive | Software Engineer</span> <span class="job-date">Aug 2017 – Oct 2019</span></p>
      <ul>
        <li>Developed internal applications using .NET Core, C#, jQuery, Bootstrap, SQL.</li>
        <li>Built and maintained API microservices and a monolithic shared library.</li>
      </ul>

      <p><span class="job-title">Online Information Services | Software Engineer</span> <span class="job-date">Sep 2014 – Jun 2017</span></p>
      <ul>
        <li>Led ETL process development using CloverDX, integrating data for reporting.</li>
        <li>Developed internal and external reports via web services, SFTP, SQL.</li>
      </ul>
    </div>

    <div class="section">
      <h2>Military Experience</h2>
      <ul>
        <li>Trained in human resources and multimedia illustration (U.S. Army Reserves).</li>
        <li>Developed technical documentation and training materials.</li>
        <li>Served as squad leader, honing leadership and problem-solving skills.</li>
      </ul>
    </div>

    <div class="section">
      <h2>Other Experience</h2>
      <ul>
        <li>Computer Geeks (Technical Support, Web Development)</li>
        <li>Pitt Community College (Tutor – Computer Science & IT Courses)</li>
        <li>Grover Gaming, Inc. (Co-op Software Engineer)</li>
      </ul>
    </div>

    <div class="section">
      <h2>Education</h2>
      <ul>
        <li>East Carolina University – B.S. Information & Computer Technology, 2020</li>
        <li>Pitt Community College – Associate in Arts, 2013</li>
      </ul>
    </div>

    <div class="section">
      <h2>Certifications</h2>
      <ul>
        <li>Certified Scrum Product Owner (Scrum Alliance)</li>
        <li>C++, Java, VB, and C# Programming Certifications (Pitt Community College)</li>
        <li>Python (Coursera)</li>
      </ul>
    </div>
  </div>

</template>

<style scoped>
.read-the-docs {
  color: #888;
}
body {
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background: #f9f9f9;
      color: #333;
      text-align: left;
    }
    .container {
      max-width: 900px;
      margin: auto;
      padding: 2rem;
      background: #fff;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: left;
    }
    h1, h2, h3 {
      color: #2c3e50;
      text-align: left;
    }
    h1 {
      margin-bottom: 0;
    }
    .section {
      margin-top: 2rem;
    }
    .subheading {
      font-weight: bold;
      color: #007bff;
    }
    ul {
      padding-left: 1.2rem;
    }
    .job-title {
      font-weight: bold;
    }
    .job-date {
      float: right;
      color: #666;
      font-size: 0.9em;
    }
    .contact {
      margin-top: 0.5rem;
      font-size: 0.95rem;
    }
</style>
