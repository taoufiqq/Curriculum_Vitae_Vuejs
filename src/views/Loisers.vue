<template>
<h2>Loisers </h2>

  <form @submit.prevent="handelSubmit">

    <div class="form-group">
        <label for="Loiser1">Loiser 1</label>
        <input type="text" class="form-control" id="loiser1"  placeholder="Loiser 1"  v-model="form2.loiser1">
        
      </div>

      <div class="form-group">
        <label for="Loiser2">Loiser 2</label>
        <input type="text" class="form-control" id="loiser2" placeholder="Loiser 2"  v-model="form2.loiser2">
      </div>

       <div class="form-group">
        <label for="Loiser3">Loiser 3</label>
        <input type="text" class="form-control" id="loiser3" placeholder="Loiser 3"  v-model="form2.loiser3">
      </div>


    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Langues",
  data() {
    return {

      form2: {

      loiser1: "",
      loiser2: "",
      loiser3: "",


      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form2',JSON.stringify(this.form2))
        redirect('/loisers')
    }
  }
};
</script>