<template>
  <div>
    <div class="body">
      <b-list-group>
        <!-- Inscrição -->
        <b-list-group-item variant="info" class="link-item">
          <a :href="lolLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="lolImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Inscrição </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Battlefy -->
        <b-list-group-item variant="danger" class="link-item">
          <a :href="battlefyLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="battlefyImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Battlefy </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Regulamento -->
        <b-list-group-item variant="success" class="link-item">
          <a :href="rulesLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="rulesImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Regulamento </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Instagram -->
        <b-list-group-item class="link-item">
          <a :href="instagramLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="instagramImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Instagram </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Discord -->
        <b-list-group-item class="link-item">
          <a :href="discordLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="discordImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Discord </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Twitch -->
        <b-list-group-item class="link-item">
          <a :href="twitchLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="twitchImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Twitch </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Youtube -->
        <b-list-group-item class="link-item">
          <a :href="youtubeLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="youtubeImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Youtube </b-col>
            </b-row></a
          >
        </b-list-group-item>

        <!-- Twitter -->
        <b-list-group-item class="link-item">
          <a :href="twitterLink">
            <b-row align-v="center">
              <b-col sm="12" md="3">
                <b-img :src="twitterImg" width="50"></b-img>
              </b-col>
              <b-col sm="12" md="9" class="link-title"> Twitter </b-col>
            </b-row></a
          >
        </b-list-group-item>
      </b-list-group>
    </div>
  </div>
</template>

<script>
export default {
  name: "Links",
  data() {
    return {
      lolImg: require("../assets/lol.png"),
      battlefyImg: require("../assets/battlefy.png"),
      rulesImg: require("../assets/docs.png"),
      instagramImg: require("../assets/instagram.png"),
      discordImg: require("../assets/discordia.png"),
      twitchImg: require("../assets/twitch.png"),
      youtubeImg: require("../assets/youtube.png"),
      twitterImg: require("../assets/twitter.png"),

      lolLink:
        "https://docs.google.com/forms/d/16cTqFOIJuYYUq8kFLmFY19ffT_yJ7CrRL4eE5IOsE2w/edit?chromeless=1",
      battlefyLink:
        "https://battlefy.com/cop%C3%A3o-e-sports/cop%C3%A3o-2%C2%B0-edi%C3%A7%C3%A3o-joinville-e-regi%C3%A3o/62e0a0976e13a21cc3d28bec/info",
      rulesLink:
        "https://docs.google.com/document/d/1xqk48z1tci0FtPgxtuwxoxBlnuNyEH1_TZx1fGjUQP0/edit?usp=drivesdk",
      instagramLink: "https://www.instagram.com/oficial.copao/",
      discordLink: "https://discord.com/invite/q7yekFPEex",
      twitchLink: "https://www.twitch.tv/copaooficial",
      youtubeLink: "https://www.youtube.com/channel/UCLn3EBtAY09Mb-JGLyCu1aw",
      twitterLink: "https://twitter.com/Copaoifc2022",
    };
  },
};
</script>

<style>
@font-face {
  font-family: "Inter";
  src: local("Inter"), url(../assets/fonts/Inter.ttf) format("truetype");
}

.body {
  margin: 0 auto !important;
  width: 65%;
}

.link-item a {
  text-decoration: none;
  color: #000;
}

.link-title {
  text-align: center;
  text-decoration: none;
  font-family: "Inter", sans-serif;
  font-weight: 300;
  font-size: 1.3rem;
}

@media only screen and (max-width: 950px) {
  /* For mobile phones: */
  .body {
    width: 100%;
  }

  .link-item {
        padding: 1.5rem 0 !important;
  }

  .link-title {
    font-size: 2.3rem;
  }
}

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  .body {
    width: 100%;
  }

  .link-title {
    margin-top: 1rem !important;
  }
}
</style>
