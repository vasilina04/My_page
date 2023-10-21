<script setup>

</script>

<template>
    <body>
      <div class="start_info">
        <img src="/src/static/I.jpg" class="My_photo" width="300">
        <div class="profile">
          <h1>Мелихова Василина Андреевна</h1>
          <h3>Будущий программист - организатор</h3>
          <h3>Владивосток</h3>
          <ul class="nobullet">
            <li>
              <a href="https://t.me/Vasilina_Melikhova">
                <img class="icon" src="/src/static/telegram_icon_131945.svg" alt="Telegram">
              </a>
            </li>
            <li>
              <a href="https://vk.com/melikhova2004">
                <img src="/src/static/vk-social-network-logo_icon-icons.com_73339.svg" alt="Vk" class="icon">
              </a>
            </li>
            <li>
              <a href="https://github.com/vasilina04">
                <img src="/src/static/github-logo_icon-icons.com_73546.svg" alt="Github" class="icon">
              </a>
            </li>
          </ul></div>
        </div>
        <h2 class ="fact" style="animation: appear 3s 5s ease;">Обо мне</h2>
        <ul class="information" style="animation: appear 3s 5s ease;">
            <li>Работаю в творческом коллективе <a href="https://vk.com/tm_kadry">ТМ "Кадры"</a></li>
            <li>Учусь на втором курсе Прикладной математики и информатики в ДВФУ</li>
            <li>Главный принцип "Не ошибается тот, кто ничего не делает."</li>
            <li>Учусь преподавать</li>
            <li>Люблю сложные задачи с нестандартными решениями</li>
        </ul>
    </body>
</template>

<style scoped>


.My_photo {
  float: left;
  border-radius: 10px;
  border: 5px solid 7d7f7d;
}

.information {
  display: flexbox;
  justify-content: left;
  margin-left: 17%;
}

li{
  margin-bottom: 10px;
}
.fact {
  display: flex;
  justify-content: left;
  /* align-items: center; */
  margin-top: 1%;
  margin-left: 18%;
  align-items: center;
}

.start_info {
  display: flex;
  justify-content: center;  
  align-items: center;
  margin-top: 2%;
  align-items: margin-left;
}

.profile{
  display: inline;
  margin-left: 4%;
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

@keyframes appear {
    0% {
        opacity: 0;
    }
    100% {
        opacity: 1;
    }
}
</style>