<template>


  <header>Responsable Magasin Prêt à Porter</header>

        <div id="civil">

        
            <img src="images/photo-identite-femme.png" />

            <h1>Sandra Pasdelit</h1>
            <p>10, rue de la bulle-tequse - 14400 Bayeux</p>
            <p>02 31 01 02 03</p>
            <p>06 01 02 03 04</p>
            <email>sandra-pasdelit14@gamail.com</email>
        </div>

        <main>
            <section id="formation">
		<header>FORMATION</header>
		<table>
                    <tbody>
			<tr>
                            <td>Sept 2015 – Juin 2016</td>
                            <th>BTS Force de Vente</th>
			</tr>
			<tr>
                            <td>espace insécable</td>
                            <td>En Alternance à Bayeux</td>
			</tr>
			<tr>
                            <td>Sept 2013 – Juin 2011</td>
                            <th>Baccalauréat Vente</th>
			</tr>
			<tr>
                            <td>espace insécable</td>
                            <td>Lycée David Sommeil Bayeux</td>
			</tr>
                    </tbody>
                </table>
            </section>
            <section id="expe">
		<header>EXPERIENCES PROFESSIONNELLES</header>

		<h1>
                    <span>Jan 2016 – Juin 2016</span><span>DesIgouanes - Responsable Magasin</span>
                    <img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" />
                </h1>
		<ul>
                    <li>Encadrement des 6 vendeuses</li>
                    <li>Gestion de l’espace de vente</li>
                    <li>Mise en valeur des nouvelles collections</li>
                    <li>Interface avec le Siège</li>
		</ul>
		<h1>
                    <span>Sept 2013 – Juin 2013</span><span>Zarma – Vendeuse Prêt à Porter</span>
                    <img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" />
                </h1>
		<ul>
                    <li>Accueil clientèle</li>
                    <li>Conseils et ventes</li>
                    <li>Gestion de caisse</li>
                    <li>Merchandising et mise en rayon</li>
		</ul>
		<h1>
                    <span>2008 –2010</span><span>Boucherie Golepas - Vendeuse saisonnière</span>
                    <img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" />
                </h1>
		<ul>
                    <li>Mise en rayon</li>
                    <li>Vente</li>
                    <li>Gestion de caisse</li>
		</ul>
            </section> <!-- fin expe -->
        </main>
        
        <aside id="divers">
            <h2>ETAT CIVIL<img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" /></h2>
            <ul>
		<li>25 ans</li>
		<li>Nationalité Française</li>
		<li>Permis B</li>
            </ul>
            <h2>INFORMATIQUE<img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" /></h2>
            <ul>
		<li>Word</li>
		<li>Excel</li>
		<li>Internet (formée à <a target="_blank" href="https://ruedelinfo.com" rel="noopener">Rue de l'info</a>)</li>
            </ul>
            <h2>SPORTS<img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" /></h2>
            <ul>
		<li>Yoga</li>
		<li>Free Fight</li>
            </ul>
            <h2>LOISIRS<img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" /></h2>
            <ul>
		<li>Break Dance</li>
		<li>Cinéma</li>
            </ul>
            <h2>VOYAGES<img src="images/TriangleP2.png" width="14" height="14" alt="triangle pour détailler" /></h2>
            <ul>
		<li>Los Angeles</li>
		<li>Tokyo</li>
		<li>Meudon-la-Forêt</li>
            </ul>
        </aside>








<!-- 
  <table class="table table-borderless">
    <thead>
      <tr>

        <th scope="col">Image</th>
        <th scope="col">Full Name</th>
        <th scope="col">Phone</th>
        <th scope="col">CIN</th>
        <th scope="col">Address</th>
        <th scope="col">City</th>
        <th scope="col">Pro Email</th>
        <th scope="col">Employer</th>
        <th scope="col">CNSS</th>
        <th scope="col">Work Address</th>

      </tr>
    </thead>
    <tbody>
      <tr>
        <td>{{form1.image}}</td>
        <td>{{form1.name}}</td>
        <td>{{form1.phone}}</td>
        <td>{{form1.cin}}</td>
        <td>{{form1.address}}</td>
        <td>{{form1.city}}</td>
        <td>{{form2.email}}</td>
        <td>{{form2.employer}}</td>
        <td>{{form2.cnss}}</td>
        <td>{{form2.workAddress}}</td>


      </tr>


    </tbody>
  </table> -->

</template>


// <script>
//   export default {



//     data() {
//       return {

//         form1: {},
//         form2: {},

//       }
//     },
//     mounted() {

//       this.form1 = JSON.parse(localStorage.getItem('form1'))
//       this.form2 = JSON.parse(localStorage.getItem('form2'))



//     }

//   }
// </script>