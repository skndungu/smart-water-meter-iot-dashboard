<template>
  <div class="home">
    <div class="home-background_img">
      <div class="home-heading">
        Lake View
        <br />
        <span>Water Co.</span>
      </div>
      <div class="home-slogan">
        <p>
          Keep it running even when the
          <br />sun shines
        </p>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home",
  components: {}
};
</script>

<style scoped>
.home {
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  z-index: -3;
  background-image: url(../assets/home_background_2.jpg);
}

.home-background_img:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  background-image: url(../assets/home_background_1.jpg);
  opacity: 0.3;
  background-size: cover;
}
.home-background_img {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  background: rgba(199, 150, 62, 0.3);
}
.home-heading {
  position: fixed;
  z-index: 200;
  top: 100px;
  bottom: 100px;
  left: 100px;
  font-size: 23pt;
  color: #f7ca44;
  opacity: 1;
}
.home-slogan > p {
  position: absolute;
  margin-top: 75vh;
  left: 100px;
  font-size: 20pt;
  color: #f7ca44;
  z-index: 200;
  font-size: 17pt;
  font-style: italic;
}
</style>