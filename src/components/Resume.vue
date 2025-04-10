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
    <p>North Carolina | (252) 417-3824 | <a href="mailto:wjg284@gmail.com">wjg284@gmail.com</a></p>

    <div class="section">
        <h2>Professional Summary</h2>
        <p>Results-driven Software Engineer & Certified Scrum Product Owner (CSPO) with 10+ years of experience in full-stack development, API integrations, and product lifecycle management. Skilled in developing scalable software solutions, leading cross-functional teams, and streamlining business processes. Adept at translating technical requirements into actionable outcomes with expertise in C#, .Net, SQL, jQuery, and Agile methodologies.</p>
    </div>

    <div class="section">
        <h2>Technical Skills</h2>
        <ul>
            <li><strong>Programming:</strong> C#, .NET Core, Entity Framework, JavaScript, Python, PHP, Java, C++</li>
            <li><strong>Databases:</strong> Microsoft SQL Server, Oracle SQL, SAP Hana, PostgreSQL</li>
            <li><strong>Cloud & DevOps:</strong> Azure, AWS, Docker, Jenkins, Kubernetes, SDLC, Unit Testing</li>
            <li><strong>Web Technologies:</strong> HTML, CSS, Bootstrap, Vue.js, jQuery, Sails.js</li>
            <li><strong>API Development:</strong> RESTful APIs, Microservices, Integration Services</li>
            <li><strong>Agile & Scrum:</strong> Product Ownership, Backlog Management, Roadmap Planning, Jira</li>
            <li><strong>ETL & Data Processing:</strong> SQL, Tray.io, CloverDX, Reporting & Analytics</li>
        </ul>
    </div>

    <div class="section">
        <h2>Professional Experience</h2>
        <ul>
            <li><strong>iPaaS.com | Integration Developer | Atlanta, GA</strong> (Dec 2024 – Mar 2025)
                <ul>
                    <li>Developed C# integrations for the iPaaS.com Marketplace to enhance automation.</li>
                    <li>Assisted integration team, testing the integration SDK and software functionality.</li>
                </ul>
            </li>
            <li><strong>Webb Design (NetApp) | Integration Specialist | San Francisco, CA</strong> (Mar 2023 – Dec 2024)
                <ul>
                    <li>Led marketing tech integration strategy, automating workflows and connections.</li>
                    <li>Developed integrations for business goals using Sails.js & PostgreSQL.</li>
                </ul>
            </li>
            <li><strong>Third Wave Business Systems | Product Owner | Wayne, NJ</strong> (Mar 2022 – Jan 2023)
                <ul>
                    <li>Defined and executed product roadmaps with third-party integrations.</li>
                    <li>Optimized eCommerce performance using SQL, iPaaS, and Agile methodologies.</li>
                </ul>
            </li>
            <li><strong>Segra | Software Engineer | Charlotte, NC</strong> (Feb 2022 – Mar 2023)
                <ul>
                    <li>Designed and implemented backend solutions to improve system automation.</li>
                    <li>Developed integrations with C#, .NET Core, JavaScript, and PowerShell.</li>
                </ul>
            </li>
            <li><strong>Listrak | Software Engineer | Lititz, PA</strong> (Apr 2021 – Jan 2022)
                <ul>
                    <li>Built full-stack SaaS digital marketing platform using C#, .Net, SQL, Vue.js.</li>
                    <li>Applied Agile methodologies with emphasis on testing, code coverage, monitoring.</li>
                </ul>
            </li>
            <li><strong>OSSID ProMach | Software Engineer | Rocky Mount, NC</strong> (Oct 2020 – Apr 2021)
                <ul>
                    <li>Built full-stack product management system, guiding API architecture and scalability.</li>
                    <li>Developed class libraries to enhance functionality.</li>
                </ul>
            </li>
            <li><strong>flyExclusive | Software Engineer | Kinston, NC</strong> (Aug 2017 – Oct 2020)
                <ul>
                    <li>Developed internal applications for operations and sales teams using .Net, C#, JQuery, Bootstrap, CSS, SQL.</li>
                    <li>Built and maintained API microservices and a monolithic shared library.</li>
                </ul>
            </li>
            <li><strong>Online Information Services | Software Engineer | Winterville, NC</strong> (Sept 2014 - Jun 2017)
                <ul>
                    <li>Led ETL process development using CloverDX, integrating data for reporting.</li>
                    <li>Developed internal and external reports via web services, SFTP, SQL.</li>
                </ul>
            </li>
        </ul>
    </div>

    <div class="section">
        <h2>Military Experience</h2>
        <p><strong>U.S. Army Reserves</strong></p>
        <ul>
            <li>Trained in human resources and multimedia illustration.</li>
            <li>Developed technical documentation and training materials for various projects.</li>
            <li>Strengthened leadership, teamwork, and problem-solving skills in high-pressure environments as squad leader.</li>
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
            <li>East Carolina University – Bachelor of Science Information & Computer Technology (2020)</li>
            <li>Pitt Community College – Associate in Arts (2013)</li>
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

    <div class="section">
        <h2>Websites</h2>
        <p><a href="https://www.linkedin.com/in/william-gates-038429b6/">LinkedIn Profile</a> | <a href="https://williamgates.space">Personal Website</a></p>
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
