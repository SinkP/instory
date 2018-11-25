<template>
  <q-layout view="lHh Lpr lFf">
    <q-layout-header>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          @click="leftDrawerOpen = !leftDrawerOpen"
          aria-label="Menu"
        >
          <q-icon name="menu" />
        </q-btn>

        <q-toolbar-title>
          InStory
        </q-toolbar-title>
      </q-toolbar>
    </q-layout-header>

    <q-layout-drawer
      v-model="leftDrawerOpen"
      :content-class="$q.theme === 'mat' ? 'bg-grey-2' : null"
    >
      <q-list
        no-border
        link
        inset-delimiter
      >
        <q-list-header>Навигация</q-list-header>
        <q-item @click.native="openURL('http://quasar-framework.org')">
          <q-item-side icon="whatshot" />
          <q-item-main label="Лучшее"/>
        </q-item>
        <q-item @click.native="openURL('http://quasar-framework.org')">
          <q-item-side icon="fiber_new" />
          <q-item-main label="Свежее"/>
        </q-item>
        <q-item @click.native="openURL('http://quasar-framework.org')">
          <q-item-side icon="dashboard" />
          <q-item-main label="Песочница"/>
        </q-item>
        <q-item @click.native="openURL('http://quasar-framework.org')">
          <q-item-side icon="assignment" />
          <q-item-main label="Блоги"/>
        </q-item>
      </q-list>
    </q-layout-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { openURL } from 'quasar';

export default {
  name: 'MyLayout',
  data() {
    return {
      leftDrawerOpen: this.$q.platform.is.desktop,
    };
  },
  methods: {
    openURL,
  },
};
</script>

<style>
  .q-toolbar {
    background-color: #222 !important;
  }
  .q-toolbar-title {
    font-weight: 200;
    font-size: 22px;
  }
</style>
