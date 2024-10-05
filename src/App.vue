<template>
  <div class="outside">
    <div class="wrapper">
      <div class="main-card">
        <div class="header">
          <img src="./assets/PHOTO-2024-05-08-19-24-49.jpg" class="profile-image" />
          <span> Canções para Festejar </span>
        </div>

        <div class="info">
          <button-redirect />
        </div>

        <div class="fotter">
          <img src="./assets/log_cancoes.png" class="logo" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonRedirect from './components/ButtonRedirect.vue';

export default {
  components: { ButtonRedirect },
  data() {
    return {
      buttons: [
        {
          text: 'Grupo Vip',
          image: './assets/grupo_vip.jpg',
          link: ''
        },
        {
          text: '',
          image: './assets/Aula_presencial.png',
          link: ''
        },
        {
          text: '',
          image: './assets/Aula_online.png',
          link: ''
        },
        {
          text: '',
          image: '',
          link: ''
        }
      ]
    };
  }
};
</script>

<style lang="scss">
@font-face {
  font-family: 'CustomFont';
  src: url('@/assets/fonts/custom-font.otf') format('opentype');
  font-weight: normal;
  font-style: normal;
}
* {
  // border: black 1px solid;
  margin: 0;
  font-family: 'Belanosima', sans-serif;
}

.outside {
  background-color: #415291;
  // height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.wrapper {
  background-color: #415291;
  margin-block: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 40rem;
}

.main-card {
  padding-block: 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
  width: 23rem;
  border: #bfaa9e solid 3px;
  border-radius: 5px;
  box-shadow: #aa9584 1px 1px 10px;
  height: 100%;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  border-radius: 5px 5px 0 0;

  span {
    color: white;
    letter-spacing: 3px;
    font-size: 1.6rem;
    margin-bottom: 2rem;
  }

  .profile-image {
    // margin-top: 5px;
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid #bfaa9e;
  }
}

.info {
  display: flex;
  gap: 1rem;
  align-items: center;
  flex-direction: column;
  border-radius: 5px;
  width: 90%;
}

.logo {
  margin-top: 9px;
  width: 10rem;
}
</style>
