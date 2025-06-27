<script setup>
import { ref } from 'vue'

const selectedProject = ref(null)

const selectProject = (index) => {
  selectedProject.value = index
}

const projects = [
        {
          role: "SET DESIGN",
          title: "JOSHUA SERAFIN FOR HORST 2025",
          image: [

          ],

          description: `“Buried in a Coffin the Size of a Grain of Rice” (Installation) and “Midnight Pearls” (film) were installed in one of the art
          pavilion at Horst festival for the 2025 edition. Within this space of meditation, prayer, silence and offering, we are invited to at
          once re-enter the body and be transported to an in-between realm. Here, darkness is embraced to discover the first rays of light. A
          portal connects the ancestral with the mortal world and allows entities to watch over the current mortal realm, offering guidance to
          those willing to receive. We find a guardian watching over an unborn entity, in utero in the swamp.
          I was part of the set design team that built the art and the pavilion before Horst Festival. `,
          location:
            "Artist: Joshua Serafin Photography: Maryan Sayd + Kristina Railaitè <br><br> On view at Horst Festival / Asiat Park Vilvoorde, Belgium",
        },
        {
          role: "PROJECT MANAGEMENT",
          title: "CONVEY 2025",
          image: [

          ],
          description: `Convey reached its third edition, establishing itself as a prominent international platform and accelerator for design. In close
          collaboration with Simple Flair studio, I had the role of project manager of the exhibition and event producer, keep deadlines
          and overseeing the brand identity and art direction for the setup and spatial design of the new location in the heart of Porta
          Venezia. The project expanded along the street, creating a cohesive and engaging territorial experience that seamlessly
          integrated various brand showcases and initiatives.`,
          location: `Branding: Giga Design Studio
          Curatorship: Simple Flair
          Graphics + Art: Anna Meck<br> <br> shown at <br>
                  Milan Design Week <br>
                  Via Rosolino Pilo 14, Milano <br>
                  10 - 13 April 2025`,
        },
        {
          role: "CREATIVE PRODUCTION",
          title: "PRADA FW25 SHOW",
          image: [

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

          ],
          description: `Interview to Suzanne Ciani - the legendary electronic music pioneer - discussing her decades-long career, transcendence in
          sound, and reshaping consciousness. <br>
          Interview by Gaia Grisanti <br>
          Photography by Yudo Kurita <br>
          Styling by Elidad <br>
          Clothes Bottega Veneta`,
          location:
            "Editor-In-Chief: Jade Removille <br> Photography: Yudo Kurita",
        },

        {
          role: "CREATIVE PRODUCTION",
          title: "ACNE STUDIOS FW23 SHOW",
          image: [

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

          ],
          description: `Definition of creative briefs and image research. <br>
          Management of all phases of the content production: managing creative partners (set design team, styling team, DOP team, <br>
          editors, models) 
          Cross-funcational alignment with internal departments (Merchandising, Product, GTM, E-commerce, Paid Media)`,
          location: "",

        },

        {
          role: "CREATIVE PRODUCTION",
          title: "LORO PIANA HOLIDAY CAMPAIGN FW24",
          image: [

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
          image: [],
          description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination.
          My task was implementing the awareness of the brand, by activating the right talents and digital creators.
          MY role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand.
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation.
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams.
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
          location: "",

        },

        {
          role: "EVENT + TALENTS COORDINATION",
          title: "LORO PIANA SS24 PRESS PRESENTATION",
          image: [

          ],
          description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination.
          My task was implementing the awareness of the brand, by activating the right talents and digital creators.
          MY role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand.
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation.
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams.
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
          location: "",
        },

        {
          role: "EVENT + TALENTS COORDINATION",
          title: "LORO PIANA FW24 PRESS PRESENTATION",
          image: [

          ],
          description: `During my in-house experience at Loro Piana, I was in charge of social media and talents coordination.
          My task was implementing the awareness of the brand, by activating the right talents and digital creators.
          MY role required the creation of and influencer strategy and digital creators strategy to increase the awareness of the brand.
          I was particularly taking care of organising the talents journey (fitting, seeding, travels, accommodations),coordinating their
          presence at events and taking care of content creation.
          This process involved a high level of budget management, fees negotiation and internal coordination with communication teams.
          Talents involved: @fredstauffer @brendahashtag @stylenotcom @highsnobiety @culted @juliahobbs`,
          location: "",
        },
      ]
</script>

<template>
  <div class="works">
    <div>
      <div
        v-for="(project, index) in projects"
        :key="index"
        @click="selectProject(index)"
        style="cursor: pointer; margin-bottom: 10px; font-weight: bold"
      >
        {{ project.title }}
    </div>
  </div>

    <div v-if="selectedProject !== null">
      <h2> {{ projects[selectedProject].title }} </h2>
      <p><strong>Ruolo:</strong> {{ projects[selectedProject].role }}</p>
      <p><strong>Descrizione:</strong> <br> <span v-html="projects[selectedProject].description"></span></p>
      <div v-if="projects[selectedProject].location"><p><strong>Location:</strong> <br> <span v-html="projects[selectedProject].location"></span></p></div>
    </div>
  </div>
</template>

<style scoped>
.works {
  color: white;
  background-color: black;
  padding: 3rem;
  height: 100vh;
}
</style>
