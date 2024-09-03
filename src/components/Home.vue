<template>
    <div class="home">
      <section class="hero">
        <div class="text">
            <h1>Sos <br><div class="space-text">El MILAGRO</div> que <br>Ellos esperan</h1>
          <p>En cada rincón, hay una vida esperando por una 
segunda oportunidad. Al adoptar, eres el milagro que
ellos necesitan. Transforma el dolor en esperanza y 
encuentra el amor verdadero en una nueva 
compañía. 
Actúa ahora y <span>cambia una vida!</span>
</p>
          <div class="buttons">
            <button class="ver-video">Ver video</button>
            <button class="adoptar">Adoptar</button>

          </div>
          <div class="line line-1"></div>

        </div>
        <div class="images">
          <img src="/src/assets/images/cat.webp" class="cat" alt="Cat">
          
          <div class="container-dog">
          <img src="/src/assets/images/dog.webp"  class="dog" alt="Dog">
        </div>
        <div class="line line-2"></div>
        <div class="line line-3"></div>
        <div class="line line-4"></div>
        </div>
        <div class="paw-print paw-print-1"></div>
      <div class="paw-print paw-print-2"></div>
      <div class="paw-print paw-print-3"></div>
      <div class="paw-print paw-print-4"></div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Home',
  }
  </script>
  
  <style scoped>
.hero {
  display: grid;
  grid-template-columns: 64.0% 1fr 1fr;
  gap: 1rem;
  padding: 2rem 0 2rem 2rem; /* Arriba, derecha, abajo, izquierda */
  background-color: #fff;
}

.text {
  grid-column: 1 / 2;
  display: flex;
  flex-direction: column;
  justify-content: center;
  font-family: "Inter", sans-serif;
}

.text h1 {
  margin-left: 6rem; /* Ajustar el espacio a la izquierda */
  font-size: 5rem;
  margin-bottom: 1rem;
  line-height: 1.2; /* Asegura un espacio uniforme entre las líneas */
}

.space-text {
  display: inline-block;
  margin-left: 5rem; /* Ajustar el espacio a la izquierda */
  color: #FEAE11;
}

.text p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  max-width: 40%;
  margin-left: 6rem; /* Ajustar el espacio a la izquierda */
}

span {
  color: #F7A501;
  font-weight: 600;
}

.buttons {
  display: flex;
  gap: 1rem;
  margin-bottom: 2rem;
  margin-left: 7rem; /* Ajustar el espacio a la izquierda */
}

.buttons button {
  padding: 0.5rem 1rem;
  cursor: pointer;
  font-size: 30px;
}

.ver-video {
  background-color: transparent;
  border-radius: 11px;
  transition: all 200ms ease-in;
}

.ver-video:hover {
  background-color: #F7A501;
  box-shadow: 5px 10px 0px 0px #F7A501;
}

.adoptar {
  background-color: #F7A501;
  border-radius: 11px;
  color: #fff;
  transition: all 200ms ease-in;
}

.adoptar:hover {
  background-color: #ffbf3e;
  box-shadow: 3px 10px 0px 0px #000000;
  color: #000000;
}

.images {
  grid-column: 2 / 4;
  display: flex;
  gap: 3rem;
}

.images img {
  object-fit: cover;
  filter: grayscale(100%);
  transition: all 200ms ease-in;
}

.images img:hover {
  filter: grayscale(0%);
}

.cat {
  width: 200px;
  height: 400px;
  border-radius: 200px;
  margin-left: 5%;
  margin-top: 30%;
  border: solid 2px #FEAE11;
  padding: 5px;
}

.dog {
  width: 700px;
  height: 700px;
}

.container-dog {
  border-radius: 200px 0px 0px 200px;
  width: 400px;
  height: 640px;
  overflow: hidden;
  border: solid 5px #ffffff;
  border-right: none;
  margin-top: 80px;
  box-shadow: 0 0 0 3px #c4c4c4; /* Borde exterior, sin difuminado */
  transition: all 200ms ease-in;


}
.container-dog:hover{
    box-shadow: 0 0 0 3px #FEAE11; /* Borde exterior, sin difuminado */
}

.line {
  position: absolute;
  height: 4px; /* Altura de la línea */
  background-color: #feaf11;
}

.line-1 {
  top: 41%; /* Ajusta la posición vertical */
  left: 3%;
  width: 7%; /* Ajusta el ancho */
  height: 4%;
}

.line-2 {
  top: 53%; /* Ajusta la posición vertical */
  left: 77%; /* Ajusta la posición horizontal */
  width: 7%; /* Ajusta el ancho */
  height: 2.5%;
}

.line-3 {
  top: 59%; /* Ajusta la posición vertical */
  left: 75%; /* Ajusta la posición horizontal */
  width: 4.2%; /* Ajusta el ancho */
  height: 2.3%;
}

.line-4 {
  bottom: 41.2%; /* Ajusta la posición vertical */
  right: 19.2%;
  width: 1.2%; /* Ajusta el ancho */
  height: 2.2%;
}

.paw-print {
  position: absolute;
  background: url('/src/assets/images/paw-print.png') no-repeat center center;
  background-size: contain;
  width: 50px; 
  height: 50px; 
  animation: float 4s ease-in-out infinite; /* Añade la animación */
}

.paw-print-1 {
  top: 45%;
  left: 50%;
  width: 200px; 
  height: 200px; 
}

.paw-print-2 {
  top: 20%;
  left: 70%;
  opacity: 0.5; /* Ajusta la opacidad para que se vean como un detalle de fondo */
  transform: rotate(25deg);
}

