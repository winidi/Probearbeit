<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        LeosRestaurant
      </h1>
      
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    'Segoe UI',
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 200;
  font-size: 100px;
  color: black;
  letter-spacing: 1px;
  margin-bottom: 200px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
