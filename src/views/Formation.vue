<template>
<h2>Formations </h2>

  <form @submit.prevent="handelSubmit">

    <div class="form-group">
        <label for="email">Formation 1</label>
        <input type="text" class="form-control" id="formation1"  placeholder="Formation 1"  v-model="form2.formation1">
        
      </div>

      <div class="form-group">
        <label for="employer">Formation 2</label>
        <input type="text" class="form-control" id="formation2" placeholder="Formation 2"  v-model="form2.formation2">
      </div>

       <div class="form-group">
        <label for="employer">Formation 3</label>
        <input type="text" class="form-control" id="formation3" placeholder="Formation 3"  v-model="form2.formation3">
      </div>

    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Formation",
  data() {
    return {

      form2: {

      formation1: "",
      formation2: "",
      formation3: "",
     

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form2',JSON.stringify(this.form2))
        redirect('/experience')
    }
  }
};
</script>
