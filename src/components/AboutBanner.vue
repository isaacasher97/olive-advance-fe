<template>
  <div id="aboutbanner" class="card bg-dark text-white">
    <img src="" class="card-img" alt="" />
    <div class="card-img-overlay">
      <h5 class="card-title">About Olive Avance</h5>
      <div class="links">
        <a href="/">Home</a>
        <a href="#"> > About</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutBanner",
};
</script>

<style scoped>
#aboutbanner {
  background: url(https://i.imgur.com/6aeOOdG.png);
  height: 100%;
  width: 100%;
  background-size: cover;
  background-repeat: no-repeat;
  padding: 25px;
  border-radius: 0;
}

img {
  background-size: cover;
  padding: 50px;
}

a {
  text-decoration: none;
  color: #fff;
}

a:hover {
  text-decoration: underline;
}

.card-img-overlay {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

@media (max-width: 600px) {
  img {
    background-size: cover;
    padding: 20px;
  }
}
</style>
