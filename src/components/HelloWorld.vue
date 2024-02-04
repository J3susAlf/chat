<template>
  <div class="container">
    <div class="centered-container">
      <div class="bg-container">
        <img class="Imagen" :src="ChatLogo" alt="Imagen">
      </div>
      <div class="container-login">

        <div class="container-title">
          <h3 class="login-heading">Chat App</h3>
        </div>

        <div class="row">   
          <div class="container-buttom">
            <!-- Sign In Form -->
            <form class="container-form">
              <div class="">
                <input type="email" class="form-control custom-input" id="floatingInput" placeholder="Ingresa tu nombre de usuario">
              </div>
              <div class="">
                <input type="password" class="form-control custom-input" id="floatingPassword" placeholder="Ingresa tu contraseña">
              </div>

              <div class="">
                <div class="container-password">
                  <a href="#">Recuperar Contraseña</a>
                </div>
              </div>

            </form>
            <div>
                <button class="btn-login" type="submit">Sign in</button>
              </div>
          </div>
        </div>

        <div class="container-register">
          <a href="#">¿No tienes cuenta? Regístrate</a>
        </div>

      </div>
      
    </div>
  </div>
</template>

<script>
import ChatLogo from '@/assets/ChatLogo.png';
export default {
  name: 'HelloWorld',
  data() {
    return {
      ChatLogo: ChatLogo,
    }
  }
}
</script>

<style scoped>
.container {
  text-align: center;
  margin-top: 100px;
  font-family: 'Poppins', sans-serif;
}

.centered-container {
  display: flex;
  justify-content: center;
  align-items: stretch;
}

.bg-container {
  width: 50%;
  background-color: #313130;
  display: flex;
  justify-content: center;
  align-items: center;
}

.Imagen {
  width: 400px;
  height: auto;
  display: block;
  margin: 0 auto;
}

.container-login {
  width: 40%;
  background-color: #313130;
  text-align: center;
  height: 550px;
/* Ajusta para que sea una columna */
  align-items: center; /* Centra los elementos en la columna */
}

.container-form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
}
.container-title{
  color: #00A8C6;
    width: 95%;
    height: 20%;
    padding: 13px;
    font-size: 25px;
}

.row {
  display: flex;
  justify-content: center;
  color: #00A8C6;
  padding: 20px 10px;
}

.custom-input {
  background: transparent;
  border: none;
  border-bottom: 2px solid #00A8C6;
  color: #fff;
  padding: 5px;
  margin: 5px;
  width: 100%;
}

.custom-input:focus {
  outline: none;
}

.btn-login {
  background-color: #00A8C6;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 52px;
}

.container-password a {
  text-decoration: none;
  color: #00A8C6;
}

.container-register a {
  background-color: #F9F2E7;
  color: #8FBE00;
  text-decoration: none;
  display: block;
  padding: 10px;
  width: 100%; /* Ocupa todo el ancho disponible */
  text-align: center; /* Centra el texto horizontalmente */
}
</style>
