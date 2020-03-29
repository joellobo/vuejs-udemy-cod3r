<template>
	<v-app>
		<Header />
		<v-content>
			<router-view></router-view>
		</v-content>
	</v-app>
</template>

<script>
import Header from './components/Header'

export default {
  components: { Header },
  created() {
	  this.$store.dispatch('initStocks')
  }
}
</script>

<style>

</style>

