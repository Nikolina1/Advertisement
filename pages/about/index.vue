<template>
  <div class="about-page">
    <section class="presentation">
      <div class="introduction">
        <div class="intro-text">
          <h1>Who we are?</h1>
          <p>This is our team</p>
        </div>
      </div>
      <div class="cover">
        <img src="~/assets/images/team.jpg" alt="matebook" />
      </div>
    </section>
    <img class="big-circle" src="~/assets/images/big-eclipse.svg" alt />
    <img class="medium-circle" src="~/assets/images/mid-eclipse.svg" alt />
    <img class="small-circle" src="~/assets/images/small-eclipse.svg" alt />

    <!-- About us -->
    <section class="section-d">
      <div class="box">
        <h2 class="content-title">About us</h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eum, suscipit. Rerum ducimus a quod, ut et voluptas obcaecati unde fuga.</p>
      </div>
      <div class="box"></div>
    </section>
  </div>
</template>

<script>
export default {
  head: {
    title: "About"
  }
};
</script>

<style scoped>
.presentation {
  display: flex;
  width: 90%;
  margin: auto;
  min-height: 80vh;
  align-items: center;
}
.introduction {
  flex: 1;
}
.intro-text h1 {
  font-size: 44px;
  font-weight: 500;
  color: #073b5e;
}
.intro-text p {
  margin-top: 5px;
  font-size: 22px;
  color: #585772;
}

.cover {
  flex: 1;
  display: flex;
  justify-content: center;
  height: 40vh;
}
.cover img {
  height: 100%;
  filter: drop-shadow(0px 5px 3px black);
  animation: drop 1.5s ease;
  border-radius: 3%;
}

.big-circle {
  position: absolute;
  top: 0px;
  right: 0px;
  z-index: -1;
  opacity: 0.5;
  height: 80%;
}
.medium-circle {
  position: absolute;
  top: 30%;
  right: 30%;
  z-index: -1;
  height: 60%;
  opacity: 0.4;
}
.small-circle {
  position: absolute;
  bottom: 0%;
  left: 20%;
  z-index: -1;
}
@keyframes drop {
  0% {
    opacity: 0;
    transform: translateY(-80px);
  }
  100% {
    opacity: 1;
    transform: translateY(0px);
  }
}
@media screen and (max-width: 1024px) {
  .presentation {
    flex-direction: column;
  }
  .introduction {
    margin-top: 5vh;
    text-align: center;
  }
  .intro-text h1 {
    font-size: 30px;
  }
  .intro-text p {
    font-size: 18px;
  }
  .cover img {
    height: 80%;
  }
  .small-circle,
  .medium-circle,
  .big-circle {
    opacity: 0.2;
  }
}
/* About */
.section-d .box {
  padding: 2em;
  color: #fff;
}
.section-d .box:first-child {
  background: #073b5e;
}
.box {
  width: 600px;
}
</style>
