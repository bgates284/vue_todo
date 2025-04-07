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
    padding: 0;
    width: 100%;
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
  
  .banner-text h2 {
    font-size: 1.5rem;
    margin: 0;
    line-height: 1.3;
  }
  
  .pic {
    width: 220px;
    height: 180px;
    border-top-right-radius: 20px;
  }
  
  /* Media Queries for Responsiveness */
  
  @media (max-width: 768px) {
    .image-banner {
      flex-direction: column; /* Stack text and image vertically */
      text-align: center; /* Center-align the text */
    }
  
    .banner-text {
      padding: 1rem; /* Reduce padding on smaller screens */
    }
  
    .banner-text h1 {
      font-size: 1.6rem; /* Adjust font size */
    }
  
    .banner-text h2 {
      font-size: 1.2rem; /* Adjust font size */
    }
  
    .pic {
      width: 150px; /* Adjust image size */
      height: 130px; /* Adjust image size */
      margin-top: 1rem; /* Add some space above the image */
    }
  }
  
  @media (max-width: 480px) {
    .banner-text h1 {
      font-size: 1.4rem; /* Smaller font size for smaller devices */
    }
  
    .banner-text h2 {
      font-size: 1rem; /* Smaller font size for smaller devices */
    }
  
    .pic {
      width: 120px; /* Further adjust image size */
      height: 100px; /* Further adjust image size */
      margin-top: 1rem; /* Space for the image */
    }
  }
  </style>
  