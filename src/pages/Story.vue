<template>
  <div class="storyBg">
    <div class="cover"></div>
    <div class="storyName">
      <router-link class="storyNameLink" to="story">Индеецы</router-link>
    </div>
    <div class="info">
      <p class="discription ">Lorem ipsum dolor sit amet, consectetur adipisicing
         elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
          ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit
          in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
      <div class="likes">
          <img src="../assets/storyLikes.png" alt="Сердечко">
          <p>12</p>
       </div>
       <div class="author">
         <router-link to="/">Sink</router-link>
       </div>
       <div class="date">
          <img src="../assets/storyDate.png" alt="Календарь">
        <p>10.04.19</p>
       </div>
       <router-link class="go" to="/">Начать прохождение</router-link>
    </div>
  </div>
</template>
<style>
  * {
    padding: 0;
    margin: 0;
  }
  .cover {
    width: 100%;
    height: 300px;
    background-image: url("../assets/final.jpg");
    background-size: cover;
    background-position: center;
  }
  .storyNameLink {
    margin-bottom: 10px;
  }
  .storyBg, body {
    background-color: #222;
  }
  .info {
    padding-left: 5%;
    display: table;
    padding-right: 5%;
  }
  .discription {
    color: #fafafa;
    text-align: justify;
    float: left;
    font-weight: 300;
    font-size: 15px;
  }
  .likes {
    float: left;
    margin-top: 30px;
  }
  .date {
    float: right;
    margin-top: 30px;
  }
  .likes > img {
    width: 25px;
    float: right;
    padding-left: 3px;
  }
  .date > img {
    width: 25px;
    float: right;
    padding-left: 3px;
  }
  .likes > p {
    color: #fff;
    font-weight: 200;
    padding-top: 2px;
    float: left;
  }
  .date > p {
    color: #fff;
    font-weight: 200;
    padding-top: 3px;
    float: left;
  }
  .author {
    /* padding-left: 5%; */
    margin-left: 20px;
    width: max-content;
    margin-top: 32px;
    float: left;
    /* margin-top: 2px; */
    /* transform: translate(-50%, 0%) */
  }
  .author > a {
    color: #fff;
    text-decoration: none;
  }
  .go {
    color: #fff;
    float: left;
    font-size: 17px;
    margin-left: 50%;
    transform: translate(-50%, 0%);
    text-decoration: none;
    border: 1px solid #fff;
    padding: 18px 0px;
    width: 100%;
    margin-top: 20px;
    margin-bottom: 20px;
    text-align: center;
    clear: both;
  }
</style>
