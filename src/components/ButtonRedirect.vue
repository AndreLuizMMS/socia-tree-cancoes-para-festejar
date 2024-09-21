<template>
  <a :href="urlRedirect" class="link-wrapper">
    <div class="button-wrapper">
      <div class="image-container">
        <img src="../assets/grupo_vip.jpg" alt="button image" />
      </div>
      <div class="info-container">
        <span>Grupo Vip</span>
      </div>
    </div>
  </a>

  <a :href="urlRedirect" class="link-wrapper">
    <div class="button-wrapper">
      <div class="image-container">
        <img src="../assets/Aula_presencial.png" alt="button image" />
      </div>
      <div class="info-container">
        <span>Agende sua Aula Presencial</span>
      </div>
    </div>
  </a>

  <a :href="urlRedirect" class="link-wrapper">
    <div class="button-wrapper">
      <div class="image-container">
        <img src="../assets/Aula_online.png" alt="button image" />
      </div>
      <div class="info-container">
        <span>Agende sua Aula On-line</span>
      </div>
    </div>
  </a>

  <a :href="urlRedirect" class="link-wrapper">
    <div class="button-wrapper">
      <div class="image-container">
        <img src="../assets/log_cancoes.png" alt="button image" />
      </div>
      <div class="info-container">
        <span>Orçamento Eventos </span>
        <br />
        <span>Canções para celebrar</span>
      </div>
    </div>
  </a>
</template>

<script>
export default {
  props: {
    text: String,
    urlRedirect: String,
    imagePath: String
  },
  mounted() {
    console.log('Image Path:', this.imagePath);
  }
};
</script>

<style scoped lang="scss">
.link-wrapper {
  width: 100%;
  border: #bfaa9e solid 3px;
  border-radius: 5px;
  box-shadow: #aa9584 1px 1px 10px;
  // background-color: #415291;
  
}

.button-wrapper {
  display: flex;
  align-items: center;
  justify-content: baseline;
  width: 100%;
  height: auto;
  gap: 0.5rem;
  padding: 5px;
}

span {
  color: white;
  font-size: 1.2rem;
  letter-spacing: 1px;
}

.image-container img {
  width: 5rem;
  border-radius: 5px;
}
</style>
