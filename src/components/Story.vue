<template>
   <div class="story">
     <div class="storyName">
       <router-link class="storyNameLink" to="story">Индеецы</router-link>
     </div>
     <div class="storyCover"></div>
     <div class="discription">
       <p class="storyDiscription">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
         Beatae, numquam, facere. Ab cum explicabo eligendi porro inventore repudiandae,
          eum ut voluptas nobis suscipit corporis impedit nam? Velit, illo ab deserunt.</p>
       <div class="storyInfo">
         <div class="storyLikes">
           <img src="../assets/storyLikes.png" alt="Сердечко">
           <p>12</p>
         </div>
         <div class="storyDate">
           <img src="../assets/storyDate.png" alt="Календарь">
           <p>10.04.19</p>
         </div>
       </div>
       <div class="storyAuthor">
         <router-link to="/">Sink</router-link>
       </div>
     </div>
   </div>
</template>

<style>
  .story {
    background-color: #222;
    width: 100%;
    height: 550px;
    border-bottom: 1px solid #6c6c6c;
  }
  .storyNameLink {
    color: #fafafa;
    font-weight: 200;
    font-size: 28px;
    display: inline-block;
    text-decoration: none;
    padding-top: 90px;
    margin-left: 50%;
    transform: translate(-50%, -50%);
    width: max-content;
  }
  .storyName {
    height: 90px;
    position: relative;
  }
  .storyCover {
    background-image: url('../assets/final.jpg');
    width: 100%;
    height: 280px;
    background-size: cover;
    background-position: center;
  }
  .storyDiscription {
    color: #fff;
    padding-top: 30px;
    font-size: 15px;
    padding-left: 5%;
    padding-right: 5%;
    font-weight: 300;
  }
  .storyInfo {
    width: 100%;
  }
  .storyLikes {
    float: left;
    padding-left: 5%;
  }
  .storyDate {
    float: right;
    padding-right: 5%;
  }
  .storyLikes > img {
    width: 25px;
    float: right;
    padding-left: 3px;
  }
  .storyDate > img {
    width: 25px;
    float: right;
    padding-left: 3px;
  }
  .storyLikes > p {
    color: #fff;
    font-weight: 200;
    padding-top: 2px;
    float: left;
  }
  .storyDate > p {
    color: #fff;
    font-weight: 200;
    padding-top: 3px;
    float: left;
  }
  .storyAuthor {
    /* padding-left: 5%; */
    margin-left: 20px;
    width: max-content;
    float: left;
    margin-top: 2px;
    /* transform: translate(-50%, 0%) */
  }
  .storyAuthor > a {
    color: #fff;
    text-decoration: none;
  }
</style>

<script>
export default {
  name: 'PageIndexx',
};
</script>
