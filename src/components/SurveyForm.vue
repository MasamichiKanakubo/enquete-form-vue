<template>
    <div>
      <h1>アンケートフォーム</h1>
      <form @submit.prevent="submitForm">
        <div>
          <label for="name">企業名:</label>
          <input type="text" id="name" v-model="formData.name" required>
        </div>
        <div>
          <label for="email">Eメール:</label>
          <input type="email" id="email" v-model="formData.email" required>
        </div>
        <div>
          <label for="age">年齢:</label>
          <input type="number" id="age" v-model.number="formData.age" required>
        </div>
        <div>
          <label>性別:</label>
          <label for="male"><input type="radio" id="male" value="male" v-model="formData.gender">男性</label>
          <label for="female"><input type="radio" id="female" value="female" v-model="formData.gender">女性</label>
        </div>
        <div>
          <label>お問い合わせ内容:</label>
          <textarea v-model="formData.message" rows="4" required></textarea>
        </div>
        <button class="custom-button" type="submit">送信</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        formData: {
          name: '',
          email: '',
          age: null,
          gender: '',
          message: ''
        }
      };
    },
    methods: {
      submitForm() {
        // フォームが送信された時の処理
        console.log('送信するデータ:', this.formData);
        // ここに後でAPI送信の処理を追加することができます
      }
    }
  };
  </script>
  
  <style scoped>
  /* スタイリングを追加（必要に応じて） */
  label {
    display: block;
    margin-bottom: 5px;
  }

  .custom-button {
  padding: 10px 20px;
  border: none;
  border-radius: 20px;
  background-color: rgb(37, 158, 144); /* 蛍光色っぽい黄緑 */
  color: white;
  font-family: 'Arial', sans-serif; /* カスタムのフォント */
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease; /* ホバー時のトランジション */
  }

  .custom-button:hover {
   background-color: rgb(18, 218, 194); /* ホバー時の色変更 */
  }
  </style>
  