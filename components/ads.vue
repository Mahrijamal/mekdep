<template>
  <section>  
        <h1>Mekdebiň bildirişleri:</h1>
        
        <div class="bildiris">
          <div class="test">
          <h1>
            Umumy Barlag Synagy 24.10.2022 ý başlanýar. Hemmäňize üstünlikler
            arzuw edýäris!
          </h1>
        </div>
        <div class="shahmaty"></div>
        <div class="kitaphana"></div>

      </div>
      <div class="first"></div>
        <div class="line"></div>
        <div class="sec"></div>    
    </section>
</template>

<script>
export default {

}
</script>

<style>

h1 {
        font-size: 20px;
        margin: 10px;
    }

    .bildiris {

        width: 100%;
        display: flex;
        padding: 10px;
        margin-bottom: 20px;
    }
        .test {
            background: url('../assets/hooper/test.png');
            background-size: cover;
            width: 35%;
            height: 40vh;
            border-radius: 10px;       
        }

        .shahmaty {
            background: url('../assets/hooper/shah.png');
            background-size: cover;
            width: 30%;
            height: 40vh;
            margin-left: 30px;
            margin-right: 30px;
            border-radius: 10px;
        }

        .kitaphana {
            background: url('../assets/hooper/bibl.png');
            background-size: cover;
            width: 35%;
            height: 40vh;
            border-radius: 10px;
        }
    
</style>