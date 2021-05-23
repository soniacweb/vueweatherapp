<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="Search...">
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">Northampton, UK</div>
          <div class="date">Monday 20th January 2020</div>
        </div>
        <div class="weather-box">
          <div class="temperature">9°c</div>
          <div class="weather">Rain</div>
        </div>
      </div>

    </main>

  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      api_key: '71a044cb9da982f291b5ccd1de19279d'
    }
  }

}
</script>

<style>
* {
margin: 0;
padding: 0;
box-sizing: border-box;
}

body {
  font-family: 'montserrat', sans-serif;
}

#app {
  background-image: url('./assets/cold-bg.jpeg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0,0,0, 0.25), rgba(0,0,0,0.75));
}

.search-box {
  width: 100%;
  margin-bottom: 30px;
}

.search-box .search-bar {
  display: block;
  width: 100%;
  padding: 15px;
  color: #313131;
  font-size: 20px;
  appearance: none;
  border: none;
  outline: none;
  background: none;

  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 0px 16px 0px 16px;
  transition: 0.4s;
  box-shadow: 0px 0px 8px rgba(255, 255, 255, 0.25);
}

.search-box .search-bar:focus { 
  background-color: rgba(255, 255, 255, 0.75);
  box-shadow: 0px 0px 16px rgba(255, 255, 255, 0.25);
  border-radius: 16px 0px 16px 0px;

}
</style>
