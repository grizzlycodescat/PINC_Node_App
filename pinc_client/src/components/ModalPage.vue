<template>
  <div class="hello">
	<h1>{{ msg }}</h1>
	<button @click="propagate">Propagate</button>
	<h3>Vue Modals</h3>
	<ul id="list">
       <draggable v-for="index in count" :key="index">
       </draggable>
    </ul>
  </div>
</template>

<script>
import draggable from '@/components/Draggable.vue';

export default {
	name: 'ModelPage',
	components: {
		draggable,
	},
	data () {
		return {
			msg: 'Welcome to the Modal Popup Page',
			template: `<draggable></draggale>`,
			count: 0,
		}
	},
	methods: {
		propagate () {
			// console.log("propagated")
			this.count++;
		}
		
	}
}
</script>
