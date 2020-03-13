<template>
  <div class="container">
    <TheNavBar />
    <nuxt />
  </div>
</template>

<script>
import TheNavBar from "@/components/TheNavBar";
export default {
  components: {
    TheNavBar
  }
};
</script>

<style>
h1 {
  color: green;
}

html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 70px;
  font-weight: lighter;
  letter-spacing: 0.5px;
  position: fixed;
  width: 100%;
  left: 0;
  top: 0;
}

.nav .logo {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.nav .logo .subheader {
  opacity: 0.7;
  font-size: 0.9rem;
  color: gray;
}

.nav .nav-content {
  font-size: 1rem;
}

.nav-content ul {
  display: flex;
  list-style: none;
}

.nav-content ul li {
  padding: 2px 10px;
}

.nav-content ul li:not(:first-of-type) {
  border-left: 1px solid rgb(255, 255, 255, 0.2);
}
</style>
