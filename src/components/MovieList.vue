<template>
  <div id="movie-container">
       Movie list
      <ul>
          <li v-for="(movie, index) in movies" :key="movie.id">
            index: {{index}}  {{movie.name}}
          </li>
      </ul>
      
      </div>
</template>

<script>
export default {
    data(){
        return {
            movies : [],
        }
    }
}
</script>

<style lang='scss' scoped>
	#movie-container {
		padding-top: 1rem;
		display: flex;
		flex-wrap: wrap;
		flex-grow: 2;
		justify-content: center;
	}
</style>