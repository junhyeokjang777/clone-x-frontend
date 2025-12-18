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
 .container {
  height: 100vh;
  display: flex;

  /* column: 자식 요소가 위 → 아래로 쌓임 (세로 방향) 
     row: 자식 요소가 왼쪽 → 오른쪽으로 쌓임 (기본값) */
  flex-direction: column;

  /* justify-content:
     주축(main axis) 기준 정렬
     column일 때 → 세로 정렬
     center: 중앙, flex-end: 아래 */
  justify-content: center;

  /* align-items:
     교차축(cross axis) 기준 정렬
     column일 때 → 가로 정렬
     center: 가운데, flex-start: 왼쪽, flex-end: 오른쪽 */
  align-items: center;
}

</style>
