<template>
  <div class="admin-auth-page">
    <div class="container-fluid">
        <div class="row">
            <div class="col-4">
        <h1>Auth Page</h1>
        <form>
            <div>
                <b-form-input v-model="displayName" placeholder="Enter your name"></b-form-input>
                <!-- <div class="mt-2">Value: {{ displayName }}</div> -->
            </div>
            <div>
                <b-form-input v-model="email" placeholder="Enter your email"></b-form-input>
                <!-- <div class="mt-2">Value: {{ email }}</div> -->
            </div>
            <div>
                <b-form-input v-model="password" placeholder="Enter your password"></b-form-input>
                <!-- <div class="mt-2">Value: {{ password }}</div> -->
            </div>
            <hr>
            <b-button variant="success" type="submit">{{ isLogin ? 'Login' : 'Sign Up' }}</b-button>
            <b-button variant="outline-primary" type="button" @click="isLogin = !isLogin">{{ isLogin ? 'Signup' : 'Login' }}</b-button>
        </form>
            </div>
        </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'AdminAuthPage',
  components: {

  },
  data() {
    return {
      isLogin: true,
      displayName: '',
      email: '',
      password: '',
    }
  }
}
</script>


