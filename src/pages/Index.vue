<template>
  <q-page>
    <div class="mod">
      <h2 class="mainHeader">Лучшие инстори</h2>
    </div>
    <story-block></story-block>
    <story-block></story-block>
  </q-page>
</template>

<style>
  * {
    padding: 0;
    margin: 0;
  }
  .mod {
    position: relative;
    height: 115px;
    background-color: #fff;
  }
  .mainHeader {
    padding-top: 115px;
    position: absolute;
    margin-left: 50%;
    font-weight: 200;
    transform: translate(-50%, -50%);
    font-size: 28px;
    width: max-content;
  }
</style>

<script>
import story from '../components/Story.vue';

export default {
  name: 'PageIndex',
  components: {
    storyBlock: story,
  },
};
</script>
