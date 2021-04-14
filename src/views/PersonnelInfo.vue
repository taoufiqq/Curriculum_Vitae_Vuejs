<template>
  <h2>Personal Information</h2>

  <form @submit.prevent="handelSubmit">


    <div class="form-group">
      <label for="name">Full Name</label>
      <input
        type="text"
        class="form-control"
        id="name"
        v-model="form1.name"
        placeholder="Full Name "
      />    
    </div>

 <div class="form-group">
      <label for="age">Age</label>
      <input
        type="number"
        class="form-control"
        id="age"
        v-model="form1.age"
        placeholder="Age"
      />
    </div>

    <div class="form-group">
      <label for="address">Address</label>
      <input
        type="text"
        class="form-control"
        id="address"
        v-model="form1.address"
        placeholder="Address"
      />
    </div>

    <div class="form-group">
      <label for="phone">Phone</label>
      <input
        type="text"
        class="form-control"
        id="phone"
        v-model="form1.phone"
        placeholder="Phone"
      />
    </div>

    <div class="form-group">
      <label for="email">EMAIL</label>
      <input
        type="email"
        class="form-control"
        id="email"
        v-model="form1.email"
        placeholder="EMAIL"
      />
    </div>

    <div class="form-group">
      <label for="specialité">Specialité</label>
      <input
        type="text"
        class="form-control"
        id="specialité"
        v-model="form1.specialité"
        placeholder="Specialité"
      />
    </div>


   

    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "PersonnelInfo",
  data() {
    return {

      form1: {

      name: "",
      age: "",
      address: "",
      phone: "",      
      email: "",
      specialité: "",
    

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form1',JSON.stringify(this.form1));
       redirect('/formation')
    }
  }
};
</script>
