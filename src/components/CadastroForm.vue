<template>
  <div>
    <h1>locaw<span>eb</span></h1>
    <div id="form">
      <form id="cad_form">
        <h2>Entre na sua conta</h2>
        <h4>Para acessar sua conta informe seu e-mail e senha</h4>
        <div class="input_container">
          <label class="label_name" for="email">E-mail</label>
          <input
            class="input_name"
            type="email"
            id="email"
            name="email"
            v-model="form_email"
            required
            placeholder="Seu e-mail"
          />
        </div>
        <div class="input_container">
          <label class="label_name" for="senha">Senha </label>
          <input
            class="input_name"
            type="password"
            id="senha"
            v-model="form_senha"
            required
            placeholder="Sua senha"
          />
          <label for="senha_esquecida" id="label_senha"
            >Esqueci minha senha</label
          >
        </div>
        <div class="input_container">
          <button
            type="submit"
            name="btn_login"
            id="btn_login"
            value="fazerLogin"
          >
            Fazer Login
          </button>
        </div>
      </form>
    </div>
    <div class="input_container">
      <label id="senha_btn" for="senha"
        >Ainda não tem conta?<span class="destaque_cad">Cadastre!</span>
      </label>
    </div>
  </div>
</template>

<script>
export default {
  name: "CadastroForm",
};
</script>

<style scoped>
/* Estilização do formulario*/

#form {
  background-color: #ffffff;
  width: 600px;
  margin: 0 auto;
  border: 2px solid beige;
  margin-bottom: 20px;
}

h1 {
  font-size: 40px;
  color: #484d50;
}

h2 {
  font-size: 24px;
  text-align: left;
  color: black;
  margin-bottom: 5px;
}

h4 {
  text-align: left;
  margin-top: 5px;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

span {
  color: #f30168;
}

#cad_form {
  max-width: 500px;
  margin: 0 auto;
}
.input_container {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;
}

#label_senha {
  text-align: right;
}

.label_name {
  text-align: left;
}

.input_name,
#btn_login {
  height: 80px;
  border-radius: 4px;
}

#btn_login {
  background: #f30168;
  width: 500px;
  border: none;
  cursor: pointer;
  text-transform: uppercase;
  color: #ffffff;
}

.destaque_cad {
  color: #f30168;
  text-decoration: underline;
  margin-left: 6px;
}
</style>

