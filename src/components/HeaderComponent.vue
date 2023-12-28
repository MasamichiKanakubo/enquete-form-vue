<template>
  <div class="survey-page">
    <header class="header">
      <div class="logo">ロゴ</div>
      <div class="header-buttons">
        <button class="request-button">資料請求</button>
        <a href="#" class="link">資料一覧</a>
      </div>
    </header>
    <!-- 以下、他のセクションやコンポーネントを追加 -->
  </div>
</template>

<script setup>
// コンポーネントのインポートなど
</script>

<style scoped>
/* ヘッダーのスタイル */
.header {
  background-color: #ffffff; /* 白い背景色 */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* 影を追加 */
  padding: 10px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

/* ロゴのスタイル */
.logo {
  font-size: 24px;
  font-weight: bold;
}

/* 資料請求ボタンのスタイル */
.request-button {
  padding: 10px 20px;
  background-color: #4CAF50; /* ボタンの背景色 */
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.request-button:hover {
  background-color: #45a049; /* ホバー時の色 */
}

/* 資料一覧リンクのスタイル */
.link {
  margin-left: 20px; /* ボタンからの間隔を設定 */
  text-decoration: none;
  color: #333333;
  font-weight: bold;
}
</style>
