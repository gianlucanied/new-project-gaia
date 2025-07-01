<script setup>
import { nextTick, ref } from "vue";

const selectedProject = ref(0);
const projectDetailsRef = ref(null);

const selectProject = async (index) => {
  selectedProject.value = index;
  await nextTick();
  projectDetailsRef.value?.scrollIntoView({ behavior: "smooth" });
};

const isVideo = (url) => {
  return url.endsWith(".mp4");
};

const projects = [
  {
    role: "SET DESIGN",
    title: "JOSHUA SERAFIN FOR HORST 2025",
    image: [
      "/immagini_video_high_res/details.jpg",
      "/immagini_video_high_res/details-2.jpg",
      "/immagini_video_high_res/HORST.jpg",
    ],
    description: `“Buried in a Coffin the Size of a Grain of Rice” (Installation) and “Midnight Pearls” (film) were installed in one of the art
          pavilion at Horst festival for the 2025 edition. <br> Within this space of meditation, prayer, silence and offering, we are invited to at
          once re-enter the body and be transported to an in-between realm. <br> Here, darkness is embraced to discover the first rays of light. <br> A
          portal connects the ancestral with the mortal world and allows entities to watch over the current mortal realm, offering guidance to
          those willing to receive. We find a guardian watching over an unborn entity, in utero in the swamp. <br>
          I was part of the set design team that built the art and the pavilion before Horst Festival. `,
    location:
      "Artist: Joshua Serafin <br> Photography: Maryan Sayd + Kristina Railaitè <br><br> On view at Horst Festival / Asiat Park Vilvoorde, Belgium",
  },
  {
    role: "PROJECT MANAGEMENT",
    title: "CONVEY 2025",
    image: [
      "/immagini_video_high_res/convey_installation-view-27-768x960.jpeg",
      "/immagini_video_high_res/convey_installation-view-26-768x960.jpg",
      "/immagini_video_high_res/convey_installation-view-18-768x960.jpg",
    ],
    description: `Convey reached its third edition, establishing itself as a prominent international platform and accelerator for design. <br> In close
          collaboration with Simple Flair studio, I had the role of project manager of the exhibition and event producer, keep deadlines
          and overseeing the brand identity and art direction for the setup and spatial design of the new location in the heart of Porta
          Venezia. <br> The project expanded along the street, creating a cohesive and engaging territorial experience that seamlessly
          integrated various brand showcases and initiatives.`,
    location: `Branding: Giga Design Studio <br>
          Curatorship: Simple Flair <br>
          Graphics + Art: Anna Meck<br> <br> shown at <br>
                      Milan Design Week <br>
                      Via Rosolino Pilo 14, Milano <br>
                      10 - 13 April 2025`,
  },
  {
    role: "CREATIVE PRODUCTION",
    title: "PRADA FW25 SHOW",
    image: [
      "/immagini_video_high_res/9.mp4",
      "/immagini_video_high_res/Download.mp4",
    ],
    description: `Definition of creative briefs and image research. <br>
          Management of all phases of the creative production: creative partners (set design team, styling team, DOP team, editors, models), fees negotiation, budget alignment. <br>
          Coordination of pre-production logistc and post-production scheduling. <br>
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
    location: "",
  },
  {
    role: "CREATIVE PRODUCTION",
    title: "PRADA ALWAYS ON",
    image: [
      "/immagini_video_high_res/Download_(1).mp4",
      "/immagini_video_high_res/Download-copy.mp4",
      "/immagini_video_high_res/Download-copy-2.mp4",
    ],
    description: `Definition of creative briefs and image research. <br>
          Management of all phases of the creative production: creative partners (set design team, styling team, DOP team, editors,
          models), fees negotiation, budget alignment. <br>
          Coordination of pre-production logistc and post-production scheduling. <br>
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
    location: "",
  },
  {
    role: "EVENT PRODUCTION",
    title: "EQUILIBRIO PROJECT 2024",
    image: [
      "/immagini_video_high_res/10.jpg",
      "/immagini_video_high_res/equilibrio_1.jpg",
      "/immagini_video_high_res/8.jpg",
    ],
    description: `Equilibrio is a yearly art residency and music festival taking place in Porto Ferro, Sardinia where emerging artists and experimental music
          merge in a 7 days community experience. <br>
          I was part of the collective, overseeing the the production of the festival (logistic, artists accommodation, food and beverage
          organisation), the set design of the space and the communication (social media content, copywriting) and business developments (connect
          with potential partners, make presentations and planning)`,
    location: "",
  },

  {
    role: "FEATURE WRITING",
    title: "SUZANNE CIANI X NR MAGAZINE",
    image: [
      "/immagini_video_high_res/17.10.24.png",
      "/immagini_video_high_res/14.58.05.png",
      "/immagini_video_high_res/1.jpg",
    ],
    description: `Interview to Suzanne Ciani - the legendary electronic music pioneer - discussing her decades-long career, transcendence in
          sound, and reshaping consciousness. <br>
          Interview by Gaia Grisanti <br>
          Photography by Yudo Kurita <br>
          Styling by Elidad <br>
          Clothes Bottega Veneta`,
    location: "Editor-In-Chief: Jade Removille <br> Photography: Yudo Kurita",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "ACNE STUDIOS FW23 SHOW",
    image: [
      "/immagini_video_high_res/FqJZSEuWcAA0uTa.jpeg",
      "/immagini_video_high_res/Screenshot2025-06-17184652.png",
      "/immagini_video_high_res/Screenshot2025-06-17184824.png",
    ],
    description: `Support in all the digital content production for FW23 Acne Studios Show: pre-production logistic and post production phases, assisting onsite for all
          social-first content, ensuring alignment with the brand guideline. <br>
          Production of ad-hoc timelines for content production, post-production and delivery for all social platforms. <br>
          Image and film coordination of KOLs, celebrities and Talents at the photocall. <br>
          Definition of the the social editorial calendars and content rollouts.`,
    location:
      "shown at Lycée Carnot 145 Boulevard Malesherbes in the 17th arrondissement, Paris",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "ACNE STUDIOS SS23 SHOW",
    image: [
      "/immagini_video_high_res/234.png",
      "/immagini_video_high_res/345.png",
      "/immagini_video_high_res/456.png",
    ],
    description: `Support in all the digital content production for FW23 Acne Studios Show: pre-production logistic and post production phases, assisting onsite for all
          social-first content, ensuring alignment with the brand guideline. <br>
          Production of ad-hoc timelines for content production, post-production and delivery for all social platforms. <br>
          Image and film coordination of KOLs, celebrities and Talents at the photocall. <br>
          Definition of the the social editorial calendars and content rollouts`,
    location:
      "shown at Palais De Tokyo 13 Av. du Président Wilson, 75116 Paris, France",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "ACNE STUDIOS DIGITAL CONTENT",
    image: [
      "/immagini_video_high_res/Download(1)copy.mp4",
      "/immagini_video_high_res/Download(2).mp4",
      "/immagini_video_high_res/Downloadcopy3.mp4",
    ],
    description: `Art direction and content production for Acne Studios Tik Tok channel, featuring runway content, <br>
          Backstage, everyday storytelling. <br>
          Production of ad-hoc timelines for content production, post-production and delivery for all social platforms. <br>
          Coordination the social editorial calendars and content rollouts.`,
    location: "",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "LORO PIANA FW24 LOOKBOOK",
    image: [
      "/immagini_video_high_res/Downloadcopy6.mp4",
      "/immagini_video_high_res/Downloadcopy5.mp4",
      "/immagini_video_high_res/Downloadcopy4.mp4",
    ],
    description: `Definition of creative briefs and image research. <br>
          Management of all phases of the content production: managing creative partners (set design team, styling team, DOP team,
          editors, models) <br>
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
    location: "",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "LORO PIANA HOLIDAY CAMPAIGN FW24",
    image: [
      "/immagini_video_high_res/Downloadcopy7.mp4",
      "/immagini_video_high_res/Downloadcopy11.00.07.mp4",
    ],
    description: `Definition of creative briefs and image research. <br>
          Management of all phases of the content production: managing creative partners (set design team, styling team, DOP team,
          editors, models) <br>
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
    location: "",
  },

  {
    role: "CREATIVE PRODUCTION",
    title: "LORO PIANA COCOONING CAMPAIGN SS23",
    image: [
      "/immagini_video_high_res/Downloadcopy8.mp4",
      "/immagini_video_high_res/Download(1)copy3.mp4",
    ],
    description: `Definition of creative briefs and image research. <br>
          Management of all phases of the content production: managing creative partners (set design team, styling team, DOP team,
          editors, models) <br>
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
    location: "",
  },

  {
    role: "EVENT + TALENTS COORDINATION",
    title: "LORO PIANA MILAN DESIGN WEEK 2024",
    image: ["/immagini_video_high_res/7.jpg", "/immagini_video_high_res/2.jpg"],
    description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination.
          My task was implementing the awareness of the brand, by activating the right talents and digital creators. <br>
          MY role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand. <br>
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation. <br>
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams. <br>
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
    location: "",
  },

  {
    role: "EVENT + TALENTS COORDINATION",
    title: "LORO PIANA SS24 PRESS PRESENTATION",
    image: [
      "/immagini_video_high_res/Screenshot2025-0604at17.47.47.png",
      "/immagini_video_high_res/6.jpeg",
      "/immagini_video_high_res/542254254.png",
    ],
    description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination. <br>
          My task was implementing the awareness of the brand, by activating the right talents and digital creators. <br>
          MY role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand. <br>
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation. <br>
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams. <br>
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
    location: "",
  },

  {
    role: "EVENT + TALENTS COORDINATION",
    title: "LORO PIANA FW24 PRESS PRESENTATION",
    image: [
      "/immagini_video_high_res/1234.png",
      "/immagini_video_high_res/527522552.png",
      "/immagini_video_high_res/55758.png",
    ],
    description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination. <br>
          My task was implementing the awareness of the brand, by activating the right talents and digital creators. <br>
          My role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand. <br>
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation. <br>
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams. <br>
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
    location: "",
  },
];
</script>

<template>
  <div class="works">
    <div class="list">
      <div class="name-list"
        v-for="(project, index) in projects"
        :key="index"
        @click="selectProject(index)"
      >
        {{ project.title }}
      </div>
    </div>

    <div class="single-work" v-if="selectedProject !== null" ref="projectDetailsRef">
      <div class="title-single">{{ projects[selectedProject].title }}</div>
      <div class="image-gallery">
        <template
          v-for="(img, imgIndex) in projects[selectedProject].image"
          :key="imgIndex"
        >
          <video
            v-if="isVideo(img)"
            :src="img"
            controls
            muted
            loop
          ></video>
          <img v-else :src="img" alt="" />
        </template>
      </div>
      <p class="role">{{ projects[selectedProject].role }}</p>
      <p><span v-html="projects[selectedProject].description"></span></p>
      <div v-if="projects[selectedProject].location">
        <p>
           <br />
          <span v-html="projects[selectedProject].location"></span>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.works {
  color: white;
  background-color: black;
  padding: 3rem;
  height: auto;
  min-height: 100vh;
}

.title-single {
  font-size: 25px;
  margin-bottom: 50px;
}

.list {
  font-family: "Andale Mono", sans-serif;
  font-size: 0.8rem;
  cursor: pointer;
  div {
    margin-bottom: 1rem;
    padding-bottom: 3px;
    border-bottom: 1px solid white;
  }
}

.role {
  margin-top: 40px;
}

.single-work {
  margin: 6rem 0;
  font-family: "Courier New", Courier, monospace;
  font-size: 15px;
}

.name-list {
  font-family: "Andale Mono", sans-serif;

}

.image-gallery {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.image-gallery img {
  width: 300px;
  height: 300px;
  object-fit: contain;
}

.image-gallery video {
  width: 300px;
  height: 400px;
  object-fit: contain;
}
</style>
