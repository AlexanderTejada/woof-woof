<template>
  <nav class="navbar">
    <div class="navbar-brand">Woof <span>Woof</span></div>
    <ul class="navbar-menu">
      <li><router-link to="/">Inicio</router-link></li>
      <li><router-link to="/adopt">Adoptar</router-link></li>
      <li><router-link to="/about">Nosotros</router-link></li>
      <li><router-link to="/give-up">Dar en adopción</router-link></li>
    </ul>
    <button class="navbar-button">Iniciar sesión</button>
    <button class="navbar-button-2">Registrarse</button>
  </nav>
</template>

  
  <script>
  export default {
    name: 'Navbar',
  }
  </script>
  
  <style scoped>
  
  .navbar {
    display: flex;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #fff;
    font-family: "Inter", sans-serif;

  }
  .navbar-brand {
    font-size: 2.5rem;
    font-weight: bold;
    margin-left: 100px;
    margin-right: 200px;



}

.navbar-brand span {
    color: #FEAE11;
  }
  .navbar-menu {
    list-style: none;
    display: flex;
    gap: 1rem;
  }
  .navbar-menu li a {
    padding: 10px;
    color: #000;
    font-weight: bold;
    font-family: "Inter", sans-serif;
    margin: 0px 20px;
    font-size: 20px;
    text-decoration: none;
    position: relative;
    display: inline-block;
    overflow: hidden; /* Asegura que el pseudo-elemento no se desborde */
}

.navbar-menu li a::after {
    content: '';
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    top: 40px;
    height: 2px; /* Grosor inicial del subrayado */
    background-color: currentColor; /* Utiliza el color del texto */
    transform: scaleX(0); /* Inicia sin mostrarse */
    transition: transform 0.3s ease, height 0.3s ease; /* Transición suave para aparecer y cambiar de grosor */
}

.navbar-menu li a:hover::after {
    transform: scaleX(1); /* Extiende el pseudo-elemento a la longitud completa */
    height: 3px; /* Aumenta el grosor al hacer hover */
}

  .navbar-button {
    background-color: #FEAE11;
    color: #fff;
    border: none;
    padding: 0.8rem 1rem;
    cursor: pointer;
    font-family: "Inter", sans-serif;
    border-radius: 5px;
    margin-left: auto;
    font-size: 20px;
    transition: all 200ms ease-in;



  }
  .navbar-button:hover{
    background-color: #ffba31;
    font-size: 21px;

  }
  .navbar-button-2 {
    background-color: #fffefc;
    color: #000000;
    border: #000000 solid 1px;
    padding: 0.8rem 1rem;
    cursor: pointer;
    font-family: "Inter", sans-serif;
    border-radius: 5px;
    margin-left: 10px;
    font-size: 20px;

    transition: all 200ms ease-in;

  }
  .navbar-button-2:hover{
    background-color: #ffba31;


  }
/* Media Queries para pantallas más pequeñas */
@media (max-width: 1500px) {
  .navbar-brand {
    font-size: 2rem;
    margin: auto;
    margin-left: 22px;
  }
  .navbar-menu li a {
    font-size: 15px;
    margin: auto;
  }
  .navbar-menu li a::after {
    content: '';
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    top: 30px;
    height: 1.5px; /* Grosor inicial del subrayado */
    background-color: currentColor; /* Utiliza el color del texto */
    transform: scaleX(0); /* Inicia sin mostrarse */
    transition: transform 0.3s ease, height 0.3s ease; /* Transición suave para aparecer y cambiar de grosor */
}

.navbar-menu li a:hover::after {
    transform: scaleX(1); /* Extiende el pseudo-elemento a la longitud completa */
    height: 3px; /* Aumenta el grosor al hacer hover */
}

  .navbar-button, .navbar-button-2 {
    padding: 0.7rem 0.9rem;
    font-size: 13px;
  }
  .navbar-button:hover{
    font-size: 14px;
  }
 
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }
  .navbar-brand {
    font-size: 1.8rem;
  }
  .navbar-menu {
    flex-direction: column;
    gap: 0.5rem;
  }
  .navbar-menu li a {
    font-size: 16px;
    margin: 0;
  }
  .navbar-button, .navbar-button-2 {
    margin-left: 0;
    margin-top: 0.5rem;
    padding: 0.6rem 0.8rem;
  }
}

@media (max-width: 480px) {
  .navbar-brand {
    font-size: 1.5rem;
  }
  .navbar-menu {
    display: none; /* Ocultar menú en móviles, puedes cambiar esto a un menú hamburguesa si lo prefieres */
  }
  .navbar-button, .navbar-button-2 {
    margin-left: 0;
    margin-top: 0.5rem;
    padding: 0.5rem 0.7rem;
  }
}
  </style>
  