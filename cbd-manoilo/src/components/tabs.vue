<template>
  <div class="tabContainer">
    <div class="tabs">
      <a v-on:click="activetab = 1" v-bind:class="[activetab === 1 ? 'active' : '']">Tab 1</a>
      <a v-on:click="activetab = 2" v-bind:class="[activetab === 2 ? 'active' : '']">Tab 2</a>
      <a v-on:click="activetab = 3" v-bind:class="[activetab === 3 ? 'active' : '']">Tab 3</a>
    </div>

    <div class="content">
      <div v-if="activetab === 1" class="tabcontent">
        Is this the real life? Is this just fantasy?
      </div>
      <div v-if="activetab === 2" class="tabcontent">
        Caught in a landslide, no escape from reality
      </div>
      <div v-if="activetab === 3" class="tabcontent">
        Open your eyes, look up to the skies and see
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Tabs",
  data() {
    return {
      activetab: 1
    };
  }
};
</script>

<style lang="scss">
@import "../styles/core/vars.scss";
.tabContainer {
  padding-top: 5rem;
  min-height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(255, 255, 255, 0.1)), url("../assets/bg-header.png");
  background-color: $bgc-color;
  min-height: 100vh;
  text-align: center;
  padding-top: 2%;
  font-size: 30px;
  width: 100%;
  height: 300px;
  position: relative;
}
</style>
