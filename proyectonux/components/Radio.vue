<template>
  <div>
    <div class="col">
      <label class="custom-radio-checkbox">
        <!-- Input oculto -->
        <input
          class="custom-radio-checkbox__input"
          type="radio"
          name="genero"
          value="mujer"
          checked
        />
        <!-- Imagen en sustitucion -->
        <span class="custom-radio-checkbox__show custom-radio-checkbox__show--radio"></span>
        <!-- Texto -->
        <span class="custom-radio-checkbox__text">Mujer</span>
      </label>
    </div>
    <p class="col">
      <label class="custom-radio-checkbox">
        <!-- Input oculto -->
        <input class="custom-radio-checkbox__input" type="radio" name="genero" value="hombre" />
        <!-- Imagen en sustitucion -->
        <span class="custom-radio-checkbox__show custom-radio-checkbox__show--radio"></span>
        <!-- Texto -->
        <span class="custom-radio-checkbox__text">Hombre</span>
      </label>
    </p>
  </div>
</template>

<style>
.custom-radio-checkbox {
  display: inline-flex;
  align-items: center;
  cursor: pointer;
  font-family: arial;
}

/* Modificador para dar la imagen de radio */
.custom-radio-checkbox__show--radio {
  background-image: none;
}

/* Oculta input original */
.custom-radio-checkbox > .custom-radio-checkbox__input {
  display: none;
}

/* Radio personalizado usando <span> */
.custom-radio-checkbox > .custom-radio-checkbox__show {
  display: inline-block;
  width: 15px;
  height: 15px;
  margin-right: 0.5rem;
  background-size: cover;
}

/* Cambia el radio personalizado cuando es pulsado */
.custom-radio-checkbox
  > .custom-radio-checkbox__input:checked
  + .custom-radio-checkbox__show--radio {
  background-color: #fa2398;
}
</style>