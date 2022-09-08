<template>
  <div class="nav_menu">
    <div class="bottom">
      <div class="content">
        <div class="logo">
          <p>Mekdep</p>
        </div>

        <ul>
          <li class="settings">
            <nuxt-link to="" class="dropbtn">Mekdep Hakynda</nuxt-link>
            <ul class="settings_content">
              <li><nuxt-link to="">Täzelikler</nuxt-link></li>
              <li><nuxt-link to="">Bäsleşikler</nuxt-link></li>
              <li><nuxt-link to="">Meýilnama</nuxt-link></li>
            </ul>
          </li>

          <li class="settings">
            <nuxt-link to="" class="dropbtn">Resminamalar</nuxt-link>
            <ul class="settings_content">
              <li><nuxt-link to="">Bahalar</nuxt-link></li>
              <li><nuxt-link to="">Güwannama</nuxt-link></li>
              <li><nuxt-link to="">Sylaglar</nuxt-link></li>
            </ul>
          </li>

          <li><nuxt-link to="/admin">Admin</nuxt-link></li>
        </ul>

        <div class="lang">
          <button class="lang_btn">TM</button>
          <button class="lang_btn">RU</button>
        </div>
      </div>
    </div>
    <div class="line"></div>
    <div class="sec"></div>
  </div>
</template>

<script>
export default {}
</script>

<style>



.line {
  width: 100%;
  height: 10px;
  border-bottom: 10px solid rgb(16, 243, 243);
}

.sec {
  width: 100%;
  height: 7px;
  margin: 0 auto;
  border-bottom: 7px solid rgb(191, 251, 251);
}
</style>