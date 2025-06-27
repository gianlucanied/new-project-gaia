<template>
  <div class="about">
    <div class="content-wrapper">
      <div class="top-section">
        <p>
          Working across multiple media and art forms, my practice spans
          creative production, art direction, strategic thinking, and research.
          Specialised in crafting visual and physical narratives that bridge
          culture, fashion, and contemporary design.
        </p>
        <p>
          Formerly: Acne Studios, Loro Piana <br />Clients: Prada, Stone Island,
          Culted, Simple Flair, NR Magazine, Convey
        </p>
      </div>

      <div class="bottom-section">
        <div>
          <p class="email">contact:
            <span class="typing-effect">
            <a href="mailto:gaia.grisanti@gmail.com">gaia.grisanti@gmail.com</a>
          </span></p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.about {
  color: white;
  padding: 6rem 0 3rem 0;
  display: flex;
  justify-content: center;
  font-family: "Courier New", Courier, monospace;
  height: 80vh;
  background-color: black;
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

@media (max-width: 768px) {
  .content-wrapper {
    max-width: 70vw;
  }
}
</style>
