<template>
  <div>
    <InputField type="text" placeholder="Email" :modelValue="email" v-model="email"/>
    <InputField type="password" placeholder="Password" :modelValue="password" v-model="password"/>

    <button @click="login">로그인하기</button>
  </div>
</template>

<script>
import InputField from '@/components/inputField.vue'

export default {
  name: 'LoginPage',
  components: { InputField },
  data() {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    login() {
      console.log(this.email, this.password)
    }
  }
}
</script>
