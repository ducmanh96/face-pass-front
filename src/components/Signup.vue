<template>
  <div class="signup">
    <h2>新規アカウントを作成</h2>
    <input type="text" placeholder="ユーザー名" v-model="username">
    <input type="password" placeholder="パスワード" v-model="password">
    <button>アカウント登録</button>
    <p>アカウントをお持ちですか？<router-link to="/signin">今すぐサインイン!!</router-link>
    </p>
  </div>
</template>

<script>
export default {
  name: 'Signup',
  data () {
    return {
      username: '',
      password: ''
    }
  },
  methods: {}
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.signup {
  margin-top: 20px;

  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-items: center
}
input {
  margin: 10px 0;
  padding: 10px;
}
</style>