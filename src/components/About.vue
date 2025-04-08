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
        Hey there — I’m William Gates, a lifelong tech tinkerer turned software engineer with over a decade of experience building scalable applications, leading product initiatives, and integrating systems that make work (and life) a little smoother. My journey into tech started back when I was a kid, pulling things apart just to see how they worked — and I’ve been hooked ever since.
      </p>
      <p>
        Professionally, I’m a full-stack developer and Certified Scrum Product Owner who thrives on solving complex problems and working across teams to turn big ideas into real solutions. I’ve worn a lot of hats over the years — from backend dev to product owner — and I love the challenge of making technology work better for people.
      </p>
      <p>
        Outside of the screen glow, I’m a father, a community-minded neighbor, and someone who’s happiest outdoors — whether I’m wrangling chickens, soaking up the sun at the beach, or getting lost in a good book or podcast.
      </p>
      <p>Let’s build something great together.</p>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap');

.image-banner {
  margin-top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(to right, #007bff, #ffffff),
              linear-gradient(to bottom, #007bff, white);
  background-blend-mode: overlay;
  padding: 2rem;
  width: 100%;
  border-radius: 20px 20px 0 0;
  overflow: hidden;
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
  border: 2px solid #007bff;
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
</style>
