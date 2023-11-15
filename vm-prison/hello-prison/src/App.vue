<script>
export default
{
  data() {
    return {
      showPrank: false
    }
  }
}
</script>
<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/prison.jpg" width="500" height="500" />
  </header>

  <main>
    <div id="main-body">
      <span>Omg vous êtes en prison</span>
      <span>RIP échappez-vous!</span>
      <div id="button-div">
        <input id="button-prank" type="button" @click="showPrank = !showPrank" value="Echappez-vous!" />
      </div>
      <span v-if="showPrank">Hé non, c'était un prank!</span>
    </div>
  </main>
</template>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
}
#main-body{
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: space-around;
}
#button-div{
  display: flex;
  justify-content: center;
}
#button-prank{
  display: flex;
  width: fit-content;
  justify-content: center;
  text-align: center;
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

</style>
