<template>
  <div>
    <AppHeader
      :projectName="projectName"
      :courseName="courseName"
      :studentName="studentName"
    />
    <SearchEngine/>
    <SearchResults :searchResults="results" />
    <app-footer />
  </div>
</template>

<script>
import  AppHeader from './components/Header.vue'
import SearchEngine from './components/SearchEngine.vue';
import SearchResults from './components/SearchResults.vue';
import AppFooter from './components/Footer.vue';
export default {
  name: 'App',
  components: {
    SearchEngine,
    SearchResults,
    AppHeader,
    AppFooter,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
