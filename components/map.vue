<template>
  <div>
    <section class="map">
      <div class="first"></div>
      <div class="line"></div>
      <div class="sec"></div>
      <div class="map-sec">
        <div class="mapInt"></div>
        <div class="intList">
          <h1>Biziň ýeňijilerimiz</h1>
          <pre>
            Gylyjow Osman - IIO Singapur - 1 orun;
            
            Leyla Amanowa - IBO Paris - 1 orun;

            Hatyja Durdyýew - IMO Moskow - 1 orun;

            Gylyjow Osman - IIO Singapur - 1 orun;

            Gylyjow Osman - IIO Singapur - 1 orun;

            Leyla Amanowa - IBO Paris - 1 orun;

            Hatyja Durdyýew - IMO Moskow - 1 orun;

            Gylyjow Osman - IIO Singapur - 1 orun;
          </pre>
        </div>
      </div>
      <div class="first"></div>
      <div class="line"></div>
      <div class="sec"></div>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style>
.map {
  width: 100%;
  height: 65vh;
}
.first {
  width: 100%;
  height: 15px;
  margin: 0 auto;
  border-bottom: 15px solid rgb(14, 136, 136);
}

.line {
  width: 100%;
  height: 10px;
  border-bottom: 10px solid rgb(7, 239, 239);
}

.sec {
  width: 100%;
  height: 7px;
  border-bottom: 7px solid rgb(185, 247, 247);
}

.map-sec {
  width: 100%;
  height: 50vh;
  display: grid;
  margin: 20px 0;
  display: flex;
  padding: 10px;
}
.mapInt {
  width: 65%;
  height: 50vh;
  background: url('../assets/hooper/map.png');
  background-size: 100%;
}

.intList {
  width: 35%;
  height: 50vh;
  background-color: bisque;
}
pre {
  margin-top: 10px;
}
</style>