<template>
  <div>
    <section class="index-banner">
      <div class="vertical-center">
        <h1>Advertisement</h1>
        <h2>This is web page on whick you can post your ad</h2>
      </div>
    </section>
    <!-- First -->
    <section class="section-a">
      <div class="content-wrap">
        <div class="content-text">
          <p>
            <br />Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe sint eligendi possimus? Unde officiis magnam laborum ipsa distinctio odio, vero dolores dicta aliquam aperiam repellendus. Perferendis officiis deserunt velit voluptas nobis sequi
            animi totam, accusantium, ex eius quia, natus quo?
          </p>
        </div>
      </div>
    </section>

    <!-- Second -->
    <section class="section-c">
      <div class="content-wrap">
        <h2 class="content-title">Something about ads</h2>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Maxime nam rerum vel earum error fugiat cupiditate, dolore eius! Minus, explicabo.</p>
      </div>
    </section>

    <!-- Third -->

    <section class="features">
      <div class="wrapper">
        <h2>This is web site about ads</h2>
        <div class="cards">
          <div class="feature-card">
            <img src="~/assets/images/home.jpg" alt />
            <h3>Advertisement</h3>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style>
.index-banner {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/images/main.jpg");
  background-position: center;
  background-size: cover;
}
.index-banner h1 {
  font-size: 60px;
  color: #073b5e;
  text-align: center;
  font-weight: 900;
  text-shadow: 2px 2px 6px #111;
  line-height: 20px;
}
.index-banner h2 {
  font-size: 28px;
  color: #345b75;
  text-align: center;
  font-weight: 200;
  font-style: italic;
  line-height: 40px;
}
/* Firts */
.section-a {
  background: #383838;
  color: rgb(255, 255, 255);
  padding-bottom: 2em;
  margin-top: 20px;
}
.section-a p {
  margin-left: 80px;
  margin-right: 80px;
  text-align: left;
}
/* Firts */
.section-c {
  background: #073b5e;
  color: #fff;
  padding: 2em;
  margin-top: 20px;
}
/* Third*/
.feature-card img {
  max-width: 100%;
  height: auto;
  position: center;
  display: block;
  margin-left: auto;
  margin-right: auto;
  filter: grayscale(100%);
  border-radius: 5px;
}
img:hover {
  box-shadow: 0 0 2px 1px #383838;
}
</style>
