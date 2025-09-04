<template>
  <div class="formNews">
    <div class="formNews__form">
      <h1>Узнайте первым о новинках</h1>
      <form class="form--mail">
        <input placeholder="Ваш e-mail*">
        <button>ПОДПИСАТЬСЯ</button>
        <p>
          Нажимая на кнопку «Подписаться», я соглашаюсь на обработку моих персональных данных и ознакомлен(а) с условиями конфиденциальности.
        </p>
      </form>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
* {
  color: black;
  box-sizing: border-box;
}

.formNews {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  padding: 20px;
  margin: 0 auto;
}

.formNews__form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 2rem;
  max-width: 800px;
  width: 100%;
  text-align: center;
}

.formNews__form h1 {
  font-weight: 300;
  font-size: 1.75rem;
  line-height: 1.2;
}

.form--mail {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  width: 100%;
  max-width: 500px;
  margin: 0 auto;
}

.form--mail input,
.form--mail button,
.form--mail p {
  width: 100%;
  padding: 0.75rem 1rem;
  font-size: 1rem;
  font-weight: 200;
  line-height: 1.5;
}

.form--mail input {
  height: auto;
  text-align: center;
  border: 1px solid #ccc;
  border-radius: 4px;
  background: #f9f9f9;
}

.form--mail button {
  background-color: #E0BEA2;
  border: none;
  color: white;
  cursor: pointer;
  border-radius: 4px;
  font-weight: 500;
  transition: background 0.3s ease;
}

.form--mail button:hover {
  background-color: #d4b094;
}

.form--mail p {
  text-align: center;
  font-size: 0.875rem;
  color: #666;
  margin-top: 0.5rem;
}
</style>