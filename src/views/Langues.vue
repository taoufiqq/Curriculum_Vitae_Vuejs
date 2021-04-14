<template>
<h2>Langues </h2>

  <form @submit.prevent="handelSubmit">
<!-- langue 1 -->
    <div class="form-group">
        <label for="Type 1">Type 1</label>
        <input type="text" class="form-control" id="type1"  placeholder="Type 1"  v-model="form4.type1">
        
      </div>
<div class="form-group">
        <label for="Langue1">Langue 1</label>
        <input type="text" class="form-control" id="langue1"  placeholder="Langue 1"  v-model="form4.langue1">
        
      </div>
<!-- langue 2 -->
<div class="form-group">
        <label for="Type2">Langue 1</label>
        <input type="text" class="form-control" id="type2"  placeholder="Type 2"  v-model="form4.type2">        
      </div>
      <div class="form-group">
        <label for="Langue2">Langue 2</label>
        <input type="text" class="form-control" id="langue2" placeholder="Langue 2"  v-model="form4.langue2">
      </div>     
<!-- langue 3 -->
<div class="form-group">
        <label for="Type3">Type 3</label>
        <input type="text" class="form-control" id="type3"  placeholder="Type 3"  v-model="form4.type3">        
      </div>
       <div class="form-group">
        <label for="Langue3">Langue 3</label>
        <input type="text" class="form-control" id="langue3" placeholder="Langue 3"  v-model="form4.langue3">
      </div>
<!-- laugue 4 -->
<div class="form-group">
        <label for="Type4">Type 4</label>
        <input type="text" class="form-control" id="type4"  placeholder="Type 4"  v-model="form4.type4">        
      </div>
      <div class="form-group">
        <label for="Langue4">Langue 4</label>
        <input type="text" class="form-control" id="langue4" placeholder="Langue 4 "  v-model="form4.langue4">
      </div>
      
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Langues",
  data() {
    return {

      form4: {

      type1: "",
      langue1: "",
      type2: "",
      langue2: "",
      type3: "",
      langue3: "",
      type4: "",
      langue4: "",

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form4',JSON.stringify(this.form4))
        redirect('/loisers')
    }
  }
};
</script>
