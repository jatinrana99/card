<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld />
  <div class="main">
  <Card>
    <template v-slot:header >
      <img src="https://images.unsplash.com/photo-1575936123452-b67c3203c357?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8aW1hZ2V8ZW58MHx8MHx8fDA%3D&w=1000&q=80" alt="" class="image">
      </template>

      <template v-slot:title>
        <h2>Photography</h2>
        </template>

        <template v-slot:body>
          <p>In the world of photography, you get to share a captured moment with other people.</p>
          </template>

          <template v-slot:footer>
            <button>Know More</button>
            </template>
    </Card>


    <Card>
    <template v-slot:header>
      <img src="./assets/Hacker-Hero-a1.webp" alt="" class="image">
      </template>

      <template v-slot:title>
        <h2>Developer</h2>
        </template>

        <template v-slot:body>
          <p>Programming today is a race between software engineers striving to build bigger and better idiot-proof programs and the Universe trying to produce bigger and better idiots.</p>
          </template>

          <template v-slot:footer>
            <button>Know How to Code</button>
            </template>
    </Card>

    <Card id="shiv">
    <template v-slot:header>
      <img src="./assets/kedar.jpg" alt="" class="image" id="shivimg">
      </template>

      <template v-slot:title>
        <h2>Shiv Ji</h2>
        </template>

        <template v-slot:body>
          <p>According to Shiva, you are free to make decisions of your own, but you are not free to run away from the consequences of those decisions.</p>
          </template>

          <template v-slot:footer>
            <button>Explore More about SHIV JI</button>
            </template>
    </Card>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Card
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

.image{
  /* border: 2px solid; */
width: 100%;
}


.main{
  display: flex;

}

#shivimg{
  height: 229px;
}

</style>
