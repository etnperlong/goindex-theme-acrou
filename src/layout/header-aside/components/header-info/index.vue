<template>
  <div class="navbar-item has-dropdown is-hoverable">
    <a class="navbar-link is-arrowless" title="$t('about.title')">
      <i class="fa fa-info-circle" aria-hidden="true"></i>
    </a>
    <div class="navbar-dropdown is-left">
      <a class="navbar-item" @click="goGithub">
        <span class="icon">
          <i class="fa fa-github" aria-hidden="true"></i>
        </span>
        {{ $t("about.github") }}
      </a>
      <a class="navbar-item" @click="goTelegram">
        <span class="icon">
          <i class="fa fa-telegram" aria-hidden="true"></i>
        </span>
        {{ $t("about.telegram") }}
      </a>
    </div>
  </div>
</template>

<script>
import util from '@/libs/util'
export default {
  data () {
    return {};
  },
  methods: {
    goGithub () {
      util.open("https://github.com/Aicirou/goindex-theme-acrou")
    },
    goTelegram () {
      util.open("https://t.me/MyKeyVans")
    },
  },
};
</script>
