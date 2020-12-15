<template>
  <div>
    <div class="card my-0">
      <div class="view">
        <img
          src="https://i.imgur.com/0ff4Nvl.jpg"
          class="black-white"
          alt=""
          style="width: 100%; height: 750px; object-fit: cover"
        />
        <div class="mask texture-mask-4"></div>
      </div>

      <div class="card-img-overlay d-flex flex-column text-light">
        <div class="container my-auto text-center">
          <h1 class="mb-4">
            <span
              class="marker marker-dark marker-title px-2"
              style="font-size: 3rem"
            >
              <strong> <em> PROList </em> </strong>
            </span>
          </h1>
          <h4 class="mb-4">
            <span class="marker marker-dark">
              Se você está em busca de uma oportunidade profissional, baseado
              nos seus conhecimentos, acesse já a nossa plataforma!
            </span>
          </h4>

          <button class="btn btn-dark btn-flat">
            <font-awesome-icon :icon="['fas', 'user-plus']" /> Criar conta
          </button>
          <button class="btn btn-dark btn-flat">
            <font-awesome-icon :icon="['fas', 'sign-in-alt']" /> Login
          </button>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="my-5 mx-md-5 mx-2 text-center">
        <h1 class="mb-4"><strong> Sobre a PROList</strong></h1>
        <h3 class="mb-4">
          <em>
            "Somos uma plataforma dedicada a ofertas de projetos profissionais
            para designers e desenvolvedores, através da análise, mapeamento e
            organização de projetos, visando melhor auxiliar aqueles que buscam
            oportunidade de renda e crescimento profissional."
          </em>
        </h3>
      </div>
    </div>
    <div class="container">
      <div class="my-5 mx-md-5 mx-2">
        <h2 class="mb-4 text-center"><strong> Como funciona? </strong></h2>
        <ol class="list-func">
          <li class="mb-3">
            Você irá realizar o seu cadastro na plataforma, informando seus
            dados, sua área de atuação e qualificações.
          </li>
          <li class="mb-3">
            A plataforma, baseando-se nas suas informações, irá recomendar
            projetos que foram previamente mapeados/organizados, que melhor se
            encaixem no seu perfil profissional.
          </li>
          <li class="mb-3">
            Você poderá trabalhar em times, dependendo da demanda do projeto.
          </li>
        </ol>
      </div>
    </div>

    <div class="container">
      <h2 class="text-center mx-md-5 mx-2 mb-4">
        Se você é designer ou desenvolvedor, venha já para a nossa plataforma!
      </h2>
      <h2 class="text-center mx-md-5 mx-2 mb-5">
        Tem alguma dúvida? Entre em contato logo abaixo!
      </h2>
    </div>

    <div class="card my-0">
      <div class="view">
        <img
          src="https://www.worldexecutivesdigest.com/wp-content/uploads/2019/11/home-office.jpeg"
          class="black-white"
          alt=""
          style="width: 100%; height: 600px; object-fit: cover"
        />
        <div class="mask texture-mask-4"></div>
      </div>

      <div class="card-img-overlay d-flex flex-column">
        <div class="container my-auto">
          <div class="col-md-8 offset-md-2 col-12">
            <div class="card card-body card-flat mx-auto d-block">
              <h3 class="mb-3">Contato</h3>
              <div class="form-row">
                <div class="col-lg-6 col-12">
                  <div class="form-group">
                    <label for="exampleInputEmail1">Nome</label>
                    <input
                      type="text"
                      class="form-control form-dark"
                      placeholder="Nome"
                    />
                  </div>
                </div>
                <div class="col-lg-6 col-12">
                  <div class="form-group">
                    <label for="exampleInputEmail1">E-mail</label>
                    <input
                      type="email"
                      class="form-control form-dark"
                      placeholder="Coloque aqui o seu e-mail"
                    />
                  </div>
                </div>
              </div>

              <div class="form-group">
                <label for="exampleInputEmail1">O que você deseja saber?</label>
                <textarea
                  class="form-control form-dark"
                  name=""
                  id=""
                  cols="30"
                  rows="5"
                ></textarea>
              </div>
              <div class="mt-4">
                <button class="btn btn-dark btn-flat mx-auto d-block">
                  <font-awesome-icon :icon="['fas', 'paper-plane']" />
                  Enviar
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <ImageFilter />
  </div>
</template>

<script>
import ImageFilter from '~/components/ImageFilter'
export default {
  components: { ImageFilter },
}
</script>
<style lang="scss">
.list-func {
  font-size: 1.5rem;
  font-family: 'Exo 2', 'Fira Code', sans-serif;
}
</style>
