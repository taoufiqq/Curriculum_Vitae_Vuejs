<template>
<h2>Formations </h2>

  <form @submit.prevent="handelSubmit">

 <div class="form-group">
        <label for="date1">Date 1</label>
        <input type="text" class="form-control" id="date1"  placeholder=" date 1"  v-model="form2.date1">
        
      </div>

    <div class="form-group">
        <label for="formation1">Formation 1</label>
        <input type="text" class="form-control" id="formation1"  placeholder="Formation 1"  v-model="form2.formation1">
        
      </div>

 <div class="form-group">
        <label for="date2">Date 2</label>
        <input type="text" class="form-control" id="date2"  placeholder="date 2"  v-model="form2.date2">
        
      </div>

      <div class="form-group">
        <label for="formation2">Formation 2</label>
        <input type="text" class="form-control" id="formation2" placeholder="Formation 2"  v-model="form2.formation2">
      </div>

 <div class="form-group">
        <label for="date3">Date 3</label>
        <input type="text" class="form-control" id="date3"  placeholder="date 3"  v-model="form2.date3">
        
      </div>

       <div class="form-group">
        <label for="formation3">Formation 3</label>
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

      date1: "",  
      formation1: "",
      date2: "",
      formation2: "",
      date3: "",
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
