<template>
<h2>Experience </h2>

  <form @submit.prevent="handelSubmit">

     <div class="form-group">
        <label for="date1">Date 1</label>
        <input type="text" class="form-control" id="date1"  placeholder=" date 1"  v-model="form3.date1">
        
      </div>


    <div class="form-group">
        <label for="experience1">Experience 1</label>
        <input type="text" class="form-control" id="experience1"  placeholder="experience1"  v-model="form3.experience1">
        
      </div>

<div class="form-group">
        <label for="date2">Date 2</label>
        <input type="text" class="form-control" id="date2"  placeholder=" date 2"  v-model="form3.date2">
        
      </div>

      <div class="form-group">
        <label for="experience2">Experience 2</label>
        <input type="text" class="form-control" id="experience2" placeholder="Experience 2"  v-model="form3.experience2">
      </div>


    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Experience",
  data() {
    return {

      form3: {

      date1: "",  
      experience1: "",
      date2: "",  
      experience2: "",

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form3',JSON.stringify(this.form3))
        redirect('/langues')
    }
  }
};
</script>
