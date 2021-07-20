
<template>
  <div class="signin">
    <h2>アプリにサインイン</h2>
    <input type="text" placeholder="ユーザー名" v-model="username">
    <input type="password" placeholder="パスワード" v-model="password">
    <button>サインイン</button>
    <p>アカウントをお持ちでないですか?<router-link to="/signup"> ぜひ作成してください！</router-link>
    </p>
  </div>
</template>

<script>
export default {
  name: 'Signin',
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
.signin {
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