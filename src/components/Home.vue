<template>
  <div class="substrate-container">
    <div class="main-container">
      <div class="logotype">ГК «ПрофМедиаСтрой»</div>
      <div class="title">Застройка<br>выставочных стендов</div>
      <div class="contacts">
        <div class="email">
          <img src="@/assets/icons/email.svg">
          <span>denissham@yandex.ru</span>
        </div>
        <div class="phone">
          <img src="@/assets/icons/phone.svg">
          <span>+7 977 854 69 28</span>
        </div>
      </div>
      <div class="send-buttons">
        <a href="mailto:denissham@yandex.ru" class="email-button">
          <div class="button">
            <img src="@/assets/icons/message.svg">
            <span>Написать</span>
          </div>
        </a>
        <a href="tel:+79778546928" class="phone-button">
          <div class="button">
            <img src="@/assets/icons/phone-button.svg">
            <span>Позвонить</span>
          </div>
        </a>
      </div>
      <div class="information">В настоящий момент сайт находится в стадии разработки</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<style scoped>
.substrate-container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  background: url(../assets/images/background.webp);
  background-size: cover;
  background-position: center;
}
.main-container {
  width: 100%;
}
.logotype {
  width: 22%;
  padding: 10px;
  box-sizing: border-box;
  margin: auto;
  font-size: 2vw;
  text-align: center;
  color: white;
  background-color: #066fba;
}
.title {
  font-size: 5vw;
  color: white;
  text-align: center;
  width: 70%;
  font-weight: bold;
  text-transform: uppercase;
  margin: 50px auto 0;
}
.contacts {
  display: flex;
  justify-content: center;
  margin-top: 50px;
}
.email {
  display: flex;
  align-items: center;
  font-size: 2vw;
  color: white;
  font-weight: bold;
}
.phone {
  display: flex;
  align-items: center;
  font-size: 2vw;
  color: white;
  font-weight: bold;
  margin-left: 50px;
}
.email > img, .phone > img {
  width: 2.5vw;
  margin-right: 10px;
}
.send-buttons {
  display: flex;
  justify-content: center;
  margin-top: 50px;
}
.email-button {
  text-decoration: none;
}
.phone-button {
  text-decoration: none;
  margin-left: 50px;
}
.button {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #009ee1;
  border-radius: 50px;
  width: 10vw;
  padding: 15px;
  transition: background-color .1s ease-in;
}
.button > span {
  font-size: 1.5vw;
  font-weight: bold;
  color: white;
}
.button > img {
  width: 1.6vw;
  margin-right: 10px;
}
.button:hover {
  background-color: #066fba;
  transition: background-color .1s ease-in;
}
.information {
  font-size: 1vw;
  color: white;
  text-align: center;
  margin-top: 50px;
  opacity: 0.5;
}
@media screen and (max-width: 800px) {
  .logotype {
    width: 55%;
    font-size: 5vw;
  }
  .title {
    font-size: 9vw;
  }
  .phone {
    margin-left: 30px;
  }
  .phone-button {
    margin-left: 30px;
  }
  .email, .phone {
    font-size: 4vw;
  }
  .email > img, .phone > img {
    width: 4vw;
  }
  .button {
    width: 30vw;
  }
  .button > span {
    font-size: 4vw;
  }
  .button > img {
    width: 3vw;
  }
  .information {
    font-size: 3vw;
  }
}
</style>
