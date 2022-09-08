<template>
  <div class="new_post">
    <form @submit.prevent="onSave">
      <div class="synp">
            <label for="">synp belgi </label>
            <input type="text" v-model="editedPost.synp" />
          </div>
      <div class="birinji">
      
        <div class="monday">
          <p>Monday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.mbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.miki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.muc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.mdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.mbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.malty" />
          </div>
        </div>

        <div class="tuesday">
          <p>Tuesday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.tbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.tiki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.tuc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.tdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.tbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.talty" />
          </div>
        </div>

        <div class="wednesday">
          <p>Wednesday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.wbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.wiki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.wuc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.wdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.wbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.walty" />
          </div>
        </div>

        <div class="thursday">
          <p>Thursday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.hbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.hiki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.huc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.hdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.hbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.halty" />
          </div>
        </div>

        <div class="friday">
          <p>Friday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.fbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.fiki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.fuc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.fdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.fbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.falty" />
          </div>
        </div>

        <div class="saturday">
          <p>Saturday</p>
          <div class="input">
            <label for="">Birinji Sapak </label>
            <input type="text" v-model="editedPost.sbir" />
          </div>

          <div class="input">
            <label for="">Ikinji Sapak </label>
            <input type="text" v-model="editedPost.siki" />
          </div>

          <div class="input">
            <label for="">Üçinji Sapak </label>
            <input type="text" v-model="editedPost.suc" />
          </div>

          <div class="input">
            <label for="">Dördünji Sapak </label>
            <input type="text" v-model="editedPost.sdort" />
          </div>

          <div class="input">
            <label for="">Bäşinji Sapak </label>
            <input type="text" v-model="editedPost.sbas" />
          </div>

          <div class="input">
            <label for="">Altynjy Sapak </label>
            <input type="text" v-model="editedPost.salty" />
          </div>
        </div>
      </div>
      <!-- <div class="input">
        <label for="">Price</label>
        <input type="number" name="" id="" v-model="editedPost.price" />
      </div>
      <div class="input">
        <label for="">IsNew</label>
        <input type="checkbox" name="new" id="" v-model="editedPost.new" />
      </div> -->

      <div class="btns">
        <button>Save</button>
        <button>Cancel</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  props: {
    card: {
      type: Object,
      required: false,
    },
  },
  data() {
    return {
      editedPost: this.card
        ? { ...this.card }
        : {
          synp: '',
            mbir: '',
            miki: '',
            muc: ' ',
            mdort: ' ',
            mbas: ' ',
            malty: ' ',
            mprice: null,
            mnew: false,

            tbir: '',
            tiki: '',
            tuc: ' ',
            tdort: ' ',
            tbas: ' ',
            talty: ' ',
            tprice: null,
            tnew: false,

            wbir: '',
            wiki: '',
            wuc: ' ',
            wdort: ' ',
            wbas: ' ',
            walty: ' ',
            wprice: null,
            wnew: false,

            hbir: '',
            hiki: '',
            huc: ' ',
            hdort: ' ',
            hbas: ' ',
            halty: ' ',
            hprice: null,
            hnew: false,

            fbir: '',
            fiki: '',
            fuc: ' ',
            fdort: ' ',
            fbas: ' ',
            falty: ' ',
            fprice: null,
            fnew: false,

            sbir: '',
            siki: '',
            suc: ' ',
            sdort: ' ',
            sbas: ' ',
            salty: ' ',
            sprice: null,
            snew: false,
            
          },
        }
  },
  methods: {
    onSave() {
      this.$emit('submit12', this.editedPost)
    },
  },
}
</script>

<style scoped>
.new_post {
  width: 60%;
  margin: 10px auto;
  background-color: lightgray;
  padding: 15px;
}
.birinji{
  display: grid;
  grid-template-columns: auto auto auto;

}
.input {
  display: flex;
  padding: 4px;
  font-size: 16px;
  text-align: center;
  height: 25px;
}
.input > label {
  display: block;
  width: 150px;
  text-align: right;
  padding-right: 10px;
}
.input > input {
  border: 1px solid black;
}
.input > textarea {
  border: 1px solid black;
  padding: 10px;
}
.btns {
  display: flex;
  align-items: center;
  justify-content: center;
}
.btns > button {
  padding: 10px 30px;
  background: lightblue;
  border-radius: 30px;
  margin-right: 30px;
}
</style>