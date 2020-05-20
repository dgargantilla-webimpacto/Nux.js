<template>
  <div class="container-fluid p-0 cf">
    <div class="row justify-content-center p-0 m-0 fila">
      <div class="contenedor">
        <div class="col">
            
            <div class="row justify-content-around fila3 mt-2 mt-sm-3">
                <div class="col-4 col-xs-5 col-sm-5 pl-2 pl-sm-3 c1">
                    <img id="img1" src="~/assets/img/go-back.svg" />
                    <span class="span1">
                        Volver
                    </span>
                </div>
                <div class="col-8 col-xs-7 col-sm-7 pr-2 c">
                    <span class="span2">
                        Ya tengo cuenta
                    </span>
                    <img id="img2" src="~/assets/img/User.svg" />
                </div> 
            </div>
            <div class="row filalogo justify-content-center mt-5">
                <img src="~/assets/img/Nutritienda-simple_logo.svg">
            </div>

            <div class="row justify-content-around mt-5 filaLoguin">
              <div class="col-8 col-sm-7 new">
                <h4 class="span3">Crear nueva cuenta</h4>
              </div>
            </div>

            <div class="row justify-content-center mt-1 filaA">
                <div class="col-12">
                    <span class="span4">Únete y disfruta de todas las ventajas: pedidos rápidos, descuento, promociones, beneficios y muchos más!</span>
                </div>
            </div>
            <div class="row justify-content-center filaicone">
                <div class="col-3">
                    <img src="~/assets/img/Delivery.svg">
                    <span>Envío gratuito</span>
                </div>
                <div class="col-3">
                    <img src="~/assets/img/best_price.svg">
                    <span>Mejor Precio</span>
                </div>
                <div class="col-3">
                    <img src="~/assets/img/lock.svg">
                    <span>Pago 100% seguro</span>
                </div>
                <div class="col-3">
                    <img src="~/assets/img/Superprice.svg">
                    <span>Ofertas exclusivas</span>
                </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  //   layout: "Registro"
  head:{
      title: 'Registrate',
  }
};
</script>

<style src="~/assets/css/style.css" scoped>

