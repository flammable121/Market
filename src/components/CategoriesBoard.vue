<template>
  <div class="categories">
    <div class="categories__content">
      <h2 class="content--title">Категории</h2>
      <div class="content--img">
        <div class="card">
          <img src="/images/categoriesBoard/1.jpg" alt="" class="card-img">
          <div class="card-overlay">Куртки</div>
        </div>
        <div class="card">
          <img src="/images/categoriesBoard/2.jpg" alt="" class="card-img">
          <div class="card-overlay">Пальто</div>
        </div>
        <div class="card">
          <img src="/images/categoriesBoard/3.jpg" alt="" class="card-img">
          <div class="card-overlay">Шубы</div>
        </div>
        <div class="card">
          <img src="/images/categoriesBoard/4.jpg" alt="" class="card-img">
          <div class="card-overlay">Парки</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
* {
  font-size: 1rem;
}

.categories {
  display: flex;
  align-items: center;
  height: 100vh;
}

.content--title {
  color: black;
  font-size: clamp(1.5rem, 6vw, 2.25rem);
  font-weight: 300;
}

.categories__content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 10%;
  width: 80%;
  gap: clamp(1.5rem, 5vh, 3.125rem);
}

.content--img {
  display: flex;
  gap: 2%;
  width: 100%;
  justify-content: space-between;
}

.content--img img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.card {
  display: flex;
  position: relative;
  overflow: hidden;
}

.card-overlay {
  font-size: clamp(0.875rem, 4vw, 1.25rem);
  font-weight: 300;
  position: absolute;
  bottom: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  width: 100%;
  height: clamp(1.875rem, 8vh, 2.5rem);
  background: rgba(224, 190, 162, 0.75);
}

@media (max-width: 1000px) {
  .content--img {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2%;
  }

  .content--img :nth-child(3),
  .content--img :nth-child(4) {
    display: none;
  }

  .card {
    max-width: 275px;
  }
}
</style>