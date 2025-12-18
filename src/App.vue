<template>
  <div class="container">
    <LoginPage />
  </div>
  
</template>

<script>
import LoginPage from './views/LoginPage.vue'

export default {
  name: 'App',
  components: { LoginPage }
}
</script>
<style>
  body{
    background-color: black;
    color: white;
  }
  .container{
    height: 100vh;
    display: flex;
    flex-direction: column;  /*플렉스에서 colum은 생성물이 밑에 하나씩 생김 row로 하면 오른쪾으로 하나씩 생김 */
    justify-content: center; /* 수직옵션end하면 가장아래, cneter하면 중간에 위치 */
    align-items: center; /* 수평옵션으로 수평에서 가운데 왼쪽, 오른쪽 위치정함 */

  }
</style>
