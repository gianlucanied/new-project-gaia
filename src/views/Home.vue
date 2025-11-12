<template>
  <div class="main">
    <div class="left-section">
      <img src="/immagini_video_high_res/Artboard-13.png" alt="" />
    </div>
    <div class="video-background-container">
      <!-- Video di sfondo per desktop -->
      <video autoplay muted loop playsinline class="background-video desktop-video">
        <source src="/sfondo_home_page_landscape.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
      <!-- Video di sfondo per mobile -->
      <video autoplay muted loop playsinline class="background-video mobile-video">
        <source src="/sfondo_homepage_iphone.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
      <div class="about">
        <div class="content-wrapper">
          <div class="top-section">
            <p>
              Working across multiple media and art forms, my practice spans
              project management, creative production, art direction, brand
              strategy and artistic research. <br />
              <br />
              Specialised in crafting visual and physical narratives that bridge
              culture, music, fashion and design. <br />
              <br />
            </p>
            <p>
              Clients: Culted, Simple Flair, Prada, Stone Island, NR Magazine
              <br />
              <br />Formerly: Acne Studios, Loro Piana
            </p>
          </div>
          <div class="bottom-section">
            <div>
              <p class="email">
                contact:
                <span class="typing-effect">
                  <a href="mailto:gaia.grisanti@gmail.com"
                    >gaia.grisanti@gmail.com</a
                  >
                </span>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="right-section">
      <img src="/immagini_video_high_res/Artboard-12.png" alt="" />
    </div>
  </div>
</template>

<style scoped>
.main {
  display: flex;
  height: 100vh;
}

.left-section,
.right-section {
  display: flex;
  flex-direction: column;
  flex: 0 0 auto;
  height: 100vh;
}

.left-section img,
.right-section img {
  width: 300px;
  height: 100%;
  object-fit: contain;
  display: block;
}

.video-background-container {
  position: relative;
  flex: 1;
  height: 100vh;
  overflow: hidden;
  /* background-color: black; */
}

.background-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 0;
}

/* Mostra solo video desktop di default */
.mobile-video {
  display: none;
}

.about {
  position: relative;
  z-index: 1;
  color: black;
  padding: 6rem 0 3rem 0;
  display: flex;
  justify-content: center;
  font-family: "Courier New", Courier, monospace;
  text-align: center;
  height: 80vh;
}

.content-wrapper {
  max-width: 50vw;
  padding: 1rem;
}

.top-section p {
  margin-bottom: 1rem;
}

.bottom-section {
  text-align: center;
  margin-top: 10rem;
}

a {
  text-decoration: none;
  color: black;
}

.bottom-section div {
  margin-top: 2rem;
  color: black;
  text-align: center;
}

.gn {
  color: black;
  font-size: 8px;
  text-align: end;
  padding: 70px 30px 30px;
  font-family: "Courier New", Courier, monospace;
  position: relative;
  z-index: 1;
}

@media (max-width: 768px) {
  /* Nascondi video desktop e mostra video mobile */
  .desktop-video {
    display: none;
  }
  
  .mobile-video {
    display: block;
  }
  
  .content-wrapper {
    max-width: 80vw;
  }
  
  .gn {
    font-size: 7px;
  }
  
  .about {
    padding: 3rem 0;
    height: auto;
  }
  
  .bottom-section {
    margin-top: 3rem;
  }
  
  .left-section,
  .right-section {
    display: none;
  }
  
  .main {
    height: auto;
  }
  
  .video-background-container {
    height: auto;
    min-height: 100vh;
  }
}
</style>