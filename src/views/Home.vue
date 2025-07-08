<template>
  <div class="video-background-container">
    <!-- Video di sfondo -->
    <video autoplay muted loop playsinline class="background-video">
      <source src="/SFONDO-ABOUT.mp4" type="video/mp4" />
      Your browser does not support the video tag.
    </video>
    <div class="about">
      <div class="content-wrapper">
        <div class="top-section">
          <p>
            Working across multiple media and art forms, my practice spans
            creative production, art direction, strategic thinking, and
            research. Specialised in crafting visual and physical narratives
            that bridge culture, fashion, and contemporary design.
          </p>
          <p>
            Clients: Culted, Simple Flair, Prada, Stone Island, NR Magazine
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
    <div class="gn">© gianlucanied</div>
  </div>
</template>

<style scoped>
.video-background-container {
  position: relative;
  width: 100%;
  min-height: 100vh;
  overflow: hidden;
  background-color: black;
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

.about {
  position: relative;
  z-index: 1;
  color: white;
  padding: 6rem 0 3rem 0;
  display: flex;
  justify-content: center;
  font-family: "Courier New", Courier, monospace;
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
  color: white;
}

.bottom-section div {
  margin-top: 2rem;
  color: white;
  text-align: center;
}

.gn {
  color: white;
  font-size: 8px;
  text-align: end;
  padding: 70px 30px 30px;
  font-family: "Courier New", Courier, monospace;
  position: relative;
  z-index: 1;
}

@media (max-width: 768px) {
  .background-video {
    display: none;
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
}

</style>
