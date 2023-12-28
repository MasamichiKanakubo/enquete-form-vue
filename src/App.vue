<template>
  <div class="survey-page">
    <header>
      <HeaderComponent />
    </header>
    <main>
      <div class="centered-form">
        <SurveyForm />
      </div>
    </main>
  </div>
</template>

<script setup>
import HeaderComponent from './components/HeaderComponent.vue';
import SurveyForm from './components/SurveyForm.vue';
</script>

<style scoped>
/* ページ全体のスタイル */
.survey-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f5f5f5;
}

/* ヘッダーのスタイル */
header {
  text-align: center;
  padding: 20px;
  background-color: #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
}

/* ロゴのスタイル */
.logo {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
}

/* 中央配置されたフォームのスタイル */
.centered-form {
  max-width: 500px;
  width: 100%;
  text-align: center;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  background-color: #fff;
}
</style>
