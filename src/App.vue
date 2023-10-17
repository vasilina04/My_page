<script setup lang="ts">
</script>

<template>
  <body>
    <img src="/src/assets/B13A0313.JPG"  class = "My_photo" width="350">
    <h1 class = "info">Мелихова Василина Андреевна</h1>
    <h4 class = "info">Будущий программист - организатор</h4>
    <a href="https://t.me/Vasilina_Melikhova">
      <img src="/src/assets/telegram_icon_131945.svg" alt="Telegram" class = "icon"></a>
    <a href="https://vk.com/melikhova2004">
      <img src="/src/assets/vk-social-network-logo_icon-icons.com_73339.svg" alt="Vk" class = "icon"></a>
    <a href="https://github.com/vasilina04">
      <img src="/src/assets/github-logo_icon-icons.com_73546.svg" alt="Github" class = "icon"></a>
    <h2 class="info">Интересные факты обо мне</h2>
    <ul>
     <li>Работаю в творческом коллективе<a href="https://vk.com/tm_kadry">ТМ "Кадры"</a></li> 
     <li>Учусь на втором курсе Прикладной математики и информатика в ДВФУ</li>
     <li>Главный принцип "Не ошибается тот, кто ничего не делает."</li>
     <li>Учусь преподавать</li>
     <li>Люблю сложные задачи с нестандартыми решением проблемы </li>
    <li>Работала в приемной комиссии 2023</li>
   </ul>

  </body>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
@media (min-width: 1024px) {
  body {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }


  body.wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
  .My_photo {
    border-radius: 10px;  /* Скругление углов изображения */
    border: 5px solid #fff; /* Цвет и ширину рамки */
    box-shadow: 2px 1px 5px #999999; /* Цвет и размер тени */
}
  .icon {
    width: 48px;
    height: 48px;
    margin-left: 12px;
    margin-right: 12px;
  }
  .info{
    margin-left: 7%;
    display: flex;
    place-items: center;
  }
</style>
