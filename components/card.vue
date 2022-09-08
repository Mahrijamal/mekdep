<template>
  <nuxt-link :to="card_link" class="card">
    <div class="cont">
      <h1 class="adss">{{ info.synp }} synpyň meýilnamasy</h1>
      <div class="klass">
     
          <div class="monday">
            <h3 class="week">Monday</h3>
            <p class = "info"> 1. {{ info.mbir }}</p>
            <p class = "info"> 2. {{ info.miki }}</p>
            <p class = "info"> 3. {{ info.muc }}</p>
            <p class = "info"> 4. {{ info.mdort }}</p>
            <p class = "info"> 5. {{ info.mbas }}</p>
            <p class = "info"> 6. {{ info.malty }}</p>
          </div>
          <div class="tuesday">
            <h3 class="week">Tuesday</h3>
            <p class = "info"> 1. {{ info.tbir }}</p>
            <p class = "info"> 2. {{ info.tiki }}</p>
            <p class = "info"> 3. {{ info.tuc }}</p>
            <p class = "info"> 4. {{ info.tdort }}</p>
            <p class = "info"> 5. {{ info.tbas }}</p>
            <p class = "info"> 6. {{ info.talty }}</p>
          </div>
          <div class="wednesday">
            <h3 class="week">Wednesday</h3>
            <p class = "info"> 1. {{ info.wbir }}</p>
            <p class = "info"> 2. {{ info.wiki }}</p>
            <p class = "info"> 3. {{ info.wuc }}</p>
            <p class = "info"> 4. {{ info.wdort }}</p>
            <p class = "info"> 5. {{ info.wbas }}</p>
            <p class = "info"> 6. {{ info.walty }}</p>
          </div>
    
          <div class="thursday">
            <h3 class="week">Thursday</h3>
            <p class = "info"> 1. {{ info.hbir }}</p>
            <p class = "info"> 2. {{ info.hiki }}</p>
            <p class = "info"> 3. {{ info.huc }}</p>
            <p class = "info"> 4. {{ info.hdort }}</p>
            <p class = "info"> 5. {{ info.hbas }}</p>
            <p class = "info"> 6. {{ info.halty }}</p>
          </div>
          <div class="friday">
            <h3 class="week">Friday</h3>
            <p class = "info"> 1. {{ info.fbir }}</p>
            <p class = "info"> 2. {{ info.fiki }}</p>
            <p class = "info"> 3. {{ info.fuc }}</p>
            <p class = "info"> 4. {{ info.fdort }}</p>
            <p class = "info"> 5. {{ info.fbas }}</p>
            <p class = "info"> 6. {{ info.falty }}</p>
          </div>
          <div class="saturday">
            <h3 class="week">Saturday</h3>
            <p class = "info"> 1. {{ info.sbir }}</p>
            <p class = "info"> 2. {{ info.siki }}</p>
            <p class = "info"> 3. {{ info.suc }}</p>
            <p class = "info"> 4. {{ info.sdort }}</p>
            <p class = "info"> 5. {{ info.sbas }}</p>
            <p class = "info"> 6. {{ info.salty }}</p>
          </div>
       
      </div>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  props: {
    info: {
      type: Object,
      required: true,
    },
    isAdmin: {
      type: Boolean,
      required: false,
    },
  },
  computed: {
    card_link() {
      return this.isAdmin ? '/admin/' + this.info.id : '/cards/' + this.info.id
    },
  },
}
</script>

<style>
   .card {
  position: relative;
  width: 100%;
  height: 45vh;
  }
.cont {
width: 100%;
height: 45vh;
background: rgb(27, 140, 108);

}
.adss{
  color: white;
}
.week {
  color: white;
  font-size: 20px;
}
.info{
  color: white;
  text-align: left;
  font-size: 16px;
  margin: 30px
}

.klass{
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  padding: 20px;
  font-size: 30px;
  text-align: center;
}

</style>