.paw-print-3 {
  bottom: 10%;
  right: 30%;
  opacity: 0.5; 
  transform: rotate(-30deg);
  width: 70px; 
  height: 70px; 
}

.paw-print-4 {
  bottom: 75%;
  right: 15%;
  opacity: 0.5; /* Ajusta la opacidad para que se vean como un detalle de fondo */
  width: 100px; 
  height: 100px; 
  transform: rotate(30deg);
}

@keyframes float {
  0%, 100% {
    transform: translateY(0) rotate(0deg);
  }
  50% {
    transform: translateY(20px) rotate(5deg);
  }
}

/* Media Queries para pantallas más pequeñas */
@media (max-width: 1500px) {
  .text p {
  max-width: 5px;
  }

  .hero {
    grid-template-columns: 1fr;
    padding: 0rem;
  }
  .text {
    grid-column: auto;
    margin-bottom: 2rem;
  }
  .text h1 {
    font-size: 4rem;
    margin-left: 4rem;
  }
  .space-text {
    margin-left: 4rem;
  }
  .text p {
    font-size: 1rem;
    margin-left: 4rem;
    max-width: 60%;
  }
  .buttons {
    margin-left: 5rem;
  }
  .buttons button {
    font-size: 24px;
  }
  .cat {
    width: 150px;
    height: 300px;
    margin-top: 115px;
  }
  .dog {
    width: 600px;
    height: 600px;
  }
  .container-dog {
    width: 300px;
    height: 500px;
    border-radius: 150px 0px 0px 150px;
    margin-top: 10px;
  }
  .line-1 {
    top: 44%; /* Ajusta la posición vertical */
    left: 5%;
    width: 60px;
    height: 23px;
  }
  .line-2 {
    top: 55%; /* Ajusta la posición vertical */
    left: 73%;
    width: 150px;
    height: 20px;
  }
  .line-3 {
    top: 61%; /* Ajusta la posición vertical */
    left: 73%;
    width: 50px;
    height: 15px;
  }
  .line-4 {
    bottom: 33%;
    right: 22.1%;
    width: 30px;
    height: 12px;
  }
  .paw-print-1 {
    width: 150px; 
    height: 150px; 
    left: 600px;
    top: 310px;

  }
  .paw-print-2 {
    width: 80px; 
    height: 80px;
  }
  .paw-print-3 {
    width: 40px; 
    height: 40px; 
    top: 550px;
  }
  .paw-print-4 {
    width: 40px; 
    height: 40px; 
    top: 75px;
  }
}

@media (max-width: 768px) {
  .hero {
    grid-template-columns: 1fr;
    padding: 1rem;
  }
  .text {
    grid-column: auto;
    margin-bottom: 2rem;
  }
  .text h1 {
    font-size: 3rem;
    margin-left: 2rem;
  }
  .space-text {
    margin-left: 2rem;
  }
  .text p {
    font-size: 0.9rem;
    margin-left: 2rem;
    max-width: 80%;
  }
  .buttons {
    margin-left: 3rem;
  }
  .buttons button {
    font-size: 20px;
  }
  .cat {
    width: 100px;
    height: 200px;
  }
  .dog {
    width: 400px;
    height: 400px;
    
  }
  .container-dog {
    width: 300px;
    height: 450px;

  }
  .line-1 {
    top: 45%; /* Ajusta la posición vertical */
    left: 7%;
    width: 50px;
    height: 4px;
  }
  .line-2 {
    top: 57%; /* Ajusta la posición vertical */
    left: 70%;
    width: 50px;
    height: 4px;
  }
  .line-3 {
    top: 63%;
    left: 68%;
    width: 30px;
    height: 4px;
  }
  .line-4 {
    bottom: 45%;
    right: 23%;
    width: 10px;
    height: 4px;
  }
  .paw-print-1 {
    width: 100px; 
    height: 100px; 
  }
  .paw-print-2 {
    width: 80px; 
    height: 80px;
  }
  .paw-print-3 {
    width: 50px; 
    height: 50px; 
  }
  .paw-print-4 {
    width: 60px; 
    height: 60px; 
  }
}

@media (max-width: 480px) {
  .hero {
    grid-template-columns: 1fr;
    padding: 1rem;
  }
  .text {
    grid-column: auto;
    margin-bottom: 2rem;
  }
  .text h1 {
    font-size: 2.5rem;
    margin-left: 1rem;
  }
  .space-text {
    margin-left: 1rem;
  }
  .text p {
    font-size: 0.8rem;
    margin-left: 1rem;
    max-width: 90%;
  }
  .buttons {
    margin-left: 2rem;
  }
  .buttons button {
    font-size: 16px;
  }
  .cat {
    width: 80px;
    height: 160px;
  }
  .dog {
    width: 300px;
    height: 300px;
  }
  .container-dog {
    width: 250px;
    height: 350px;
  }
  .line-1 {
    top: 47%;
    left: 10%;
    width: 40px;
    height: 4px;
  }
  .line-2 {
    top: 60%;
    left: 65%;
    width: 40px;
    height: 4px;
  }
  .line-3 {
    top: 66%;
    left: 63%;
    width: 20px;
    height: 4px;
  }
  .line-4 {
    bottom: 47%;
    right: 25%;
    width: 8px;
    height: 4px;
  }
  .paw-print-1 {
    width: 80px; 
    height: 80px; 
  }
  .paw-print-2 {
    width: 60px; 
    height: 60px;
  }
  .paw-print-3 {
    width: 40px; 
    height: 40px; 
  }
  .paw-print-4 {
    width: 50px; 
    height: 50px; 
  }
}


  </style>
  