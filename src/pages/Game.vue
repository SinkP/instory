<template lang="html">
  <q-page class="bgImage">
    <div class="bgColor">
      <h1 class="paragraphName">Индеецы</h1>
      <p>Разнообразный и богатый опыт реализация намеченных плановых заданий
        способствует подготовки и реализации форм развития. Разнообразный и
        богатый опыт реализация намеченных плановых заданий требуют определения
         и уточнения системы обучения кадров, соответствует насущным потребностям.

        Повседневная практика показывает, что рамки и место обучения кадров
        в значительной степени обуславливает создание системы обучения кадров,
        соответствует насущным потребностям. Значимость этих проблем настолько
        очевидна, что постоянное информационно-пропагандистское обеспечение нашей
         деятельности влечет за собой процесс внедрения и модернизации системы
         обучения кадров, соответствует насущным потребностям. Таким образом начало
         повседневной работы по формированию позиции требуют от нас анализа дальнейших
         направлений развития.</p>
      <ul class="so">
        <li><router-link class="to" to="/">Куда-то</router-link></li>
        <li><router-link class="to" to="/">Куда-то</router-link></li>
        <li><router-link class="to" to="/">Куда-то</router-link></li>
        <li><router-link class="to" to="/">Куда-то</router-link></li>
      </ul>
    </div>
  </q-page>
</template>

<script>
export default {
};
</script>

<style lang="css">
  .q-layout-page-container {
    background-image: url("../assets/final.jpg");
    background-size: cover;
    background-position: center;
  }
  .bgImage {
    padding-top: 1px;
    background: rgba(0, 0, 0, .45);
  }
  .bgColor > h1 {
    text-align: center;
    color: white;
    padding: 40px 0 40px;
    font-size: 25.6px;
    font-size: 1.7rem;
    /* font-weight: bold; */
    margin: 0;
    text-shadow: 0.3px 0.3px 4px #000;
  }
  .bgColor > p {
    line-height: 1.3;
    word-spacing: 2.5px;
    color: white;
    font-size: 14.5px;
    text-align: left;
    padding: 0px 20px;
    text-shadow: 0.4px 0.4px 3px #000;
  }
  .so {
    list-style-type: none;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    padding-top: 5px;
    padding-bottom: 40px;
    padding-left: 15px;
    margin: 0;
  }
  .so > li {
    margin-bottom: 50px;
    max-width: 95%;
    width: max-content;
    margin-top: 25px;
    margin-left: 50%;
    transform: translate(-50%, 0%);
    text-align: center;
  }
  .to {
    border: 1px solid #fff;
    padding: 14px 27px;
    color: #fff;
    text-decoration: none;

  }
</style>
