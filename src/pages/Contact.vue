<template>
  <Layout>
    <h1>Contact us</h1>

    <v-container>
      <v-row>
          <v-row>
            <v-col cols="12" xs="4" md="4" lg="4" xl="4">
              <v-img src="https://upload.wikimedia.org/wikipedia/en/b/b8/A_Beautiful_Mind_Poster.jpg" aspect-ratio="0.95" />
            </v-col>
            <v-col cols="12" xs="8" md="8" lg="8" xl="8">
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error doloremque omnis animi, eligendi magni a voluptatum, vitae, consequuntur rerum illum odit fugit assumenda rem dolores inventore iste reprehenderit maxime! Iusto.</p>
            </v-col>
          </v-row>
      </v-row>
      <v-row>
            <v-col cols="12" xs="4" md="4" lg="4" xl="4">
              <v-img src="https://upload.wikimedia.org/wikipedia/en/f/fb/Gladiator_%282000_film_poster%29.png" aspect-ratio="0.95" />
            </v-col>
            <v-col cols="12" xs="8" md="8" lg="8" class="pr-12">
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error doloremque omnis animi, eligendi magni a voluptatum, vitae, consequuntur rerum illum odit fugit assumenda rem dolores inventore iste reprehenderit maxime! Iusto.</p>
            </v-col>
      </v-row>
    </v-container>
    

  </Layout>
</template>

<style>
  .home-links a {
    margin-right: 1rem;
  }

  .title_text {
    font-family: 'Open Sans', sans-serif;
    font-style: normal;
    font-size: 21px;
    color: #0b0909;
    line-height: 28px;
    font-weight: 300;
  }

  .main_text {
    font-family: "Palatino Linotype", "Book Antiqua", Palatino, serif;
    font-style: normal;
    font-size: 14px;
    color: #777777;
    line-height: 25px;
    margin:20px;
  }

  .break_text {
    font-family: 'Open Sans', sans-serif;
    font-style: thin;
    font-size: 24px;
    color: #000000;
    line-height: 54px;
    text-align: center;
    font-weight: 100;
  }
</style>

<script>

export default {
  metaInfo: {
    title: 'Contact us'
  }
}
</script>
