<template>
  <h2>Personal Information</h2>

  <form @submit.prevent="handelSubmit">


      <!-- <div class="col-sm-6">
      <div class="input-block">
        <label for="">First Name</label>
        <input type="text" class="form-control">
      </div>
    </div>
    <div class="col-sm-6">
      <div class="input-block">
        <label for="">Last Name</label>
        <input type="text" class="form-control">
      </div>
    </div> -->

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
        type="text"
        class="form-control"
        id="age"
        v-model="form1.image"
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
        type="text"
        class="form-control"
        id="email"
        v-model="form1.cin"
        placeholder="EMAIL"
      />
    </div>

       <div class="form-group">
      <label for="image">IMAGE</label>
      <input
        type="text"
        class="form-control"
        id="image"
        v-model="form1.address"
        placeholder="IMAGE"
      />
    </div>



   

    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {

      form1: {

      name: "",
      phone: "",
      cin: "",
      image: "",
      address: "",
    

      }

     
    };
  },
  methods : {
    handelSubmit(){

       localStorage.setItem('form1',JSON.stringify(this.form1));
       redirect('/ProInfo')
    }
  }
};
</script>
