<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-btn class="mx-2" fab dark small color="primary">
        <v-icon dark> mdi-plus </v-icon>
      </v-btn></v-app-bar
    >
    <v-main>
      <HelloWorld />
      <div>
        <h3>Your Id: <span id="myId"></span></h3>
        <h3>Online Users (click to connect)</h3>
        <div id="users"></div>

        <section>
          <div>
            <form id="fileInfo">
              <input type="file" id="fileInput" name="files" />
            </form>
            <!-- <button disabled id="sendFile">Send</button>
               <button disabled id="abortButton">Abort</button> -->
          </div>

          <div class="progress">
            <div class="label">Send progress:</div>
            <progress id="sendProgress" max="0" value="0"></progress>
          </div>

          <div class="progress">
            <div class="label">Receive progress:</div>
            <progress id="receiveProgress" max="0" value="0"></progress>
          </div>

          <div id="bitrate"></div>
          <a id="download"></a>
          <span id="status"></span>
        </section>
      </div>
    </v-main>

    <div>
      <HomeFooter />
    </div>
  </v-app>
</template>
 
<script>
import HelloWorld from "./components/HelloWorld";
import HomeFooter from "./components/HomeFooter.vue";

export default {
  name: "App",

  components: {
    HomeFooter,
    HelloWorld,
  },

  methods: {},

  data: () => ({
    //
  }),
};
</script>
