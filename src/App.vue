<script setup lang="ts">
</script>

<template>
    <body>
      <div class="start_info">
        <img src="/src/assets/B13A0313.JPG" class="My_photo" width="350">
        <div class="profile">
          <h1>Мелихова Василина Андреевна</h1>
          <h3>Будущий программист - организатор</h3>
          <ul class="nobullet">
            <li>
              <a href="https://t.me/Vasilina_Melikhova">
                <img src="/src/assets/telegram_icon_131945.svg" alt="Telegram" class="icon">
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
    margin-left: 50%;
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
</style>