<template>
  <div class="home">
    <div class="row">
      <div class="col-lg-6 text-center">
        <h1>App Medts</h1>
        <p class="" style="text-align: justify">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat ab
          quibusdam obcaecati odio ut nihil laboriosam commodi nulla asperiores
          temporibus cumque iure, quod neque beatae eveniet, ducimus eligendi
          autem earum.
        </p>
      </div>
      <div class="col-lg-6">
        <card-comp :btns="btnArray" class="mx-auto card-comp">
          <form>
            <div class="mb-3 mt-2">
              <input
                type="email"
                class="form-control"
                placeholder="Ingresa tu email"
              />
            </div>
            <div class="mb-3 mt-2">
              <input
                type="password"
                class="form-control"
                placeholder="Contraseña"
              />
            </div>
          </form>
        </card-comp>
      </div>
    </div>
  </div>
</template>

<script>
import CardComp from "@/components/CardComp.vue";
export default {
  name: "HomeView",
  components: {
    CardComp,
  },
  data() {
    return {
      btnArray: [
        {
          title: "Iniciar Sesión",
          txt: "Iniciar sesión",
          class: "btn-primary",
        },
      ],
    };
  },
};
</script>

<style>
/*  */
.home {
  max-width: 895px;
  margin: auto;
  
}
.img-cont {
  display: flex;
  flex-direction: column;
}
img {
  max-width: 315px;
  margin: 1em auto 0 auto;
}
.card-comp {
  max-width: 398px;
  margin-top: 2.6em;
}
@media (min-width: 992px) {
  .home {
    margin: 4em auto;
  }
  img {
    margin: 0;
    margin-top: 5.6em;
  }
  h2 {
    margin: 0;
    margin-top: -0.8em;
    margin-left: 0.8em;
  }
}
</style>
