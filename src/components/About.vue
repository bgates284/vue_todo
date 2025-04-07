<template>
    <div class="image-banner">
      <div class="banner-text">
        <h1>Software Engineer</h1>
        <h2> & </h2>
        <h2>Certified Scrum Product Owner</h2>
      </div>
      <img class="pic" src="/Images/ProfileImage2.png" />
    </div>
  </template>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap');
  
  .image-banner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(to right, #007bff, #ffffff),
                linear-gradient(to bottom,#007bff, white);
    background-blend-mode: overlay;
    padding: 0rem;
    width: 100%;
    /* box-sizing: border-box; */
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
    overflow: hidden;
    position: relative;
    margin-top: 5px;
  }
  
  .banner-text {
    flex: 1;
    color: rgb(4, 0, 0);
    font-family: 'Playfair Display', serif;
    padding: 2rem;
  }
  
  .banner-text h1 {
    font-size: 2rem;
    margin: 0;
    line-height: 1.3;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  
  .pic {
    width: 220px;
    height: 180px;
    border-top-right-radius: 20px;
  }

  </style>
  