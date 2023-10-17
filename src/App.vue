<script setup>

import { ref } from 'vue';
const rotateX = ref(0);
const rotateY = ref(0);
const hue = ref();
const saturation = ref(0);
const lightness = ref(0);
const getMousePos = (e) => {
  const width = e.target.clientWidth;
  const height = e.target.clientHeight;
  const {clientX, clientY} = 0;
  const {innerWidth, innerHeight} = window;
  const x = (clientX / innerHeight) * width - width/2;
  const y = (clientY / innerHeight) * height -height/2;
  rotateX.value = x / 10 + 'deg';
  rotateY.value = y / 10 + 'deg';
  hue.value = (clientY / height) + (clientX / width) *360;
  saturation.value = (clientY / height) + (clientX / width) *100 +'%';
  lightness.value = 50 + '%';
}
const resetPos = () => {
  rotateX.value = 0;
  rotateY.value = 0;
  hue.value = 0;
  saturation.value = 0;
  lightness.value =0;
}


</script>

<template>
    <body>
      <div class="start_info">
        <img src="/src/assets/B13A0313.JPG" class="My_photo" width="350">
        <div class="profile">
          <h1>Мелихова Василина Андреевна</h1>
          <h4>Будущий программист - организатор</h4>
          <h4>Владивосток</h4>
          <ul class="nobullet">
            <li>
              <a href="https://t.me/Vasilina_Melikhova">
                <img @mousemove="getMousePos"
                    @mouseleave="resetPos"
                    class="png" src="/src/assets/telegram_icon_131945.svg" alt="Telegram" width="48"
        height="48">
              </a>
            </li>
            <li>
              <a href="https://vk.com/melikhova2004">
                <img src="/src/assets/vk-social-network-logo_icon-icons.com_73339.svg" alt="Vk" class="icon">
              </a>
            </li>
            <li>
              <a href="https://github.com/vasilina04">
                <img src="/src/assets/github-logo_icon-icons.com_73546.svg" alt="Github" class="icon">
              </a>
            </li>
          </ul></div>
        </div>
      <div class = "fact">
        <h2 class="info">Интересные факты обо мне</h2>
      <ul>
        <li>Работаю в творческом коллективе <a href="https://vk.com/tm_kadry">ТМ "Кадры"</a></li>
        <li>Учусь на втором курсе Прикладной математики и информатики в ДВФУ</li>
        <li>Главный принцип "Не ошибается тот, кто ничего не делает."</li>
        <li>Учусь преподавать</li>
        <li>Люблю сложные задачи с нестандартными решениями</li>
        <li>Работала в приемной комиссии 2023</li>
      </ul></div>

    </body>
</template>

<style scoped>
@media (min-height: 100px) {
  header {
    display: flex;
    place-items: center;
  }
}
body {
    display: inline-block;
    margin-top: 10%;
    margin-left: 10%;
    margin-bottom: 10%;
  }

.My_photo {
  float: left;
  border-radius: 10px;
  border: 5px solid #fff;
  box-shadow: 2px 1px 5px #999999;
}

.start_info {
  display: flex;
  align-items: margin-left;
}

.profile{
  display: inline;
  margin-left: 10%;
}

.icon {
  width: 48px;
  height: 48px;
  margin: 0 12px;
}

.info {
  margin-left: 7%;
  display: flex;
  align-items: center;
}

ul.nobullet {
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.png {
  display: flex;
  transition: all 0.2s linear;
  transform: rotateX(v-bind(rotateY)) rotateY(v-bind(rotateX));
  filter: drop-shadow(0 0 10px hsl(v-bind(hue), v-bind(saturation), v-bind(lightness), 1));
}

body {
  animation-duration: 10s;
  animation-name: slidein;
}

@keyframes slidein {
  from {
    margin-left: 70%;
    width: 500%;
  }

  to {
    margin-left: 10%;
    width: 100%;
  }
}
  
</style>