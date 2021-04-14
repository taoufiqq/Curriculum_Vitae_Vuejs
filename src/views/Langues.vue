<template>
<h2>Langues </h2>

  <form @submit.prevent="handelSubmit">

    <div class="form-group">
        <label for="Langue1">Langue 1</label>
        <input type="text" class="form-control" id="langue1"  placeholder="Langue 1"  v-model="form2.angue1">
        
      </div>

      <div class="form-group">
        <label for="Langue2">Langue 2</label>
        <input type="text" class="form-control" id="langue2" placeholder="Langue 2"  v-model="form2.langue2">
      </div>

       <div class="form-group">
        <label for="Langue3">Langue 3</label>
        <input type="text" class="form-control" id="langue3" placeholder="Langue 3"  v-model="form2.langue3">
      </div>

      <div class="form-group">
        <label for="Langue4">Langue 4</label>
        <input type="text" class="form-control" id="langue4" placeholder="Langue 4 "  v-model="form2.langue4">
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

      langue1: "",
      langue2: "",
      langue3: "",
      langue4: "",

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
