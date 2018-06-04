<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
	<button @click="propagate">Propagate</button>

	<h3>Vue Modals</h3>
	<draggable></draggable>
  </div>
</template>

<script>
import draggable from './components/Draggable.vue';
export default {
	name: 'HelloWorld',
	components: {
		draggable,
	},
	data () {
		return {
			msg: 'Welcome to the Modal Popup Page'
		}
	},
	methods: {
		propagate () {
			// console.log("propagated");
			// list.append(<li> <h1>Test Passed</h1> </li>);

		}
	}
}
</script>
