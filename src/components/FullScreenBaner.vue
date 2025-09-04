<template>
  <div class="fullScreenBaner">
    <img class="fullScreenBaner__img" src="/public/images/fullScreenBaner/1.jpg" alt="1">
    <img class="fullScreenBaner__img" src="/public/images/fullScreenBaner/2.jpg" alt="2">
    <img class="fullScreenBaner__img" src="/public/images/fullScreenBaner/3.jpg" alt="3">
    <div class="overlay"></div>
    <div class="content">
      <h1>Новая коллекция</h1>
      <div class="strip"></div>
      <p>Смотреть новинки ></p>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss">
body {
  color: #fff;
  margin: 0;
  font-size: 16px;
}

.fullScreenBaner {
  display: flex;
  width: 100vw;
  position: relative;
  min-height: 100vh;
}

.fullScreenBaner__img {
  width: 33.33%;
  height: 100vh;
  object-fit: cover;
  flex-shrink: 0;
}

.fullScreenBaner .overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.3);
  z-index: 2;
}

.fullScreenBaner .content {
  display: flex;
  flex-direction: column;
  height: 100%;
  width: 100%;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 3;
  font-weight: 300;
  gap: 2.5vh;
}

.fullScreenBaner .content h1 {
  font-size: clamp(2rem, 8vw, 3rem);
  font-weight: 300;
  margin: 0;
  text-align: center;
  padding: 0 5%;
}

.fullScreenBaner .content p {
  font-size: clamp(1rem, 4vw, 1.25rem);
  margin: 0;
  text-align: center;
  max-width: 60ch;
}

.fullScreenBaner .content .strip {
  width: 8vw;
  height: 1px;
  background-color: white;
  margin-top: 1vh;
}

@media (max-width: 1000px) {
  .fullScreenBaner__img:nth-child(2),
  .fullScreenBaner__img:nth-child(3) {
    display: none;
  }

  .fullScreenBaner__img {
    width: 100vw;
  }

  .fullScreenBaner .content {
    gap: 4vh;
    padding: 0 5vw;
  }

  .fullScreenBaner .content h1 {
    font-size: clamp(1.75rem, 10vw, 3rem);
  }

  .fullScreenBaner .content p {
    font-size: clamp(0.9rem, 3.5vw, 1.125rem);
  }

  .fullScreenBaner .content .strip {
    width: 10vw;
  }
}

@media (max-height: 600px) {
  .fullScreenBaner .content {
    gap: 1.5vh;
  }

  .fullScreenBaner .content h1 {
    font-size: 2rem;
  }

  .fullScreenBaner .content p {
    font-size: 1rem;
  }

  .fullScreenBaner .content .strip {
    width: 6vw;
  }
}
</style>