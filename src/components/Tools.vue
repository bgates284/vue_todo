<script>
export default {
  name: 'Tools',
  data() {
    return {
      tools: [
        { name: 'Adobe', url: 'https://www.adobe.com/', img: '/public/Images/adobe.png' },
        { name: 'Apple', url: 'https://www.apple.com/', img: '/public/Images/apple.png' },
        { name: 'Arduino', url: 'https://www.arduino.cc/', img: '/public/Images/arduino.png' },
        { name: 'Azure', url: 'https://azure.microsoft.com/', img: '/public/Images/azure.png' },
        { name: 'Bootstrap', url: 'https://getbootstrap.com/', img: '/public/Images/bootstrap.jpg' },
        { name: 'ChatGPT', url: 'https://chat.openai.com/', img: '/public/Images/ChatGPT.png' },
        { name: 'Confluence', url: 'https://www.atlassian.com/software/confluence', img: '/public/Images/confluence.png' },
        { name: 'Copilot', url: 'https://copilot.microsoft.com/', img: '/public/Images/Copilot.png' },
        { name: 'Coursera', url: 'https://www.coursera.org/', img: '/public/Images/coursera.png' },
        { name: 'CSS', url: 'https://developer.mozilla.org/en-US/docs/Web/CSS', img: '/public/Images/css.png' },
        { name: 'Dotnet', url: 'https://dotnet.microsoft.com/', img: '/public/Images/dotnet.jpg' },
        { name: 'Entity Framework', url: 'https://learn.microsoft.com/en-us/ef/', img: '/public/Images/EntityFramework.png' },
        { name: 'Figma', url: 'https://www.figma.com/', img: '/public/Images/Figma.png' },
        { name: 'FileZilla', url: 'https://filezilla-project.org/', img: '/public/Images/filezilla.png' },
        { name: 'Git', url: 'https://git-scm.com/', img: '/public/Images/git.png' },
        { name: 'Hacker News', url: 'https://news.ycombinator.com/', img: '/public/Images/hackernews.png' },
        { name: 'Hyper-V', url: 'https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/', img: '/public/Images/hyperv.png' },
        { name: 'IIS', url: 'https://www.iis.net/', img: '/public/Images/iis.png' },
        { name: 'Jira', url: 'https://www.atlassian.com/software/jira', img: '/public/Images/jira.png' },
        { name: 'jQuery', url: 'https://jquery.com/', img: '/public/Images/jQuery.png' },
        { name: 'JavaScript', url: 'https://www.javascript.com/', img: '/public/Images/js.png' },
        { name: 'LINQ', url: 'https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/', img: '/public/Images/linq.jpg' },
        { name: 'Miro', url: 'https://miro.com/', img: '/public/Images/Miro.png' },
        { name: 'Notepad++', url: 'https://notepad-plus-plus.org/', img: '/public/Images/notepad.png' },
        { name: 'Oracle SQL', url: 'https://www.oracle.com/database/technologies/appdev/sql.html', img: '/public/Images/oracleSQL.png' },
        { name: 'Paint.NET', url: 'https://www.getpaint.net/', img: '/public/Images/paintdotnet.png' },
        { name: 'PostgreSQL', url: 'https://www.postgresql.org/', img: '/public/Images/postgresql.png' },
        { name: 'Postman', url: 'https://www.postman.com/', img: '/public/Images/postman.png' },
        { name: 'Python', url: 'https://www.python.org/', img: '/public/Images/python.jpg' },
        { name: 'Raspberry Pi', url: 'https://www.raspberrypi.com/products/raspberry-pi-4-model-b/', img: '/public/Images/raspberrypi.jpg' },
        { name: 'Sails.js', url: 'https://sailsjs.com/', img: '/public/Images/sailsJS.png' },
        { name: 'SecTools', url: 'https://sectools.org/', img: '/public/Images/sectools.jpg' },
        { name: 'SQL', url: 'https://www.w3schools.com/sql/', img: '/public/Images/sql.png' },
        { name: 'SQL Server', url: 'https://www.microsoft.com/en-us/sql-server/sql-server-downloads', img: '/public/Images/sqlserver.png' },
        { name: 'Stack Overflow', url: 'https://stackoverflow.com/', img: '/public/Images/stackoverflow.png' },
        { name: 'Swift', url: 'https://developer.apple.com/swift/', img: '/public/Images/swift.png' },
        { name: 'Ultimate Boot CD', url: 'https://www.ultimatebootcd.com/', img: '/public/Images/ultimatebootcd.jpg' },
        { name: 'Visual Studio', url: 'https://visualstudio.microsoft.com/', img: '/public/Images/visual studio.jpg' },
        { name: 'VS Code', url: 'https://code.visualstudio.com/', img: '/public/Images/visualstudiocode.jpg' },
        { name: 'Vue.js', url: 'https://vuejs.org/', img: '/public/Images/vuejs.png' },
        { name: 'W3Schools', url: 'https://www.w3schools.com/', img: '/public/Images/w3schoole.jpg' },
        { name: 'Windows', url: 'https://www.microsoft.com/en-us/software-download/windows10', img: '/public/Images/windows.png' },
        { name: 'Wireshark', url: 'https://www.wireshark.org/', img: '/public/Images/wireshark.png' },
        { name: 'XAMPP', url: 'https://www.apachefriends.org/index.html', img: '/public/Images/xamp.png' },
        { name: 'Xcode', url: 'https://developer.apple.com/xcode/', img: '/public/Images/xcode.jpg' }
      ]
    };
  }
}
</script>

<template>
    <div class="tool-grid">
      <a
        v-for="tool in tools"
        :key="tool.name"
        :href="tool.url"
        class="tool-item"
        target="_blank"
        rel="noopener"
      >
      <img :src="tool.img" :alt="tool.name" class="tool-img" />
      </a>
    </div>
  </template>
  

  
  <style scoped>
  .tool-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.5rem;
    padding: 2rem;
  }
  .tool-item {
    width: 80px;
    height: 80px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .tool-item:hover {
    transform: scale(1.1);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
  }
  .tool-img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    border-radius: 50%;
  }
  </style>
  