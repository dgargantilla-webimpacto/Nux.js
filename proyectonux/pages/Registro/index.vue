<template>
  <div class="container-fluid p-0 cf">
    <div class="row justify-content-center p-0 m-0 fila">
      <div class="contenedor">
        <div class="col">
          <div class="row justify-content-around fila3 mt-2 mt-sm-3">
            <div class="col-4 col-xs-5 col-sm-5 pl-2 pl-sm-3 c1">
              <img id="img1" src="~/assets/img/go-back.svg" />
              <span class="span1">Volver</span>
            </div>
            <div class="col-8 col-xs-7 col-sm-7 pr-2 c">
              <span class="span2">Ya tengo cuenta</span>
              <img id="img2" src="~/assets/img/User.svg" />
            </div>
          </div>
          <div class="row filalogo justify-content-center mt-5">
            <img src="~/assets/img/Nutritienda-simple_logo.svg" />
          </div>

          <div class="row justify-content-around mt-5 filaLoguin">
            <div class="col-8 col-sm-10 new">
              <h4 class="span3">Crear nueva cuenta</h4>
            </div>
          </div>

          <div class="row justify-content-center mt-1 filaA">
            <div class="col-12">
              <span
                class="span4"
              >Únete y disfruta de todas las ventajas: pedidos rápidos, descuento, promociones, beneficios y muchos más!</span>
            </div>
          </div>
          <div class="row justify-content-center mt-3 filaicone">
            <div class="col-3 col-sm-2">
              <img src="~/assets/img/Delivery.svg" />
              <span>Envío gratuito</span>
            </div>
            <div class="col-3 col-sm-2">
              <img src="~/assets/img/best_price.svg" />
              <span>Mejor Precio</span>
            </div>
            <div class="col-3 col-sm-2">
              <img src="~/assets/img/lock.svg" />
              <span>Pago 100% seguro</span>
            </div>
            <div class="col-3 col-sm-2">
              <img src="~/assets/img/Superprice.svg" />
              <span>Ofertas exclusivas</span>
            </div>
          </div>

          <div class="row justify-content-center align-items-center mt-3 mt-sm-4 filaA2">
            <hr class="hr" />
            <span class="span5">ACCESO RÁPIDO CON REDES SOCIALES</span>
            <hr class="hr" />
          </div>

          <div class="row justify-content-center mt-4 filaA3">
            <div class="col-2 m-2 m-sm-1">
              <img src="~/assets/img/connect-Facebook-42px.svg" />
            </div>
            <div class="col-2 m-2 m-sm-1">
              <img src="~/assets/img/connect-Google-42px.svg" />
            </div>
            <div class="col-2 m-2 m-sm-1">
              <img src="~/assets/img/connect-Twitter-42px.svg" />
            </div>
          </div>

          <div class="row justify-content-center align-items-center mt-4 mt-sm-0 filaA2">
            <hr class="hr2" />
            <span class="span5">ACCESO CON EMAIL Y CONTRASEÑA</span>
            <hr class="hr2" />
          </div>
          <div class="row justify-content-start align-items-center pl-2 g">
            <Radio nombre1="Hombre" nombre2="Mujer" />
          </div>
          <div class="row justify-content-center align-items-center pl-2 pr-2 mt-3">
            <div class="col-6 pr-2">
              <div class="form-group">
                <label>Nombre</label>
                <input type="text" class="form-control" id />
              </div>
            </div>
            <div class="col-6 pl-2">
              <div class="form-group">
                <label>Apellidos</label>
                <input type="text" class="form-control" id />
              </div>
            </div>
          </div>
          <div class="row justify-content-center pl-2 pr-2">
            <div class="col-12 col-sm-6">
              <!-- <div class="row justify-content-start pl-2 pr-2 birth"> -->
              <label>Tu cumpleaños</label>
              <!-- </div> -->
              <Cumpleaños />
            </div>

            <div class="col-12 col-sm-6 mt-2">
              <div class="form-group">
                <label>Email</label>
                <input type="text" class="form-control" placeholder="Ej: tu@email.com" id />
              </div>
            </div>
          </div>
          <div class="row justify-content-center pl-2 pr-2">
            <div class="col-6 pr-2">
              <Contraseña nombre="Contraseña" />
            </div>
            <div class="col-6 pl-2">
              <Contraseña nombre="Repetir contraseña" />
            </div>
          </div>
          <div class="row pl-2 pr-2 mt-4 mb-4">
            <div class="col-10 mb-2 colcheck">
              <Cbox contenido="Suscríbete a la Newsletter" />
              <small
                id="helpId"
                class="form-text text-muted"
              >Acceso exclusivo a noticias, nuevos productos, descuentos, sorteos y promociones especiales.</small>
            </div>
            <div class="col-12">
              <Cbox contenido="Confirmo que he leído y acepto la política de privacidad." />
            </div>
          </div>
          <div class="row pl-1 pr-1 pb-4">
            <div class="col-12">
              <Boton contenido="Regístrate" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Radio from "@/components/Radio";
import Cumpleaños from "@/components/Cumpleaños";
import Contraseña from "@/components/Contraseña";
import Cbox from "@/components/Cbox";
import Boton from "@/components/Boton";
export default {
  //   layout: "Registro"
  head: {
    title: "Registrate"
  },
  components: {
    Radio,
    Cumpleaños,
    Contraseña,
    Cbox,
    Boton
  }
};
</script>

<style src="~/assets/css/style.css" scoped>
