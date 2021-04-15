<template>
  <div id="CV">
    <div id="infoPersonnel">
      <h4>{{ form1.name }}</h4>
      <p>{{ form1.age }}</p>
      <p>{{ form1.address }}</p>
      <p>{{ form1.phone }}</p>
      <email>{{ form1.email }}</email>
    </div>

    <div id="title">
      <h2>{{ form1.specialité }}</h2>
    </div>

    <div id="pics">
      <img src="../assets/user.png" />
    </div>

    <div class="formation">
      <h4>FORMATION</h4>
    </div>

    <table>
      <tbody>
        <tr>
          <td>{{ form2.date1 }}</td>
          <th>{{ form2.formation1 }}</th>
        </tr>
        <tr>
          <td>{{ form2.date2 }}</td>
          <th>{{ form2.formation2 }}</th>
        </tr>
        <tr>
          <td>{{ form2.date3 }}</td>
          <th>{{ form2.formation3 }}</th>
        </tr>
      </tbody>
    </table>

    <div class="formation">
      <h4>EXPÉRIENCES PROFESSIONNELLES</h4>
    </div>
    <table>
      <tbody>
        <tr>
          <td>{{ form3.date1 }}</td>
          <th>{{ form3.experience1 }}</th>
        </tr>
        <tr>
          <td>{{ form3.date2 }}</td>
          <th>{{ form3.experience2 }}</th>
        </tr>
      </tbody>
    </table>

    <div class="formation">
      <h4>LANGUES</h4>
    </div>

    <table>
      <tbody>
        <tr>
          <td>{{ form4.type1 }}</td>
          <th>{{ form4.langue1 }}</th>
        </tr>
        <tr>
          <td>{{ form4.type2 }}</td>
          <th>{{ form4.langue2 }}</th>
        </tr>
        <tr>
          <td>{{ form4.type3 }}</td>
          <th>{{ form4.langue3 }}</th>
        </tr>
        <tr>
          <td>{{ form4.type4 }}</td>
          <th>{{ form4.langue4 }}</th>
        </tr>
      </tbody>
    </table>

    <div class="formation">
      <h4>CENTRES D’INTERET</h4>
    </div>
    <table>
      <tbody>
        <tr>
          <th>{{ form5.loiser1 }}</th>
        </tr>
        <tr>
          <th>{{ form5.loiser2 }}</th>
        </tr>
        <tr>
          <th>{{ form5.loiser3 }}</th>
        </tr>
      </tbody>
    </table>
    <router-link to="/download">
        <button>download</button>
    </router-link>
  </div>
</template>


 <script>

export default {
  name: "curriculum_Vitae",
  data() {
    return {
      form1: {},
      form2: {},
      form3: {},
      form4: {},
      form5: {},

      show: true
    };
  },
  mounted() {
    this.form1 = JSON.parse(localStorage.getItem("form1"));
    this.form2 = JSON.parse(localStorage.getItem("form2"));
    this.form3 = JSON.parse(localStorage.getItem("form3"));
    this.form4 = JSON.parse(localStorage.getItem("form4"));
    this.form5 = JSON.parse(localStorage.getItem("form5"));
  },
  methods: {
    goToDownload() {
      
    },
  },
};
</script>
