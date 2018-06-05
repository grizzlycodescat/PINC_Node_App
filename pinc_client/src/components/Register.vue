<template>
	<div class="hello">
		<h1>{{ msg }}</h1>
		<input type="text" v-model="userName" name="userName" placeholder="User Name">
		<br>
		<input type="password" v-model="password" name="password" placeholder="Password">
		<br>
		<button @click="register">Register</button>
	</div>
</template>

<script>
import authService from '@/services/authService';
export default {
  	name: 'HelloWorld',
  	data () {
    	return {
	      userName: '',
	      password: '',
	      msg: 'Register'
	    }
	},
	methods: {
		async register () {
			const response = await authService.register({
				userName: this.userName,
				password: this.password
			})
			this.$router.push("modalpage")
			// console.log("reg button was clicked", this.userName, this.password)
			// console.log(response.data);
		}
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
