<template>
  <nav class="navbar has-shadow is-spaced" role="navigation" aria-label="main navigation">
    <div class="container">
      <div class="navbar-brand">
        <span class="navbar-item">
          <router-link to="/">
            <h1 class="title is-3">KOUDOU</h1>
            <!-- ここに地域名 -->
          </router-link>
        </span>
        <a
          role="button"
          @click="burgerOpen = !burgerOpen"
          @tap="burgerOpen = !burgerOpen"
          class="navbar-burger"
          :class="{ 'is-active': burgerOpen }"
          aria-label="menu"
          aria-expanded="false"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>
      <div class="navbar-menu" :class="{ 'is-active': burgerOpen }">
        <div class="navbar-start"></div>
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <button class="button is-primary" @click="localeModal = !localeModal">
                <span class="icon" style="margin-left: 0px;">
                  <i class="fas fa-globe-asia fa-lg"></i>
                </span>
                <strong>{{ $t("message.locale") }}</strong>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="locale-modal" class="modal" :class="{ 'is-active': localeModal }">
      <div class="modal-background" @click="localeModal = false"></div>
      <div class="modal-content">
        <div class="box">
          <div class="field">
            <div class="control">
              <label class="radio">
                <input
                  type="radio"
                  value="ja"
                  v-model="$parent.$i18n.locale"
                  @click="localeModal = false"
                />
                日本語
              </label>
            </div>
          </div>
          <div class="field">
            <div class="control">
              <label class="radio">
                <input
                  type="radio"
                  value="en"
                  v-model="$parent.$i18n.locale"
                  @click="localeModal = false"
                />
                English
              </label>
            </div>
          </div>
        </div>
      </div>
      <button class="modal-close is-large" aria-label="close" @click="localeModal = false"></button>
    </div>
  </nav>
</template>

<i18n>
{
  "en": {
    "message": {
      "locale": "Region & Language"
    }
  },
  "ja": {
    "message": {
      "locale": "言語・地域を選択"
    }
  }
}
</i18n>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'AppBar',
  data: () => {
    return {
      localeModal: false,
      burgerOpen: false,
    };
  },
});
</script>
