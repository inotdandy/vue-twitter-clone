<template>
  <div>
    @{{user.username}} - {{ fullName }} Follwers {{ followUser() }}
  </div>
</template>

<script>


export default {
  name: 'Home',
  data(){
    return {
      followers: 0,
      user: {
        firstName: 'John',
        lastName: 'Doe',
        username: 'johnD',
        email: 'johndoe@test.com',
        isAdmin: true
      }
    }
  },
  computed: {
    fullName(){
      return `${this.user.firstName} ${this.user.lastName}`
    }
  },
  methods:{
    followUser(){
      return this.followers
    }
  },
  components: {
   
  }
}
</script>
