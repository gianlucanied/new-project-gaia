<script setup>
const isVideo = (url) => {
  return url.endsWith(".mp4");
};

const projects = [
  {
    role: "CREATIVE PRODUCTION",
    title: "PRADA - CREATIVE PRODUCTION",

    image: [
      "/immagini_video_high_res/prada/1.mp4",
      "/immagini_video_high_res/prada/2.mp4",
      "/immagini_video_high_res/prada/3.mp4",
      "/immagini_video_high_res/prada/4.mp4",
      "/immagini_video_high_res/prada/5.mp4",
      "/immagini_video_high_res/prada/6.mp4",
      "/immagini_video_high_res/prada/7.mp4",

    ],
    description: `Management of all phases of the creative production (art buying, logistics, rentals, location scouting) and post-production. <br/><br/>
Campaigns I worked with include:
<ul>
<li>Prada SS26 Campaign</li>
<li>Prada SS26 Womenswear Show</li>
<li>Prada SS26 Menswear Show</li>
<li>Prada Holiday 2025 Campaign</li>
<li>Prada FW25 ADV Campaign</li>
<li>Prada Leather Goods Campaign</li>
<li>Prada Fine Jewellery Campaign</li>
<li>Prada FW25 Womenswear Show</li>
</ul>`,
  },
  {
    role: "PROJECT MANAGEMENT",
    title: "CONVEY MILAN DESIGN WEEK 2025 - EXHIBITION PRODUCTION",
    image: [
      "/immagini_video_high_res/convey_installation-view-27-768x960.jpeg",
      "/immagini_video_high_res/convey_installation-view-26-768x960.jpg",
      "/immagini_video_high_res/convey_installation-view-18-768x960.jpg",
      "/immagini_video_high_res/convey11.jpg",

    ],
    description: `Convey reached its third edition, establishing itself as a prominent international platform and accelerator for design. <br/>
In close collaboration with Simple Flair studio, I had the role of project manager of the exhibition and event producer, keep deadlines and overseeing the brand identity
and art direction for the setup and spatial design of the new location in the heart of Porta Venezia. <br/>
The project expanded along the street, creating a cohesive and engaging territorial experience that seamlessly integrated various brand showcases and initiatives.`,
    location: `Branding: Giga Design Studio <br>
          Curatorship: Simple Flair <br>
          Graphics + Art: Anna Meck<br> <br> shown at <br>
                      Milan Design Week <br>
                      Via Rosolino Pilo 14, Milano <br>
                      10 - 13 April 2025 <br> <br>
                      Photography: Maryan Sayd + Kristina Railaitè <br> <br>
On view at Horst Festival / Asiat Park Vilvoorde, Belgium`,
  },
  {
    role: "SET DESIGN",
    title: "JOSHUA SERAFIN FOR HORST FESTIVAL - SET DESIGN",
    image: [
      "/immagini_video_high_res/josh.jpg",
      "/immagini_video_high_res/josh1.jpg",
      "/immagini_video_high_res/HORST.jpg",
    ],
    description: `"Buried in a Coffin the Size of a Grain of Rice" (Installation) and "Midnight Pearls" (film) were installed in one of the art pavilion at Horst festival for the 2025
edition. <br>
Within this space of meditation, prayer, silence and offering, we are invited to at once re-enter the body and be transported to an in-between realm. <br>
Here, darkness is embraced to discover the first rays of light. <br>
A portal connects the ancestral with the mortal world and allows entities to watch over the current mortal realm, offering guidance to those willing to receive. We find a
guardian watching over an unborn entity, in utero in the swamp. <br>
I was part of the set design team that built the art and the pavilion before Horst Festival.`,
    location: `Artist: Joshua Serafin <br>
Photography: Maryan Sayd + Kristina Railaitè <br> <br>
On view at Horst Festival / Asiat Park Vilvoorde, Belgium`,
  },
  {
    role: "CREATIVE PRODUCTION",
    title: "DIESEL - CREATIVE PRODUCTION",
    image: [
      "/immagini_video_high_res/diesel/1.mp4",
      "/immagini_video_high_res/diesel/23.mp4",
      "/immagini_video_high_res/diesel/234.mp4",
    ],
    description: `Management of all phases of the creative production (art buying, logistics, rentals, livestream partners, location scouting) and post-production. <br>
Campaigns I worked with include:
<ul> 
      <li>Diesel SS26 Show & Livestream with Lyas</li>
        </ul>`,
    location: ``,
  },
  {
    role: "CREATIVE PRODUCTION",
    title: "ACNE STUDIOS - CREATIVE PRODUCTION",
    image: [
      "/immagini_video_high_res/acnestudios/acne.mp4",
      "/immagini_video_high_res/acnestudios/acne1.mp4",
      "/immagini_video_high_res/acnestudios/acne3.mp4",
    ],
    description: `Management of all phases of the creative production (art buying, logistics, rentals, location scouting) and post-production.<br>
    Campaigns I worked with include:
    <ul> 
      <li>Acne Studios TikTok Always On content</li>
      <li>Acne Studios FW23 Show</li>
      <li>Acne Studios FW23 ADV Campaign</li>
      <li> Acne Studios SS23 Show</li>
    </ul>`,
    location: ``,
  },
  {
    role: "FEATURE WRITING",
    title: "SUZANNE CIANI / NR MAGAZINE - CONTENT WRITING",
    image: [
      "/immagini_video_high_res/1.jpg",
      "/immagini_video_high_res/14.58.05.png",
      "/immagini_video_high_res/17.10.24.png",
    ],
    description: `Interview to Suzanne Ciani - the legendary electronic music pioneer - discussing her decades-long career, transcendence in sound, and reshaping consciousness. <br>
Interview by Gaia Grisanti <br>
Photography by Yudo Kurita <br>
Styling by Elidad <br>
Clothes Bottega Veneta <br> <br>
Editor-In-Chief: Jade Removille <br>
Photography: Yudo Kurita`,
    location: "",
  },

  {
    role: "",
    title: "EQUILIBRIO PROJECT 2024 - PRODUCTION & SMM",
    image: [
      "/immagini_video_high_res/equilibrio/eq.jpg",
      "/immagini_video_high_res/equilibrio/eq1.jpg",
      "/immagini_video_high_res/equilibrio/equilibrio_1.jpg",
    ],
    description: `Equilibrio is a yearly art residency and music festival taking place in Porto Ferro, Sardinia where emerging artists and experimental music
merge in a 7 days community experience. <br>
I was part of the collective, overseeing the the production of the festival (logistic, artists accommodation, food and beverage
organisation), the set design of the space and the communication (social media content, copywriting) and business developments (connect
with potential partners, make presentations and planning).`,
    location: "Posters: Ekaterina Shuvchinskaia",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "LORO PIANA - CREATIVE PRODUCTION",
    image: [
      "/immagini_video_high_res/loro-piana/loro.mp4",
      "/immagini_video_high_res/loro-piana/loro1.mp4",
      "/immagini_video_high_res/loro-piana/loro2.mp4",
      "/immagini_video_high_res/loro-piana/loro3.mp4",
    ],
    description: `Management of all phases of the creative production, art buying and post-production. <br>
Campaigns I worked with include:
<ul> 
      <li>Loro Piana Holiday 2024 Campaign</li>
      <li>Loro Piana FW24 Campaign</li>
      <li>Loro Piana SS24 Campaign</li>
      <li>Loro Piana Cocooning Campaign</li>
      <li> Loro Piana FW24, SS24, FW23 Campaigns</li>
    </ul>`,
    location: ``,
  },
];
</script>

<template>
  <!-- Contenuto principale -->
  <div class="works">
    <div class="single-work" v-for="(project, index) in projects" :key="index">
      <div class="title-single">{{ project.title }}</div>
      <div class="image-gallery">
        <template v-for="(img, imgIndex) in project.image" :key="imgIndex">
          <video v-if="isVideo(img)" :src="img" controls muted loop></video>
          <img v-else :src="img" alt="" />
        </template>
      </div>
      <p class="role">{{ project.role }}</p>
      <p><span v-html="project.description"></span></p>
      <div v-if="project.location">
        <p>
          <br />
          <span v-html="project.location"></span>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.works {
  color: black;
  background-color: white;
  padding: 3rem;
  height: auto;
  min-height: 100vh;
  position: relative;
  z-index: 1;
}

.title-single {
  font-size: 25px;
  margin-bottom: 50px;
}

.role {
  margin-top: 40px;
}

.single-work {
  margin: 2rem 0;
  font-family: "Courier New", Courier, monospace;
  font-size: 15px;
}

.image-gallery {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.image-gallery img,
.image-gallery video {
  width: 250px;
  height: 350px;
  object-fit: cover;
}
</style>