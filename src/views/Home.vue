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
            Formerly: Acne Studios, Loro Piana <br />Clients: Prada, Stone
            Island, Culted, Simple Flair, NR Magazine, Convey
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
          <div class="gn">
        <a href="https://gianlucanieddu.netlify.app/">© gianlucanied</a>
      </div>
  </div>
</template>

<style scoped>
.video-background-container {
  position: relative;
  width: 100%;
  min-height: 100vh;
  overflow: hidden;
}

.background-video {
  position: fixed;
  top: 50%;
  left: 50%;
  width: 100vw;
  height: 100vh;
  transform: translate(-50%, -50%);
  object-fit: cover; /* <-- Copre tutto lo schermo */
  z-index: -1;
}

.about {
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
  font-size: 15px;
  text-align: end;
  padding: 50px;
  font-family: "Courier New", Courier, monospace;
}

/* ✅ MEDIA QUERY CORRETTO */
@media (max-width: 768px) {
  .content-wrapper {
    max-width: 80vw;
  }

  .gn a {
    font-size: 10px;
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
