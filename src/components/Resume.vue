<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
 <h1>William Gates</h1>
    <p>North Carolina | (252) 417-3824 | <a href="mailto:wjg284@gmail.com">wjg284@gmail.com</a></p>

    <div class="content">
        <h2>Professional Summary</h2>
        <p>Enterprise Integration Engineer and Certified Scrum Product Owner with extensive experience designing API-driven integrations, leading enterprise software implementations, and building scalable automation solutions. Skilled in translating business requirements into technical architectures while serving as the bridge between engineering teams, customers, and product organizations. Experienced leveraging AI-assisted development, modern integration platforms, and cloud technologies to accelerate delivery, improve operational efficiency, and solve complex enterprise integration challenges.</p>

        <h2>Technical Skills</h2>
        <ul>
            <li>Programming: C#, .NET Core, Entity Framework, JavaScript, Python, PHP, Java, C++, OOP, TDD, SOLID</li>
            <li>Databases: Microsoft SQL Server, Oracle SQL, SAP Hana, PostgreSQL</li>
            <li>Cloud & DevOps: Azure, AWS, Docker, Jenkins, Kubernetes</li>
            <li>API Development: RESTful APIs, Microservices, Integration Services</li>
            <li>Agile & Scrum: Product Ownership, Backlog Management, Roadmap Planning, Jira</li>
            <li>ETL & Data Processing: SQL, Tray.io, PowerAutomate CloverDX, Reporting & Analytics</li>
        </ul>

        <h2>AI &amp; Automation</h2>
        <ul>
            <li>AI Platforms: ChatGPT, Claude, GitHub Copilot, Cursor, OpenAI Codex, Gemini</li>
            <li>LLM Development: Prompt Engineering, AI-Assisted Coding, Debugging, Documentation, Code Review</li>
            <li>AI Integration: REST APIs, OpenAI-Compatible APIs, Function Calling, Tool Integration, JSON Schema</li>
            <li>Agentic Systems: AI Agents, Model Context Protocol (MCP), Agentic Workflows, Context Engineering</li>
            <li>Automation: Python Automation, Workflow Automation, AI-Driven Process Optimization</li>
        </ul>

        <h2>Professional Experience</h2>

        <h3>PayIt | Technical Integration Manager | Kansas City, MO | Jun 2025 - Jul 2026</h3>
        <ul>
            <li>Working directly with government agencies and other clients to understand their existing systems and define integration requirements.</li>
            <li>Designing, developing, and implementing integrations using MuleSoft, SQL, APIs, and other middleware tools.</li>
            <li>Ensuring seamless data flow between disparate systems by designing effective data mappings and transformations.</li>
            <li>Building and managing APIs to facilitate secure and scalable integrations between client systems and our platform.</li>
        </ul>

        <h3>iPaaS.com | Integration Developer | Atlanta, GA | Dec 2024 – Jun 2025</h3>
        <ul>
            <li>Developed C# integrations for the iPaaS.com Marketplace to enhance automation.</li>
            <li>Assisted integration team, testing the integration SDK and software functionality.</li>
        </ul>

        <h3>Webb Design (NetApp) | Integration Specialist | San Francisco, CA | Mar 2024 – Dec 2024</h3>
        <ul>
            <li>Designed and deployed a full-stack reporting dashboard using Sails.js, Vue.js, and PostgreSQL.</li>
            <li>Created automation pipelines via Tray.io and Power Automate for cross-departmental workflows.</li>
            <li>Led marketing technology integration efforts, reducing manual reporting by 60%.</li>
        </ul>

        <h3>Third Wave Business Systems | Product Owner | Wayne, NJ | Mar 2023 – Jan 2024</h3>
        <ul>
            <li>Co-led SAP eCommerce platform integrations with Shopify and Amazon.</li>
            <li>Defined and prioritized roadmap features based on stakeholder needs and tech feasibility.</li>
            <li>Authored user stories for Agile sprints, enabling efficient collaboration with dev teams.</li>
        </ul>

        <h3>Segra | Software Engineer | Charlotte, NC | Feb 2022 – Mar 2023</h3>
        <ul>
            <li>Developed backend automation tools for ERP/CRM systems using ASP.NET Core, C#, SQL.</li>
            <li>Refactored SQL, SSRS, and PowerShell scripts to enhance maintainability and execution speed.</li>
        </ul>

        <h3>Listrak | Software Engineer | Litiz, PA | Apr 2021 – Jan 2022</h3>
        <ul>
            <li>Engineered features for a full-stack SaaS digital marketing platform using C#, .NET, SQL, and Vue.js.</li>
            <li>Practiced Agile principles emphasizing test coverage, performance monitoring, and deployment readiness.</li>
            <li>Integrated client-driven enhancements into core platform features across releases.</li>
        </ul>

        <h3>OSSID ProMach | Software Engineer | Rocky Mount, NC | Oct 2020 – Apr 2021</h3>
        <ul>
            <li>Created a WPF-based labeling solution interfacing with packaging machines via TCP/IP.</li>
            <li>Built modular C#/.NET Core class libraries for reusable business logic.</li>
            <li>Developed UI components with runtime reflection to support varied client configurations. </li>
        </ul>

        <h3>FlyExclusive | Software Engineer | Kinston, NC | Aug 2017 – Oct 2020</h3>
        <ul>
            <li>Designed a greenfield aircraft maintenance system used by multiple departments using ASP.Net Core, C#, SQL.</li>
            <li>Built and maintained API microservices and a monolithic shared library.</li>
            <li>Managed CI/CD with TDD, Azure, analytics </li>
        </ul>

        <h3>Online Information Services | Software Engineer | Winterville, NC | Sept 2014 – Jun 2017</h3>
        <ul>
            <li>Led ETL efforts using CloverDX, managing high-volume data transformations.</li>
            <li>Automated regulatory notice delivery with external vendors.</li>
            <li>Developed internal and external reports via web services, SFTP, SQL</li>
        </ul>

        <h2>Military Experience</h2>
        <p>U.S. Army Reserves</p>
        <ul>
            <li>Trained in human resources and multimedia illustration.</li>
            <li>Developed technical documentation and training materials for various projects.</li>
        </ul>

        <h2>Education</h2>
        <p>East Carolina University - Bachelor of Science, Information and Computer Technology (2020)</p>
        
        <p>Pitt Community College - Associate in Arts, Computer Programming (2013)</p>

        <h2>Certifications</h2>
        <ul>
            <li>Certified Scrum Product Owner (Scrum Alliance)</li>
            <li>C++, Java, VB, and C# Programming Certifications (Pitt Community College)</li>
            <li>Python (Coursera)</li>
        </ul>

        <h2>Websites</h2>
        <p><a href="https://www.linkedin.com/in/william-gates-038429b6/">LinkedIn</a> | <a href="https://williamgates.space">Portfolio</a>| <a href="https://github.com/bgates284">GitHub</a>| <a href="https://mvcportfolio-h3fdhzh7e9gfe2f6.canadaeast-01.azurewebsites.net/">ASP.NET Core Project</a></p>
    </div>

</template>

<style>
/* body {
    font-family: Arial, sans-serif;
    line-height: 1.4;
    max-width: 800px;
    margin: auto;
    padding: 20px;
    text-align: center;
} */
.content {
    text-align: left;
    margin: auto;
    width: 90%;
}
h1, h2 {
    margin-top: 20px;
    border-bottom: 2px solid #333;
    padding-bottom: 5px;
}
ul {
    padding-left: 20px;
    margin: 5px 0;
}
li {
    margin-bottom: 3px;
}
</style>

