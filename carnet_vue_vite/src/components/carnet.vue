<template>
  <div class="container">
    <div class="row carnet">
      <div class="col-4 carnet-aside">
        <div class="header d-flex justify-content-between">
          <h5>CEDULA DE INDENTIDAD</h5>
          <img id="chile-flag" src="../assets/img/chile_bandera.png" alt="Chile Flag" />
        </div>
        <img class="user-photo" src="../assets/img/foto_elon.jpg" alt="User Photo" />
        <p class="run">RUN {{ run }}</p>
      </div>

      <div class="col-8 carnet-main">
        <header>
          <h1 class="text-left">REPUBLICA DE CHILE</h1>
          <h6 class="servicio text-left">SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</h6>
        </header>

        <section>
          <div class="row">
            <div class="col-12">
              <article class="text-start"> 
                <header>APELLIDOS</header>
                <span>{{ apellidos }}</span>
              </article>
            </div>
          </div>
          
          <div class="row">
            <div class="col-12">
              <article class="text-start"> 
                <header>NOMBRES</header>
                <span>{{ nombres }}</span>
              </article>
            </div>
          </div>

          <div class="row">
            <div class="col-6">
              <article class="text-start"> 
                <header>NACIONALIDAD</header>
                <span>{{ nacionalidad }}</span>
              </article>
            </div>
            <div class="col-6">
              <article class="text-start"> 
                <header>SEXO</header>
                <span>{{ sexo }}</span>
              </article>
            </div>
          </div>

          <div class="row">
            <div class="col-6">
              <article class="text-start"> 
                <header>FECHA DE NACIMIENTO</header>
                <span>{{ fechaNacimiento }}</span>
              </article>
            </div>
            <div class="col-6">
              <article class="text-start"> 
                <header>NÚMERO DOCUMENTO</header>
                <span>{{ numeroDocumento }}</span>
              </article>
            </div>
          </div>

          <div class="row">
            <div class="col-6">
              <article class="text-start"> 
                <header>FECHA DE EMISIÓN</header>
                <span>{{ fechaEmision }}</span>
              </article>
            </div>
            <div class="col-6">
              <article class="text-start"> 
                <header>FECHA DE VENCIMIENTO</header>
                <span>{{ fechaVencimiento }}</span>
              </article>
            </div>
          </div>

          <div class="row">
            <div class="col-12">
              <article class="text-start"> 
                <header>FIRMA DEL TITULAR</header>
                <span>{{ firma }}</span>
              </article>
            </div>
          </div>
</section>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      run: '22.222.222-2',
      apellidos: 'MUSK',
      nombres: 'ELON REEVE',
      nacionalidad: 'SUDAFRICANO',
      sexo: 'M',
      fechaNacimiento: '28 JUN 1971',
      numeroDocumento: '222.222.222',
      fechaEmision: '01 ENE 2025',
      fechaVencimiento: '01 ENE 2030',
      firma: 'X Æ A-12',
    };
  },
};
</script>

<style scoped>
#chile-flag {
  height: 2rem;
}

.header {
  align-self: flex-start;
}

.carnet {
  background: #c8deed;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 2px black;
  padding: 15px;
}

.carnet-aside {
  display: flex;
  flex-direction: column;
  justify-content: left;
}

.carnet-main {
  text-align: left;
}

.user-photo {
  margin-top: 10px;
  width: auto;
  height: 13rem;
  border-radius: 5px;
}

.run {
  font-size: 12px;
  font-weight: bold;
}

h1 {
  font-size: 24px; 
  margin: 0;
  font-weight: bold;
  color: #0235a4;
}

.servicio {
  font-size: 16px; 
  font-weight: bold; 
  color: #0235a4; 
  margin-top: 5px; 
}

article header {
  font-weight: bold;
  color: #0235a4;
  font-size: 10px; 
}

section article span {
  font-size: 13px;
  font-weight: 600;
}
</style>
