<template>
  <div id="nav">
    <router-link to="/">PersonalInfo</router-link> |
    <router-link to="/formation">Formations</router-link> |
    <router-link to="/experience">Experiences</router-link>|
    <router-link to="/langues">Langues</router-link> |
    <router-link to="/loisers">Loisers</router-link> |
    <router-link to="/curriculum_Vitae">CV</router-link> 
  </div>
  <router-view/>
</template>

<style>
body{
  background-color: lightgray;
}
form{
  width: 50%;
  margin-left: 25%;
 

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #42b983;
}







 body>header{
        font-size: 3em;
        font-weight: bold;
        color: blue;
        margin-bottom: 1em ; /*50px/3em;*/
    }
 
    /* titres du bloc main */
    #formation>header, #expe>header {
        font-size: 2em; /* 32 px */
        margin: 0.625em  0px; /* 20px/32px */
        padding : 0.7% ; /*5px/706px */ 
        font-weight: bold;
        color: white;
        background-color: blue;
    }
 
    /* titre et bloc main à gauche */
/* DEPLACE DANS LE fichier cvpc.css
    body>header, main{
        display: block;
        float:left;
        width:73% ; /* 750px/1026px */
/*    }*/
 
    /* diplômes */
    #formation table th {
        text-align: left;
        font-size: 1.2em;
    }
    /* espaces entre 2 formations */
    #formation table tr:nth-child(2n) td {
        padding-bottom: 1em; /* 16px */
    }
 
    
    /* bloc photo + adresse  et divers */
/* DEPLACE DANS LE fichier cvpc.css
    #civil, #divers {
        float:right;
        width: 24%;
        background-color: blue;
        color:white;
        padding: .5em  0.8% ;
    }
*/
    /* pas de triangles pour détails à la demande */



</style>
