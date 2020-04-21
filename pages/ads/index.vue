<template>
  <div class="ads-page">
    <section class="showcase">
      <div class="bg-image"></div>
      <div class="content-wrap">
        <h1>A list of all ads</h1>
        <p>On this page you can see all posted ads</p>
      </div>
    </section>

    <!-- Firts ad -->
    <section class="section-a">
      <div class="content-wrap">
        <h2 class="content-title">Firts ad</h2>
        <div class="content-text">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe sint eligendi possimus? Unde officiis magnam laborum ipsa distinctio odio, vero dolores dicta aliquam aperiam repellendus. Perferendis officiis deserunt velit voluptas nobis sequi
            animi totam, accusantium, ex eius quia, natus quo?
          </p>
        </div>
      </div>
    </section>

    <!-- Second ad  -->
    <section class="section-c">
      <div class="content-wrap">
        <h2 class="content-title">Second ad</h2>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Maxime nam rerum vel earum error fugiat cupiditate, dolore eius! Minus, explicabo.</p>
      </div>
    </section>

    <!-- Important information -->
    <section class="section-d">
      <div class="box">
        <h2 class="content-title">Important information</h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eum, suscipit. Rerum ducimus a quod, ut et voluptas obcaecati unde fuga.</p>
      </div>
      <div class="box">
        <h2 class="content-title">About Our Company</h2>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio earum porro deserunt, deleniti, quae facere repudiandae, officiis est exercitationem nobis iusto doloremque! Soluta excepturi in aut suscipit amet temporibus quo?</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>


<style scoped>
.showcase {
  min-height: 450px;
}

.showcase h1 {
  color: #073b5e;
  font-size: 50px;
  text-align: center;
}

.showcase p {
  color: #4e616d;
  font-size: 30px;
  text-align: center;
}

.showcase .bg-image {
  position: absolute;
  background: rgb(154, 163, 218) url("~assets/images/cover.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 450px;
  z-index: -1;
  opacity: 0.4;
  margin-top: -42px;
}

.showcase h1 {
  padding-top: 100px;
  padding-bottom: 0;
}

.showcase .content-wrap,
.section-a .content-wrap {
  padding: 0 1.5em;
}

/* Firts ad */

.section-a {
  background: #eaeaea;
  color: #333;
  padding-bottom: 2em;
  margin-top: -40px;
}

/* Second ad */

.section-c {
  background: #fff;
  color: #333;
  padding: 2em;
}

/* Important information */

.section-d .box {
  padding: 2em;
  color: #fff;
}

.section-d .box:first-child {
  background: #073b5e;
}
</style>
