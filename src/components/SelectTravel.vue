<script setup>
import axios from 'axios';


</script>

<template>
  <div class="tickets">
    <select name="origin" id="origin" class="tickets-select-box">
      <option value="" selected disabled>¿De donde partes?</option>
      <option >{{station}}</option>
    </select>
    <select name="destination" id="destination" class="tickets-select-box">
      <option value="" selected disabled>¿A donde vas?</option>
      <option value="Victoria">Victoria</option>
      <option value="PUA">PUA</option>
      <option value="Perquenco">Perquenco</option>
      <option value="Quillem">Quillem</option>
      <option value="Lautaro">Lautaro</option>
      <option value="Lautaro Centro">Lautaro Centro</option>
      <option value="Pillanlelbun">Pillanlelbun</option>
      <option value="Cajon">Cajon</option>
      <option value="Temuco">Temuco</option>
    </select>
    <input type="date" id="travel-date" name="date" class="tickets-select-box">
    <button class="tickets-confirm-button" onclick="window.location.href = 'select-travel.html';">Buscar</button>
  </div>
</template>

<style scoped>
.tickets{

  overflow: hidden;
  display: flex;
  width: 75%;
  min-width: 666px;
  padding: 0.625rem 1rem;
  align-items: center;
  gap: 0.3125rem;
  border-radius: 0.9375rem;
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  backdrop-filter: blur(10px);
  justify-content: space-between;
}

.tickets-select-box{
  opacity: 60%;
  font-family: "Inter";
  font-weight: 500;
  display: flex;
  width: 27%;
  height: 4rem;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  border-radius: 0.9375rem;
  text-align: center;
  font-size: x-large;
}

.tickets-confirm-button{
  color: #000;
  width: 13%;
  font-size: x-large;
  display: flex;
  height: 4rem;
  padding: 0.625rem 1.8125rem;
  justify-content: center;
  align-items: center;
  background: #F7D40A;
  border-radius: 0.9375rem;
}

.standard-text-input{
  height: 2.625rem;
  flex: 1 0 0;
  background: #FFF;
  border-radius: 1.25rem;
}
</style>