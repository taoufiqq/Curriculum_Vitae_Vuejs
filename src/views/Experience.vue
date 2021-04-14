<template>
<h2>Experience </h2>

  <form @submit.prevent="handelSubmit">

    <div class="form-group">
        <label for="experience1">Experience 1</label>
        <input type="text" class="form-control" id="experience1"  placeholder="experience1"  v-model="form2.experience1">
        
      </div>

      <div class="form-group">
        <label for="experience2">Experience 2</label>
        <input type="text" class="form-control" id="experience2" placeholder="Experience 2"  v-model="form2.experience2">
      </div>

       <div class="form-group">
        <label for="experience3">Experience 3</label>
        <input type="text" class="form-control" id="experience3" placeholder="Experience 3"  v-model="form2.experience3">
      </div>

    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Experience",
  data() {
    return {

      form2: {

      experience1: "",
      experience2: "",
      experience3: "",
     

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form2',JSON.stringify(this.form2))
        redirect('/langues')
    }
  }
};
</script>
