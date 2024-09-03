<template>
    <div class="about">
      <section class="about-hero">
        <h1>Nosotros</h1>

        <p>En Woof Woof, estamos dedicados a encontrar hogares amorosos para mascotas necesitadas. Creemos en la adopción responsable y en transformar vidas tanto de animales como de personas.</p>

      </section>
      <section class="about-team">
        <h2>Conoce a nuestro equipo</h2>

        <div class="team-members">
          <div class="team-member">
            <h3>Juan Pérez</h3>
            <p>Fundador y Director</p>
          </div>
          <div class="team-member">
            <h3>María López</h3>
            <p>Co-Fundadora y Gerente de Adopciones</p>
          </div>
          <!-- Añade más miembros del equipo según sea necesario -->
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'About',
  }
  </script>
  
  <style scoped>
  .about {
    font-family: "Inter", sans-serif;
    padding: 2rem;
    background-color: #fff;
  }
  
  .about-hero {
    text-align: center;
    margin-bottom: 2rem;
  }
  
  .about-hero h1 {
    font-size: 3rem;
    color: #FEAE11;
    margin-bottom: 1rem;
  }
  
  .about-hero p {
    font-size: 1.2rem;
    max-width: 600px;
    margin: 0 auto;
  }
  
  .about-team {
    text-align: center;
  }
  
  .about-team h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
  }
  
  .team-members {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
  }
  
  .team-member {
    text-align: center;
    max-width: 200px;
  }
  
  .team-member img {
    width: 100%;
    border-radius: 50%;
    margin-bottom: 1rem;
  }
  
  .team-member h3 {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
  }
  
  .team-member p {
    font-size: 1rem;
    color: #555;
  }
  </style>
  