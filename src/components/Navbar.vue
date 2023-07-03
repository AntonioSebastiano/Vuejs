<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top">
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#" @click="goToHome">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" @click="goToAbout">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" @click="goToServices">Services</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" @click="goToContact">Contact</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'MainNavbar',
  methods: {
    goToAbout() {
      this.$router.push('/about');
    },
    goToContact() {
      this.$router.push('/contact');
    },
    goToServices() {
      this.$router.push('/services');
    },
    goToHome() {
      this.$router.push('/');
    },
  },
}
</script>

<style>
.navbar {
  background-color: #004080; /* Colore di sfondo distintivo */
  position: fixed;
  top: 0;
  width: 100%;
  transition: background-color 0.3s; /* Transizione del colore di sfondo */
}

.navbar-nav .nav-item .nav-link {
  transition: color 0.s; /* Transizione del colore del testo */
  color: #ffffffab;
}

.navbar-nav .nav-item .nav-link:hover,
.navbar-toggler:focus {
  color: #fff; /* Cambio colore del testo al passaggio del mouse o al focus */
}

.navbar-toggler {
  border: none;
  outline: none;
}

.navbar-toggler-icon {
  background-color: #fff; /* Colore dell'icona del toggler */
}

.nav-link {
  font-size: 16px;
}

.navbar-brand {
  font-size: 24px;
  font-weight: bold;
  margin-right: 15px;
}

/* Personalizzazioni per pulsanti arrotondati */
.btn {
  border-radius: 50px;
}

/* Personalizzazioni per effetto parallasse */
.navbar {
  background-image: url('../assets/img.jpg');
  transition: background-color 0.3s;
  /* Aggiunta del contorno */
  box-shadow: 0px 7px 10px rgba(94, 94, 94, 0.2);
  border-bottom: 2px solid #000000;
  height: 60px; /* Altezza desiderata */
}
</style>
